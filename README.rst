======
pyttsx
======

Cross-platform Python wrapper for text-to-speech synthesis

This specific fork has been created to allow the the TTS data to be optionally saved to disk as a WAV file.

If other file formats are required, additional libraries or executables (such as LAME or FFMPEG) can be used for format conversion and are outside the scope of this library.

Status
===========

At this point in time, file output works for Windows. Linux is coming soon, while unfortunately OSX will take some time without another contributor.


Quickstart
==========

::

   import pyttsx
   engine = pyttsx.init()
   engine.say('Greetings!')
   engine.say('How are you today?')
   engine.runAndWait()

See http://pyttsx.readthedocs.org/ for documentation of the full API.

Included drivers
================

* nsss - NSSpeechSynthesizer on Mac OS X 10.5 and higher
* sapi5 - SAPI5 on Windows XP, Windows Vista, and (untested) Windows 7
* espeak - eSpeak on any distro / platform that can host the shared library (e.g., Ubuntu / Fedora Linux)

Contributing drivers
====================

Email the author if you have wrapped or are interested in wrapping another text-to-speech engine for use with pyttsx.

Project links
=============

* Python Package Index for downloads (http://pypi.python.org/pyttsx)
* GitHub site for source, bugs, and q&a (https://github.com/parente/pyttsx)
* ReadTheDocs for docs (http://pyttsx.readthedocs.org)

See Also
========

https://github.com/parente/espeakbox - espeak in a 16.5 MB Docker container with a simple REST API

License
=======

Copyright (c) 2009, 2013 Peter Parente
All rights reserved.

http://creativecommons.org/licenses/BSD/
