# Week 11: Advanced GitHub

## Approaches to shared labor

- __Committing and journalling__; select a set of modifications - of changes -, turn them into a sort of package, write what they actually mean, and then store them as a single step.

- __Simultaneous changes__ by multiple editors (the Google doc model) create potential for unjustified collective choices: erase a paragraph, modify it heavily and so on. The changes are irretrievable and irreversible.

- __Branching__: allows for a control of voluntary changes - I decide what I commit and upload (thereby avoiding the absolute mess of an automatic storing of versions, like the one in Google Docs); I can access any of those changes, which can branch into multiple paths.

## Practice

- Assignment: open a new repository (__folder__) called `lab_notes`; _push_ our `lab_notes to this _repository_.

	1. Let us do the `git init` thing in our `lab_notes` folder.

	1. Check whether `git init` worked by looking at the hidden folders and files with the `ls -a` command. If we find a __.git__ folder, the thing worked well.

	1. My actual lab notes are currently a mess! I have at least three files, each containing a variable amount of information, without dates or order! I will place all of my versions (drafts of different parts of the course) inside the `lab_notes` folder in my hard drive.
	
	1. Now, I will simply commit all of my files as an initial stage of my work.
	
		11. I first use `git add` to add each file to my _stage_.
		
		11. To check what I have done or not done, I should use `git status`.

		11. Finally, I will `git commit` my changes. To add a comment, I will add the `-m` flag.
	
		11. Let us upload these changes! We do this by __pushing__.

			111. To upload, we first have to tell git where our remote repository is. We do this by using the `git remote add origin` command line, followed by the url of our remote repository.
		
			111. We then push our changes by using the `git push -u origin master` command.
	
	1. Nice. Now, let us create 11 `lab_notes` files, one for each week. I will use `touch` to create each one of these.

	1. I will now proceed to copy and paste my notes into each of these files.