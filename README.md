# tex-ruledpaper

This system employs LuaTeX to produce lined paper, which may be used as-is or as a template to write on blank paper. Page size, margins, the different rules' thickness and line spacing might be configured.

Both DVI and PDF might be produced, the former being used to in turn generate printable PostScript.


##  Usage

The Tup build system manages the process, which comprises two steps: configuration and build.

###  Configuration
Parameters are specified in the usual way, in a `tup.config` file. You might be interested in using variants.

Examples are provided in the [configs.tup](configs.tup) directory. It should be possible to proceed to the build step by just copying any of them to the root as `tup.config`.

###  Build
The build step follows the standard procedure:

    $  tup

####  Requirements

 -  the [Tup build system](http://gittup.org/tup/)
 -  a LuaTeX engine
 -  if going the DVI route, [dvips](http://tug.org/texinfohtml/dvips.html) to generate printable PostScript
