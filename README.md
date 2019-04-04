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

###example :

~~~
./disassembler.py -i wozmon.rom -a ff00
FF00    D8         CLD
FF01    58         CLI
FF02    A0 7F      LDY #$7F
FF04    8C 12D0    STY $D012
FF07    A9 A7      LDA #$A7
FF09    8D 11D0    STA $D011
FF0C    8D 13D0    STA $D013
FF0F    C9 DF      CMP #$DF
FF11    F0 13      BEQ $13
FF13    C9 9B      CMP #$9B
FF15    F0 03      BEQ $03
...
~~~
