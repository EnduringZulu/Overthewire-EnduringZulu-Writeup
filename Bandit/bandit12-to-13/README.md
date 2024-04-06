Bandit Level 12 → Level 13
Level Goal

The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)

<code>bandit12@bandit:~$</code> ls<br>
data.txt<br>
<code>bandit12@bandit:~$</code> pwd<br>
/home/bandit12<br>
<code>bandit12@bandit:~$</code> mkdir /tmp/babe123<br>
<code>bandit12@bandit:~$</code> cp data.txt /tmp/babe123<br>
<code>bandit12@bandit:~$</code> cd /tmp/babe123<br>
<code>bandit12@bandit:/tmp/babe123$</code> mv data.txt babe<br>
<code>bandit12@bandit:/tmp/babe123$</code> xxd -r babe > babe2<br>
<code>bandit12@bandit:/tmp/babe123$</code> file babe2<br>
babe2: gzip compressed data, was "data2.bin", last modified: Thu Oct  5 06:19:20 2023, max compression, from Unix, original size modulo 2^32 573<br>
<code>bandit12@bandit:/tmp/babe123$</code> mv babe2 babe2.gz<br>
<code>bandit12@bandit:/tmp/babe123$</code> gzip -d babe2.gz<br>
<code>bandit12@bandit:/tmp/babe123$</code> file babe2<br>
babe2: bzip2 compressed data, block size = 900k<br>
<code>bandit12@bandit:/tmp/babe123$</code> mv babe2 babe2.bz2<br>
<code>bandit12@bandit:/tmp/babe123$</code> ls<br>
babe  babe2.bz2<br>
<code>bandit12@bandit:/tmp/babe123$</code> bzip2 -d babe2.bz2<br>
<code>bandit12@bandit:/tmp/babe123$</code> ls<br>
babe  babe2<br>
<code>bandit12@bandit:/tmp/babe123$</code> file babe2<br>
babe2: gzip compressed data, was "data4.bin", last modified: Thu Oct  5 06:19:20 2023, max compression, from Unix, original size modulo 2^32 20480<br>
<code>bandit12@bandit:/tmp/babe123$</code> mv babe2 babe2.gz<br>
<code>bandit12@bandit:/tmp/babe123$</code> gzip -d babe2.gz<br>
<code>bandit12@bandit:/tmp/babe123$</code> ls<br>
babe  babe2<br>
<code>bandit12@bandit:/tmp/babe123$</code> file babe2<br>
babe2: POSIX tar archive (GNU)<br>
<code>bandit12@bandit:/tmp/babe123$</code> mv babe2 babe2.tar<br>
<code>bandit12@bandit:/tmp/babe123$</code> tar -xvf babe2.tar<br>
data5.bin<br>
<code>bandit12@bandit:/tmp/babe123$</code> file data5.bin<br>
data5.bin: POSIX tar archive (GNU)<br>
<code>bandit12@bandit:/tmp/babe123$</code> mv data5.bin data5.tar<br>
<code>bandit12@bandit:/tmp/babe123$</code> tar -xvf data5.tar<br>
data6.bin<br>
<code>bandit12@bandit:/tmp/babe123$</code> file data6.bin<br>
data6.bin: bzip2 compressed data, block size = 900k<br>
<code>bandit12@bandit:/tmp/babe123$</code> mv data6.bin data6.bz2<br>
<code>bandit12@bandit:/tmp/babe123$</code> bzip2 -d data6.bz2<br>
<code>bandit12@bandit:/tmp/babe123$</code> ls<br>
babe  babe2.tar  data5.tar  data6<br>
<code>bandit12@bandit:/tmp/babe123$</code> file data6<br>
data6: POSIX tar archive (GNU)<br>
<code>bandit12@bandit:/tmp/babe123$</code> mv data6 data6.tar<br>
<code>bandit12@bandit:/tmp/babe123$</code> tar -xvf data6.tar<br>
data8.bin<br>
<code>bandit12@bandit:/tmp/babe123$</code> file data8.bin<br>
data8.bin: gzip compressed data, was "data9.bin", last modified: Thu Oct  5 06:19:20 2023, max compression, from Unix, original size modulo 2^32 49<br>
<code>bandit12@bandit:/tmp/babe123$</code> mv data8.bin data8.gz<br>
<code>bandit12@bandit:/tmp/babe123$</code> gzip -d data8.gz<br>
<code>bandit12@bandit:/tmp/babe123$</code> ls<br>
babe  babe2.tar  data5.tar  data6.tar  data8<br>
<code>bandit12@bandit:/tmp/babe123$</code> file data8<br>
data8: ASCII text<br>
<code>bandit12@bandit:/tmp/babe123$</code> cat data8<br>
The password is wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw<br>

<br><b>PAIN...</b>