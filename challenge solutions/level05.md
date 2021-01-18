# overthewire
 challenge submissions @ overthewire
 
## level goal: Find the password

instructions mentioned the password was on stored on the only human-readable file

### solution

  `cd inhere`
  
  `ls` and `find` showed 9 different files in the form `-fileXX` (00-09)
  
  same as the level02 solution. - is difficult to deal with.
  `-cat ./-fileXX` read them. All messed with the terminal and had to use the `reset` command to continue exploring
  
  `-file07` contained the only readable password
  
  
  `cat ./file07` returned: `koReBOKuIDDepwhWk7jZC0RTdopnAYKh`
  
  password: `koReBOKuIDDepwhWk7jZC0RTdopnAYKh`


