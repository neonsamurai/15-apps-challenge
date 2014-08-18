15-apps-challenge
=================

Challenge yourself by writing 3 different apps with 5 different languages! Learn TDD. Learn new programming languages. Learn new frameworks. And have a lot of fun :)

About
=====

This is a challenge for everybody who wants to broaden her knowledge about
programming languages, libraries and frameworks as well as training test driven
development also known as TDD.

If you don't know what TDD is or why it is important I recommend watching this
talk on Youtube: https://www.youtube.com/watch?v=HhwElTL-mdI and follow this
tutorial: https://github.com/orfjackal/tdd-tetris-tutorial.

The idea is to pick 5 different programming languages, some of which you
already are proficient with and some you don't know yet, and develop 3
different applications in those languages applying the test driven development
process.

The Rules
=========

- Fork this repository.
- Add a subdirectory, using your Github username as the directory's name.
- Develop your apps test driven.
- Put the source code of each app in a sub directory ('/cp', '/notepad',
  '/sha256').
- Within the application directories create sub directories for each language
  (ie. '/cpp', '/java' etc.).
- All requirements of each application must be met. They are described in the
  following chapter 'The Apps'.
- If you want your code to be shared in this repository, send me a pull request.

The Apps
========

We are going to develop three different apps in 5 different languages. A CLI
application, a GUI application and a web application. The requirements for each
application are listed below.

Happy coding :)

CP clone (CLI)
--------------

- It should be invoked with the command 'mycp'.
- It should take two inputs:
  - source, which is a file you want to copy
  - destination, which is the destination file name where you want to copy the
    file
- It should copy the file in source to the file in destination when invoked
  correctly
- It should fail copying if the paths to source or destination cannot be
  resolved.
- It should fail copying if source is a directory.
- It should allow an optional flag -r.
- It should regard source and destination as directories if the flag -r is set.
- It should recursively copy files from source to destination if the flag -r is
  set.
- It should fail copying if source or destination is a file and the flag -r is set.

Notepad clone (GUI)
-------------------

SHA256 REST service (Web app)
-----------------------------
