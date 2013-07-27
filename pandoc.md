title: pandoc
tags: pandoc document-generation
date: 2013-07-24
-------------------

### [pandoc](http://johnmacfarlane.net/pandoc/)

usage: pandoc -o output-file input-file

It reads markdown (and probably others) and infers the output type based on the extension.

If you need to install it on Windows w/o Admin rights then remember you can extract the MSI using:

text

    msiexec /a pandoc-version.msi /qb TARGETDIR=somepath
