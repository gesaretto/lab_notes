Materialism
	- It is hard to consider oneself an expert user of contemporary OS. Differently from other skills, the use of IT does not automatically lead to knowledge.
	- Computer - originally giant machine in an office; a shared environment.
	- A terminal is the accessible part of a machine - its interface. Not all modern machines have a terminal.
	- Collective computers are no longer common. But an idea of collective computing persists - and is actually returning - through the concept of cloud.
	- Our personal terminals mirror those of the 70s and 80s.
	- A terminal application emulates the actual terminal.
	- The set of commands that I send to a terminal are part of a batch (? bash). Those are available to each terminal every time.
	- My terminal is emulating the traditional terminal. It is emulating an access to a different machine.
	- Unix and unix derivatives. Unix OS are special ways of accessing a machine. Unix systems are bound together by a general philosophy of computing; there are parts of this philosophy in both Mac and, of course, Android systems.
	- These ways of accessing and manipulating data have been under development since the 80s; they will probably still be used for a very long time.
	- The advantage of Unix based systems is their durability: the code used is Plaintext - readable by humans - and their source code is open.
	- The most essential operations happening in a machine are processed through a binary code; but with Unix, the closest level to this binary - nonhuman - language is a code that we can understand.
	- Unix is longlasting and human friendly. It has to be readable.
	- Interface - have a look at MS Word: some of the buttons and the commands are unknown to most users; besides, its interface will always be significantly different from that of another program. In Unix based systems, the interface is uniform across different softwares. The idea is that of having many small programs that all look and do the same.
	- It is important to consider the potential complexity of any software that we are using.

- - - - - - - - - -

Practice from the Terminal.

	- pwd: gives you the position of where you currently are. The directory where you currently are.
	-  the / indicates the root position.
	- ls: lists the contents of the current directory.
	- mkdir:  creates a new directory.
	- man [+ command]: gives you instructions about the command that you are interested in. "man" stands for "manual". It originally was an actual paper manual.
	- clear: it clears the prompt.
	- cd: change directory.
	- cd ..: leave current directory - move to the above directory.
	- cd -: go to the previous directory.
	- pushd: pushes a stack of directories (?).
	- popd: pops a stack of directories (?).
		- Baboun has built a Unix partition within my Windows system. I have no way of accessing my standard Windows partition from this terminal.
		- The structure of Unix partitions is the same across different Unix systems (from Debian to Android).
	- cd ~: automatically brings you to the "home" directory. There is always one.
		- "bin" is the directory containing all of the basic Unix commands - the small programs that make the entire system words.
		- All Unix commands have a syntax. Usually it is:
			[Verb] - [Adverb] - [Object]
			- The [Verb] is the command itself.
			- The [Adverb] is a modifier for the command.
			- The [Object] is, of course, the destination of the command.
			- Everything in Unix has a path. Any command - [Verb] - actually operates on a path.
	- ls .: the "point" means "execute this command HERE"; it is useful whenever a command asks for an explicit path as an object. In most cases it is not useful.
	- "find" "grab" "send" & "?": are incredibly sophisticated tools to search through my machine.
- Unix has a bias towards plain text data. Plaintext data is portable and sustainable. It will probably last for long and it will always be readable. By humans even. Well, maybe not really. But it certainly does not require a proprietary software in order to be decyphered.
- Plaintext is incredibly easy to process. Data mining and copying are definitely more feasible within a plaintext archive.
	- Learn to use "TAB"! Whenever you type the first two or three characters of a command, an autocomplete integrated system will automatically determine whether the command I am trying to use exists or not.
	- Remember that the entire Unix environment is strictly case sensitive.
	- cat: "concatenate files and print on the standard ouptut".
		- Levels of encryption.
