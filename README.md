# cia-adventure
[qb64](https://github.com/QB64Official/qb64) port of Hugh Lampert's CIA Adventure, a 1980 interactive fiction title fort the TRS-80

## What is this?
This is a quick-n-dirty forward port of an "interactive fiction" game (that is, a text adventure) written in 1980 for TRS-80 Level II BASIC (an early Microsoft BASIC) to the modern QB64 compiler. Essentially, I did just enough work to make the syntax errors go away and compilation succeed.

Back in the extremely early 80s, probably 1980 or 1981, I had a cassette of "CIA Adventure" for the TRS-80 Model I — at the time we bought the computer, the thing was just called "a TRS-80", and the "Model I" thing was a retronym when other models came into existence — and since I was a little kid I had no idea how the hell to play this game. I mean, I'd played text adventures before but this game stumped me. I wasn't willing to cheat and read the program's code, so I just never finished it.

## What's here?

Runnable game binaries are at the [Releases page](https://github.com/majick/cia-adventure/releases)

The ported source is in: `cia-port.bas`.  As is customary for the modern era, the `.bas` file is source code. 

In `orig/ciaadvn8.txt` is the source from which the port was made. It was detokenized from `orig/variants/tokenized/ciaadvn8.bas`

In `orig/variants/tokenized` are the various original versions of the CIA Adventure game, as tokenized BASIC files for Level II BASIC. As is customary for the platform, ".bas" files are tokenized BASIC; that's because these are actually `/BAS` files as represented on the TRSDOS filesystem.

In `orig/variants/src` are detokenized ("source") versions of the same. They were detokenized using [trs80-tool](https://www.my-trs-80.com/tool/).

`model100/` contains the port to the TRS-80 Model 100 (and Tandy 102), with source and tokenized BASIC provided. I only did cursory testing of my porting work, which mostly consisted of fixing `IF` statements to include `THEN` statements (much like I had to do for the qb64 port) and some stuff for making the ORDERS display fit on the smaller screen.

[![No Maintenance Intended](http://unmaintained.tech/badge.svg)](http://unmaintained.tech/)
