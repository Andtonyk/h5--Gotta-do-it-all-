Huom! Kaikki testit on toteuttu seuraavanlaisella koneella: Windows 10 OS:llä, Google Chrome selaimella ja koneena on toiminut Legion 5 kannettava. 16Gt RAM, AMD Ryzen 7 5800H, NVIDIA Geforce 3070 ja 200GB vapaata levytilaa SSD-levyasemalla.
# h5--Gotta do it all! ...Or at the very least try!
## h5-tehtävän dokumentaatio

### A) Uuden virtuaalisen koneen luominen ja uuden verkkoympäristön muodostaminen
Tässä tehtävässä aloitan uuden virtuaalisen koneen luomisen ja toivottavasti päätän tehtävän onnistuneen uuden verkkoympäristön luomiseen.

Uuden virtuaalisen koneen muodostaminen alkoi samoilla toimilla, kuin ensimmäisenkin. Avasin VM:n ja avasin debian-paketin, jonka pohjalta pääsin aloittamaan halutun virtuaalisen koneen muodostamista.

Alku sisälsi totutusti muodostettavan uuden VM:n nimen, OS:n tyypin sekä sijainnin valitsemisia. Tärkeimpiä oli "Skip Unattended Installation" kohdan täppääminen.

![Uuden debianin asennus](https://github.com/Andtonyk/h1---Debian/assets/149326156/af992c97-6757-4d89-aff1-938f77878f1b)

Valitsin uudelle muodostettavalle VM:lle jo muodostetun VM:n kovalevyn talletustilaksi.

![Uuden debianin asennus - kovalevyn asetukset](https://github.com/Andtonyk/h1---Debian/assets/149326156/ee3e6b71-641a-47ea-b7b8-e05c5f3f25e0)

Prosessoreita asetin käyttöön 4 kappaletta ja muistia varasin 4096MB

![Uuden debianin asennus - koneen rauta](https://github.com/Andtonyk/h1---Debian/assets/149326156/4bbae283-35ff-431b-8cbd-6a14acc695b2)

### VM:n avaaminen

Uusi muodostettu Debian ympäristö avautui onnistuneesti, joten klikkasin työpöydällä olleesta "Install Debian" pikakuvakkeesta käyttöjärjestelmän aktivoimista.

![Ensimmainen kaynnistys](https://github.com/Andtonyk/h1---Debian/assets/149326156/8bfa8425-b2b4-4367-a816-530c645fea97)

![Ensimmainen kaynnistys onnistui](https://github.com/Andtonyk/h1---Debian/assets/149326156/c7b08f41-2d73-4206-8aa6-f8662a624b17)

Aloitin uuden käynnistyneen debianin kautta itse asennettavan OS:n asetuksien määrittämisen.
Käytin pohjana aiemin toteutetun VM:n asetuksia.

Pidin käyttöjärjestelmän kielen oletuksellisena.

![Asentamisen alkaminen](https://github.com/Andtonyk/h1---Debian/assets/149326156/7fb61b68-d434-4ec5-8faa-d1d4348e0311)

Alueeksi valitsin Euroopan ja tarkemmaksi sijainniksi asetin Suomen. 

![Asentamisen alkaminen - aikavyöhyke](https://github.com/Andtonyk/h1---Debian/assets/149326156/8e98c15f-8fc1-4665-924a-dbaac0a14b7c)

Näppäimistön asetin tottelemaan suomenkielistä näppäimistö mallia.

![Asentamisen alkaminen - nappaimisto](https://github.com/Andtonyk/h1---Debian/assets/149326156/515700c6-ab9d-4b0d-a026-9688e6040085)

Koska asetin uuden VM:n tallettamaan tietojaan samalle, jo muodostetulle alueelle kuin ensimmäisen VM:ni. Piti minun kiinnittää vertaisasentamiseen lisähuomiota.

![Asentamisen alkaminen - asentamisen kovalevy](https://github.com/Andtonyk/h1---Debian/assets/149326156/9666fdc3-acb3-42ca-8a60-d6621dc3b8f6)

Muodostin uudelle VM:lle uuden käyttäjätunnuksen ja tein sille vahvan salasanan.

![Asentamisen alkaminen - kayttajatunnus ja salasana Andreas](https://github.com/Andtonyk/h1---Debian/assets/149326156/c8c15797-2f53-4c9c-b4c4-dfcc776d1765)

Tarkistettuani asunnuksen yhteenvedon siirryin itse asennukseen.

![Debianin asetukset](https://github.com/Andtonyk/h1---Debian/assets/149326156/90dfc58f-166a-4fd9-a85c-c13e909a9883)

Asennuksen aikana ei tullut virheilmoituksia ja se kesti noin 7 minuuttia.

![Asennus kaynnissa](https://github.com/Andtonyk/h1---Debian/assets/149326156/ebb4021f-a96d-43a5-99a9-acf426ab2142)

Asennuksen päätyttyä sain kuittauksen siitä, että kaikki olisi toteutunut asennuksessa ongelmitta.

![Asentamisen valmistuminen - 7 min](https://github.com/Andtonyk/h1---Debian/assets/149326156/0294c6bd-f602-4b40-90d0-493a2ba90a9b)

### Käyttöjärjestelmä on kunnossa, kohti määrityksellisiä haasteita
Kun asennus oli päättynyt, avasin terminalin ja aloitin toteuttamaan verkkosivujen muodostukseen sekä palvelimen hallintaan liittyviä toimia.

Micro- sekä Nano editoiren asentaminen
![Terminal - Micro asennettu](https://github.com/Andtonyk/h1---Debian/assets/149326156/14b69f11-b0b9-4f8e-9aa6-ba3ef5a1acfb)

Curlin- asentaminen

![Terminal - Curl ladattu](https://github.com/Andtonyk/h1---Debian/assets/149326156/6ad6cbf4-c433-46a0-8b08-9b07e88d1e7a)

Apache2- asentaminen

![Terminal - Apache2 hankkiminen](https://github.com/Andtonyk/h1---Debian/assets/149326156/3f374af1-0294-47ba-9688-2b3e8f61525d)

Kun Apache2 oli asentunut, varmistin sen aktiivisuuden enable-komennolla.

![Terminal - Apache2 enabled](https://github.com/Andtonyk/h1---Debian/assets/149326156/eed510b8-60b5-4817-911b-108587aa96f8)

Tämän jälkeen tarkistin ls-komennolla Apache2-rakenteen kansioiden tilan.


![Terminal - apache 2 - kansion nakyma](https://github.com/Andtonyk/h1---Debian/assets/149326156/361849e4-9c68-4a29-b7de-06c14cccaca9)

Kun Apache2 näytti olevan kunnossa, tein vielä terminalin kautta päivityksien ajon.

![Terminal - kaynnistys ja paivitys](https://github.com/Andtonyk/h1---Debian/assets/149326156/66d9d11c-cd28-401d-b773-f5497aaa3f06)

IP-osoite listaus

![IP-osoite lista](https://github.com/Andtonyk/h1---Debian/assets/149326156/386ba631-342c-4da1-aba4-07e8fd7a63c6)

Verkkoyhteys toimii ja Terokarvinen.com sivusto näkyy ongelmitta.

![Terokarvinen com nakyy](https://github.com/Andtonyk/h1---Debian/assets/149326156/d039b449-22b7-4d68-b0bd-b8676655b9bc)

Apache2 näkyy localhostissa

![Apache2 localhost nakyma ennen muutoksia](https://github.com/Andtonyk/h1---Debian/assets/149326156/8c252877-336c-47d1-9247-0fdf468a0725)

Koska Apache2:n perusnäkymä oli onnistunut, siirryin muodostamaan tietoja uutta palvelimelle asetettavaa sivua varten.
Tämän tein terminalissa aloittamalla komennolla cd /etc/apache2/sites-available ja muodostamalla tämän jälkeen .conf tiedoston komennolla: micro andreas.example.com.conf

![Apache2 uudelleen kaynnistys](https://github.com/Andtonyk/h1---Debian/assets/149326156/c0c63114-3176-4c6d-87e3-b8a6e88de7bb)

Syötin tiedostoon alla olevan kuvan mukaiset tiedot. Onneksi huomasin kuvakaappausesta tehneeni kirjoitus virheen ja muokkasin sanan Rewquire muotoon Require

![perustettavan sivun tiedot apache2ssa](https://github.com/Andtonyk/h1---Debian/assets/149326156/0ae5968f-542a-4496-8c5b-ff53c60a12ab)

Kun ensimmäinen muokkaus oli ohi muodostin sivun html-aineistoa varten uuden kansion komennolla mkdir -p /home/andreas/publicsites/andreas.example.com

![Muodostettu kansio uudelle sivulle](https://github.com/Andtonyk/h1---Debian/assets/149326156/693bbff5-3571-485e-b4d3-923f0e16726f)

Lisäsin kyseiseen kansioon komennolla micro index.html sivua koskevat html-perusrakenteet testausta varten.

![Muodostetaan index html tunnus](https://github.com/Andtonyk/h1---Debian/assets/149326156/e9f2107c-56f7-4564-ba4a-6bbf549658f1)

Tein sisällön alla olevan kuvan mukaisesti

![index html](https://github.com/Andtonyk/h1---Debian/assets/149326156/b4b1fad5-4650-4767-8e4d-32f2d0025f71)

Tämän jälkeen varmistin että localhost näkymä oli muuttunut vastaamaan muokkausta. Näin oli onneksi tapahtunut.

![Testisivu v4 localhost](https://github.com/Andtonyk/h1---Debian/assets/149326156/e255e22f-1ac1-4e3a-98af-1e712b6deeab)

Sen jälkeen varmistelin vielä asetuksien oikeellisuutta, tässä käytin aiempia tehtäviäni sekä Teron ohjeistusta: https://terokarvinen.com/2018/04/10/name-based-virtual-hosts-on-apache-multiple-websites-to-single-ip-address/ sekä Apachen ohjetta https://httpd.apache.org/docs/2.4/vhosts/name-based.html

Näillä sain pitkällisen taistelun jälkeen sivun näkyville apacheen myös nimihaussa. Valitettavasti tästä vaiheesta en muistanut dokumentoida tekemiäni muutoksia.

![Testisivun nakyvyys nimihaussa](https://github.com/Andtonyk/h1---Debian/assets/149326156/c5fbd778-df9e-415b-83f4-15494a9aba3b)

Tämän jälkeen asensin palomuurin ja tein portti poikkeuksia.
![Terminal - palomuurin asentaminen ja uuden kauttajan luominen - kayttaja sal kayttaja](https://github.com/Andtonyk/h1---Debian/assets/149326156/9293b030-3c4b-4855-beb6-1e163f2b641a)

### B) Pubkey?


### C) Host- ja Dig-komennot

Man-komento hostista kertoi, että host-komento tarjoaa helpon työkalun DNS-rakenteiden tarkasteluun.
![man host selitys](https://github.com/Andtonyk/h1---Debian/assets/149326156/d68f97f8-f8d7-40ef-bdc6-ae9c099270b9)

Komennolla saatu listaus antaa kuvaa osoitteistosta. IP-osoite vaikuttaisi olevan sama, kuin henkilön hankkiman domain-tarjoajan välittämä IP-osoite.

![host nakyma terminalissa](https://github.com/Andtonyk/h1---Debian/assets/149326156/c2f04889-38a1-4d4b-a1f6-06f755644c01)

![namecheap ip-osoite](https://github.com/Andtonyk/h1---Debian/assets/149326156/8eb45827-e9c6-4a3b-a622-1fe5044e1f28)

Man-komento digistä antaa kuvan siitä, että se on tarkoitettu syvällisempään DNS-kartoitukseen ja analysointiin, kuin pinnallisempi "host".
Se suorittaa samankaltaisen DNS-kyselyn, mutta listaa sen antamista vastauksista myös tarkempaa infoa. Kuten host-komento, listaa dig-komentokin domain-tarjoajan IP-osoitteen kohde osoitteena.

![man dig selitys](https://github.com/Andtonyk/h1---Debian/assets/149326156/ea39d0ab-7840-4ae1-8487-570c26c31984)

![Dig andreask me](https://github.com/Andtonyk/h1---Debian/assets/149326156/7a93e765-5719-4793-904b-294da27608c4)
