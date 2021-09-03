# CoCo3Loader
A machine code loader that let's you load and run your ML program anywhere in memory including where the BASIC loader is in memory

The zip file has everything you need to use the tool.  If you're on an x86 Mac you can use the programs as is.  If not you will have to compile the CC3SLZX0V2.3.BAS program with QB64 and you will also need the zx0 file compiled from Einar Saukas, https://github.com/einar-saukas/ZX0


Once you have the CC3SLZX0V2.3 file compiled and the zx0 file compiled and in the same directory use the ./CC3SLZX0V2.3 on your CoCo 3 binary program.

Here's a summary of how to use the program (from the BASIC code):

PRINT "cc3slzx0 - CoCo 3 Super Loader using zx0 compression v2.0 by Glen Hewlett"
PRINT
PRINT "Usage: cc3slzx0 FILENAME.BIN [-oOUTNAME.BIN] [-q] [-b] [-h] [-v] [*.scn or *.csv]"
PRINT
PRINT "Summary: Turns a CoCo 3 Machine Language program into a compressed version and is loadable even if it over writes BASIC ROM locations"
PRINT "Gets rid of limitations of where in the 512k or 2Meg of RAM you want your program to be in memory"
PRINT
PRINT "Where:"
PRINT "FILENAME.BIN   is the name of your big CoCo 3 program, it must end with .BIN"
PRINT "-oOUTNAME.BIN  is the name of the output file to be created otherwise it defaults to GO.BIN"
PRINT
PRINT "-q     Uses quick ZX0 compression, which is faster but doesn't compress as well as not using this option which then uses the default full ZX0 compression"
PRINT "-b     Blank all 16 palette slots to zero after the program loads to hide any weird screens being shown before your program has started"
PRINT "-h     This quick help screen"
PRINT "-vx    Amount of info to display while generating the new file x can be 0 1 or 2.  Default x=0 where no extra info is shown"
PRINT
PRINT "*.scn  A binary file that must end with .scn will be shown on the CoCo 3 text screen while loading"
PRINT "*.csv  A csv text files that must end with .csv will be shown on the CoCo 3 text screen while loading"
PRINT "       You can only use one .scn or one .csv file."
PRINT
