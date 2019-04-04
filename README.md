# 6502-disassembler
A simple 6502 disassembler made in Python

Only supports the mos official opcodes

~~~
./disassembler.py -h
usage: disassembler.py [-h] -i <input file> [-o <output file>]
                       [-a <start address>]

6502 disassembler in python by Arthur Ferreira

optional arguments:
  -h, --help          show this help message and exit
  -i <input file>     the 6502 binary file to disassemble
  -o <output file>    stdout if not specified
  -a <start address>  in Hexadecimal (FF00 for example)
~~~
example :

~~~
/disassembler -a ff00 -i wozmon.rom 
0000    CLD
0001    CLI
0003    LDY #$7F
0006    STY $D012
0008    LDA #$A7
000B    STA $D011
000E    STA $D013
...
~~~
