# Transportlaagprotocollen

##	TCP / IP

TCP/IP is een set van communicatieprotocollen die worden gebruikt om computers met elkaar te laten communiceren over een netwerk. Het protocol bestaat uit twee delen: het Transmission Control Protocol (TCP) en het Internet Protocol (IP). TCP wordt gebruikt om ervoor te zorgen dat gegevens veilig en betrouwbaar worden verzonden tussen computers, terwijl IP ervoor zorgt dat de gegevens op de juiste bestemming terechtkomen.
TCP / IP werkt dus zowel op de transportlaag, als op de netwerklaag.




### Het TCP-protocol
TCP (Transmission Control Protocol) is een protocol dat wordt gebruikt voor het verzenden en ontvangen van gegevens tussen computers over een netwerk. TCP maakt deel uit van de TCP/IP-protocolfamilie, die de basis vormt van het internet.

#### Het virtueel verbinden van applicaties
TCP verbindt eigenlijk 2 applicaties (cliënt en server-applicatie) met elkaar. Deze bevinden zich normaal op een andere computer, op een ander netwerk.

Voor het addresseren van de 2 applicaties hebben we dus 2 zaken nodig: 
* het IP-adres, waarmee we de juiste computer adresseren
* een poortnummer, waarmee we de juiste applicatie adresseren. 

##### Poorten

In een computersysteem krijgt elk proces dat via het internet communiceert een uniek poortnummer toegewezen. Poortnummers worden gebruikt om te identificeren welk proces of welke applicatie gegevens verzendt of ontvangt via het netwerk. Ze maken het mogelijk dat meerdere processen op dezelfde computer tegelijkertijd verbinding kunnen maken met verschillende servers op het internet, zonder dat ze elkaar in de weg zitten.

Bijvoorbeeld, als een webbrowser een webpagina aanvraagt van een webserver, gebruikt de browser een willekeurig poortnummer om verbinding te maken met de webserver. De webserver stuurt vervolgens de gevraagde pagina terug naar het poortnummer dat de browser heeft gebruikt om de verbinding tot stand te brengen. Op deze manier kan de browser meerdere verbindingen tegelijkertijd maken met verschillende webservers en kan de server ook verbinding maken met meerdere clients tegelijkertijd.

Er zijn twee soorten poorten: bekende poorten en dynamische poorten. Bekende poorten hebben een vast nummer en worden gebruikt door veelgebruikte applicaties zoals e-mail, webbrowsers en FTP-clients. Dynamische poorten zijn poorten die tijdelijk worden toegewezen aan applicaties wanneer ze worden gestart.

Hier zijn enkele veelgebruikte poorten en hun functies:

* Poort 80: HTTP (Hypertext Transfer Protocol) - gebruikt voor webbrowsers om webpagina's op te halen
* Poort 443: HTTPS (Hypertext Transfer Protocol Secure) - gebruikt voor veilige webpagina's met versleutelde gegevens
* Poort 25: SMTP (Simple Mail Transfer Protocol) - gebruikt voor het verzenden van e-mail
* Poort 110: POP3 (Post Office Protocol version 3) - gebruikt voor het ophalen van e-mail
* Poort 143: IMAP (Internet Message Access Protocol) - gebruikt voor het ophalen van e-mail op een server

##### Algemene werking
TCP houdt geen rekening met tussenliggende verbindingen, en werkt alsof 2 computers rechtstreeks met elkaar verbonden zijn. 
* verbinding maken tussen 2 computers: Er wordt een verbinding gemaakt tussen 2 computers voor het verzenden van bepaalde informatie (drieweghandshake). Er wordt informatie uitgewisseld over de grootte van het pakketje, en de gewenste overdrachtsnelheid.
* Segmenteren van gegevens: Deze informatie wordt in segmentjes verdeeld, en genummerd, zodat deze informatie bij de ontvanger opnieuw kan samengesteld worden, en naar de juiste poort kan doorgestuurd worden. 


* Biedt een verzekerde gegevensoverdracht: TCP verstuurt elk segment met behulp van IP. Het IP is een best-effort protocol, en kan dus niet garanderen dat alle segmentjes toekomen. TCP controleert dus of elk (genummerd) segmentje toegekomen is. De ontvangende computer doet een foutcontrole op de pakketjes, stuurt voor elk ontvangen segment een berichtje (goed aangekomen of niet) naar de verzender. Als een pakketje na een bepaalde tijd niet toegekomen is, wordt er een verzoek verstuurd om opnieuw te versturen.





##### congestie-controle mechanisme

