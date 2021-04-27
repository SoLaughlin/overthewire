# overthewire
 challenge submissions @ overthewire
 
## level goal: Find the password

Stored in data.txt as a base 64 encoded string

### solution

`ls` # showed the data.txt file
`cat data.txt` # showed only one string. 
`cat data.txt | tr "[A-Za-Z]" "[N-ZM-An-zm-a]"` #takes all instances of A-Z and replaces then with 13 characters furthe rin the alphabet. A=N, b=o etc

`ssh bandit12@bandit.labs.overthewire.org -p 2220`
`5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu`




