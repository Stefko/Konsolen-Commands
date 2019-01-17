# Konsolen-Commands
## -> ProjectName
## Bash commands to manage e.g. a Contao4-Installation via SSH

### mySQL Dump erstellen:
	mysqldump -hDATENBANKHOST -uDBUSER -pDBPASSWORT --opt DBNAME | gzip > FOLDER/FILENAME.sql.gz

### Komplette Site per SSH packen:
    tar cvfz FILENAME_$(date "+%Y-%m-%d_%H-%M-%S").tar.gz FOLDER/

### Site per SSH entpacken:
	tar -xvzf FILENAME.tar.gz

### [MAC-Dateien (._*) wieder löschen:](http://www.linux-praxis.de/linux1/befehle7.html)

	find . -iname "._*" -delete

### mySQL Dump zurückspielen:
	mysql -hDBHOST -uDBUSER -pDBPASSWORT DBNAME < FILENAME.sql.gz

### mySQL Dump zurückspielen wenn gz gepackt:
	gunzip -c dbXXXXXXX.sql.gz | mysql --host=dbxxxxx.hosting-data.io --user=dboXXXXXXX --password=geheimes_Passwort dbXXXXXXX

# 

##### [Anleitung bei Ionos](https://www.ionos.de/hilfe//index.php?id=2835)



