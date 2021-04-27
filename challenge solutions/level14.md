# overthewire
 challenge submissions @ overthewire
 
## level goal: Find the password

The password for the next level is stored in /etc/bandit_pass/bandit14 
and can only be read by user bandit14. For this level, you don’t get the next password, 
but you get a private SSH key that can be used to log into the next level. 
Note: localhost is a hostname that refers to the machine you are working on

### solution

`ls` # showed the ssh.private key
I copied the key into a text file on my system
`man ssh` # showed an -i key for an identity file. ssh -i filename target
`ssh -i ssh.private bandit14@bandit.labs.overthewire.org -p 2220`
`cd /etc/bandit_pass`
`cat bandit14` #showed password

host:`ssh bandit14@bandit.labs.overthewire.org -p 2220`
password: `4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e`




