# overthewire
 challenge submissions @ overthewire
 
## level goal: Access level 2 by finding the password and use this password to log into bandit2

instructions mentioned the password was on a file named -.

  `ls` showed the existance of - file
  
  however when using :`cat -` nothing was returned
  this is because - is common syntax for a stdin file and the `cat` command recognises it as such
  
  to get around this I prefixed the filename with a path
  `cat .\-` returned : `CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9`
  
  password : `CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9`
