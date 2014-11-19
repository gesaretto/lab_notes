# Week 11

- Committing and journalling (?); select a set of modifications - of changes -, turn them into a sort of package, write what they actually mean, and then store them as a single step.
- Simultaneous changes by multiple editors (the Google doc model) - creates potential for unjustified collective choices (?): erase a paragraph, modify it heavily and so on. The changes are irretrievable and irreversible.
- Branching: allows for a control of voluntary changes - I decide what I commit and upload (thereby avoiding the absolute mess of an automatic storing of versions, like the one in Google Docs); I can access any of those changes, which can branch into multiple paths.

## Assignment

- Open a new repository (__folder__) called __lab_notes__; push our __lab_notes__ to this _repository_.

1. Let us do the __git init__ thing in our __Lab_notes__ folder.
1. Check whether __git init__ worked by looking at the hidden folders and files with the __ls -a__ command. If we find a _.git_ folder, the thing worked well.
1. My actual lab notes are currently a mess! I have at least three files, each containing a variable amount of information, without dates or order! I will place all of my versions (drafts of different parts of the course) inside the __lab_notes__ folder in my hard drive.
1. Now, I will simply commit all of my files as an initial stage of my work.
11. I first use __git add__ to add each file to my _stage_.
11. To check what I have done or not done, I should use __git status__.
11. Finally, I will __git commit__ my changes. To add a comment, I will add the __-m__ flag.
11. Let us upload these changes! We do this by _pushing_.
111. To upload, we first have to tell git where our remote repository is. We do this by using the __git remote add origin__ command line, followed by the url of our remote repository.
111. We then push our changes by using the __git push -u origin master__ command.
1. Nice. Now, let us create 11 lab_notes files, one for each week. I will use __touch__ to create each one of these.
1. I will now proceed to copy and paste my notes into each of these files.
