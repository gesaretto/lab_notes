# Week 10

### What is Git?

- Imagine having a journal that keeps track of every sort of activity we do; a ledger. That is Git. How does this journal work?
	- We have a __project__ (that is, in the format used by git, a _folder_); this folder, this project, holds a number of documents. Every time that a change is made within the folder, or project, we possess a new version of the project.
	- This is the __file system__ level.
- We add a second layer to this __file system__ layer; it is the __journal__, or _git_, level.
- Between the __folder__ and the __journal__ we have an intermediate level, the _stage_. This is a __desk__, holding a number of open files and stages.
- This __journal__ consists of a collection of fixed and packed __stages__.

### How does this thing work?

- First we ask Git to set up a structure; we will use the command __git init__. Whenever we want to add files to this structure, we will use the command __git add__. Finally, when we will write down our labor in our digital journal, we will use the __git commit__ command.
> Notice that __git add__ and __git commit__ are different commands, corresponding to two different moments. We can add files to our ledger, but we do not really need to transform them into full stages.
- What else can we do? Well, we can bring everything online with the __git push__ command: it will save a copy of our journal on the cloud.
- The __stage__ is a sort of bag where we store stuff.
- Now, for the collaborative part.

### How does it help us do stuff with other people?

- Just imagine sharing a ledger, a set of stages, a number of versions. We can synchronise our work within a general timeline.

## _ACTION_

- How do we list hidden files? With __ls -a__. It will show us a hidden directory within our test directory; it has been created by __git__.
- We created the _git_ hidden directory through the command __git init__.
- We can verify the status of our _journal_ through the command __git status__.
- Git is keeping track of our activity! Try creating a new file, and check with __git status__.
- Let us _commit_ our files! To add a note to our __git commit__ step, we add the flag __-m__: let us tell __git__ what we did.
- All of our changes and backup are being stored in the hidden __.git__ directory. Be careful! If we need to get rid of the __git__ journal, we just need to remove this hidden directory with something like: __rm -rf .git/__.
- Notice that __git hub__ truly requires _plaintext_ to work properly.
