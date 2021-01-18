# overthewire
 challenge submissions @ overthewire
 
## level goal: Find the password

instructions mentioned the password filled 3 conditions:
only human-readable file
non excecutable file
1033 bytes in size



### solution

`cd inhere` #found 20 directories
`find` # showed they all had multiple files


`find -size 1033c` #by searching for the findutils documentation I found that I could search by size.
only one file of exactly 1033 bytes existed in `maybehere07`

`cat .file2` returned `DXjZPULLxYr17uwoI01bNLQbtFemEgo7` #plus whitespace

I lucked out here in finding the -size operator to give me the exact one solution.

I may come back to this solution to learn more, anything I figure out will be under the other solutions header

#### other solutions