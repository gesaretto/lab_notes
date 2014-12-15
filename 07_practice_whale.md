#Week 7: Hunting the Whale

> __D.T.__: And now, for an assignment!

1. Analyze the treatment of gender in Moby Dick. Look for words that have to do with _gender_.
11. Create a new project directory; get a copy of Moby Dick; create two lists: one for maleness, the other one for "femaleness".
11. Use **grep** to get the context of every male word and every female word (creating two split versions).
11. Get rid of common English words (the, end, but, etc.).
11. List the words that were near the male and the female words. You will find out what words are most often associated with female and male concepts.

> __D.T.__: Careful, because this will be crucial: some of these commands, such as __grep__, can have _files_ as attributes.

##The answer

> __D.T.__: General advice. Use the programming approach: take an apparently insurmountable problem, then break it down into smaller pieces.

### Pseudo-code
0. Create a project directory.
1. Grab the text of the novel[1].
2. Make two lists: one of words related to humans, one to animals.
3. Find all those words in the text, grab context, and save to file.
4. Separate lines into words (tokenize). Make new files that contain word lists.
5. Make a print out of all the words that are in File A but not in file B and the other way around.

### Code

1. ``mkdir whale/``
1. ``touch animal_words.txt``
1. ``echo -e "whale\nrat\nsquid\noctopus\nfish\nfin\nleviathan\nmanatee\nwalrus\nkraken" >animal_words.txt``
1. ``touch human_words.txt``
1. ``echo -e "human\nman\nperson" >human_words.txt``
1. ``wget -O moby.txt http://www.gutenberg.org/cache/epub/2701/pg2701.txt``
1. ``grep -w -i -f human_words.txt moby.txt | sed 's/\s/\n/g' | tr -d [:punct:] | sort | uniq -i >human_context.txt``
1. ``grep -w -i -f animal_words.txt moby.txt | sed 's/\s/\n/g' | tr -d [:punct:] | sort | uniq -i >animal_context.txt``
1. ``grep -Fxv -f human_context.txt animal_context.txt >animal_only.txt``
1. ``grep -Fxv -f animal_context.txt human_context.txt >human_only.txt``

[1]: <http://www.gutenberg.org/cache/epub/2701/pg2701.txt>
