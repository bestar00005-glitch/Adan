tools from the x11-repo repository
~ $ a2ping
Attempt to call undefined import method with arguments ("1") via package "just" (Perhaps you forgot to load the package?) at /data/data/com.termux/files/usr/bin/texlive/a2ping line 349.
a2ping.pl 2.84p, 2019-11-17 -- Written by <pts@fazekas.hu> from April 2003.
This is free software, GNU GPL >=2.0. There is NO WARRANTY.
(epstopdf 2.7 Copyright 1998-2001 by Sebastian Rahtz et al.)

Usage:  a2ping.pl [options] <inputfile> [[<outformat>:] <outputfile>]
Run with --doc to read documentation as a UNIX man(1) page.
Options: --help print this help message
--(no)compress  use compression                   (def: best)
--(no)hires     scan HiResBoundingBox             (def: yes)
--(no)exact     scan ExactBoundingBox             (def: no)
--(no)verbose   verbose debug informations        (def: no)
--(no)below     allow below+left_from baseline    (def: no)
--(no)tmpunlink unlink temporary files            (def: yes)
--(no)antialias render shades at outlines (def: scale3no) (=scale3yes =no =yes)
--(no)lossy     allow lossy image filters (EPS->PDF) (def: yes)
--(no)keepoldmediabox keep only old, [0 0]-based MediaBox in PDF (def: no)
--gs-cmd=       path to Ghostscript               (def: gs or gswin32c)
--gs-ccmd=      path to Ghostscript, 4 bbox calc  (def: gs or gswin32c)
--gsextra=      extra arg to gs
--extra=        extra arg to external prg (i.e pdftops)
--bboxfrom=     adsc|compute-gs|pagesize          (def: guess)
--papersize=    unchanged|force-unknown|600bpx5cm (def: default) (bp)
--threshold=    min color for 1 in 8->1 bit conv  (def: 128)
Possible input formats: PS EPS PDF JPEG GIF TIFF PNG PNM PCX BMP LBM XPM TGA
Possible output formats: BMP EPS GIF JPEG PBM PCL5 PDF PDF1 PGM PNG PPM PS TIFF XPM XWD markedEPS markedPS
Examples for producing 'test.pdf':
  * a2ping.pl test.eps
  * produce postscript | a2ping.pl -v - test.pdf
Example: look for HiResBoundingBox and produce corrected PostScript:
  * a2ping.pl -d --nogs -hires test.ps>testcorr.ps
~ $ a2ping.pl
