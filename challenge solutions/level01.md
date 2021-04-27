# overthewire
 challenge submissions @ overthewire
 
## level goal: Find the password

The password for the next level is stored in a file called readme located in the home directory. 
Use this password to log into bandit1 using SSH. 
Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

### solution

1.`ls` showed the existance of a readme file
2.`cat readme` returned : `boJ9jbbUNNfktd78OOpsqOltutMc3MY1`
  
 to access next level
 
3.`ssh bandit1@bandit.labs.overthewire.org -p 2220`
4. password: `boJ9jbbUNNfktd78OOpsqOltutMc3MY1`
