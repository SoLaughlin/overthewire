# overthewire
 challenge submissions @ overthewire
 
## level goal: Find the password

The credentials for the next level can be retrieved by submitting the password of the current level to a port on localhost in the range 31000 to 32000. First find out which of these ports have a server listening on them. 
Then find out which of those speak SSL and which don’t. 
There is only 1 server that will give the next credentials, the others will simply send back to you whatever you send to it.

### solution

`nmap localhost -p31000-32000` #showed 5 open ports but with no information on the services
`nmap -sV localhost -p31000-32000`#gave more information on each of the services. Two had SSL, one ssl/echo, one ssl/unknown
ports of interest: 
31518 ssl/echo
31790 ssl/unkown #personal note to come back and check if I can get more information on the services

I'll try the ssl/echo first although I suspect it will just echo back whatever I send it.

`openssl`
OpenSSL> s_client localhost:31518 -servername localhost  #realised servername was redundant after this
myinput: cluFn7wTiGryunymYOu4RcffSxQluehd
output: cluFn7wTiGryunymYOu4RcffSxQluehd

as expected, tried the other port.


OpenSSL> s_client -connect localhost:31790
myinput: cluFn7wTiGryunymYOu4RcffSxQluehd
output: an RSA private key. Copied the contents to ssh.private

after trying to use ssh.private using 

`ssh -i ssh.private bandit16@bandit.labs.overthewire.org -p 2220`
the file had bad permissions. Forgot to make it read only
`chmod 400 ssh.private`
`ssh -i ssh.private bandit17@bandit.labs.overthewire.org -p 2220`
success!
`cd /etc/bandit_pass`
`cat bandit17`





host:`ssh bandit16@bandit.labs.overthewire.org -p 2220`
password: `xLYVMN9WE5zQ5vHacb0sZEVqbrp7nBTn`




