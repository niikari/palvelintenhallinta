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

## b) Kaikki kirjataan. Näytä omalla git-varastollasi esimerkit komennoista ‘git log’, ‘git diff’ ja ‘git blame’. Selitä tulokset.

Samalla kun testattiin komentoja, niin kokeilin miten kuvakaappauksen saa lisättyä osaksi dokumenttia.
Aloitettu syöttämällä:

	$ git log

Tästä saatu tulos:

![Image](https://github.com/niikari/palvelintenhallinta/blob/main/gitlog.JPG?raw=true)

Näkyy kaikki tehdyt commitit ja missä branchissa tällä hetkellä olen muutoksia tekemässä (HEAD -> main).
Kaikki commitit on merkitty hashilla, mukana commitin tekijän tieto ja commit viesti. Näkyvillä on useampi tehty commit.

	$ git diff

Tästä saatu tulos:

![Image](https://github.com/niikari/palvelintenhallinta/blob/main/git%20diff.JPG?raw=true)

Näyttää muutokset, joita on tehty, mutta ei vielä commit tehty. Puhutaan eroista riveissä (tyhjä rivi lasketaan muutokseksi)


	$ git blame

Mikä on blame? Atlassianin [Link](https://www.atlassian.com/git/tutorials/inspecting-a-repository/git-blame) mukaan on monipuolinen
debuggaus työkalu. Pystyy hakemaan esim. yhteen tiettyyn tiedostoon tehtyjen muutosten tekijät ja tarkat tiedot commitista.

Tämän ajosta saatu tulos:

![Image](https://github.com/niikari/palvelintenhallinta/blob/main/git%20blame.JPG?raw=true)

Näkyvillä on lisätietoja mitä voi laittaa käskyn mukana. Esim.:

	$ git blame -L 1,5 README.md

-L optiolla rajataan hakua tiedoston sisältä - tässä tapauksessa haetaan riveille 1-5 tehtyjä muutoksia

## c) Huppis! Tee tyhmä muutos gittiin, älä tee commit:tia. Tuhoa huonot muutokset ‘git reset --hard’. Huomaa, että tässä toiminnossa ei ole peruutusnappia.

Kuvakaappaus vaiheista, jotka tehty:

![Image](https://github.com/niikari/palvelintenhallinta/blob/main/Dumb.JPG?raw=true)









