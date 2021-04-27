# overthewire
 challenge submissions @ overthewire

## level goal: Find the password

Stored in data.txt as a hexdump that has been compressed multiple times

### solution

`ls` # showed the data.txt file
`cat data.txt` # showed a hexdump
`xxd -r data.txt newdata.txt` #output gibbirish
`file newdata.txt` # showed it was a gzip
`mv newdata.txt newdata.gz` #converted file to gzip
`gzip -d newdata.gz` #decompress \/unzip the file
`find newdata` #bzip file. From here changed to bzip/gzip/tar multiple times.
``#decompressed until an ascii file
`cat filename`# password

host:`ssh bandit13@bandit.labs.overthewire.org -p 2220`
password: `8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL`




