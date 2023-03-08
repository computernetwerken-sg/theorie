# Basis computernetwerken

## Welke diensten kunnen in een computernetwerk worden aangeboden?
Sleutelboek p 8

##	Het client-servermodel 

Het client-servermodel is een voor de samenwerking tussen twee of meer programma's, die zich op verschillende computers kunnen bevinden. Kenmerkend in het model is:
* de server is permanent beschikbaar (‘altijd aan’) en is reactief
* een client is bij gelegenheid actief en neemt het initiatief tot communicatie met de server
Een aantal voorbeelden van het client-servermodel zijn e-mail, het www, NFS, FTP, Telnet, SSH, online-FPS, betalingsverkeer,…
Een alternatief netwerkmodel is een peer-to-peerarchitectuur. Omdat dit veel complexer is, en ook niet zo vaak voorkomt, bespreken we dit niet in deze cursus.

### Server

Een server is een computer of een programma dat diensten verleent aan clients. In de eerste betekenis wordt met server de fysieke computer aangeduid waarop een programma draait dat deze diensten verleent.

Een server is dus een computer waarop een programma draait die een dienst levert aan clients. Een computer kan meerdere diensten combineren: zo kan je op één computer (server in de hardwarebetekenis van het woord) meerdere diensten (server in de softwarebetekenis van het woord) leveren.

Een server is normaal altijd aan: deze dienst mag nooit onderbroken worden.

#### Gangbare servertypen
 
•	Bestandsserver
•	Applicatieserver
•	Webserver
•	Mailserver
•	Databaseserver
•	Time-server
•	Printerserver
•	FTP-server
•	DHCP-server
•	DNS-server
•	Proxyserver
•	IRC-server
•	Gameserver
•	Virtual private server
•	Telnet-server
•	Opensource-server
•	Media streaming server
 
#### Besturingssystemen
Servers zijn nogal technisch, en worden beheerd door specialisten. De meest gebruikte besturingssystemen zijn Windows server, Linux (open source) en Unix.

### Client (applicatie)

Een client is een applicatie of een computersysteem met toegang tot een ander systeem, de server, via een netwerk. Men spreekt hierbij van een client-servermodel. 
De client neemt initiatief tot communicatie met de server met als doel bijvoorbeeld het opvragen van gegevens, het overdragen van gegevens of het uitvoeren van een actie op de server. Het begrip wordt zowel gebruikt voor een programma dat communiceert met een serverprogramma, als voor een volledige machine die van de diensten van een server gebruikmaakt.
Doorgaans bestaat een clientprogramma onder andere uit een gebruikersinterface, zoals een grafische gebruikersinterface (GUI), en is het voor de eindgebruiker totaal transparant, welk deel van het werk door de client wordt verricht, en welk deel door de server. Voorbeelden van clients zijn e-mailclients en webbrowsers, maar ook een game (op computer of op spelconsole) kan een cliënt zijn van een server, indien er bvb multiplayer gespeeld wordt.
De Client applicatie is vaak het front-end development onderdeel van een applicatie. De front-end ontwikkeling is het programmeren van de “voorkant” van de applicatie. De voorkant is datgene wat zichtbaar is voor de bezoeker van bijvoorbeeld een website: de afbeeldingen, de layout, het lettertypen, kortom het dashboard van de gebruiker.

## Netwerkkaart 
###	Wat is een netwerkkaart / hoe wordt deze geïdentificeerd?
Sleutelboek computernetwerken p 54

#### Is een netwerkkaart en een interface hetzelfde?
Nee, een interface en een netwerkkaart zijn niet hetzelfde, hoewel ze soms wel in verband worden gebracht met elkaar.

Een interface is een softwarematige of hardwarematige component waarmee een apparaat communiceert met andere apparaten of systemen. Een interface kan bijvoorbeeld een grafische gebruikersinterface (GUI) zijn die een gebruiker helpt om te communiceren met een computerprogramma, of het kan een netwerkinterface zijn die een apparaat in staat stelt om te communiceren met andere apparaten in een netwerk.

Een netwerkkaart daarentegen is een specifieke hardwarecomponent die wordt gebruikt om een apparaat aan te sluiten op een netwerk, meestal via een Ethernet-kabel of draadloze verbinding. Een netwerkkaart kan als interface fungeren tussen het apparaat en het netwerk, maar een interface kan ook andere functies hebben die niet gerelateerd zijn aan netwerkcommunicatie.

Kortom, een netwerkkaart is een specifiek type interface dat wordt gebruikt voor netwerkcommunicatie, maar niet alle interfaces zijn netwerkkaarten.

## Transportmedia

### Algemeen
Sleutelboek computernetwerken p 55 ev
4.1	Kenmerken
4.2	Coaxiale kabel
4.3	Twisted pair
Je kan zelf een netwerkkabel maken
4.4	Glasvezel
4.5	Powerline
4.6	WiFI
•	IEEE 802.11ac (WiFi 5) werkt enkel in de 5GHz-band, dit via meerdere antennes.
•	IEEE 802.11ax (WiFi 6 voor 2,4 en 5 GHz, WiFi 6E voor 6 GHz) is een opvolger van 802.11ac en introduceerde een nieuwe frequentieband; 6 GHz.[11]
•	IEEE 802.11be (WiFi 7) Extremely High Throughput (EHT) introduceert 320 MHz bandbreedte, 16 spatial streams en 4096-QAM. Met een maximale doorvoer van 46 gigabits per seconde

