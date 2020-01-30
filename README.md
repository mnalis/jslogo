jslogo - Logo in JavaScript modified to resemble FMS-Logo
=========================================================

This forked version is modified so it more closely emulate
[FMSLogo](http://fmslogo.sourceforge.net/) sometimes used to tech kids programming, 
which is [not yet able to run on GNU/Linux](https://sourceforge.net/p/fmslogo/feature-requests/1/)

FMSLogo-alike forked version is hosted at https://mnalis.com/skola/jslogo-fms/ for playing with live.
See [TODO](TODO-FMSLogo.txt) for more information. For now, you need to click on "Examples" and run 
"FMSLogo compatibility initialisation" example to get FMSLogo compatibility.

[Language Reference](https://htmlpreview.github.com/?https://github.com/mnalis/jslogo-fms/blob/master/language.html) -
this attempts to implement a subset of [UCBLogo](https://www.cs.berkeley.edu/~bh/v2ch14/manual.html)
defined in in *Brian Harvey's Computer Science Logo Style*

Logo Examples
-------------
    to star repeat 5 [ fd 100 rt 144 ] end
    star
    to square :length repeat 4 [ fd :length rt 90 ] end
    repeat 36 [ square 50 rt 10 ]
    to randomcolor setcolor pick [ red orange yellow green blue violet ] end
    repeat 36 [ randomcolor square random 200 rt 10 ]
    window pu repeat 72 [ setlabelheight repcount fd repcount * 2.5 label "Logo bk repcount * 2.5 rt 10 ]

Logo Links
----------
* [Logo](https://en.wikipedia.org/wiki/Logo_%28programming_language%29) on Wikipedia
* Other Logo implementations that run in a Web browser:
  * [papert - logo in your browser](http://logo.twentygototen.org/) ([source code](https://code.google.com/p/papert/))
  * [Curly Logo](https://github.com/drj11/curlylogo)
* [The Logo Foundation](http://el.media.mit.edu/logo-foundation/)
* [Berkeley Logo (UCBLogo)](https://www.cs.berkeley.edu/~bh/logo.html)
* [The Logo Tree Project](http://elica.net/download/papers/LogoTreeProject.pdf)
* [Ian Bicking on Logo](http://blog.ianbicking.org/2007/10/19/logo/)
* [PyLogo](http://pylogo.sourceforge.net/)
* [Introduction to Computer Programming](http://www.bfoit.org/itp/itp.html)

To Do
-----
* Document deviations from FMS Logo implementation (and try to implement most often used features and document in language.html!)
* Document deviations from UCB Logo standard
* Make these examples all work: [Logo 15-word challenge](http://www.mathcats.com/gallery/15wordcontest.html)
* Tail-call optimization
* Make execution async so you can watch the turtle move
