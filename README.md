# filelock
Password encrypt/decrypt a file. 

Usage: filelock { encrypt | decrypt } \<filename\>
  
  mode 'encrypt': pass as mode when you wish to encrypt a file.\n
  mode 'decrypt': pass as mode when you wish to decrypt a file.\n
  help '-h': pass as the sole argument to see this banner. \n



## Example Usage

    $ chmod -x ./filelock
    $ ls
      myfile.txt
    $ ./filelock encrypt ./myfile.txt
      enter aes-256-cbc encryption password: 
      Verifying - enter aes-256-cbc encryption password:
    $ ls
      encrypted_myfile.txt 
      myfile.txt
    $ ./filelock decrypt ./encrypted_myfile.txt
      enter aes-256-cbc decryption password:
    $ ls
      decrypted_myfile.txt
      myfile.txt
