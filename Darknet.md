# Darknet lisätehtävä  

Minulla ei ole aikaisempaa kokemusta darknetin käytöst, mutta se on kiinnostanut minua, joten tämä on hyvä lisätehtävä.  
Tarkoituksena on kokeilla kolme eri Darknet:iä. Ensimmäisenä I2P.  

## I2P  
Testasin I2P:tä Debianissa asentamalla sen I2P sivulta. Asennus oli haastava, koska yritin ensiksi repositoryn kautta, mutta se ei onnistunut. Debian jota käytän ei ollut yhteensopiva I2P paketin kanssa. Kotin asentaa pakettia, mutta sain virheilmoituksia  
allekirjoitusavaimesta. Päädyin lataamaan I2P sivuilta Java-pohjaisen ohjelman. Käytin terminaalia käynnistääkseni installerin, ja sain ohjelman asennettua. Itse asennushetkellä unohdin ottaa kuvakaappauksen, mutta alla näkyy lataustiedestoa Download kansiossani, 
ja samalla myös kuinka käynnistän I2p:n.  

<img width="1920" height="921" alt="Screenshot From 2026-02-10 09-29-59" src="https://github.com/user-attachments/assets/1b7379d3-3191-4746-a937-c7fb258e765f" />  

Sain käynnistettyä I2P Firefoxissa. Verkon tila oli aluksi hyvin kauan Network:Testing, jonka takia en päässyt selaamaan eri sivustoja. Jatkoin tehtävää seuraavana päiväna, jolloin sain verkon tilaksi Network:Firewalled. Koitin avata Router Consollista  
useampia verkkosivuja, mutta sain aina virheilmoituksen enkä päässyt sivustoihin. Router Consolessa oli myös seuraavanlainen viesti (alleviivattu punaisella):  
<img width="1920" height="921" alt="Screenshot From 2026-02-10 09-07-48" src="https://github.com/user-attachments/assets/b67cbd5b-907a-4f29-9816-30fcdbc3576d" />  
Käsittääkseni tuo selittää miksi en päässyt sivustoille.  
### Uhkamalli  
I2P pyrkii piilottamaan viestinnäin sisällön ja osapuolten sijainnin, jolloin se estää käyttäjän tunnistamisen.

### Protokolla  
I2P käyttää omaa salattua protokollaa, jossa liikenne kulkee usean solmun kautta yksisuuntaisissa tunneleissa.

### Toimintaperiaate  
I2P on hajautettu vertaisverkko. Käyttäjien liikenne reititetään muiden solmujen kautta, joka parantaa anonymiteettiä, mutta hidastaa yhteyksiä.  
https://geti2p.net/en/docs/how/intro  

## Freenet  
Latasin Freenetin virallisilta sivuilta Java-pohjaisen asennustiedoston. Käynnistin sen terminaalissa komennolla java -jar. Asennus avasi Freenetin paikallisen käyttöliittymän selaimeen, ja pääsin aloittamaan verkon käytön. Alla kuvakaappaus komennoista.  
<img width="1920" height="885" alt="Screenshot From 2026-02-10 13-55-39" src="https://github.com/user-attachments/assets/6824b840-75a9-4fb2-ab23-1ffcbdeeb753" />  
Aluksi verkkoon yhdistämminen vei hetken, sillä node etsi muita vertaiskoneita. Muodostettuani yhteyden, avasin “Freenet First Steps” sivun ja  Clean-Spider-hakemiston. Omiin silmiini varinkin jälkemmäinen tuntuu sekavalta enkä kauheasti ymmärrä siitä mitään, mutta oli silti kiinnostavaa päästä sinne.  
Itse verkkoon pääseminen vei vain noin 5min, mikä oli erittäin nopeaa  verrattuna I2P, jonne odotin ainakin 20min. Muutenkin koko prosessi oli kivuttomampi, joka johtuu siitä että tajusin lataamaan heti Java-pohjaisen asennnustiedoston.  

<img width="1920" height="921" alt="Screenshot From 2026-02-10 13-59-09" src="https://github.com/user-attachments/assets/02615619-b136-4f2d-b95a-405308da9b6c" />  
<img width="1920" height="921" alt="Screenshot From 2026-02-10 14-06-41" src="https://github.com/user-attachments/assets/0ce2a549-e091-4776-a0d4-157b4a952d6a" />  
<img width="1920" height="921" alt="Screenshot From 2026-02-10 14-04-43" src="https://github.com/user-attachments/assets/cb6eee5d-8039-422c-8f54-b21cfd7cd6a3" />  

###Uhkamalli  
Freenet on suunniteltu suojaamaan käyttäjiä sensuurilta ja valvonnalta. Sen tavoitteena on estää ulkopuolisia näkemästä kuka julkaisee tai hakee sisältöä  

###Protokolla ja toimintaperiaate  
Freenet toimii hajautetussa vertaisverkossa (P2P), jossa ei ole keskitettyä palvelinta. Data tallennetaan salattuna eri käyttäjien nodeihin, ja liikenne kulkee useiden koneiden kautta. Tämän vuoksi sisällön alkuperää ja käyttäjiä on vaikea jäljittää.  
https://www.hyphanet.org/index.html  

