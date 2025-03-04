was provided with zip which was extracted to find sam.jpg <br>
(tried many things binwalk, exif, stegsolve etc.)<br>
extracting strings we get some Brainfuck code as the bottom, put it into a compiler and you get a drive link. <br>
you get a 'data' ;) file. see its hexdump and you will notice adjacent bytes are swapped. use ```dd if=corrupt.jpg of=fixed.jpg bs=2 conv=swab``` to correct it and you will end up with the final jpg containing the flag.<br>
drive link: ```https://drive.google.com/file/d/1JWqdBJzgQhLUI-xLTwLCWwYi2Ydk4W6-/view?usp=sharing```
