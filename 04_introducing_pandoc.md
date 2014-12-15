#Week 4: Introducing Pandoc

- What does PANDOC do? It is a sort of conversion editor that translates your format into whatever format you want. **What?!** Is this true or even possible? It does it. It transforms any textual format into any other format. Give it a try. Become a *believer*.

- Please be aware of the fact that our new best friend, **Pandoc**, actually functions solely through a terminal interface. Textual commands will have to be learnt.

- __YaML__ is a little block of code that Pandoc automatically adds to any text it produces or converts. It contains information such as the title of the document, its author, and the bibliography that it is using. It can be personalized in order to add any sort of additional indication that we might need (but asome coding skills will be required).

- Some practice with PANDOC will be required.

- The command line: `pandoc -so notes.pdf Lab_Notes.md`
	- Variables:
	
		- **s** stands for **smart**;
		
		- **o** stands for *now guess what I am using* (he does so according to the extension we have used for the source and **the target** file).
	
	- Order of SVO:
	
		- **target** first (notes.pdf);
	
		- **source** second (Lab_notes.md).

> An important note of wisdom from Dennis Tenen: there is no such thing as a pure file name. We are always using a complete path, then a file name. The path can be virtually omitted, but it is still there.

> An additional note of wisdom from Dennis Tenen: reasonable standard (__reasonable default__) is an essential part of the Linux philosophy.

> Third note of wisdom: command-line tools do __one thing well__. That is why they can just be evoked once, and their only true variables (commands, inputs) are the flags that I can add to the principal command.