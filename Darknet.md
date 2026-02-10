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
