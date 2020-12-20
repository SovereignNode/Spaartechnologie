---
layout: page
title: Stap 2 - Leer over bitcoin wallets
show_in_menu: false
disable_anchors: true
---

## Veelgestelde vragen over bitcoin wallets
*Doel: Verkennen wat een bitcoin wallet is en welke verschillende vormen ze kunnen aannemen*

### Wat is een wallet?
Een bitcoin wallet is net zoals een portemonnee. Het is een manier om waarde op te slaan. Het belangrijkste verschil met een echte portemonnee is dat een bitcoin wallet niet echt waarde opslaat binnenin die portemonnee. Bitcoins bestaan enkel op het grootboek dat we de blockchain noemen. Een bitcoin wallet beheert de sleutels die nodig zijn om te ontvangen en te versturen via de blockchain.

### Wat zijn seed woorden?
*Seed* woorden (ook wel *mnemonic* of geheustensteun genoemd) zijn een reeks van 12 of 24 willekeurig gekozen woorden die aangemaakt worden wanneer je een nieuwe wallet opent. Deze woorden dienen als de belangrijkste back-up van jouw volledige wallet en dienen niet gedeeld te worden met anderen. Bewaar deze woorden veilig want iedereen die toegang heeft tot deze woorden kan jouw bitcoin stelen.

### Wat is een passphrase?
Een *passphrase* of wachtwoord (ook wel 13e/25e woord genoemd) is een extra woord dat door de gebruiker gekozen wordt met de bedoeling een extra laag veiligheid toe te voegen aan jouw back-up. Wanneer jouw seed woorden in verkeerde handen vallen dan heeft een aanvaller nog steeds jouw extra wachtwoord nodig om toegang te krijgen tot jouw bitcoin. Bewaar jouw seed woorden en wachtwoord nooit samen op dezelfde plaats.

### Wat is een private key?
Een *private key* of geheime sleutel wordt afgeleid van jouw seed woorden. De kennis van de geheime sleutel is een bewijs dat de entiteit die de sleutel bezit toegang heeft om bitcoin uit te geven vanaf het overeenstemmend adres. Jouw wallet creeërt een geheime sleutel voor ieder adres dat aangemaakt wordt. Vandaag zullen de meeste gebruikers van bitcoin nooit in aanraking komen met geheime sleutels aangezien dit over het algemeen automatisch wordt beheert door de wallet software.

### Wat is een public key?
*Public keys* of publieke sleutels worden gebruikt in een transactie om te verifiëren dat de eigenaar van de overeenstemmende geheime sleutel een correcte handtekening zet als bewijs dat hij eigenaar is van het geld dat verstuurd wordt. Opnieuw geldt dat de gebruiker gewoonlijk niet in aanraking komt met deze publieke sleutels aangezien dit door de software van jouw wallet wordt gedaan.

### Wat is een extended public key?
Een *extended public key* (of uitgebreide publieke sleutel) kan gezien worden als de hoofdweergave in jouw bitcoin wallet. Doorgaans noemen we dit een xpub. Met zo'n xpub kan je alle adressen van jouw wallet genereren en bekijken. Let dus op met wie je deze xpub deelt want het geeft volledige inzage in jouw portemonnee. Wanneer je een wallet gebruikt die niet verbonden is met een node die je zelf draait dan is het zeer waarschijnlijk dat een derde partij jouw xpub kent en dus kan opvolgen hoeveel bitcoin jij hebt. Naast xpubs zijn er ook ypubs en zpubs die beide dezelfde functie hebben.

### Wat is een adres?
Een adres is een combinatie van cijfers en letters die uniek is voor jouw wallet. Dit kan je delen met andere om bitcoin te ontvangen. Wallets kunnen een oneindige hoeveelheid adressen aanmaken. Het is een goed idee om nooit hetzelfde adres twee keer te gebruiken om jouw privacy te beschermen. De meeste wallets doen dit automatisch voor jou en maken een nieuw adres aan telkens wanneer je geld wil ontvangen. De software houdt alle gebruikte adressen bij en toont je volledige balans.

### Wat is een mobile wallet?
Een *mobile wallet* is een wallet die op jouw GSM staat. Het laat je toe om snel en makkelijk toegang te hebben tot jouw bitcoin met als nadeel dat het risico bestaat dat je jouw toestel verliest en dus mogelijk ook jouw bitcoin. Dit scenario mag geen probleem vormen indien je correct jouw *seed woorden* neergeschreven hebt op papier zodat je jouw wallet opnieuw kan aanmaken op een ander toestel.

### Wat is een desktop wallet?
Een *desktop wallet* is een wallet die op jouw computer staat. Deze komen doorgaans met iets meer functionaliteit dan wallets voor jouw smartphone maar kunnen ook ingewikkelder zijn. Computers zijn toestellen die verbonden zijn met het internet en zijn vatbaar voor malware. Let dus op en wees voorzichtig bij het installeren van software.

### Wat is een multi-sig wallet?
Een *multi-signature wallet* is een wallet die meer dan één geheime sleutel vereist om een transactie te ondertekenen. Dit kan variëren van twee uit in totaal drie sleutels tot 15 uit 20 sleutels. Deze keuze is aan de gebruiker wanneer de wallet wordt aangemaakt. Multi-sig is veel veiliger dan een enkele handtekening maar het is ook een stukje moeilijker om aan te maken, back-ups te beheren en om transacties mee te doen. Niet aan te raden voor nieuwe gebruikers.

