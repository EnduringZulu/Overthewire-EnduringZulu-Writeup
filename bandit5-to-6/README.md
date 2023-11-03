# bandit5 -> bandit6<br/>
To do:<br/>
- human-readable
- 1033 bytes in size
- not executeable<br/><br/>
```bandit5@bandit:~$ ls```<br/>
```inhere```<br/>
```bandit5@bandit:~$ cd inhere/```<br/>
```bandit5@bandit:~/inhere$ ls```<br/>
```maybehere00  maybehere04  maybehere08  maybehere12  maybehere16```<br/>
```maybehere01  maybehere05  maybehere09  maybehere13  maybehere17```<br/>
```maybehere02  maybehere06  maybehere10  maybehere14  maybehere18```<br/>
```maybehere03  maybehere07  maybehere11  maybehere15  maybehere19```<br/>
```bandit5@bandit:~/inhere$ find -type f -size 1033c -not -executable```<br/>
```./maybehere07/.file2```<br/>
```bandit5@bandit:~/inhere$ cat ./maybehere07/.file2```<br/>
```P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU```<br/><br/>

The password for bandit6 is ```P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU``` .