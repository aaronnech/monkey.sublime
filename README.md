monkey.sublime
==============

This bundle lets you to use the multi-platform editor [Sublime Text](http://www.sublimetext.com) as an IDE for the [monkey programming language](http://www.monkeycoder.co.nz). It is based on [monkey.tmbundle](https://github.com/gingerbeardman/monkey.tmbundle).

## Features

**Auto Completion of Keywords**  
Press the Tab key to expand to the first match after typing part of a keyword, Option+Escape will present a list of matches for you to choose from

**Build Systems**  
Quick and easy build by pressing ⌘B, current build system can be set in the Tools menu

**Syntax Colouring**
...and more to come

## Mac OS X

### Installation

Unzip to "~/Library/Application Support/Sublime Text/Packages/".

Next, you will need to add your monkey/bin folder to your system wide path. This is currently a bit awkward but will hopefully become easier as Sublime Text continues to be improved.

### Path
You will first need to confirm your monkey/bin location is in your shell path:

    echo "export PATH=\$PATH:/user/folder/monkey/bin" >> ~/.profile

Next, add the shell path to the system-wide environment:

    defaults write ${HOME}/.MacOSX/environment PATH "${PATH}"

Alternatively, you can manually edit `~/.MacOSX/environment.plist` or use the  [RCEnvironment](http://www.rubicode.com/Software/RCEnvironment/) preference pane. Either way, the goal is to add your monkey/bin path to the PATH variable in your environment.

You will need to restart for the changes to take effect.

## Windows

Support for Microsoft Windows is present. You will need to add your monkey/bin folder to the system PATH.

## Linux

There is currently no Linux support as Monkey does not currently support it.

## Changelog

**2011-06-01**  
- added one build system per target, should default to HTML5 but may need specifying manually  

**2011-05-31**  
- updated language definition to the latest one from monkey.tmbundle (v40)  

**2011-05-19**  
- updated language definition to the latest one from monkey.tmbundle (v39)  

**2011-04-20**  
- added workaround for path issue  
- added installation notes  
- fixes for some broken snippets  
- added file_regex so errors can be located  

**2011-04-19**  
- added multiple command line parameters, thanks to Adam Woodall  

**2011-04-18**  
- added build system (path to trans needs to be hard coded - you will have to edit the Monkey.sublime-build file)  

**2011-04-08**  
- Initial release  

## To do

- support for tab [completions](http://sublimetext.info/docs/extensibility/completions.html)  
- support for context sensitive help through a [command](http://sublimetext.info/docs/extensibility/plugins.html#types-of-commands)  

