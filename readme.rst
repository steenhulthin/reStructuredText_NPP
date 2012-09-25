=================================================================================
 reStructuredText_NPP_ - reStructuredText basic syntax higlighting for Notepad++
=================================================================================
:Author: Steen Hulthin Rasmussen <kontakt@percipio.dk> 
:Date: |date|
:Description: reStructuredText_NPP_ is a User Defined Language for `Notepad++`_ that provides basic syntax higlighting for reStructuredText_. 
:License: reStructuredText_NPP_ is licensensed under *The MIT License* (see http://opensource.org/licenses/mit-license.php or the license.txt file)

.. |date| date::
.. _reStructuredText_NPP: https://github.com/steenhulthin/reStructuredText_NPP
.. _`Notepad++`: http://www.notepad-plus-plus.org/
.. _reStructuredText: http://en.wikipedia.org/wiki/ReStructuredText

Install 
=================
#. Make sure you have `Notepad++`_ installed with the option to use %APPDATA% (which is the default).
#. Download and unzip the zipped reStructuredText.xml from the download tab (This is the only file you need in order to use reStructuredText_NPP_.) 
#. Start `Notepad++`_ and open the "User Defined Dialogue..." (Under View -> User Defined Dialogue...) 
.. image:: documentation/select_user-defined_dialogue.png
#. Click "import" and select the unzipped reStructuredText.xml file.
.. image:: documentation/import_user_define_language.png
#. Restart `Notepad++`_

Features
==========
reStructuredText_NPP_ provides basic syntax highlighting. reStructuredText_NPP_ is not a full lexer for reStructuredText and does *not* highlight all elements of reStructuredText markup specification (correctly). 

Highlighted element::
* tables
* directives
* Bullet lists
* Enumerated Lists
* Field Lists (works, with exception field with space characters)
* Line Blocks (Only the | [pipe] characters is highlighted)
* Transitions
* Footnotes
* Citations
* Hyperlinks (with a few exceptions)
* Substitution

