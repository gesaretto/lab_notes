#Week 6: Textual Research and Manipulation

> __D.T.__: file are files: they do not depend from anything else; when, instead, I am installing some sort of elaborate software - Firefox, OpenOffice or so on - an elaborate group of files, interrelated and dependent from both themselves and other files in the hard drive, is simultaneously copied in different areas of the hard disk. Therefore, installing is an elaborate and flexible manner of copying.

> __D.T.__: people who use Macs (posers) had to install additional software in order to attend today's class; programs usually rely on current versions of files installed by the operating system. How does Linux work? Linux has a vast repository of all the software that is available for any version of its operating system; the repository is also careful not to incur in any software conflict.

> __D.T.__: programming languages similarly possess repositories. Think of Ruby and Python: they have repositories that work in the same way, libraries from which we can obtain software without bothering about conflicts, and dependencies.

##Friends!
* `head`: *It shows us the first few lines of the file.*
* `tail`: *It shows us the final few lines of the file.*
* `cat`

##Network
* `wget`: *Used to download stuff from the interwebs.*

> __D.T.__: let us think about files and extensions. We know what file names are, and we know what extensions are. For instance, when we have a **.pdf** file, the operating system and the user know that the file, regardless of its specific name, is only readable by Adobe. Somewhere in our operating system, the **.pdf** extension is associated with the specific software Acrobat Reader - so that, whenever we automatically open the file, Acrobat Reader is automatically used. If we change the extension, the operating system will not know what software to use when opening the file. *But* the file will anyway be readable - because the first few lines of the file contain the essential information that make it readable for its corresponding software. If we change the extension, the file is still readable. If we change the first few lines, regardless the extension, we **won't** be able to open it.

> *So, what have we learnt?* The extension is the sort of **attunement** that my operating system might need in order to correctly open a file.

##Search
* `locate`: *Use it to find files.* **Locate** uses a database of files that is located somewhere in my hard disk. 
* `find`
* `grep`
* `awk`

> __D.T.__: someone who's able to use these four tools is __insanely cool__.

> __D.T.__: patterns can become extremely complicated; but starting, for instance, with a star `*`, can be helpful and easy. Try removing all files that end with **.pdf** - the command would be: ``rm -r *.pdf``.

* `find`: Here is a sample command ``find . -name "*.md"``. What does the dot `.` mean? It means that we will start looking in the current directory. If we used `/`, __find__ would start by looking in the _root directory_.

* `*` The asterisk is a convenient wild-card. It can be used to substitute any string within a file name that I currently looking for. It can also be combined in different formulas (i.e.: ``find . -name "ora*.tx*"``).

* `find` uses the full range of _regular expressions_. It is an incredibly powerful tool to look for any sort of string.

> And now, for a little experiment. Find a digital copy of Moby Dick! Now get it with __wget__ and the full url. Then, use __grep__ on the file itself, and look for a string within the file.

* `grep` You can use it to look for strings within a specified file; for instance ``grep "Moby" moby_dick.txt`` will look for the string "Moby" within the file "moby_dick.txt". Easy-peasy. If I want to look for a string within all the files contained in a directory, all that I have to do is using an asterisk instead of the specific file - ``grep "Moby" *``. The asterisk works as a wildcard for any file contained in the directory.

	* `grep` If I want to look within the files within the directories contained in the current directory (therefore, extending the search to the subdirectories of the current directories), I have to use the _recursive_ modifier __-r__.

	* `grep`: Let us count the number of times that the number of times that the word "whale" is used in the novel. Here is the very simple command ``grep "whale" moby_dick.txt | wc``. __wc__ is the command used to deliver a word count; it expresses its result in the form _lines_, _words_, _characters_. Also notice that a byte is a character. Therefore, the number of occurrences in the novel will be the first datum in my output. __NB__: __wc__ is useless if we consider those words that occurr twice in a single line.

* `wc` is used to count lines and words. Otherwise pretty useless!

* `sort` it is worth playing a little with this. It puts the output in __alphabetical order__. _Cool stuff._

* `uniq` it counts the unique occurrences of a line within a specific file.

> __D.T.__: Unix-based systems have a built-in idea of what a character, a line, and a word are. They are an intrinsic part of the foundations of these operative systems.

> __D.T.__: Start thinking about the physicality that is beyond our comprehension of _software_.

* `sed`: This cool function is used to substitute words from a file. Here is a sample: ``sed s/mauricio/arturo sbombazzi/ mauricio.txt`` will substitute each occurrence of the string ``"mauricio"`` with an occurrence of the string ``"arturo sbombazzi"``. __N.B.__: this is only a substitution occurring at the level of _output_. If we want to actually _modify_ or _transform_ the source text, we have to use the modifier, or _flag_, __-i__. Then I will have a different file. In order to substitute _every occurrence_ of a word within a file, we have to use a second modifier, appended to the instruction - and that is __g__. Here is an example: ``sed 's/mauricio/arturo sbombazzi/g' heymauricio.txt``.