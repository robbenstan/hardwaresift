hardwaresift
============

Class project to propose an architecture for enhancing or implementing the SIFT algorithm

Compilation notes
=================
for vlfeat:
make DEBUG=1 DISABLE_THREADS=yes DISABLE_SSE2=yes
for siftpp:
edit Makefile to
CXXFLAGS           += -I. -Wall -g -p -O0 -DNDEBUG

Testing notes
================
gdb --args ./g64/sift --verbose -O 3 -S 3 --first-octave 0 ../hardwaresift/canonical.pgm
gdb -tui --args ./g64/sift --verbose -O 3 -S 3 --first-octave 0 ../hardwaresift/canonical.pgm
layout split
