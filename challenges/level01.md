# overthewire
 challenge submissions @ overthewire
 
## level goal: Access level 1 by finding the password and use this password to log into bandit1

instructions mentioned the password was on a readme file.

  `ls` showed the existance of a readme file
  `cat readme` returned : `boJ9jbbUNNfktd78OOpsqOltutMc3MY1`
  
  to access next level 
  `$ ssh bandit1@bandit.labs.overthewire.org -p 2220`
  username: `bandit1`
  password: `boJ9jbbUNNfktd78OOpsqOltutMc3MY1`
