# Aasta Tegija - IT Spetsialisti võistluse testimiseks mõeldud projekt
====================================================

Antud rakendus on koostatud PHP ja MySQL põhjal. Rakendus tuleb kasutada et testida klientmasina seadistust ning veebiserveri seadistus ja gitlabi serveri tööd.

### Ettevalmistus

Järgmised paketid on vajalikud:

* php
```
sudo apt-get install php7.4 libapache2-mod-php7.4 php7.4-mysql
```

* MySQL
```
sudo apt-get install mysql-server
```

* .htaccess
```
sudo a2enmode rewrite
```
### Paigaldamine

Paigaldamiseks on võimalik kasutada järgmist viisi:

Projekti failid on võimalik kloneerida arvutisse git abil

```
git glone https://github.com/AnnaKarutina/at21.git
```

Või laadida manuaalselt [aadressilt](https://github.com/AnnaKarutina/at21).

## Projekti seadistus 

Projekti seadistus asub [constants.php](https://github.com/AnnaKarutina/at21/blob/main/app/config/constants.php) failis

* DB_USER konstandi väärtus peab vastama andmebaasis olevale - andmebaasi kasutaja nimi
* DB_PASS konstandi väärtus peab vastama andmebaasis olevale - andmebaasi kasutaja parool
* DB_NAME konstandi väärtus peab vastama andmebaasis olevale - andmebaasi nimetus, kus asuvad projektiga seotud tabelid

## Admebaasi struktuur ja seadistus

Andmebaasi struktuuri dump fail on leitaitav [siin](https://github.com/AnnaKarutina/at21/blob/main/app/docs/db.sql). Mugavalt saab seda exportida läbi phpMyAdmin keskkonda.


## Testimine

Testimiseks tuleb vaadata veebilehitsejal projekti näiteks aadressil:
```
http://localhost/at21/users/register
```

## Built With

* [PHP](http://php.net/) - Programmeerimiskeel 
* [MySQL](https://dev.mysql.com/) - Andmebaas

## Versioneerimine

kasutame [SemVer](http://semver.org/) versioneerimiseks.
Hetkel meil on üks versioon 1.0.0

## License

Antud projekt on MIT License litsentsiga.
