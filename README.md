# Konsolen-Commands
## Bash commands to manage e.g. a Contao4-Installation via SSH

#### Komplette Site per SSH packen:
    tar cvfz FILENAME_$(date "+%Y-%m-%d_%H-%M-%S").tar.gz FOLDER/

#### Site per SSH entpacken:
	tar -xvzf FILENAME.tar.gz

#### mySQL Dump erstellen:
	mysqldump -hDATENBANKHOST -uDBUSER -pDBPASSWORT --opt DBNAME | gzip > FOLDER/FILENAME.sql.gz

##### mySQL Dump zurückspielen:
	mysql -hDBHOST -uDBUSER -pDBPASSWORT DBNAME < FILENAME.sql.gz



##### [Anleitung bei Ionos](https://www.ionos.de/hilfe//index.php?id=2835)

# 

#### [MAC-Dateien (._*) wieder löschen:](http://www.linux-praxis.de/linux1/befehle7.html)

	find . -iname "._*" -delete