### EletroMagnetische Interferentie (EMI)

Elektromagnetische interferentie (EMI) is een veelvoorkomend probleem dat kan optreden op netwerkkabels, zoals twisted pair en coax. EMI wordt veroorzaakt door elektromagnetische velden die worden opgewekt door andere elektronische apparaten in de buurt, zoals elektrische motoren, verlichting, radiosignalen en mobiele telefoons. Deze elektromagnetische velden kunnen de signaaloverdracht op de kabels verstoren en zo de prestaties van het netwerk beïnvloeden.
Twisted pair-kabels hebben het voordeel dat ze een natuurlijke afscherming tegen EMI hebben door hun draaiingen. Hoe meer de kabel is gedraaid, hoe minder last er is van EMI. 
Coaxkabels hebben daarentegen een speciale opbouw die de interferentie van elektromagnetische velden vermindert. Ze hebben een centrale geleider (die zorgt voor de gegevensoverdracht) die wordt omgeven door een isolerende laag en een gevlochten afscherming van koperdraden, die voorkomt dat externe elektromagnetische velden doordringen tot de centrale geleider.
Oorzaken van EMI:
•	Elektrische apparaten: Elektrische apparaten, zoals motoren en verlichting, genereren elektromagnetische velden die kunnen interfereren met de signalen op de netwerkkabels.
•	Radiosignalen: Radiosignalen, zoals die van mobiele telefoons en radio- en tv-zenders, kunnen ook EMI veroorzaken.
•	Slecht ontworpen apparatuur: Slecht ontworpen apparatuur kan gevoeliger zijn voor EMI en kan het probleem verergeren.

Gevolgen van EMI:
•	Vermindering van signaalkwaliteit: EMI kan de kwaliteit van het signaal op de kabel verminderen, wat kan leiden tot vertragingen en verminderde prestaties van het netwerk.
•	Verlies van gegevens: Bij hoge niveaus van EMI kunnen gegevens op de kabel verloren gaan of beschadigd raken, waardoor ze niet goed worden ontvangen.
•	Verminderde snelheid: EMI kan de snelheid van het netwerk verminderen, wat kan leiden tot lagere doorvoersnelheden en een slechte gebruikerservaring.

Om EMI op netwerkkabels te verminderen, kunnen de volgende maatregelen worden genomen:
•	Kies een goed afgeschermde kabel: Kies kabels met een goede afscherming om de interferentie van elektromagnetische velden te verminderen.
•	Gebruik afgeschermde connectoren: Zorg ervoor dat de connectoren van de kabel ook afgeschermd zijn om EMI te verminderen.
•	Vermijd interferentiebronnen: Plaats het netwerk zo ver mogelijk weg van bronnen van EMI, zoals elektrische apparaten.
•	Gebruik repeaters: Gebruik repeaters om het signaal te versterken en de afstand tussen apparaten te vergroten.
Door deze maatregelen te nemen, kan de impact van EMI op netwerkkabels worden verminderd en kan de prestatie van het netwerk worden verbeterd.
6	Netwerktopologieën
Sleutelboek computernetwerken p 28-30.

###	Collision domain

Een bepaald transportmedium kan slechts 1 signaal per keer transporteren. Indien meerdere toestellen op hetzelfde moment een signaal op hetzelfde medium plaatsen, worden beide signalen onbruikbaar, en moeten ze opnieuw verstuurd worden.
Hoe meer toestellen aangesloten worden op hetzelfde medium, hoe groter de kans op een botsing - collision. 
Broadcast domain is dus dat deel van een netwerk, van alle toestellen die op hetzelfde medium aangesloten zijn, en die kunnen botsen. Daarvoor worden in een sternetwerk tegenwoordig altijd switches gebruikt (ipv hubs), zo is er slechts een kleine kans op botsing.
Bij draadloze netwerken is dit wel een belangrijke factor: hoe meer computers aangesloten op een netwerk, hoe groter de kans op een botsing, hoe meer berichten opnieuw verstuurd moeten worden, en hoe trager het netwerk dus werkt.

###	Broadcast domain
Een broadcast domain bevat alle computers in hetzelfde netwerk. Alle computers aangesloten op dezelfde switch behoren dus tot hetzelfde broadcast domain. 
Broadcast domains worden van elkaar gescheiden door routers.

###	LAN en  WAN

LAN staat voor Local Area Network en verwijst naar een netwerk dat zich bevindt binnen een beperkt gebied, zoals een kantoor, school of huis. Dit soort netwerken worden vaak gebruikt om apparaten met elkaar te verbinden, zoals computers, printers en servers, zodat ze gegevens kunnen uitwisselen en resources kunnen delen.

WAN staat voor Wide Area Network en verwijst naar een netwerk dat zich uitstrekt over een groot geografisch gebied, zoals een stad, een land of zelfs de hele wereld. WAN's maken gebruik van verschillende technologieën, zoals telefoonlijnen, glasvezelkabels, satellieten en radiofrequenties, om grote hoeveelheden gegevens over grote afstanden te verzenden.
