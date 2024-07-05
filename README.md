# Radio Hami broadcast tools

Broadcast tools repo for Radio Hami 2024 project, in Joensuu, Finland.

The whole team is Finnish-speaking so...

Tänne vaan kaikki issuet ja koodinpätkät, mitä operaatiosta syntyy. Jos myöhemmin tulee halua tehdä orkesterointia niin näiden pohjalta voi lähteä rakentelemaan.

## Vaatimusmäärittely

Jakelukoneella on seuraavat vaatimukset:

* Kyky vastaanottaa ääntä AES67:lla ja välittää monitorointiääntä takaisin
* Äänen prosessointi hunajaiseksi
* MPX:n muodostaminen (192kHz mono) FM-lähetyksiä varten
* DAB-ensemblen multipleksaus ja digitaaliäänikanavan/kanavien enkoodaus.
* E1-sarjaliikenteen muodostaminen DAB-modulaattoria varten
* Nettiradiostriimien muodostaminen (Opus ja MP3) nettiradiojakelua varten
* Kyky selvityä uudelleenkäynnistyksistä (palvelut lähtevät päälle oikein bootissa)
* Kyky selviytyä tietokoneen jumiutumisesta (hw watchdog)
* Referenssitaltioinnin tekeminen lähetyksestä
* Metatietojen tuottaminen eri medioihin (nettiradio, RDS, Journaline?)
* Vikasietoinen levyjärjestelmä (RAID1 tai RAID5 sekä snapshottausta tukeva levyjärjestelmä)
