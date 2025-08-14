---
title: 
description: 
published: true
date: 2025-08-14T09:09:53.090Z
tags: 
editor: markdown
dateCreated: 2025-08-14T06:41:43.683Z
---

# Peken käyttö


<p><strong>Ohjeet:</strong> <a href="https://peke.plab.fi/help" target="_blank">Peke Help -sivusto</a></p>


## Esittely

Peke on Lapin ammattikorkeakoulun FrostBit-ohjelmistolaboratorion ylläpitämä GitLab-palvelin, jota koulun henkilökunta sekä opiskelijat voivat käyttää ohjelmistoprojektien hallintaan, versionhallintaan sekä tiimityöskentelyn mahdollistamiseen.

## Uuden projektin luonti

Jotta voit hyödyntää GitLabin tarjoamia ominaisuuksia, sinun täytyy ensin luoda uusi projekti. GitLabin projektia kutsutaan monessa muussa Git-versionhallintaa tarjoavassa palvelussa repositorioksi.

Luo uusi projekti valitsemalla **Projects**-välilehti. Tämän jälkeen klikkaa **New project** -nappia.

![Kuva 1](/pekeohjesivukuvat/kuva1.png)![Kuva 2](/pekeohjesivukuvat/kuva2.png)

Tämän jälkeen sinulle aukeaa uusi näkymä, jossa voit luoda joko uuden tyhjän projektin (**Create blank project**), luoda projektin jostain valmiista mallista (**Create from template**) tai tuoda projektin jostain muusta palvelusta (**Import project**). Luodaan uusi projekti klikkaamalla **Create blank project** -nappia.

![Kuva 3](/pekeohjesivukuvat/kuva3.png)  
![Kuva 5](/pekeohjesivukuvat/kuva5.png)

Tässä näkymässä sinun tulee antaa projektille jokin nimi. Tämän jälkeen valitse **Project URL** -kohdasta projektille nimiavaruus. Nimiavaruus voi olla joko ryhmä tai oma käyttäjänimesi.

![Kuva 4](/pekeohjesivukuvat/kuva4.png)  
![Kuva 6](/pekeohjesivukuvat/kuva6.png)

Projektilla on kolme erilaista näkyvyysasetusta:

Projektilla on kolme erilaista näkyvyysasetusta.
Yksityisessä projektissa (**Private**) jokaiselle jäsenelle täytyy erikseen määrittää oikeudet projektiin. Jos valitset ryhmän **(Group)** Project URL -kohtaan, jokaiselle valitun ryhmän jäsenelle annetaan oikeudet automaattisesti. Ryhmä täytyy kuitenkin luoda ennen uutta projektia, jotta se olisi valittavissa.

Sisäisessä projektissa (**Internal**) oikeudet ovat kaikilla muilla kirjautuneilla käyttäjillä, paitsi ulkoisilla käyttäjillä. Käyttäjätili voidaan erikseen määrittää ulkoiseksi käyttäjäksi. 

Julkisessa projektissa kaikilla on pääsy projektiin, olit joko kirjautunut käyttäjä tai et. Valitse tämä vain, jos tiedät mitä olet tekemässä. **Älä koskaan jaa salaisuuksia (API-avaimet, salausavaimet...)  julkisesti! Jakaminen saattaa aiheuttaa oikeuksien menettämisen tai pahimmassa tapauksessa kalliin laskun!**


![Kuva 8](/pekeohjesivukuvat/kuva8.png)

Tämän jälkeen voit valita luodaanko projektin juureen uusi README.md markdown-tiedosto (**Initialize repository with a README**). Valitse tämä, jos olet luomassa täysin uutta projektia, etkä esimerkiksi lisäämässä jo olemassa olevaa koodia kansioon.
Toisena voit valita analysoidaanko koodia tietoturvariskien varalta (**Enable Static Application Security Testing (SAST).**)
Kolmantena voit valita tarkistetaanko, että sisältääkö koodisi salaisuuksia (**Enable Secret Detection**). 
Tämän jälkeen paina Luo projekti (**Create project**) -nappia luodaksesi projektin.


Tämän jälkeen paina Luo projekti (**Create project**) -nappia.

![Kuva 9](/pekeohjesivukuvat/kuva9.png)  
![Kuva 10](/pekeohjesivukuvat/kuva10.png)

