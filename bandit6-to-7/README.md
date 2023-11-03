# bandit6 -> bandit7<br/>
To do:<br/><br/>
- owned by user bandit7
- owned by group bandit6
- 33 bytes in size
```bandit6@bandit:~$ ls```<br/>
```bandit6@bandit:~$ cd ..```<br/>
```bandit6@bandit:/home$ cd ..```<br/>
```bandit6@bandit:/$ find 2>/dev/null -user bandit7 -group bandit6 -size 33c``` <br/>
```./var/lib/dpkg/info/bandit7.password```<br/>
(<b>2>/dev/null</b> for skip permission denied)<br/>
Ref:https://stackoverflow.com/questions/762348/how-can-i-exclude-all-permission-denied-messages-from-find <br/>
```bandit6@bandit:/$ cat ./var/lib/dpkg/info/bandit7.password```<br/>
```z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S```<br/><br/>

The password for bandit7 is ```z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S``` .