## ZeroNet  
Latasin ZeroNetin GitHub-sivulta .tar.gz-paketin wget-komennolla. Purin tiedoston tar xvpfz -komennolla, siirryin purettuun kansioon ja käynnistin ohjelman komennolla ./ZeroNet.sh. Kyseiset komennot löytyvät ZeroNetin Githubista: https://github.com/HelloZeroNet/ZeroNet#user-content-how-to-join.  
<img width="1920" height="921" alt="Screenshot From 2026-02-10 16-01-00" src="https://github.com/user-attachments/assets/5e827780-3a6a-4a5e-89ba-e8f9c5f2eb33" />


Käynnistämällä ohjelman pääsin HelloZeroNet sivulle: 
<img width="1920" height="921" alt="Screenshot From 2026-02-10 15-04-00" src="https://github.com/user-attachments/assets/2a6476c4-c441-45f5-90ff-52213030bacb" />  
Alussa minulla oli ongelmia kun koitin avata muita sivuja. Ongelmana oli saada yhteys nodeihin. Selain näytti virheitä kuten tracker connection error ja content.json download failed, mikä tarkoitti että ohjelma ei löytänyt vertaisverkosta muita käyttäjiä eikä pystynyt lataamaan sivun sisältöä.  
<img width="1920" height="921" alt="Screenshot From 2026-02-10 15-20-19" src="https://github.com/user-attachments/assets/eeb6f392-eb6d-4a24-91bf-692348e5b799" />  
Odotettuani pitkään, käynnistin ZeroNetin aluksi Torin kautta (--tor always), mutta yhteyden muodostaminen epäonnistui sitäkin kautta, ja sivujen lataaminen ei vieläkään onnistunut. Käynnistin ohjelman uudelleen ilman Toria (--tor disable), ja ZeroNet muodosti vihdoin suoran vertaisyhteyden ja sain sivut avattua normaalisi. PÄäsin esimerkiksi sivulle ZeroTAlk.
<img width="1920" height="921" alt="Screenshot From 2026-02-10 15-39-42" src="https://github.com/user-attachments/assets/93595568-f362-4a42-9453-05ab5fb207c0" />
<img width="1920" height="921" alt="Screenshot From 2026-02-10 15-37-16" src="https://github.com/user-attachments/assets/2ca813c5-950f-47b0-bf5a-c393152cb97d" />  

## Uhkamalli  
ZeroNetin tavoite on sensuurin vastustus ja hajautettu sisällön jakaminen. Uhkamallissa voidaan olettaa että hyökkääjä voi yrittää estää sivuja tai seurata niiden liikennettä. Mutta koska data on jaettu usealle eri vertaiskäyttäjälle, hyökkääjä ei voi sulkeea yksittäistä palvelinta.  
## Protokolla  
ZeroNet käyttää vertaisverkkoa (P2P) ja BitTorrent tiedonsiirtoa. Sivustot allekirjoitetaan kryptografisilla avaimilla, jotta niiden sisältö voidaan varmistaa aidoksi. Halutessaan käyttäjä voi ohjata liikenteen Tor-verkon kautta parantaakseen anonyymiteettiä.  
## Toimintaperiaate  
ZeroNetissä sivut ladataan muilta käyttäjiltä eikä keskuspalvelinta ole. Käyttäjän avatessa sivun, se latautuu omalle koneelle, ja jakaa sitä samalla eteenpäin muille. Tämän takia verkko on vaikeapi sensuroida, mutta siinä on heikompi anonyymiteetti kuin I2P:ssä ja Freenetissä.  

### Vertailu
I2P keskittyy vahvaan anonymiteettiin, sillä liikenne kulkee useiden solmujen läpi, salatuissa yhteyksissä.  Se tekee käyttäjän jäljittämisestä vaikeaa. Samalla verkko on sen takia myös aika hidas ja vaikea käyttää.  
Freenetin isoimpana ideana on sensuurin kiertäminen ja anyymi tiedon jakaminen. Data talletuu hajautetusti muiden käyttäjien koneille, eikä keskuspalvelinta ole. Käsittääkseni se tarjoaa  hyvän anonyymiteetin, mutta vaikutti aika hitaalta ja vanhanaikaiselta.  
ZeroNet toimii myös vertaisverkossa, mutta keskittyy enemmän hajautettuun web-hostingiin, eikä täydelliseen immuuniteettiin. Sivut latautuvat muilta käyttäjiltä BitTorrent-tyyppisesti. Se oli nopeampi kuin I2P ja Freenet, ja käyttöliittymä vaikutti käyttäjäystävällisemmältä.  
Yhteenvetona vaikutukseni kolmesta testatusta darknetistä:
I2P: Vaikutti turvallisimmalta anonymiteetin näkökulmasta.  
Freenet: Vaikutti vahvimmalta sensuurin vastustamisessa.   
ZeroNet: Vaikutti helpoimmalta käyttää.  
Kaikkia yhdistää hajautettu rakenne, mutta ne eroavat siinä, kuinka paljon painottavat anonyymiteettiä, käytettävyyttä ja nopeutta.  


## Lähteet  
https://geti2p.net/en/docs/how/intro  
https://www.hyphanet.org/index.html  
https://zeronet.io/docs/  
ChatGPT: käytin tekoälyä kysyäkseni komentoja linuxeen jäätyäni jumiin muutaman kerran, ja ymmärtääkseni itse komennot paremmin. Teksti on minun kirjoittamani, eikä tekoälyllä generoitu.





