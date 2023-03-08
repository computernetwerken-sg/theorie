# Routering 

Routering is een functie van de netwerklaag in het netwerklaagmodel. De netwerklaag is verantwoordelijk voor het verzenden en routeren van gegevens tussen verschillende netwerken en apparaten. Het maakt gebruik van IP-adressen om gegevens te identificeren en routeringstabellen om te bepalen welke route de gegevens moeten volgen om hun bestemming te bereiken. 
Routing is het proces van het doorsturen van gegevens vanaf de bron naar de bestemming via verschillende netwerken. Het doel van routing is om gegevens zo efficiënt mogelijk te verzenden van het ene apparaat naar het andere. Hier zijn enkele belangrijke punten om te begrijpen over routing in computernetwerken:

*	Elk apparaat op het netwerk heeft een uniek IP-adres dat wordt gebruikt om gegevens te identificeren en te verzenden.
*	Routeringstabellen worden gebruikt om te bepalen welke weg de gegevens moeten volgen om de bestemming te bereiken.
*	Er zijn verschillende routingprotocollen beschikbaar, zoals OSPF en BGP, die worden gebruikt om de beste route te bepalen op basis van verschillende criteria, zoals snelheid, kosten en betrouwbaarheid.
*	Er zijn twee soorten routing: statische routing, waarbij de routes handmatig worden geconfigureerd, en dynamische routing, waarbij de routes automatisch worden bijgewerkt op basis van wijzigingen in het netwerk.
*	Een goede configuratie en beheer van de routing is essentieel om een stabiele en efficiënte netwerkverbinding te garanderen.
*	Door een goed begrip van routing en de verschillende technologieën en protocollen die beschikbaar zijn, kan een efficiënte en betrouwbare netwerkverbinding worden gerealiseerd.

##	TCP / IP

###	Het IP-protocol

Het IP-protocol (Internet Protocol) is een netwerkprotocol dat wordt gebruikt om gegevens te verzenden over het internet en andere computernetwerken. Het maakt deel uit van de netwerklaag van het TCP/IP-model en is verantwoordelijk voor het routeren van gegevenspakketten van de bron naar de bestemming.
Wanneer gegevens worden verzonden vanaf een bronapparaat naar een bestemmingsapparaat via het internet, worden de gegevens opgesplitst in kleine pakketjes. Elk pakketje bevat een deel van de gegevens, samen met het IP-adres van de bron en het IP-adres van de bestemming. Het pakketje wordt vervolgens verzonden via het netwerk naar de bestemming.

Het IP-protocol heeft twee belangrijke taken: adreszuivering en routering. # adreszuivering
#### adreszuivering
Adreszuivering is het proces van pakketjes maken, en het toevoegen van een IP-adres aan elk pakketje om het te identificeren en te verzenden naar de juiste bestemming. 

#### Routering
Routering is het proces van het bepalen van de beste route voor het pakketje om de bestemming te bereiken, op basis van de beschikbare netwerkverbindingen en routers.


#### best-effort principe
Het IP-protocol maakt gebruik van het beste effort-principe, wat betekent dat het pakketje wordt verzonden zonder garantie van levering of kwaliteit van de verbinding. Het kan dus voorkomen dat pakketjes verloren gaan of vertraging oplopen in het netwerk. Dit wordt opgevangen door hogere lagen van het TCP/IP-model, zoals TCP (Transmission Control Protocol), die de betrouwbaarheid van de verbinding garanderen.

Kortom, het IP-protocol is de basis van communicatie over het internet en andere computernetwerken. Het verzendt gegevenspakketjes van de bron naar de bestemming door middel van adreszuivering en routering. Het is een belangrijk onderdeel van het TCP/IP-model en wordt gebruikt in combinatie met andere protocollen om betrouwbare communicatie te garanderen.


## Het TCP-protocol
TCP (Transmission Control Protocol) is een protocol dat wordt gebruikt voor het verzenden en ontvangen van gegevens tussen computers over een netwerk. TCP maakt deel uit van de TCP/IP-protocolfamilie, die de basis vormt van het internet.

