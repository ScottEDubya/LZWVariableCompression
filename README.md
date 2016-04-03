# LZWVariableCompression
LZW algorithm for creating a code table that grows from 9-16 bits

Opens a file, then using the more space friendly version of LZW, it saves 9 bit numbers until the table fills, then it saves 10 bit numbers... etc.
once the 16 bit table is filled, the table will stop growing. 

To compress:
arg[2]: c arg[3]: filetocompress

To decompress:
arg[2]: e arg[3]: filetodecompress

file.txt will become file.txt.lzw when compressed,
when decompressed, it will become 2file.txt. 
