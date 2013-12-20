GotoSelectionDef
=============

Description
-----------

Small plugin for Sublime Text that pre-fills the Goto Word overlay with the selected text or current word.


Installation
------------

GotoSelection can be installed by:

* Cloning this repository in Packages

		Change directory into your Sublime Text Packages folder
		git clone git://github.com/FordAldrich/GotoSelection.git

* Downloading the files manually and placing them in a directory under your Sublime Text Packages folder (such as GotoSelectionDef)

	I'd recommend placing them in a unique directory, as opposed to simply dropping them in your User folder.


Usage
-----

GotoSelectionDef is a plugin that, when invoked, will pre-fill a Goto Anything overlay box with the currently selected text and
prepend it with '#'. It is a poor's man Goto Definition for a single file. It is useful since Sublime Text does not index
variables for inbuilt Goto Definition feature.
If there is no current selection, then GotoSelectionDef will use the "word" under the cursor.  By default, GotoSelectionDef uses 
the word separators defined in Default Settings (or User Settings, if you've overridden the defaults).  This behavior can
be changed by editing GotoSelectionDef.py to reflect your needs.  Instructions to set up custom word separators are found
within the code file.

The default key binding for GotoSelectionDef is "ctrl + ;", which can be edited by the user by making the appropriate changes
in Packages/GotoSelectionDef/Default.sublime-keymap


Credits
-------
A fork of git://github.com/FordAldrich/GotoSelection.git

"Inspiration for this little plugin came from my own needs and a variety of requests I found while searching for a solution 
to my problem; namely, I felt that project navigation could be streamlined if I could pre-fill the magic Goto Anything overlay.

In situations where class names often match file names, GotoSelection can make it easier to rapidly open the source code for a 
given class, and can also help in looking up methods and such within the current open file."