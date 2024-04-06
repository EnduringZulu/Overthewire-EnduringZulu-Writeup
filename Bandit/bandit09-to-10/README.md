# bandit9 -> bandit10<br/>
To do:<br/>
<b>stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.</b><br/><br/>
```bandit9@bandit:~$``` ls<br/>
data.txt<br/>
```bandit9@bandit:~$``` strings data.txt <br/>
<b>you will find a lot of text, but there’s some line has “ ===== password“)</b><br/>
```bandit9@bandit:~$``` strings data.txt | grep '===='<br/>
x]T========== theG)"<br/>
========== passwordk^<br/>
========== is<br/>
========== G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s<br/>

The password for bandit10 is ```G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s``` .
