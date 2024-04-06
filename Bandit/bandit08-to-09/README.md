# bandit8 -> bandit9<br/>
To do: <br/>
stored in the file data.txt and is the only line of text that occurs only once<br/>
( using uniq ref: https://saixiii.com/uniq-linux-command/ )<br/><br/>
```bandit8@bandit:~$ ls```<br/>
```data.txt```<br/>
```bandit8@bandit:~$ sort data.txt | uniq -c | grep '1 ' ```<br/>
```      1 EN632PlfYiZbn3PhVK3XOGSlNInNE00t```<br/>
( “ sort ” for sorting first , “ uniq -c “ for counting the duplicate , “ grep ” for finding )<br/>



The password for bandit9 is ```EN632PlfYiZbn3PhVK3XOGSlNInNE00t``` .