## Toisten käyttäjien kutsuminen yksityiseen projektiin

Mene projektin sivulle ja valitse vasemmalta **Manage** ja **Members**.

![Kuva 11](/pekeohjesivukuvat/kuva11.png)

**Invite Members** -napista klikkaamalla voit kutsua yksittäisiä käyttäjiä.
**Invite a group** -napista voit kutsua ryhmän jäsenet projektiisi
**Import from a project** kutsuu kaikki käyttäjät jostain toisesta projektista. Tässä käyttäjille määritetään samat roolit, kuin heillä on toisessakin projektissa.


![Kuva 12](/pekeohjesivukuvat/kuva12.png)

Hae kutsuttava käyttäjä käyttäjänimellä tai syötä sähköpostiosoite, niin kutsu lähetetään sinne. Käytä Lapin AMK:n tapauksessa opiskelijoiden ja henkilöstön @lapinamk.fi-päätteisiä sähköposteja. Sen jälkeen valitse käyttäjälle rooli sekä valinnaisesti päivä, jolloin käyttäjän oikeudet projektiin vanhenevat.
Lisää eri roolien oikeuksista voi lukea: 
[https://peke.plab.fi/help/user/permissions.md]

![Kuva 13](/pekeohjesivukuvat/kuva13.png)

## Projektin kloonaus  

Kloonaus tarkoittaa projektin kopioimista omalle koneellesi niin, että siitä luodaan uusi identtinen versio. Voit tehdä tähän kloonattuun versioon muutoksia, ilman että ne näkyvät suoraan GitLabista löytyvässä versiossa.  

Kloonaa projektikansio koneellesi menemällä halutun projektin sivulle, klikkaa sieltä Code-nappia ja kopioi sieltä projektin HTTPS-osoite. Tämän jälkeen voit joko käyttää kloonaamiseen Gittiä komentorivin kautta tai GitHub Desktop -sovellusta.  

![](/pekeohjesivukuvat/kuva14.png)

### Komentorivi  

[https://git-scm.com/downloads]

Avaa tietokoneellasi komentorivi haluamaasi kansioon ja suorita komento “git clone projektisiosoitetähän”. Jotta tämä toimii koneellasi, täytyy sinulla olla Git asennettuna  

![](/pekeohjesivukuvat/kuva15.png)

Jos kloonaat Pekestä ensimmäistä kertaa, sinua pyydetään kirjautumaan sisään. Syötä Peke-käyttäjänimesi sekä -salasanasi.  

![](/pekeohjesivukuvat/kuva16.png)

Jos kaikki onnistui, kloonattu projekti pitäisi nyt löytyä koneeltasi.  

![](/pekeohjesivukuvat/kuva17.png)

## GitHub Desktop  

[https://github.com/apps/desktop]


Avaa GitHub Desktop sovellus ja klikkaa File valikosta Clone repository  

![](/pekeohjesivukuvat/kuva18.png)

Koska kloonaamme nyt GitLabista, valitse URL-välilehti ja liitä siihen repositorion osoite sekä valitse haluamasi kansio, johon projekti kloonataan.  Tämän jälkeen paina kloonaa (Clone) -nappia.  

![](/pekeohjesivukuvat/kuva19.png)

Jos kloonaat Pekestä ensimmäistä kertaa, sinua pyydetään kirjautumaan sisään. Syötä tähän Peke-käyttäjänimesi ja -salasanasi.  

![](/pekeohjesivukuvat/kuva20.png)

Jos kaikki onnistui, projekti löytyy nyt koneeltasi.  

![](/pekeohjesivukuvat/kuva21.png)

![](/pekeohjesivukuvat/kuva22.png)

## Issues  

GitLabin **Issue** on eräänlainen tehtävä, joita käyttäjät voivat määrittää projekteissa. Ne ovat tärkeä osa GitLabin projektinhallintaa. Niiden avulla pystytään ylläpitämään tehtävälistaa, määräämään tehtäviä eri käyttäjille sekä seuraamaan projektin etenemistä.  

### Issuen luonti  

Mene projektin sivulle ja valitse vasemmalta **Plan** ja **Issues**. Tämän jälkeen valitse **New Issue**.  

![](/pekeohjesivukuvat/kuva23.png)

![](/pekeohjesivukuvat/kuva24.png)

Määritä issuen tyyppi (**Type**) ja anna sille otsikko (**Title**). **Description**-kohtaan voit antaa laajemman kuvauksen tehtävästä.  

**Assignee**-kohdasta voit valita käyttäjän, jolle tehtävä määritetään.  

**Labels**-kohdasta voit määrittää nimikkeet issuelle. Voit luoda omia nimikkeitä. Näitä voi myöhemmin käyttää tehtävien lajitteluun.  

**Milestone**-kohtaan voidaan määrittää mihin välietappiin issue kuuluu. Milestone täytyy luoda ennen issueta, jotta se olisi valittavissa tässä kohdassa.  

**Dates**-kohtaan voi määrittää tehtävälle aikavälin.  

**Contacts**-kohtaan voidaan määrittää tehtävälle yhteyshenkilön tiedot.  

**Turn on confidentiality** -kohdasta voi rajoittaa issuen näkyvyyden vain Plannerin tai sitä vahvemmat oikeudet omaaville rooleille.  

![](/pekeohjesivukuvat/kuva25.png)

![](/pekeohjesivukuvat/kuva26.png)

Kun issue on valmis, klikkaa **Create issue** -nappia. Tämän jälkeen issuen voi löytää **Plan/Issues** välilehdeltä.  

![](/pekeohjesivukuvat/kuva27.png)

## Labels  

Nimikkeillä (Labels) voit lajitella projektin eri tehtäviä. Mukautettuja nimikkeitä käyttämällä voit muokata Issue Boardista juuri sinun projektiisi sopivan.  

### Nimikkeiden (Label) luonti  

Mene projektin sivulle ja valitse vasemmalta **Manage** ja **Labels**. Tämän jälkeen paina **New label** –nappia.  

![](http://localhost/pekeohjesivukuvat/kuva28.png)![](http://localhost/pekeohjesivukuvat/kuva29.png)

Määritä nimikkeelle otsikko (**Title**) sekä halutessasi kuvaus (**Description**). Valitse myös nimikettä kuvaava väri. Luo uusi nimike painamalla **Create label** –nappia.  

![](/pekeohjesivukuvat/kuva30.png)

## Issue Board  

Issue-taulu on tehokas työkalu projektin tehtävien hallinnointiin. Se tarjoaa selkeän, kanban-tyyppisen näkymän projektin työtilanteesta.  
### Issue boardin hallinnointi  

Mene projektin sivulle ja valitse vasemmalta **Plan** ja **Issue boards**.  

![](/pekeohjesivukuvat/kuva31.png)

Perusnäkymässä sinulla on näkyvissä Open ja Closed –sarakkeet. Voit piilottaa ne klikkaamalla oikeassa laidassa olevaa hammasrattaan kuvaa.  

![](/pekeohjesivukuvat/kuva32.png)

Avautuvasta valikosta voit piilottaa sarakkeet ottamalla ruksin pois **Show the Open list** ja **Show the Closed list** -kohdista. Täältä voit myös vaihtaa Issue boardin nimen tai poistaa Issue boardin. Tallenna muutokset painamalla **Save changes** -nappia.  

![](/pekeohjesivukuvat/kuva33.png)

### Uuden sarakkeen lisäys  

Paina **Issue boards** sivulla näkyvää **New list** -nappia  

![](/pekeohjesivukuvat/kuva34.png)

Valitse valikosta nimike, jonka haluat lisätä. Tämän jälkeen paina **Add to board** –nappia.  

![](/pekeohjesivukuvat/kuva35.png) ![](/pekeohjesivukuvat/kuva36.png)

![](/pekeohjesivukuvat/kuva37.png)

Kun uusi sarake on lisätty, voit siirtää Issuen sarakkeesta toiseen vedä ja pudota -tyylillä. Voit myös vaihdella sarakkeiden järjestystä samalla tyylillä.  

![](/pekeohjesivukuvat/kuva38.png)

Muista siirtää Issuet aina niille kuuluviin sarakkeisiin. Esimerkiksi tässä tapauksessa tehtävää aloittaessa siirrä Issue TODO -sarakkeesta Work In Progress -sarakkeeseen. Näin Issue board pysyy ajantasalla ja projektin etenemisen seuranta onnistuu yhdellä katsauksella.  

![](/pekeohjesivukuvat/kuva39.png)