# bandit11 -> bandit12<br/>
To do:<br/>
<b>stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions</b> <br/>Ref: https://medium.com/@piyush.kochhar1/rot13-a-missing-guide-c811427cfe6e <br/>

```bandit11@bandit:~$ ls```<br/>
```data.txt```<br/>
```bandit11@bandit:~$ cat data.txt ```<br/>
```Gur cnffjbeq vf WIAOOSFzMjXXBC0KoSKBbJ8puQm5lIEi```<br/>
```bandit11@bandit:~$ echo Gur cnffjbeq vf WIAOOSFzMjXXBC0KoSKBbJ8puQm5lIEi | tr [A-M][N-Z] [N-Z][A-M] | tr [a-m][n-z] [n-z][a-m]```<br/>
```The password is JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv```<br/>

The password for bandit12 is ```JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv``` .<br/>
