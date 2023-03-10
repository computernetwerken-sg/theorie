###	Het IP-protocol

Het IP-protocol (Internet Protocol) is een netwerkprotocol dat wordt gebruikt om gegevens te verzenden over het internet en andere computernetwerken. Het maakt deel uit van de netwerklaag van het TCP/IP-model en is verantwoordelijk voor het routeren van gegevenspakketten van de bron naar de bestemming.
Wanneer gegevens worden verzonden vanaf een bronapparaat naar een bestemmingsapparaat via het internet, worden de gegevens opgesplitst in kleine pakketjes. Elk pakketje bevat een deel van de gegevens, samen met het IP-adres van de bron en het IP-adres van de bestemming. Het pakketje wordt vervolgens verzonden via het netwerk naar de bestemming.

Het IP-protocol heeft twee belangrijke taken: fragmenteren en routering.
#### Fragmenteren
Met fragmenteren bedoelen we het maken van pakketjes, en het toevoegen van het IP-adres van verzender en ontvanger aan de header van elk pakketje om het te identificeren en te verzenden naar de juiste bestemming. 

#### Routering
Routering is het proces van het bepalen van de beste route voor het pakketje om de bestemming te bereiken, op basis van de beschikbare netwerkverbindingen en routers.


#### Het best-effort principe
Het IP-protocol maakt gebruik van het best effort-principe, wat betekent dat het pakketje wordt verzonden zonder garantie van levering of kwaliteit van de verbinding. Het kan dus voorkomen dat pakketjes verloren gaan of vertraging oplopen in het netwerk. Dit kan worden opgevangen door het gebruik van het hoger gelegen TCP (Transmission Control Protocol), die de betrouwbaarheid van de verbinding garanderen.

Kortom, het IP-protocol is de basis van communicatie over het internet en andere computernetwerken. Het verzendt gegevenspakketjes van de bron naar de bestemming door middel van adreszuivering en routering. Het is een belangrijk onderdeel van het TCP/IP-model en wordt gebruikt in combinatie met andere protocollen om betrouwbare communicatie te garanderen.


## Het DHCP protocol

DHCP staat voor Dynamic Host Configuration Protocol en is een netwerkprotocol dat wordt gebruikt om IP-adressen en andere netwerkconfiguraties automatisch toe te wijzen aan apparaten die zijn verbonden met een netwerk. Hieronder vindt u enkele belangrijke punten om te begrijpen over de werking van DHCP:

*	Wanneer een apparaat wordt aangesloten op een netwerk, stuurt het apparaat een verzoek naar het netwerk voor een IP-adres en andere configuratie-informatie. (DHCP-request)
*	De DHCP-server ontvangt dit verzoek en kent een IP-adres en andere netwerkconfiguraties toe aan het apparaat.
Dit proces gebeurt automatisch en dynamisch, wat betekent dat een apparaat een nieuw IP-adres kan krijgen elke keer dat het opnieuw verbinding maakt met het netwerk.
DHCP bespaart tijd en maakt netwerkbeheer efficiënter door het handmatig toewijzen van IP-adressen en andere netwerkconfiguraties te vervangen.