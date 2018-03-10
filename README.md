Anaconda Build Packages for gexiv2
==================================

Patrick Wagstrom &lt;patrick@wagstrom.net&gt;

April 2017

Did you have a simple task that you started on that somehow got _way_ out of
control? That's the story here. I had a bunch of daycare photos that I wanted
to auotmatically download, automatically crop out white borders, add GPS tags,
and set various EXIF tags such as description and date. Oh yeah, and I wanted
to do it using Python 3, because it's 2017 and no one should be usig Python 2
for new projects anymore. Unfortuately, this led me down the rabbit hole of
unmaintained projects that don't work with Python 3 because they either have
`print` statements, use old library names like `urllib2` or other simple
errors. While some of these have been ported or modified, such a
[pillow][pillow] as a replacement for the relatively unmaintained [Python
Imaging Library (PIL)][pil]. Others were much harder to work with, like
IPTCInfo.

On the plus side, I know that gexiv2 works. So, let's make this work nicely
with Anaconda, because it's a good way to make sure that you understand the
dependencies.

Thus, the journe down the rabbit hole began.

Pre-requisties
--------------

This package requires my [exiv2][exiv2-conda] package for Conda. So, get that first, follow the instructions there, then install this package.

Usage
-----

    conda build .
    conda install gexiv2 --use-local


License
-------

This code is licensed under the MIT license. The code for exiv2 is licensed under the GPLv2 or later.

[exiv2]: https://github.com/pridkett/exiv2-conda
[pil]:
[pillow]: