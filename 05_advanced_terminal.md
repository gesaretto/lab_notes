#Week 5: Advanced Terminal

#GPS

_Where am I?_

- `pwd` Path to __local directory__.
- `ls`
- __tab__: this command completes the current command. It is an _autocompletion_ function.  **Tab the world.**
- `cat` _Displays a file as a stream of text._
- `man` _Invokes the __manual__ for a command; ex.: `man cp` tells us all flags and adverbs for `copy`._
- `-h`
- `-help`
- `history` _Displays the __history__ of what that has been done during this session. (Better, it remembers a determined amount of lines.)_
- `cd` _Change Directory._
- `echo` _Reproduces the text on screen_; 
	- OR, if followed by the operator `>`, it _reproduces it within a file (rewriting the file)_; 
	- OR, if followed by the operator `>>`, it _appends it within __a new file__ (adding the contents)._
- `clear` _Clears the current screen._

##Files

- `mkdir` Creates a directory.
- `touch` Creates a new file.
- `cp` **:(** _It copies the contents of a file inside another file. And it **replaces** them!_
- `mw` **:(** _It moves a file._
- `rm` **:(** _It removes a file._

##Operators

- `>` _Replaces the contents of a file._ __:(__
- `>>` _Appends to the contents of a file._
- `|` _This breaks down a long screen output into smaller portions visible one at a time._
	- `less` is a _paginator_ for this specific function; it lets you scroll along a text.
- `!` _We are not doing this now._

##Search
- `find`
- `grep` _Used after the pipe `|`, it returns the result of a search._
- `rwk`

##Paths/Shortcuts
- `/`: __root__
- `~`: __home__
- `-`: __previous__


##Flags##
_Flags are truly universal._

- `-i` _This asks for confirmation before executing the actual command._
- `-r` __Super dangerous.__ _It means recursively; when applied to **remove**, for instance, it deletes each file within a directory, then the directory itself._

> Dennis' Pep Talk: 
>
> - Linux philosophy: 
>      1. use simple commands; 
>      2. produce plaintext.
>      
> Combine 1) and 2) and you will get a very powerful set of tools. Think of _Streaming data_ and _projecting data_, therefore controlling the vector that is __communication__ - and __text__.
Linux is a *textual system*.

- - -

###__Syntax__:

- All that I have on my command list are **Verbs**. To this **Verbs** I can append **Adverbs** and finally *Objects**.

- Let us now imagine that we are the **Parser**. The **Parser** considers **SPACE** and **SYNTAX**. 

> - Important note from DT: always use files that have **No spaces in it**. 
	
> - And try **not to use capitals**.

> Good policy: add a backslash when you are talking about a directory: *trash/*.

> An essential secret: we are just using shortcuts here, especially when moving files within a same directory or from a directory to the upper or lower. It should always be remembered that in truth the command is referring to longer, elaborate paths that start from the root folder every time. If we use current directory and upper directory, we are using **relative paths** (?); if we define the entirety of a directory position - the entire path - we are using its **absoultue path**.

> Food for thought: start thinking about **textual streams**.