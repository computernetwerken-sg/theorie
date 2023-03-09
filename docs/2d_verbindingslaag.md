

#	De verbindingslaag

## Netwerkkaart 

###	Wat is een netwerkkaart / hoe wordt deze geïdentificeerd?

Een netwerkkaart is een specifieke hardwarecomponent die wordt gebruikt om een apparaat aan te sluiten op een netwerk, meestal via een Ethernet-kabel of draadloze verbinding. Een netwerkkaart kan als interface fungeren tussen het apparaat en het netwerk. Elke netwerkkaart heeft zijn eigen mac-adres.
Een computer kan meerder netwerkkaarten hebben, en dus ook meerdere mac-adressen.

#### Is een netwerkkaart en een interface hetzelfde?
Nee, een interface en een netwerkkaart zijn niet hetzelfde, hoewel ze soms wel in verband worden gebracht met elkaar.

Een interface is een softwarematige of hardwarematige component waarmee een apparaat communiceert met andere apparaten of systemen. Een interface kan bijvoorbeeld een grafische gebruikersinterface (GUI) zijn die een gebruiker helpt om te communiceren met een computerprogramma, of het kan een netwerkinterface zijn die een apparaat in staat stelt om te communiceren met andere apparaten in een netwerk.

Een netwerkkaart daarentegen is een specifieke hardwarecomponent die wordt gebruikt om een apparaat aan te sluiten op een netwerk, meestal via een Ethernet-kabel of draadloze verbinding. Een netwerkkaart kan als interface fungeren tussen het apparaat en het netwerk, maar een interface kan ook andere functies hebben die niet gerelateerd zijn aan netwerkcommunicatie.

Kortom, een netwerkkaart is een specifiek type interface dat wordt gebruikt voor netwerkcommunicatie, maar niet alle interfaces zijn netwerkkaarten.

## Mac-adressen

De verbindingslaag, ook wel bekend als de data link laag, is de laag in het netwerkprotocolmodel die verantwoordelijk is voor het overbrengen van gegevens tussen toestellen op hetzelfde netwerk, zoals tussen een computer en een switch op een Ethernet-netwerk.

De verbindingslaag gebruikt MAC-adressen (Media Access Control-adressen) om netwerkapparaten te identificeren en te communiceren. Elk netwerkapparaat heeft een uniek MAC-adres dat is ingebakken in de netwerkadapter van het apparaat. Netwerkapparaten communiceren dus met elkaar via hun MAC-adres.

## ARP

ARP staat voor Address Resolution Protocol. Het is een protocol dat wordt gebruikt in computernetwerken om een IP-adres te koppelen aan het fysieke MAC-adres van een apparaat. 
Wanneer een apparaat op het netwerk gegevens wil verzenden naar een ander apparaat, moet het het MAC-adres van de ontvanger kennen om de gegevens naar het juiste apparaat te kunnen verzenden. ARP wordt gebruikt om dit te bereiken.

Het ARP-protocol werkt als volgt:
* Het apparaat dat gegevens wil verzenden (de zender) zoekt in de ARP-cache (een tijdelijke opslag van recent gebruikte MAC-adressen) om te zien of het MAC-adres van de ontvanger al bekend is.
je kan de arp-cache opvragen op je computer op de CLI met het commando "arp -a"
* Als het MAC-adres niet bekend is, stuurt de zender een ARP-verzoek naar het netwerk waarin het IP-adres van de ontvanger wordt vermeld.
* Het apparaat met het bijbehorende IP-adres ontvangt het ARP-verzoek en stuurt een ARP-reactie terug met het bijbehorende MAC-adres.
* De zender ontvangt het ARP-antwoord en kan nu de gegevens verzenden naar de juiste bestemming.

ARP is een belangrijk protocol voor het verzenden van gegevens over het netwerk. 


##	Collision domain

Een bepaald transportmedium kan slechts 1 signaal per keer transporteren. 

Indien meerdere toestellen op hetzelfde moment een signaal op hetzelfde medium plaatsen, worden beide signalen onbruikbaar, en moeten ze opnieuw verstuurd worden.
Hoe meer toestellen aangesloten worden op hetzelfde medium, hoe groter de kans op een botsing - collision. 
Broadcast domain is dus dat deel van een netwerk, van alle toestellen die op hetzelfde medium aangesloten zijn, en die kunnen botsen. Daarvoor worden in een sternetwerk tegenwoordig altijd switches gebruikt (ipv hubs), zo is er slechts een kleine kans op botsing. Bij busnetwerken was dit ook een probleem, maar deze topologie wordt tegenwoordig bijna niet meer gebruikt.

Bij draadloze netwerken is dit wel een belangrijke factor: hoe meer computers aangesloten op een wifi-netwerk, hoe groter de kans op een botsing, hoe meer berichten opnieuw verstuurd moeten worden, en hoe trager het netwerk dus werkt.

##	Broadcast domain
Een broadcast domain bevat alle computers in hetzelfde netwerk. Alle computers aangesloten op dezelfde switch behoren dus tot hetzelfde broadcast domain. 
Broadcast domains worden van elkaar gescheiden door routers.

##	LAN en  WAN

LAN staat voor Local Area Network en verwijst naar een netwerk dat zich bevindt binnen een beperkt gebied, zoals een kantoor, school of huis. Dit soort netwerken worden vaak gebruikt om apparaten met elkaar te verbinden, zoals computers, printers en servers, zodat ze gegevens kunnen uitwisselen en resources kunnen delen.

WAN staat voor Wide Area Network en verwijst naar een netwerk dat zich uitstrekt over een groot geografisch gebied, zoals een stad, een land of zelfs de hele wereld. WAN's maken gebruik van verschillende technologieën, zoals telefoonlijnen, glasvezelkabels, satellieten en radiofrequenties, om grote hoeveelheden gegevens over grote afstanden te verzenden.
