ALBOW - A Little Bit of Widgetry for PyGame
-------------------------------------------


CHANGES MADE BY D.C.-G.
-------------------------

This version of ALBOW is a twisted one.
CodeWarrior0 modified it for its own purpose in MCEdit and I also
tweaked it for translation purposes.

See 'ORIGINAL README' for , eh, original readme...

Basically, this modification adds a new module to localise the texts
in the
widgets.

It looks for locale files in a sub folder 'lang' according to the
system (sys.getlocale) default, or user specified locale.

The locale files are text files where 'entries' are defined.


Syntax example
--------------

o0 This is the first entry.
t0 Ceci est la première entrée.
o1 Here is the second one.
You can see it is splitted on two lines.
t1 Voici la deuxième.
Vous pouvez constater qu'elle est sur deux lignes.

The 'oN' markers on the begining of a line marks the original string;
the 'tN', the translations.
Strings can be splited on several lines and contain any sort of
haracters (thus, be aware of unicode).

Files are named according to their language name, e.g. fr_FR.trn for
french.
The extension .trn is an arbitrary convention.
The file 'template.trn' is given to be used as a base for other ones.
It contains the strings used in Albow; they are not translated.


Remarkable stuff
----------------

* 'oN' and 'tN' markers *must* be followed with a space.
* Every character in the original an translated strings will be
  preserved, even white spaces.
* .trn files should be encoded with utf-8 no BOM encoding (Notepad++
  does it very well).
* As a convention, english is considered as the default language, and
  the file en_EN.trn would never be present.


ORIGINAL README
---------------

Version 1.1

This is a rather basic, no-frills widget set for creating a GUI using
PyGame. It has been developed over the course of my last three
PyWeek competition entries.

Contents
--------

albow       Package containing the Python modules. Put it
            on your PYTHONPATH or in the top level directory
            of your PyGame application.
            
demo.py     A demonstration of most of Albow's functionality.
            Run it using
            
                 pythonw albow.py

doc         Documentation in html format. Start with index.html.

Resources   Some resources used by demo.py. Also contains some
            default fonts (Vera.ttf and VeraBd.ttf) that you can
            use in your applications if you wish.

License
-------

This is free software. You may use it, redistribute it and create and
distribute derivative works from it without restriction.

The Bitstream Vera fonts in the Resources/fonts directory are covered
by their own (very liberal) license, a copy of which is included in
that directory.

Author
------

Gregory Ewing
greg.ewing@canterbury.ac.nz
