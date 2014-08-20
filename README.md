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
- It should fail copying if source or destination is a file and the flag -r is
  set.
- It should provide a summary of its functionality when invoked with the wrong
  number of parameters or an unsupported flag.

Notepad clone (GUI)
-------------------

- It should display a window on startup.
- It should have a menu bar on the top of the window.
- It should have a text editing area which takes the rest of the window's
  space.
- The text area should resize when the window is resized by the user.
- The text area should provide scrollbars when the text is larger than the
  boundaries of the text editing area.
- It should provide standard text manipulation controls like cursor movement,
  page up/down, backspace and delete.
- The menu bar should have a menu named 'File' with menu items 'New...',
  'Open...', 'Save' and 'Exit'.
- The menu bar should have a menu named 'Edit' with menu items 'Copy', 'Cut',
  'Paste'.
- The menu bar should have a menu named 'Help' with the menu item 'About'.
- It should open a file chooser dialogue when clicking the 'File - Open...'
  Menu item.
- It should close the file chooser dialogue and open the file in the text
  editing area when clicking 'Open' in the file chooser dialogue.
- It should empty the text editing area when clicking the 'File - New' menu item.
- It should save the file to disk when clicking the 'File - Save' menu
  item. Save it to the file's location when it is not a new file. Open a file
  chooser dialogue if the file is new, so that the user can choose location and
  name of the file.
- It should close the application when clicking the 'File - Exit' menu item.
- It should allow selecting text in the text area either with the mouse or by
  using the shift key and cursor keys.
- It should copy selected text to the clipboard when clicking 'Edit - Copy'
  menu item or pressing CTRL+C.
- It should delete the selected text from the text editing area and copy it to
  the clipboard when clicking the 'Edit - Cut' menu item or pressing CTRL+X
- It should paste text from the clipboard into the text editing area when
  clicking the 'Edit - Paste' menu item or pressing CTRL+V. The text should be
  pasted after the cursor position if no text is selected. If text is selected
  the text should be deleted before pasting.
- It should provide a short info text about the Challenge and the author of the
  application when clicking the 'Help - About' menu item.

SHA256 REST service (Web app)
-----------------------------
- It should adhere to the standard requirements of a RESTful service as stated
  here: http://en.wikipedia.org/wiki/Representational_state_transfer (see:
  'Applied to web services')
- It should display an about page on the root url.
- It should make the root of the api available at '/api/'.
- It should make the sha256 service available at '/api/sha256/'.
- It should take a string as post data at '/api/sha256/' and return the sha256
  representation of that string.
