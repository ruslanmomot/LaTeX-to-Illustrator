## LaTeX to Illustrator (Mac OS)
Adobe Illustrator jsx script for Mac OS to insert LaTeX formulas directly into the document.

This is a Mac OS version of script from [latex-community.org](http://latex-community.org/) developed by Hartmut Lemmel ([link](http://latex-community.org/know-how/latexs-friends/61-latexs-friends-others/381-combining-latex-and-illustrator)).
Some pieces of code are taken from https://github.com/fabiantheblind/exec-term.

###Installation:
- Download the script (jsx file) and open it with any text editor.
- Change the following two lines:
```javascript
// the path to pdflatex
var pdflatexexe="/usr/texbin/pdflatex";
// the temp folder where scripts will be stored and executed (full path)
var temppath="";
```
- Move it to the following folder */Applications/Adobe Illustrator CS6/Presets.localized/en_US/Scripts* (note that the path might be different in your particular case).
- Run your Illustrator.
- The Script is accessible as *latex2illustrator* from *File -> Scripts* menu (unless you changed the name of the file).

###Usage:
- To run the script you need to have an Illustrator document already opened.
- After you run the script, enter LaTeX command normally, e.g. ``` $$\sin{x} + \frac{\cos{x}}{2}$$```.
- After you see the terminal compiling the script and closing, you will need to go back to Illustrator.
- [Here - stackexchange](http://graphicdesign.stackexchange.com/questions/63439/how-to-set-keyboard-shortcut-to-run-script-in-illustrator) you can find a discussion on how to assign a shortcut for a script using Automator
*Note: The script was tested on Illustrator CS6.*

###Future:
- Font size selector
