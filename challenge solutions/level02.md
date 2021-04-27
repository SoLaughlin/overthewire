# overthewire
 challenge submissions @ overthewire
 
## level goal: Find the password

The password for the next level is stored in a file called - located in the home directory

### solution



  1. `ls` showed the existance of - file
  
  2. however when using :`cat -` nothing was returned
  this is because - is common syntax for a stdin file and the `cat` command recognises it as such
  for why I used this [https://unix.stackexchange.com/questions/16357/usage-of-dash-in-place-of-a-filename:]
  
  3. to get around this I prefixed the filename with a path
  `cat .\-` returned : `CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9`
  
  4.`ssh bandit2@bandit.labs.overthewire.org -p 2220`
  5. password: `CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9`
