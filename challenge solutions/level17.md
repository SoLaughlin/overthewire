# overthewire
 challenge submissions @ overthewire
 
## level goal: Find the password

The password for the next level can be retrieved by submitting the password of the current level to port 30001 on 
localhost using SSL encryption.

### solution

`openssl`
OpenSSL> `s_client -connect localhost:30001 -servername localhost`
Got a tonne of returned information on the server outputted to the screen.
tried entering the password from bandit15
Correct!
cluFn7wTiGryunymYOu4RcffSxQluehd


host:`ssh bandit14@bandit.labs.overthewire.org -p 2220`
password: `cluFn7wTiGryunymYOu4RcffSxQluehd`