Daarnaast is TCP ook verantwoordelijk voor het controleren van de stroom van gegevens tussen computers. Dit betekent dat als er op een bepaalde plaats op het net te veel gegevens in één keer passeren (er is congestie, of file), TCP de stroom van gegevens kan vertragen om te voorkomen dat de ontvangende computer overbelast raakt.

Ten slotte maakt TCP ook gebruik van een driewegshandshake om een verbinding tussen twee computers tot stand te brengen voordat gegevens kunnen worden verzonden. Dit betekent dat beide computers moeten bevestigen dat ze klaar zijn om gegevens uit te wisselen voordat ze dat daadwerkelijk kunnen doen.

Kortom, TCP is een belangrijk protocol voor het verzenden van gegevens over het internet, omdat het ervoor zorgt dat gegevens betrouwbaar worden afgeleverd en dat de stroom van gegevens wordt gecontroleerd om overbelasting te voorkomen.





## UDP

UDP is een variant van TCP, wordt ook gebruikt voor de verzending van gegevens over een netwerk, werkt net als TCP met poortnummers, en ook met het IP protocol. 
We zouden dus eigenlijk kunnen spreken over UDP/TCP. Dit gebeurt niet, UDP heeft geen zo'n belangrijke invloed op het internet (congestiecontrole etc) als TCP

##### Verbindingsloos protocol: onzekere gegevensoverdracht
Het belangrijkste verschil tussen UDP en TCP is dat UDP een verbindingsloos protocol is, terwijl TCP een verbindingsgeoriënteerd protocol is. Dit betekent dat UDP geen verbinding opzet tussen de zender en de ontvanger, terwijl TCP dat wel doet. Bij UDP worden gegevens gewoon verzonden naar de ontvanger zonder dat er een bevestiging wordt ontvangen. 
Dit maakt UDP snel, maar minder betrouwbaar, omdat er geen garantie is dat de gegevens aankomen en in de juiste volgorde worden ontvangen. UDP is daarom geschikt voor toepassingen waar snelheid belangrijker is dan betrouwbaarheid, zoals online gaming of streaming van video.

TCP, aan de andere kant, zorgt voor een betrouwbare verbinding tussen de zender en de ontvanger. Wanneer gegevens worden verzonden via TCP, wordt er een verbinding opgezet tussen de zender en de ontvanger voordat de gegevens worden verzonden. Dit betekent dat er een bevestiging wordt ontvangen dat de gegevens zijn aangekomen en in de juiste volgorde zijn ontvangen. TCP is daarom geschikt voor toepassingen waar betrouwbaarheid belangrijker is dan snelheid, zoals het downloaden van bestanden of het versturen van e-mails.

##### Sneller als TCP
Een ander verschil tussen UDP en TCP is dat TCP meer overhead heeft dan UDP. Dit komt doordat TCP meer gegevens gebruikt om de verbinding op te zetten en te onderhouden. Hierdoor is TCP langzamer dan UDP en is het minder geschikt voor toepassingen waar snelheid van belang is.

Kortom, UDP en TCP zijn beide protocollen voor de verzending van gegevens over een netwerk, maar ze verschillen in snelheid, betrouwbaarheid en overhead. UDP is snel, maar minder betrouwbaar, terwijl TCP betrouwbaar is, maar minder snel en heeft meer overhead. De keuze tussen UDP en TCP hangt af van de specifieke toepassing en de prioriteit van snelheid versus betrouwbaarheid.


Hieronder staan enkele voorbeelden van TCP- en UDP-toepassingen:

###### TCP:

* HTTP (Hypertext Transfer Protocol): wordt gebruikt voor het verzenden van webpagina's via internet
* FTP (File Transfer Protocol): wordt gebruikt voor het verzenden van bestanden over internet
* SMTP (Simple Mail Transfer Protocol): wordt gebruikt voor het verzenden van e-mails
* SSH (Secure Shell): wordt gebruikt voor beveiligde toegang tot een server
* Telnet: wordt gebruikt voor op afstand inloggen op een server

###### UDP:

* DNS (Domain Name System): wordt gebruikt voor het vertalen van domeinnamen naar IP-adressen
* DHCP (Dynamic Host Configuration Protocol): wordt gebruikt voor het toewijzen van IP-adressen aan apparaten in een netwerk
* VoIP (Voice over IP): wordt gebruikt voor het verzenden van spraak over internet
* Video streaming: wordt gebruikt voor het streamen van video's over internet, zoals YouTube of Netflix
* Online gaming: wordt gebruikt voor real-time online gaming, waar snelheid belangrijker is dan betrouwbaarheid.

Dit zijn slechts enkele voorbeelden van de vele toepassingen van TCP en UDP. Welk protocol het meest geschikt is, hangt af van de specifieke toepassing en de prioriteit van snelheid versus betrouwbaarheid.
