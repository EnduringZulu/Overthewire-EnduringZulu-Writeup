Natas Level 6 → Level 7

Username: natas7
URL:      http://natas7.natas.labs.overthewire.org

Right Click -> Inspect
![alt text](image.png)
hint: password for webuser natas8 is in /etc/natas_webpass/natas8 -->

Go to "Home" page
![alt text]This website uses PHP which is directed to index.php?page=home</code><br>
It's like directory home<br>
![alt text](image-2.png)

Change from <code>index.php?page=home</code> to <code>index.php?page=/etc/natas_webpass/natas8</code> for that directory path(from hints).
![alt text](image-3.png)

Finished!!!
![alt text](image-4.png)
a6bZCNYwdKqN5cGP11ZdtPg0iImQQhAB 