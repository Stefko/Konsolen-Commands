# Konsolen-Commands
## Bash commands to manage e.g. a Contao4-Installation via SSH

#### Komplette Site per SSH packen:
    tar cvfz FILENAME_$(date "+%Y-%m-%d_%H-%M-%S").tar.gz FOLDER/

#### Site per SSH entpacken:
	tar -xvzf FILENAME.tar.gz

#### mySQL Dump erstellen:
	mysqldump -hDATENBANKHOST -uDBUSER -pDBPASSWORT --opt DBNAME | gzip > FOLDER/FILENAME.sql.gz

##### mySQL Dump zurückspielen:
	mysql -hDATENBANKHOST -uDBUSER -pDBPASSWORT DBNAME < FILENAME.sql.gz



[Anleitung bei Ionos](https://hilfe-center.1und1.de/hosting/1und1-webhosting-c10085285/datenbanken-c10082637/mysql-c10082650/bedienung-c10082751/mysql-datenbank-ueber-ssh-sichern-und-wiederherstellen-a10783397.html)