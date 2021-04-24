# overthewire
 challenge submissions @ overthewire
 
## level goal: Find the password

instructions mentioned the password filled 3 conditions and was on the server not the directory:
owned by user bandit7
owned by group bandit6
33 bytes in size


### solution

`cd /` # took me to the root
`find -user bandit7 -group bandit6 -size 33c` #showed me a file named that


`cat "that file"` returned `HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs`



