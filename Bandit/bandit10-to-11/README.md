# bandit10 -> bandit11<br/>
To do:<br/><br/>
```bandit10@bandit:~$``` ls<br/>
data.txt<br/>
```bandit10@bandit:~$``` base64 --help<br/>
Usage: base64 [OPTION]... [FILE]<br/>
Base64 encode or decode FILE, or standard input, to standard output.<br/>

With no FILE, or when FILE is -, read standard input.<br/>

Mandatory arguments to long options are mandatory for short options too.<br/>
  -d, --decode          decode data<br/>
  -i, --ignore-garbage  when decoding, ignore non-alphabet characters<br/>
  -w, --wrap=COLS       wrap encoded lines after COLS character (default 76).<br/>
                          Use 0 to disable line wrapping<br/>
      --help     display this help and exit<br/>
      --version  output version information and exit<br/>

The data are encoded as described for the base64 alphabet in RFC 4648.<br/>
When decoding, the input may contain newlines in addition to the bytes of<br/>
the formal base64 alphabet.  Use --ignore-garbage to attempt to recover<br/>
from any other non-alphabet bytes in the encoded stream.<br/>

GNU coreutils online help: <https://www.gnu.org/software/coreutils/><br/>
Full documentation <https://www.gnu.org/software/coreutils/base64><br/>
or available locally via: info '(coreutils) base64 invocation'<br/>

```bandit10@bandit:~$``` cat data.txt | base64 -d<br/>
The password is 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM<br/>

The password for bandit11 is ```6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM``` .<br/>
