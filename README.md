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