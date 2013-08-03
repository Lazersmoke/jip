jip
===

A miniature package manager for ease of life.

For Users
=========
To install jip, run
    sudo ./installJip
in a terminal. When you want to install a package, use:
    sudo jip pacakge_to_install.jip

For Developers and Packagers
============================
1.  Create a directory.
2.  Enter Directory.
3.  Make a Directory called "depends".
4.  Put all <i>Librarys</i> (.a, .so, etc) that your program depends on in that folder.
5.  Make a Directory called "runs".
6.  Put all <i>Programs</i> that your program depends on in that folder.
7.  Make a Directory called "userruns".
6.  Put all <i>Programs</i> that a <b>typical</b> end user would run from the <b>command line</b> in that folder. I can't stress this enough.
8.  Create a .tar.gz named "YourProgram-YourVersion-SeeNoteBelow.tar.gz" that contains depends, runs, and userruns directly under the G-zip
7600.  Rename your .tar.gz to a .jip
9.  Publish your .jip, and point users towards this page or your own hosting of jip

NOTE: Possible naming schemes include:
-   TicTacToe-v1.0.0-beta.jip
-   TicTacToe-version1.jip
-   TicTacToe-version1-beta.jip
-   TicTacToe-v1.0.0.jip
-   tictactoe-v1.0.0-beta.jip
-   tictactoe-version1.jip
-   tictactoe-version1-beta.jip
-   tictactoe-v1.0.0.jip  
i.e. there is no standard version scheme and anything after the version is not neccessary, but should be preceded by a hyphen if present

Technical: The directories in your archives will be copied to /usr/local/jip/depends, /usr/local/jip/runs, and /usr/local/jip/userruns.