TCP zorgt ervoor dat gegevens betrouwbaar worden afgeleverd door ervoor te zorgen dat elk gegevenspakketje dat wordt verzonden, wordt gecontroleerd op fouten en indien nodig opnieuw wordt verzonden. Dit gebeurt door middel van bevestigingen (ACKs) en sequentienummers die aan elke gegevensstroom worden toegewezen. Dit betekent dat als er onderweg een pakketje verloren gaat, het opnieuw wordt verzonden totdat het correct is ontvangen.

TCP is ook verantwoordelijk voor het controleren van de stroom van gegevens tussen computers. Dit betekent dat als een computer te veel gegevens in één keer probeert te verzenden, TCP de stroom van gegevens kan beperken om te voorkomen dat de ontvangende computer overbelast raakt.

Ten slotte maakt TCP ook gebruik van een driewegshandshake om een verbinding tussen twee computers tot stand te brengen voordat gegevens kunnen worden verzonden. Dit betekent dat beide computers moeten bevestigen dat ze klaar zijn om gegevens uit te wisselen voordat ze dat daadwerkelijk kunnen doen.

Kortom, TCP is een belangrijk protocol voor het verzenden van gegevens over het internet, omdat het ervoor zorgt dat gegevens betrouwbaar worden afgeleverd en dat de stroom van gegevens wordt gecontroleerd om overbelasting te voorkomen.

## TCP/IP
TCP/IP is een set van communicatieprotocollen die worden gebruikt om computers met elkaar te laten communiceren over een netwerk. Het protocol bestaat uit twee delen: het Transmission Control Protocol (TCP) en het Internet Protocol (IP). TCP wordt gebruikt om ervoor te zorgen dat gegevens veilig en betrouwbaar worden verzonden tussen computers, terwijl IP ervoor zorgt dat de gegevens op de juiste bestemming terechtkomen.

Om de communicatie tussen computers mogelijk te maken, worden er poorten gebruikt. Een poort is een nummer dat aan een specifieke applicatie wordt toegewezen, zodat de applicatie kan worden geïdentificeerd en gegevens kan verzenden en ontvangen via het netwerk.

Er zijn twee soorten poorten: bekende poorten en dynamische poorten. Bekende poorten hebben een vast nummer en worden gebruikt door veelgebruikte applicaties zoals e-mail, webbrowsers en FTP-clients. Dynamische poorten zijn poorten die tijdelijk worden toegewezen aan applicaties wanneer ze worden gestart.

Hier zijn enkele veelgebruikte poorten en hun functies:

* Poort 80: HTTP (Hypertext Transfer Protocol) - gebruikt voor webbrowsers om webpagina's op te halen
* Poort 443: HTTPS (Hypertext Transfer Protocol Secure) - gebruikt voor veilige webpagina's met versleutelde gegevens
* Poort 25: SMTP (Simple Mail Transfer Protocol) - gebruikt voor het verzenden van e-mail
* Poort 110: POP3 (Post Office Protocol version 3) - gebruikt voor het ophalen van e-mail
* Poort 143: IMAP (Internet Message Access Protocol) - gebruikt voor het ophalen van e-mail op een server

### Werking
Om pakketten te versturen en te ontvangen, is het belangrijk om het IP-adres van de bestemming te kennen. Een IP-adres is een uniek identificatienummer dat aan elke computer of apparaat is toegewezen dat is aangesloten op een netwerk. Het IP-adres vertelt het netwerk waar het pakket naartoe moet worden gestuurd. Het IP-adres is vergelijkbaar met het adres op een enveloppe waarmee je een brief naar de juiste persoon op het juiste adres stuurt.

Naast het IP-adres is ook het poortnummer belangrijk om pakketten te versturen en te ontvangen. Een poortnummer is een nummer dat aan een specifieke toepassing is toegewezen, zodat gegevens van en naar die toepassing kunnen worden gestuurd. Een poortnummer is vergelijkbaar met de kamer- of afdelingsnummer op een adres, dat vertelt waar binnen een gebouw de brief moet worden afgeleverd.

