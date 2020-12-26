---
layout: page
title: Stap 4 - Betaal met Lightning
show_in_menu: false
disable_anchors: true
---

## Razendsnelle betalingen met Lightning
Om betalingen te doen is de Bitcoin blockchain niet ideaal. De kosten om een transactie te doen kunnen soms oplopen en het duurt altijd even voor een betaling bevestigd wordt. Met Lightning netwerk kan je in een oogwenk betalen met bitcoin.

### Bitcoin schalen
Voorlopig volstaat om te begrijpen dat Lightning een laag is die bovenop het Bitcoin protocol gebouwd wordt. In tegenstelling tot wat vaak beweerd wordt, is een blockchain geen revolutionaire uitvinding van Satoshi Nakamoto. Een blockchain is eigenlijk gewoon een zeer inefficiënte database. Bitcoin transacties zijn gewoon tekst en die transacties worden overal ter wereld opgeslaan door nodes in hun kopie van de blockchain. Gemiddeld iedere tien minuten vinden miners een nieuwe blok wanneer ze de oplossing van de Proof-of-Work puzzel vinden. Per blok kan er 1 megabyte aan transacties toegevoegd worden aan de langste keten. Om uw transactie te laten toevoegen aan die keten moet je dus bieden. Miners zullen voorang geven aan de hoogste bieders zodat ze meer inkomsten halen uit hun werk en investering.

Je hebt het misschien al gemerkt maar een transactie op de basislaag van Bitcoin kan duur zijn. Zeker als snelheid belangrijk is, moet je daar wat voor over hebben. De grootte van de blokken was in het verleden een belangrijk strijdpunt tussen gebruikers van Bitcoin. Sommigen wilden de blokken vergroten naar 2 megabyte of 8 megabyte en anderen vonden dit geen goed idee. Het leidde tot een ware "burgeroorlog" die uiteindelijk beslecht werd door de afsplitsing van een groep die grotere blokken wilden. Dit werd Bitcoin Cash en de originele Bitcoin ging verder met de oorspronkelijke grootte van 1MB.

Ik wil hier geen lang artikel schrijven over de voor-en-nadelen van kleine of grote blokken. Bitcoin Cash bestaat nog altijd maar is grotendeels verdwenen van het toneel. De prijs van Bitcoin Cash zakt verder weg en is vandaag nog 0.015 BTC waard. De conclusie van deze hele episode is volgens mij dat je Bitcoin niet zomaar kan veranderen. Als je niet een overgrote meerderheid van het netwerk overtuigd van uw verandering dan komt die er niet. Dat is maar goed ook. Een netwerk waar ondertussen meer dan 350 miljard euro aan waarde in zit blijft best resistent aan veranderingen die doorgedrukt worden door enkele partijen in achterkamertjes. Operatoren van nodes beslissen welke software ze draaien en ze hoeven nergens mee akkoord te gaan als ze dat niet willen.

[image]

Een meer realistische optie om Bitcoin te schalen is om te werken in lagen. Ook het internet werd opgebouwd en geschaald met verschillende lagen van protocollen die op elkaar verderbouwen zoals IP, TCP, HTTP, HTTPs. Met Bitcoin zal dat niet anders zijn. De Bitcoin blockchain, de fundamentele laag, kan gebruikt worden door andere protocollen daar bovenop. Een voorbeeld van zo'n 'tweede laag' is het Lightning Netwerk.

### Hoe werkt Lightning?
Je kan Lightning best vergelijken met een rekening die je aanhoudt in jouw favoriete café. Jij, een vaste klant, en de barman besluiten om niet telkens af te rekenen met een betaling na iedere bestelling. Jullie klikken alle twee een hoeveelheid Bitcoin vast in Lightning. Je behoudt controle over dit geld maar het staat niet meer klaar op de blockchain om uit te geven. Jullie openen een "kanaal" tussen jouw Bitcoin en dat van de barman. Na iedere bestelling geven jullie aan elkaar door hoeveel je nog moet. Na een tijdje besluiten jullie af te rekenen en gaat het geld terug naar de basislaag.

Toegegeven, dit is wellicht iets te simplistisch maar dat is ongeveer hoe het werkt. In de toekomst kan ik hier zeker meer informatie over geven maar voorlopig volstaat dit. Lightning is dus een tweede laag bovenop de Bitcoin blockchain. Het geld verlaat het systeem niet maar wordt vastgezet voor een tijdje. Vervolgens wissel je informatie uit met elkaar over de huidige "staat" van jullie deel van het geld. Wanneer een partij wil afrekenen dan betaal je uw transactiekost en sluit je het kanaal.

Betalingen voor koffie zullen niet op de basislaag van Bitcoin kunnen. Het is niet realistisch om 7 miljard mensen hun betalingen te laten doen met de eerste laag. Verschillende andere oplossingen zullen de basislaag gebruiken om "af te rekenen".

Genoeg gepraat. We gaan Lightning gebruiken!

### Jouw Lightning wallet opladen
Een Lightning wallet aanmaken en opladen met Blue Wallet is kinderspel.

**Let op**: plaats geen grote bedragen in deze wallet. Blue Wallet gebruikt voor Lightning een [**custodial**](faq.md#wat-is-een-custodial-wallet) wallet. Dit betekent dat je de sleutels niet meer zelf beheert. Blue Wallet doe dit voor jou achter de schermen.

Ga terug naar de app van Blue Wallet. We maken opnieuw een nieuwe wallet aan. Kies voor `Voeg nu toe` en selecteer `Lightning` (tweede optie). Geef de wallet een naam en druk op `Aanmaken`.

![ln-create](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/ln-create.png?raw=true)

Blue Wallet toont je een back-up. Dit is geen kopie van *seed woorden* maar dient enkel voor authenticatie bij Blue Wallet indien je de wallet wil herstellen. Neem een foto van deze back-up of kopieer de URL die onderaan getoond wordt.

**Blue wallet beheert het geld in deze wallet**.

![ln-backup](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/ln-backup.png?raw=true)

Je komt opnieuw terecht in het hoofdmenu. Open de Lightning wallet en kies voor `fondsen beheren`. Kies vervolgens voor `Bijvullen`.
![ln-menu](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/ln-menu.png?raw=true)

![ln-bijvullen](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/ln-bijvullen.png?raw=true)

Kies de wallet van waaruit je het geld wil overmaken. Bepaal het bedrag om te versturen naar de Lightning wallet. Met de twee pijltjes kan je wisselen tussen BTC, sats of €. Kies opnieuw een *fee* voor de transactie. Druk op `Volgende` en `Nu verzenden`.
![ln-tx](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/ln-tx.png?raw=true)

Nu wachten we af tot de transactie wordt bevestigd. In de volgende stap kunnen we hiermee aan de slag.

------

[Terug naar overzicht](overzicht.md) --
[Verder gaan](stap5.md)
