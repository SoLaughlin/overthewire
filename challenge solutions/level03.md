# overthewire
 challenge submissions @ overthewire
 
## level goal: Access level 3 by finding the password

instructions mentioned the password was on a file named spaces in this file name.

  `ls` showed the file
  
  however when using :`cat spaces in this file name` returned nothing
  spaces are now allowed in filenames(not always the case) but terminals have problems translating them. 
  
  By using `tab` it autofilled to `spaces\ in\ this\ filename`

  I also found this solution to the problem [https://askubuntu.com/questions/516772/how-to-access-files-directories-with-spaces-in-the-name:]
  
 
  `cat spaces\ in\ this\ filename` returned : `UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK`
  
  password : `UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK`
