PocketSphinx 1.0.0
===============================================================================

This is PocketSphinx, one of Carnegie Mellon University's open source large
vocabulary, speaker-independent continuous speech recognition engines.

Although this was at one point a research system, active development
has largely ceased and it has become very, very far from the state of the art.

**Please see the LICENSE file for terms of use.**

Installation
------------------------------------------------------------------------------

We now use CMake for building, which should give reasonable results
across Linux, MacOS and Windows.  In addition, the audio library,
which never really built or worked correctly on any platform at all,
has simply been removed.

There is no longer any dependency on SphinxBase, because there is no
reason for SphinxBase to exist.  You can just link against the
PocketSphinx library, which now includes all of its functionality.

So you can do something like this:

```
mkdir build
cd build
cmake ..
make
make install
```

