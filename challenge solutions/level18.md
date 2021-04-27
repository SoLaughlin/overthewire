# overthewire
 challenge submissions @ overthewire
 
## level goal: Find the password

There are 2 files in the homedirectory: passwords.old and passwords.new. 
The password for the next level is in passwords.new and is the only line that has been changed between passwords.old 
and passwords.new

### solution

`ls` passwords.old passwords.new
`diff passwords.old passwords.new`

//
output:
42c42
< kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd
---
> w0Yfolrc5bwjS4qw5mq1nnQi6mF03bii

//

old password: w0Yfolrc5bwjS4qw5mq1nnQi6mF03bii

new password: kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd 






host:`ssh bandit18@bandit.labs.overthewire.org -p 2220`
password: `kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd`

Connection was immediately closed and a message Byebye ! given.





