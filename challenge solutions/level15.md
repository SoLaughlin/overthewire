# overthewire
 challenge submissions @ overthewire
 
## level goal: Find the password

The password for the next level can be retrieved by submitting the password of the current level
to port 30000 on localhost.

### solution

`nc localhost 30000` attempted to use netcat to connect. Didn't recieve any text so thought nc didn't work.
`tellnet localhost 30000` # returned connected to local host...
`4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e` #entered the password from bandit14
//output
Correct!
BfMYroe26WYalil77FoDi9qh59eK5xNr

I returned to the `nc localhost 30000` and checked that if I entered the password I got the flag. I did


host:`ssh bandit14@bandit.labs.overthewire.org -p 2220`
password: `BfMYroe26WYalil77FoDi9qh59eK5xNr`




