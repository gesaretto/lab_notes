--------- Week III ----------------

Think of data and data flows as vectors; then, think about the entirety of literary production and **life itself**(?) as the production of vectors - as vectors themselves.

Blogging ------------------->
		[Word Press - XML - XML Editor]

Academic writing ---------->
		[MS Word - Doc - .pdf]

Mail --------------------->
		[MS Outlook - ...]

Now, our goal is to concentrate the entirety of this production and place it within a single box; we will have a single format (which will be, if you want, plaintext), a single editor (we still have to choice) and complementary systems for publishing, backup and so on.

What about a single editor, then? It would amplify our possibilities of interaction/intervention on every aspect of our textual production.

Plaintext: why not markdown, then? It is a plaintext format, it is easy to use and it is truly versatile. Let us get started!

	*** Markdown as a FORMAT, independently from the editor ***

How to emphasize a text? With asterisks.

	*emphasis*

Or with two asterisks.

	**emphasis!**

How to write headings? With hashtags.

#Most important title#
##Important title#
###Least important title###

The extension for Markdown is **.md**. From now on, these notes will be written in *markdown*.

Here, when I TAB something I indicate that the text that I am writing has some sort of CODE quality. It is an environment where, all of a sudden, space and formatting visually matter.

	Here is a text under tab.

More Interesting features. Imagine I have to insert a note. Here^[1].

[1] Note: this is interesting stuff. The notes are not really working.

' code '

'''' code block that is related to code that I do not want to be different from what I am actually writing and how I am formatting it. '''

Let's put a Link here. [Deboscio.](www.ildeboscio.it).
` Hey this is a tick and this is important code that has to be preserved forever. `

` :D `

``` 
Welcome to the JUNGLE! SPACE IS STILL RELEVANT HERE!                          YOWZ.    Yawz. 
```

### A new section. About what you should be doing.

Please take some time to consider options for visualization and editing. Very fascinating stuff happening inside of this section that will start *NOW*.

` TICK `

```

Tick?

```

### Another section. PANDOC.

What does PANDOC do? It is a sort of conversion editor that translates your format into whatever format you want. **What?!** Is this true or even possible? It does it. It transforms any textual format into any other format. Give it a try. Become a *believer*.

- Please be aware of the fact that our new best friend, **Pandoc**, actually functions solely through a terminal interface. Textual commands will have to be learnt.

- YaML is a little block of code that Pandoc automatically adds to any text it produces or converts. It contains information such as the title of the document, its author, and the bibliography that it is using. It can be personalized in order to add any sort of additional indication that we might need (but asome coding skills will be required).

- Some practice with PANDOC will be required.

- `:browse confirm saveas
pandoc -so notes.pdf Lab_Notes.md
	- Variables: 
		- **s** stands for **smart**;
		- **o** stands for *now guess what I am using* (he does so according to the extension we have used for the source and **the target** file).
	- Order of SVO:
		- **target** first (notes.pdf);
		- **source** second (Lab_notes.md).

> An important note of wisdom from Dennis Tenen: there is no such thing as a pure file name. We are always using a complete path, then a file name. The path can be virtually omitted, but it is still there.

> An additional note of wisdom from Dennis Tenen: reasonable standard (reasonable default) is an essential part of the Linux philosophy.

> Third note of wisdom: command-line tools do one thing well. That is why they can just be evoked once, and their only true variables (commands, inputs) are the flags that I can add to the principal command.

What does TAB do?

	Tab.

				Mega TAB.

Is tab telling my editor that I am talking about important coding issues?

			ESSENTIAL CODING ISSUES.

				#CODING DAILY#

Notice that the Hashtags are not turned into titles now. Please, be surprised.
**Bedazzlement.** 