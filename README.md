# color-theme-x #

## Introduction ##

color-theme-x is an Emacs Lisp package that converts Emacs color
themes to X11 resource settings.  Applying color themes in this way
allows Emacs to start up significantly faster than by loading the
theme from Lisp code.

I forked color-theme-x from the file I found on the
[Emacs wiki](http://emacswiki.org/emacs/color-theme-x.el) because I
had some problems with getting it to work consistently.

## Installation ##

1. Place color-theme-x.el somewhere on your Emacs load path.
2. Add (require 'color-theme-x) to your .emacs

I'm working on making color-theme-x available in Marmalade.

## Usage ##

1. M-x color-theme-x RET <name> RET
2. This will create a buffer named \*color-theme-xresources\*.  Copy the
contents of that buffer to your ~/.Xresources file.
3. Run xrdb -merge ~/.Xresources


