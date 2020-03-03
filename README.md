
# R intro

This repository contains materials used in an introductory level R course at university of Eastern Finland. For now, all the material here is written Finnish

## R-kurssi

T��lt� l�yd�t suomenkielisen materiaalin, joka tukee UEF:in R-kurssin suorittamista (R-kieli 3622223, 2 op). Jokaisen viikon materiaalit p�ivitet��n t�nne. Alla on ohjeet tarvittavien asioiden asentamiseen UEF:in koneille.


# RStudio

Erona Moodlessa l�ytyviin ohjeisiin, tuutoroinnissa k�ytet��n R-ohjelmoinnin tukena RStudiota. ohjelmointiymp�rist� eli IDE (integrated development environment), joka tekee koodaamisesta huomattavasti mukavampaa.

## RStudion asennus

N�iden ohjeiden avulla saat asennettua RStudion ja sen mukana R:n UEF:in koneille. Omalle koneelle asennettaessa t�ytyy ensin asentaa R, ja sitten RStudio. Ohjeet l�ytyv�t helposti Googlesta, esim [t��lt�](https://courses.edx.org/courses/UTAustinX/UT.7.01x/3T2014/56c5437b88fa43cf828bff5371c6a924/).

RStudion saa asennettua UEF:in koneilla Sofware Centerin kautta. Software Center l�ytyy Windowsin omalla haulla.

<img src="software_center.jpg" alt="" width="300"/>

RStudio:n voi asentaa Software Centerist�, ja RStudion pit�isi sen j�lkeen olla k�ytett�viss�.

<img src="RStudio_sc.jpg" alt="" width="300"/>


## RStudion k�ytt�

RStudion n�kym�ss� on nelj� osaa:

<img src="RStudio_tutorial_edited.jpg" alt="" width="600"/>

#### 1. Editori. 

Editorilla kirjoitetaan R-koodia sis�lt�vi� tiedostoja, eli R-skriptej�. Uuden skriptin saa auki painamalla File -> New File -> R Script (tai Ctrl + Shift + N). Skripteihin tutustutaan my�hemmin kurssilla, mutta ne ovat yksinkertaisuudessaan kokoelma R-komentoja, jotka yhdess� tekev�t jotain, esimerkiksi analysoivat jonkin tutkimusprojektin datan tai piirt�v�t valmiista tuloksista kuvaajia.

Editoriin kirjoitettua koodia voi ajaa rivi kerrallaan painamalla rivin kohdalla Ctrl + Enter. Useamman rivin voi my�s maalata ja suorittaa kerrallaan. Yl�reunassa oleva "Source"-nappi ajaa kaiken nykyisen tiedoston koodin.

R-skriptej� voi tallentaa ihan kuin muitakin tiedostoja. R-skpriptien  tiedostop��te on .R

#### 2. Konsoli.

Konsolissa "ajetaan" eli suoritetaan R-komentoja. Jos editoriin kirjoitettua koodia ajetaan, RStudio ajaa komennot automaattisesti konsolissa. Konsolissa pelkk� Enter riitt� koodirivin suorittamiseen. Voit kokeilla kirjoittaa konsoliin jonkun laskutoimituksen, kuten ```2 * 3``` ja painaa Enter, jolloin tuloksen pit�isi tulostua konsoliin. Voit my�s kokeilla kirjoittaa laskuja editoriin, ja painaa Ctrl + Enter, jolloin pit�isi tapahtua sama asia.

Suurin ero konsolin ja editorin v�lill� on se, ett� **konsoliin kirjoitetut komennot eiv�t tallennu mihink��n tiedostoon**. Jos siis haluat s��st�� koodisi, se tulee kirjoittaa editoriin ja tallentaa .R-tiedostoon. Saman istunnon aikana tehtyj� komentoja voi konsolissa selata yl�s- ja alas-nuolila.

Moodlen ohjeissa ja videoissa k�ytet��n R:�� puhtaasta R-konsolista. Voit siis kuvitella, ett� kurssin videoissa n�kyy vain RStudion t�m� osa, ja muut osat ovat vain helpottamassa ty�t�si.

#### 3. Ty�tila

Ty�tilassa n�kyv�t R-istunnon aikana luodut muuttujat. N�ist� lis�� ensimm�isen viikon materiaalissa.

#### 4. Kuvaajat / Paketit / Manuaali

T�ss� osassa on monta k�yt�nn�llist� v�lilehte�:

- Plots: t�nne ilmestyv�t R:ll� piirretyt kuvaajat
- Packages: T��lt� voi hallita asennettuja paketteja (alla ohjeet t�ll� kurssilla tarvittavien pakettien asennukseen)
- Help: T��ll� voi selata R:n manuaalia, jossa on ohjeet jokaiselle R-komennolla. Voit kokeilla ajaa editorissa tai konsolissa komennon ```?print```, joka avaa ```print```-funktion ohjesivun.


### Kurssin teht�vien tekeminen RStudiolla

Suurin osa kurssin teht�vist� on melko lyhyit�, joten ne voi tarvittaessa tehd� suoraan konsoliin. Suosittelen kuitenkin kirjoittamaan varsinkin pidemm�t ja monimutkaisemmat teht�v�t muistiin editoriin. Valitettavasti kurssin teht�vien aktivointi aiheuttaa RStudion toiminnassa hieman outouksia, koska kurssin teht�vi� ei ole suunniteltu RStudiolla teht�viksi. Aina kun editorista ajaa komennon, editorin tilalle aukeaa "kysymys"-ikkuna. T�st� ei kuitenkaan tarvitse v�litt��, vaan ikkunan voi sulkea.

**HUOM:** kurssin osioiden teht�vi� ei voi tallentaa kesken osion, vaan jokainen osio on teht�v� kerralla kokonaan. Jos kuitenkin kirjoitat koodia editoriin ja tallennat teht�vi� .R-tiedostoon, voit tarvittaessa aloittaa osion toisena p�iv�n� uudestaan ja ajaa edellisell� kerralla kirjoittamasi komennot helposti tiedostosta. Teht�vi� voi palauttaa vain UEFAD-verkon koneilla!.

Teht�vien tekemisen voi aloittaa komennolla ```Rkurssi::Rkurssi(123456)```, kun numeron 123456 korvaa omalla opiskelijanumerolla ja seuraamalla avautuvia ohjeita. T�t� varten tulee kuitenkin asentaa ```Rkurssi```-paketti. T�h�n on ohjeet alla.

## Kurssilla tarvittavien R-pakettien asennus

R-ohjelmoinnissa asennetaan usein R-paketteja. Paketit ovat kokonaisuuksia, jotka lis��v�t R:��n ominaisuuksia. Esimerkiksi t�lle kurssille tarvittavat paketit arpovat opiskelijalle teht�vi� kurssin aihepiirist� ja l�hett�v�t tiedon osioiden suorituksesta opettajalle.

Ensin asennetaan paketti ```sendmailR```. Valitaan RStudion oikean alakulman osasta Packages -> Install. Avautuvaan ikkunaan kirjoitetaan paketin nimeksi "sendmailR" ja asennetaan paketti. CRAN (Comprehensive R Archive Network) on paikka, johon iso osa R-paketeista on tallennettu, jotta ne on helppo asentaa.

<img src="package_install.jpg" alt="" width="700"/>

 Itse teht�vi� arpova ```Rkurssi```-paketti ei ole CRAN:issa, vaan se pit�� ladata kurssin Moodle-sivulta ```Rkurssi.zip```-tiedostona. Paketin asennusta varten valitaan Install-ikkunasta "Install from"-vaihtoehdoksi "Package Archive File", ja valitaan aukeavasta ikkunasta juuri ladattu  ```Rkurssi.zip```
 
 <img src="install_rkurssi.jpg" alt="" width="300"/>