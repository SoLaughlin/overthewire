# overthewire
 challenge submissions @ overthewire
 
## level goal: Find the password

Stored in data.txt beside only few human readable lines, preceded by several '='

### solution

`ls` # showed the data.txt file
`strings data.txt | grep "==="` # shows strings and searches those strings for multiple =

`ssh bandit10@bandit.labs.overthewire.org -p 2220`
`truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk`




