# filelock
Password encrypt/decrypt a file. 

Usage: filelock.sh { encrypt | decrypt } \<filename\>
  
  mode 'encrypt': pass as mode when you wish to encrypt a file.
  mode 'decrypt': pass as mode when you wish to decrypt a file.
  help '-h': pass as the sole argument to see this banner. 



## Example Usage

    $ chmod -x ./filelock.sh
    $ ls
      myfile.txt
    $ ./filelock.sh encrypt ./myfile.txt
      enter aes-256-cbc encryption password: 
      Verifying - enter aes-256-cbc encryption password:
    $ ls
      encrypted_myfile.txt 
      myfile.txt
    $ ./filelock.sh decrypt ./encrypted_myfile.txt
      enter aes-256-cbc decryption password:
    $ ls
      decrypted_myfile.txt
      myfile.txt
