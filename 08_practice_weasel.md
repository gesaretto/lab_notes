#Week 8: Weasel Words
> __D.T.__: The second exercise is called "weasel words".

2. Create a directory.
3. Place in it three files in plaintext that we used. 
4. Create a list of "weasel words" (clearly, significant, agency). 
5. The assignment will be sent to us. And we will have fun!

##The answer

###Pseudo-code

1. Write a list of weasel words (weasel_words.txt).
1. Look for those words in each of the three files; print out the output into three new files (*_weasel.txt).
1. Transform the list of weasel words (weasel_words.txt) into a script for the "sed" command by adding "s/" and "/WEASELWEASEL/" at the beginning and at the end of each line (weasel_script).
1. Use the new script with the "sed" command in order to substitute the weasel words contained in the passages printed out in step 2; save the output as three new files (*_final.txt).

###Code

1. 	``nano weasel.txt``
1.  	``grep -f weasel.txt paper_film.txt >paper_film_weasel.txt``
1. 	``grep -f weasel.txt paper_race.txt >paper_race_weasel.txt``
1. 	``grep -f weasel.txt columbia_statement.txt >columbia_weasel_original.txt``
1. 	``sed 's_[a-z]*_s/&/WEASELWEASEL/_' weasel.txt >weasel_script``
1. 	``sed -f weasel_script paper_race_weasel.txt >paper_race_final_txt``
1. 	``sed -f weasel_script paper_film_weasel.txt >paper_film_final.txt``
1. 	``sed -f weasel_script columbia_weasel_original.txt >columbia_statement_final.txt``