Wanneer een apparaat een pakket verzendt,UDP en TCP zijn beide protocollen die worden gebruikt voor de verzending van gegevens over een netwerk, maar er zijn belangrijke verschillen tussen de twee protocollen.


### UDP

UDP is een variant van TCP, wordt ook gebruikt voor de verzending van gegevens over een netwerk, werkt net als TCP met poortnummers, en ook met het IP protocol. Er zijn echter enkele belangrijke verschillen:

Het belangrijkste verschil tussen UDP en TCP is dat UDP een verbindingsloos protocol is, terwijl TCP een verbindingsgeoriënteerd protocol is. Dit betekent dat UDP geen verbinding opzet tussen de zender en de ontvanger, terwijl TCP dat wel doet. Bij UDP worden gegevens gewoon verzonden naar de ontvanger zonder dat er een bevestiging wordt ontvangen. Dit maakt UDP snel, maar minder betrouwbaar, omdat er geen garantie is dat de gegevens aankomen en in de juiste volgorde worden ontvangen. UDP is daarom geschikt voor toepassingen waar snelheid belangrijker is dan betrouwbaarheid, zoals online gaming of streaming van video.

TCP, aan de andere kant, zorgt voor een betrouwbare verbinding tussen de zender en de ontvanger. Wanneer gegevens worden verzonden via TCP, wordt er een verbinding opgezet tussen de zender en de ontvanger voordat de gegevens worden verzonden. Dit betekent dat er een bevestiging wordt ontvangen dat de gegevens zijn aangekomen en in de juiste volgorde zijn ontvangen. TCP is daarom geschikt voor toepassingen waar betrouwbaarheid belangrijker is dan snelheid, zoals het downloaden van bestanden of het versturen van e-mails.

Een ander verschil tussen UDP en TCP is dat TCP meer overhead heeft dan UDP. Dit komt doordat TCP meer gegevens gebruikt om de verbinding op te zetten en te onderhouden. Hierdoor is TCP langzamer dan UDP en is het minder geschikt voor toepassingen waar snelheid van belang is.

Kortom, UDP en TCP zijn beide protocollen voor de verzending van gegevens over een netwerk, maar ze verschillen in snelheid, betrouwbaarheid en overhead. UDP is snel, maar minder betrouwbaar, terwijl TCP betrouwbaar is, maar minder snel en heeft meer overhead. De keuze tussen UDP en TCP hangt af van de specifieke toepassing en de prioriteit van snelheid versus betrouwbaarheid.


Hieronder staan enkele voorbeelden van TCP- en UDP-toepassingen:

#### TCP:

* HTTP (Hypertext Transfer Protocol): wordt gebruikt voor het verzenden van webpagina's via internet
* FTP (File Transfer Protocol): wordt gebruikt voor het verzenden van bestanden over internet
* SMTP (Simple Mail Transfer Protocol): wordt gebruikt voor het verzenden van e-mails
* SSH (Secure Shell): wordt gebruikt voor beveiligde toegang tot een server
* Telnet: wordt gebruikt voor op afstand inloggen op een server

#### UDP:

* DNS (Domain Name System): wordt gebruikt voor het vertalen van domeinnamen naar IP-adressen
* DHCP (Dynamic Host Configuration Protocol): wordt gebruikt voor het toewijzen van IP-adressen aan apparaten in een netwerk
* VoIP (Voice over IP): wordt gebruikt voor het verzenden van spraak over internet
* Video streaming: wordt gebruikt voor het streamen van video's over internet, zoals YouTube of Netflix
* Online gaming: wordt gebruikt voor real-time online gaming, waar snelheid belangrijker is dan betrouwbaarheid.

Dit zijn slechts enkele voorbeelden van de vele toepassingen van TCP en UDP. Welk protocol het meest geschikt is, hangt af van de specifieke toepassing en de prioriteit van snelheid versus betrouwbaarheid.


##	Mac-adressen en ARP

De verbindingslaag, ook wel bekend als de data link laag, is de laag in het netwerkprotocolmodel die verantwoordelijk is voor het overbrengen van gegevens tussen aangrenzende netwerken, zoals tussen een computer en een switch op een Ethernet-netwerk.

