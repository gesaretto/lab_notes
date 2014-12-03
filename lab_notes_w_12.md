# Week 12

- Minimally viable computing (?).
- Take a topic that I like and write a _tutorial_ about it (about one page).
- Possible topics:
    1. Markdown & plaintext
        - bibliography
    1. File-system
    1. Terminal
        - find
        - sed
        - ...
    1. Networking
        - Ping
        - Traceroute
    1. Crypto
        - psomethingp
    1. Repositories
        - apt
        - brew
    1. Git
        - Version control
    1. File permissions

## A small tutorial on _pull request_
- Completely mysterious stuff is being drawn on the whiteboard.
- In general, the system apparently works through copies of an original, primary repository; each discrete user works on the copy of a primary repository; whenever an integration of both is needed, it is up to the owner of the primary repository to decide whether the improvements of the copy are better than the ones in the primary (original).

### A digression by D.T.
- Limited access to a terminal; that was a thing until little time ago - there was only a terminal, and multiple users, each one with an account and a different set of capabilities and authorizations.
- The rise of the personal computer: several discrete units, one for each person; a decentralized system that presupposed the a existence of a one to one relationship between each user and each machine.
- Birth of a centralized system: the __internet__, of course. Let us think about the _cloud_: it is a vast primary server, to which we access whenever we need to retrieve information.
- Now a lot is moving towards the cloud: software, for instance, will be more and more accessed online, and only available on a remote system of servers.
- There is a tradition of multiple users on traditional OSs, anyway; __users__ are baked in my system.

### Practice:

- Try typing ``ls -l`` from the terminal; you will be shown a list of files, complete with information about size, date of creation, and so on.
- Look at the two columns in the middle: one is a user, the second is a group.
- The first column on the left shows us the __permissions__:
    - ``drwxr-xr-x``
        - rwx | rwx | rwx
        - To the first section corresponds the _user_ (__u__), to the second the _group_ (__g__), to the third _everybody else_ (__d__). ``rwx`` stands for __r__ ead __w__ rite e __x__ ecute.
        - If we want to change the permissions, we use the command ``chmod``:
            - If, for instance, we want to change the permissions for the _group_ by granting to it _writing privileges_, I use the command ``chmod g+w test.txt``.
            - To access commands and files that are only available to administrators, I use the command ``sudo``, that stands for __super user__.
            