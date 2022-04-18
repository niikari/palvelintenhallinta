# H3 versionhallinta

## a) MarkDown. Tee tämän tehtävän raportti MarkDownina. Helpointa on tehdä raportti GitHub-varastoon, jolloin md-päätteiset tiedostot muotoillaan automaattisesti. Tyhjä rivi tekee kappalejaon, risuaita ‘#’ tekee otsikon, sisennys merkitsee koodinpätkän.
Aloitettu tekemällä uusi markdown tiedosto "h3-versionhallinta.md"

	$ nano h3-versionhallinta.md

Oma repository oli GitHubissa jo valmiiksi, linkitettynä kansioon, jossa tiedosto sijaitsee. Joten vain lisätty:

	$ git add .
	$ git commit -m "Eka markdown"
	$ git pull
	$ git push

## b) Pull first. Tee useita muutoksia git-varastoosi. Tee muutama muutos, jossa yksi commit koskee useampaa tiedostoa. Anna hyvä kuvaukset (commit message), yksi englanninkielinen lause imperatiivissa (määräysmuodossa) "Add top level menu to Foobar synchronizer"
Tehty kaksi uutta tiedostoa, joihin molempiin laitettu jotain tekstiä.

	$ echo "muutos repoon" > ekamuutos.txt
	$ echo "toinen muutos repoon" > tokamuutos.txt
	$ git add .
	$ git commit -m "Added new files"
	$ git pull
	$ git push

Tämän jälkeen muokattu ensimmäistä tiedostoa.

	$ echo "Add new line" >> ekamuutos.txt
	$ git commit -am "Made changes, added new line"
	$ git pull
	$ git push

Siirryin eteenpäin, tämä aihe ennalta suht tuttua (commit -viestit voisivat toki olla parempia(kin))

![Image](https://github.com/niikari/palvelintenhallinta/blob/main/gitlog.JPG?raw=true)