### Wat zijn watch-only wallets?
Een *watch-only wallet* of enkel-kijken is een wallet die gebruikt maakt van jouw *extended public key* of xpub. Deze sleutel stelt je in staat om de balans van een wallet te volgen. Enkel-kijken wallets bevatten geen geheime sleutels en kunnen niet gebruikt worden om bitcoin uit te geven. Let op met het delen van xpubs want iedereen die hier toegang toe heeft kan jouw balans zien.

### Wat is een custodial wallet?
Een *custodial* wallet is een beheerde wallet. Een derde partij beheert de sleutels van jouw wallet. Met beheerde wallets kan veel complexiteit verborgen worden met als nadeel dat je niet meer in controle bent over jouw geld. Beheerde wallets worden bijvoorbeeld aangeboden door beurzen. Hou nooit grote hoeveelheden bitcoin in een beheerde wallet.


### Wat is een non-custodial wallet?
Een *non-custodial* wallet of niet-beheerde wallet is een wallet waar jij volledige controle hebt over jouw geheime sleutels. Bitcoin werd ontworpen om gebruik te maken van geheime en publieke sleutels en dit blijft de beste manier om het netwerk te gebruiken. Gebruik altijd wallets die je toelaten om zelf jouw *seed woorden* neer te schrijven bij de creatie van jouw portemonnee. Zo ben je vrij zeker dat je een non-custodial wallet gebruikt.

### Hoe weet ik welke fee te gebruiken voor een transactie?
Om een transactie te versturen moet je altijd een fee betalen aan het netwerk. Deze fee wordt ontvangen door miners wanneer jouw transactie in een blok geplaatst wordt. De keuze van jouw fee hangt af van de snelheid waarmee je de transactie wilt uitvoeren en hoe druk het netwerk op het moment van versturen is. De meeste wallets geven een schatting en laten je toe om dit aan te passen naar jouw behoefte.

### Wat is een QR code?
Een QR code is een visuele voorstellen van data. Ze worden in Bitcoin vaak gebruikt om lange en moeilijk te lezen adressen om te zetten in een soort van barcode. Deze code kan gescant worden door de wallet van de verzender. Het is doorgaans een slecht idee om handmatig adressen in te typen. Een foutje en snel gebeurt waardoor de bitcoins naar een verkeerd adres zouden gaan. Controleer altijd de juistheid van adressen vooraleer je een transactie afrondt.

### Wat is een block explorer?
Een *block explorer* of blokverkenner is een website of applicatie die je toelaat om de details van een bepaalde blok op de blockchain te bekijken. Je vindt er data zoals aantal transacties in een blok, adres van de verzender, adres van de ontvanger, betaalde kosten, verstuurde hoeveelheid, de blokhoogte en de bloktijd.

## Beheer je sleutels met Blue Wallet
*Doel: Importeer de wallet van Relai in Blue Wallet en maak een nieuwe aan.*

Na de theorie komt de praktijk. In dit deel gebruiken we een gebruiksvriendelijke mobile wallet. In [Stap 1](documentation/stap1.md) gebruikten we reeds onze eerste mobile wallet. Relai is een non-custodial wallet aangezien je een back-up nam van de 12 woorden die getoond werden.

In het eerste deel importeren we deze *seed woorden* die we kregen van Relai in Blue Wallet. Dit toont aan dat je geld dus niet opgeslaan wordt in een app op je smartphone. Jouw bitcoin worden beheert door de woorden die je neerpende.

### Importeer de wallet van Relai in Blue Wallet
1. Download <a href="https://bluewallet.io/" target="_blank">Blue Wallet</a>.
    voor [Android](https://play.google.com/store/apps/details?id=io.bluewallet.bluewallet)
    voor [iOS](https://itunes.apple.com/app/bluewallet-bitcoin-wallet/id1376878040)
2. Druk op 'Add now'
3. Geef de wallet een naam (bvb. Relai)
4. Druk 'Import wallet'
5. Geef de 12 woorden in die je op papier neergeschreven hebt in [Stap 1](documentation/stap1.md).
6. Wacht tot Blue Wallet jouw balans ophaalt.

Je hebt nu dezelfde wallet op twee plaatsen. De eigendom van jouw bitcoin wordt op het netwerk afgedwongen met sleutels. De 12 *seed woorden* (*mnemonic* of geheugensteun) die Relai toonde zijn een voorstelling van die sleutels. Door deze woorden in Blue Wallet in te geven kan je ook in Blue Wallet deze bitcoin bekijken en uitgeven.

### Maak een nieuwe wallet aan in Blue Wallet
1. Druk op 'Add now'
2. Geef de wallet een naam (bvb. Spaarpotje)
3. Kies het type wallet. Je hoeft hier niets aan te passen
4. Druk op 'Create'
5. Noteer de 12 woorden op papier. Bewaar dit op een veilige plaats.
------

[Verder gaan](stap3.md) --
[Terug naar overzicht](overzicht.md)
