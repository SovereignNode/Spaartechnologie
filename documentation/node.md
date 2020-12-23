---
layout: page
title: Wat is een node?
show_in_menu: false
disable_anchors: true
---

## Bitcoin nodes
Wanneer je met Bitcoin begint, zal je ongetwijfeld horen over nodes. In dit artikel leg ik uit wat het is en hoe jij kan starten met jouw eigen Bitcoin node.

### Wat is een node?

Een node is een computer die de Bitcoin-software draait. Die computer is dan een knooppunt in het peer-to-peer netwerk. Jouw persoonlijke node bevat jouw eigen kopie van de Bitcoin-blokchain en dwingt de spelregels van het netwerk af. Je kan het best zien als een portaal naar het Bitcoin ecosysteem vergelijkbaar met een router die je toegang geeft tot het internet. Een node stuurt transacties uit naar het netwerk, verifieert dat de bitcoin die je ontvangt echt zijn en beschermt je privacy aangezien je van niemand anders afhankelijk bent om deel te nemen.

[image]

### Waarom moet ik een node draaien?

Jouw node = jouw regels. Wanneer je een wallet verbindt met jouw eigen node dan hoef je niemand anders te vertrouwen om jouw inkomende transacties te verifiëren. Een node beschermt jou tegen valsmunters en het houdt het netwerk decentraal en verspreid. Wanneer je niet jouw eigen node gebruikt dan vertrouw je iemand anders om je te vertellen hoeveel bitcoin je precies hebt en om transacties te versturen of te ontvangen. Het mooie aan Bitcoin is dat je niemand anders hoeft te vertrouwen maar dan moet je wel een eigen node opstarten.
Waar moet ik op letten bij het draaien van een node?

Een node draait best 24/7 dus houd je best rekening met een elektriciteitskost die afhankelijk is van de hardware die je gebruikt. De meeste nodes draaien op mini-computers zoals een Raspberry Pi waardoor de kosten te verwaarlozen zijn. Daarnaast zal een node constant nieuwe blokken downloaden en verifiëren. Dit zal zo’n 20GB per maand verbruiken van jouw internetlimiet. De initiële download van alle blokken zal een goeie 350GB kosten. Controleer bij jouw internetprovider hoeveel jouw limiet is.

### Welke soorten nodes zijn er?

Het is mogelijk om een node te draaien op jouw huidige computer door simpelweg Bitcoin Core (de bekendste implementatie van een bitcoin node) te downloaden. Dit is de eenvoudigste en goedkoopste optie. Het nadeel hiervan is dat jouw computer meestal niet constant aan staat waardoor de software telkens opnieuw moet synchroniseren met nieuwe blokken sinds het laatst afgesloten werd. Er zijn ‘plug-and-play’-opties zoals MyNode en Nodl. Deze nodes bevatten alles wat je nodig hebt en vereisen enkel stroom en internet om van start te gaan. Ze zijn ook iets duurder. Tot slot, opteren veel mensen om zelf hardware te kopen en zelf de Bitcoin software te installeren met een Raspberry Pi. Dit is in mijn ogen de leukste optie en klinkt moeilijker dan het is.
Wat kan een node nog?

Dat hangt sterk af van de software die je draait. Enkele gebruikelijke extra toepassingen zijn een Lightning-node, een Electrum-server of een eigen block-explorer (zoals blockstream.info of mempool.space). Je kan ook een betalingsterminal installeren zoals BTCPay Server. Paketten zoals MyNode bevatten al deze toepassingen zonder al te veel extra gedoe.

[image]

### Wat is de initiële-blok-download?

Wanneer je voor het eerst de software opstart begint de initiële-blok-download (IBD). De software start in 2009 en download en verifieert de volledige transactiegeschiedenis van het netwerk. Het slaat een kopie op alle transacties; jouw persoonlijke kopie van de blockchain. Wanneer de synchronisatie voltooid is, kan de node controleren dat de bitcoin die jij ontvangt legitiem en echt zijn. De software zal valsspelers onverbiddelijk weigeren. De synchronisatietijd is afhankelijk van de hardware en internetsnelheid. Gemiddeld reken je best op 4-7 dagen.

### Wat is een pruned node?

Je kan jouw node de opdracht geven om oude data te verwijderen wanneer de keten volledig gesynchroniseerd is. Dat kan handig zijn wanneer je niet veel plaats meer hebt op jouw computer. Het heeft wel nadelen. Het is moeilijker om oude transacties te verifiëren en je laat niet toe dat andere nodes die online komen jouw node gebruiken om gegevens te downloaden.
Kan ik de node van iemand anders gebruiken?

Dat kan zeker. Het is zelfs de standaardoptie van veel wallets maar ideaal is het niet omwille van de redenen hierboven aangehaald. Als je een vriend hebt die je vertrouwt kan je ook zijn/haar node gebruiken. Dit is een verbetering ten opzichte van de node gebruiken van een onbekende derde-partij. Maar de ultieme manier om deel te nemen aan het Bitcoin netwerk is met jouw eigen node.

### Eigen node draaien
TBC
