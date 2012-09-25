=================================================================================
 reStructuredText_NPP_ - reStructuredText basic syntax higlighting for Notepad++
=================================================================================
:Author: Steen Hulthin Rasmussen <kontakt@percipio.dk> 
:Date: |date|
:Description: reStructuredText_NPP_ is a User Defined Language for Notepad++_ that provides basic syntax higlighting for reStructuredText_. 
:License: reStructuredText_NPP_ is licensensed under *The MIT License* (see http://opensource.org/licenses/mit-license.php or the license.txt file)

.. |date| date::
.. _reStructuredText_NPP: https://github.com/steenhulthin/reStructuredText_NPP
.. _Notepad++: http://www.notepad-plus-plus.org/
.. _reStructuredText: http://en.wikipedia.org/wiki/ReStructuredText

Install 
=================
#. Make sure you have Notepad++_ installed with the option to use %APPDATA% (which is the default).
#. Download the zipped reStructuredText.xml from the download tab (This is the only file you need in order to use reStructuredText_NPP_.) 
#. Copy/move cmdUnit to a folder. 
#. Create a empty test.cmd file to contain your tests (you can call it anything you like - but it should have the extension .cmd).
#. Go to the 'Usage' section.

Usage
=============
In your test file you call cmdUnit.cmd <test name> AssertAreEqual <expected value> <actual value>.

example::

 Call cmdUnit.cmd MyFirstCmdUnitTest AssertAreEqual HelloCmdUnit HelloWorld
 
From a command prompt run your test file::

 test.cmd

`That test will fail`_ (and return exit code 1). 

    .. _`That test will fail`: https://bitbucket.org/percipio/cmdunit/src/13d3e16f0795/documentation/firstFailingTestRun.png

Let's fix the test::

 Call cmdUnit.cmd MyFirstCmdUnitTest AssertAreEqual HelloCmdUnit HelloCmdUnit

From a command prompt run your test file again::

 test.cmd

`The test now passes`_ (and return exit code 0). 

    .. _`The test now passes`: https://bitbucket.org/percipio/cmdunit/src/9e70820a965b/documentation/firstPassingTestRun.png
 
__ http://semver.org

FUQ - Frequently Unasked Questions
==================================
#. :Q: What language is cmdUnit written in?
   :A: CmdUnit is written in windows command line.

#. :Q: Why should I use CmdUnit when I can use Powershell_?
   :A: You should not. Use Powershell_ and  psunit (http://psunit.org/) or something similar.

#. :Q: Why should I test my .cmd scripts - it would take longer to write the tests than rewriting the scripts themselves from scratch?
   :A: Up to you, but is your scripts included in your CI_ builds? You can do that with CmdUnit tests. 

#. :Q: I'm on Linux/BSD/Mac/Solaris/Cray/amstrad464/C64/zx81. Can I use CmdUnit?
   :A: No. (well, maybe if you really, really wanted. But why would you?)
   
#. :Q: Is this project really providing value to the world? 
   :A: It does to me. And I'm sometimes present in what you call *the world*. 
   
#. :Q: How can I help the project?
   :A: Try it out, give feedback/write code and/or spread the word.
   
#. :Q: Is CmdUnit stable?
   :A: No. Currently CmdUnit is just a newborn. Versioning follows `semantic versioning`__.
   
Acknowledgement
===============
CmdUnit would never have come into existence if it wasn't for IT guys that insist that Powershell_ is a security risk on Windows Server 2003. 

.. _Powershell: https://en.wikipedia.org/wiki/Windows_PowerShell
.. _CI: https://en.wikipedia.org/wiki/Continuous_integration