De verbindingslaag gebruikt MAC-adressen (Media Access Control-adressen) om netwerkapparaten te identificeren en te communiceren. Elk netwerkapparaat heeft een uniek MAC-adres dat is ingebakken in de netwerkadapter van het apparaat.

Waarom gebruikt de verbindingslaag MAC-adressen in plaats van IP-adressen?
MAC-adressen zijn gegarandeerd uniek en worden toegewezen aan netwerkapparaten door hun fabrikanten. Hierdoor is het gemakkelijk om een uniek apparaat te identificeren op het netwerk, zelfs als het IP-adres van het apparaat verandert.

ARP staat voor Address Resolution Protocol. Het is een protocol dat wordt gebruikt in computernetwerken om een IP-adres te koppelen aan het fysieke MAC-adres van een apparaat.
Wanneer een apparaat op het netwerk gegevens wil verzenden naar een ander apparaat, moet het het MAC-adres van de ontvanger kennen om de gegevens naar het juiste apparaat te kunnen verzenden. ARP wordt gebruikt om dit te bereiken.

Het ARP-protocol werkt als volgt:
Het apparaat dat gegevens wil verzenden (de zender) zoekt in de ARP-cache (een tijdelijke opslag van recent gebruikte MAC-adressen) om te zien of het MAC-adres van de ontvanger al bekend is.
Als het MAC-adres niet bekend is, stuurt de zender een ARP-verzoek naar het netwerk waarin het IP-adres van de ontvanger wordt vermeld.
Het apparaat met het bijbehorende IP-adres ontvangt het ARP-verzoek en stuurt een ARP-reactie terug met het bijbehorende MAC-adres.
De zender ontvangt het ARP-antwoord en kan nu de gegevens verzenden naar de juiste bestemming.
ARP is een belangrijk protocol voor het verzenden van gegevens over het netwerk. Zonder ARP zou het verzenden van gegevens veel langzamer en inefficiënter zijn, omdat de zender handmatig het MAC-adres van de ontvanger zou moeten achterhalen voordat gegevens kunnen worden verzonden.
je kan de arp-cache opvragen op je computer op de CLI met het commando "arp -a"

### Het DHCP protocol

DHCP staat voor Dynamic Host Configuration Protocol en is een netwerkprotocol dat wordt gebruikt om IP-adressen en andere netwerkconfiguraties automatisch toe te wijzen aan apparaten die zijn verbonden met een netwerk. Hieronder vindt u enkele belangrijke punten om te begrijpen over de werking van DHCP:

*	Wanneer een apparaat wordt aangesloten op een netwerk, stuurt het apparaat een verzoek naar het netwerk voor een IP-adres en andere configuratie-informatie. (DHCP-request)
*	De DHCP-server ontvangt dit verzoek en kent een IP-adres en andere netwerkconfiguraties toe aan het apparaat.
Dit proces gebeurt automatisch en dynamisch, wat betekent dat een apparaat een nieuw IP-adres kan krijgen elke keer dat het opnieuw verbinding maakt met het netwerk.
DHCP bespaart tijd en maakt netwerkbeheer efficiënter door het handmatig toewijzen van IP-adressen en andere netwerkconfiguraties te vervangen.

### Beschrijf de werking van DNS.

DNS staat voor Domain Name System en is een netwerkprotocol dat wordt gebruikt om hostnamen (zoals www.example.com) om te zetten in IP-adressen (zoals 192.0.2.1) die computers begrijpen. Hieronder vindt u enkele belangrijke punten om te begrijpen over de werking van DNS:
* Wanneer u een website wilt bezoeken, typt u de hostnaam in de webbrowser (zoals www.example.com).
*	De webbrowser stuurt vervolgens een verzoek naar een DNS-server om het bijbehorende IP-adres van de hostnaam op te halen.
*	De DNS-server zoekt het IP-adres op in zijn database en stuurt het terug naar de webbrowser.
*	De webbrowser gebruikt het IP-adres om verbinding te maken met de webserver waarop de website wordt gehost.
*	Dit hele proces gebeurt achter de schermen en is voor de meeste gebruikers onzichtbaar.
*
