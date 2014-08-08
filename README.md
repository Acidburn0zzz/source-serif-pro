# Source Serif Pro

Source Serif Pro is a set of OpenType fonts to complement the [Source Sans Pro](https://github.com/adobe-fonts/source-sans-pro) family. 
In addition to a functional OpenType font, this open source project provides all of the source files that were used to build this OpenType font by using the AFDKO makeotf tool.

## Download font binaries (OTF, TTF, WOFF, EOT and SVG files)

The font binaries are available in the [release branch](../../tree/release).
They can also be downloaded from [SourceForge](https://sourceforge.net/projects/sourceserifpro.adobe/files/).

## Installation instructions

* [Mac OS X](http://support.apple.com/kb/HT2509)
* [Windows](http://windows.microsoft.com/en-us/windows-vista/install-or-uninstall-fonts)
* [Linux/Unix-based systems](https://github.com/adobe-fonts/source-code-pro/issues/17#issuecomment-8967116)

## Building from source

### Requirements

To build the binary font files from source, you need to have installed the
[Adobe Font Development Kit for OpenType](http://www.adobe.com/devnet/opentype/afdko.html) (AFDKO). The AFDKO
tools are widely used for font development today, and are part of most font
editor applications.

### Building one font

The key to building OTF or TTF fonts is `makeotf`, which is part of the AFDKO toolset.  
Information and usage instructions can be found by executing `makeotf -h`.

In this repository, all necessary files are in place for building the OTF and TTF fonts.  
For example, build a binary OTF font for the Regular style like this:

```sh
$ cd Roman/Regular/
$ makeotf -r
```

### Building all fonts

For convenience, a shell script named `build.sh` is provided in the root directory.  
It builds all OTFs and TTFs, and can be executed by typing:

```sh
$ ./build.sh
```

## Getting Involved

Send suggestions for changes to the Source Serif OpenType font project maintainer, [Frank Grießhammer](mailto:opensourcefonts@adobe.com?subject=[GitHub] Source Serif Pro), for consideration.

## Further information

For information about the design and background of Source Serif, please refer to the [official font readme file](http://htmlpreview.github.io/?https://github.com/adobe-fonts/source-serif-pro/blob/master/SourceSerifProReadMe.html).
