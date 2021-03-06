---
layout: page
title: Stap 2 - Leer over bitcoin wallets
show_in_menu: false
disable_anchors: true
---
## Principes

* Maak altijd een back-up van wallets
* Bewaar back-ups op een veilige plaats
* De wachtwoordzin of *seed* is de sleutel van jouw kluis met bitcoin

## Wat is een wallet?
Een bitcoin wallet is zoals een portemonnee. Het is een manier om waarde op te slaan. Het belangrijkste verschil met een echte portemonnee is dat de bitcoin zich niet letterlijk in de portemonnee bevinden. Bitcoin bestaan enkel op het grootboek dat we de [blockchain](definities.md#blockchain) noemen. Duizenden leden op het netwerk houden een kopie van dit grootboek bij. Het grootboek is in essentie een databank met alle [transacties](definities.md#transacties) op het netwerk sinds het begin in 2009. Voortdurend controleren de leden van het netwerk of alle transacties wel een geldige handtekening hebben. Om een geldige transactie te versturen heb je de juiste sleutel nodig. Een bitcoin wallet kan je dus beter begrijpen als een sleutelhanger.

**Een bitcoin wallet beheert de sleutels die nodig zijn om bitcoin te ontvangen en te versturen.**

In de [Stap 1](stap1.md) gebruikten we reeds een bitcoin wallet. Je geld bevindt zich niet letterlijk in de app van Relai. Je kan de back-up van die wallet gebruiken in een andere wallet om je saldo te bekijken, adressen aan te maken of om bitcoin te versturen. Zolang je de **seed** of back-up van je sleutels hebt voor het adres waar je bitcoin op staan, kan je ze uitgeven.

[infographic]

## Blue Wallet
*Doel: Importeer de wallet uit Stap 1 in Blue Wallet en maak nieuwe wallet aan.*

We gebruiken opnieuw een wallet op je smartphone. Relai is een niet-beheerde of [*non-custodial*](definities.md#non-custodial) wallet aangezien je een back-up nam van je seed (de 12 woorden die getoond werden). Dit is in tegenstelling tot een beheerde of [*custodial*](definities.md#custodial) wallet die de sleutels van de wallet in jouw plaats beheert. In dit laatste geval kan je niet zeggen dat je effectief eigenaar bent van je bitcoin. Je hangt namelijk af van een derde partij die jullie afspraak moet nakomen en je de bitcoins moet geven wanneer je daar om vraagt. Gebruik altijd *niet-beheerde* wallets -- **niet jouw sleutels, niet jouw bitcoin**.

Om te beginnen importeren we de *seed* die we als back-up kregen van Relai in Blue Wallet. Dit toont aan dat je geld dus niet opgeslagen wordt in een app op je smartphone. Jouw bitcoin worden beheerd door de woorden die je neerpende.

### Importeer de wallet van Relai in Blue Wallet

Download [Blue Wallet](https://bluewallet.io/){:target="_blank"} op je telefoon. De software is beschikbaar voor [Android](https://play.google.com/store/apps/details?id=io.bluewallet.bluewallet){:target="_blank"} en voor [iOS](https://itunes.apple.com/app/bluewallet-bitcoin-wallet/id1376878040){:target="_blank"}.

We maken een wallet aan door `Voeg nu toe` te kiezen. Kies voor `Wallet importeren` onderaan in het menu.

![bluewallet-toevoegen](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/bwvoegtoe.png?raw=true)

Voer de 12 woorden in die je op papier noteerde in [Stap 1](stap1.md). Dit is jouw *seed* (ook wel jouw *mnemonic phrase* genoemd). Deze wachtwoordzin is een geheugensteun voor jouw sleutels. De volgorde van de woorden is belangrijk. Laat tussen ieder woord een spatie. Druk vervolgens op `importeren`.

![bluewallet-import](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/bwimport.png?raw=true)

Nu gaat je wallet aan de slag. De software leidt van je sleutels alle adressen af en zoekt naar je saldo. Wacht tot Blue Wallet je wallet met succes importeert.[^1]

[^1]: Jij hebt voorlopig nog geen kopie van alle transacties. Je deelt dus al je adressen mee aan Blue Wallet waarmee zij kunnen controleren hoeveel bitcoin in je wallet zitten. Dit is slecht voor jouw privacy. Later zullen we zien hoe je dit kan verbeteren.

Je hebt nu dezelfde wallet op twee plaatsen. De eigendom van jouw bitcoin wordt op het netwerk afgedwongen met sleutels. De *seed* (*mnemonic* of geheugensteun) die Relai toonde zijn een voorstelling van die sleutels. Door deze woorden in Blue Wallet in te geven kan je ook in Blue Wallet deze bitcoin bekijken en uitgeven.

Als laatste stap passen we nog wat instellingen aan van onze wallet. Druk op de aangemaakte wallet en ga naar het instellingen-menu rechtsboven.

![bluewallet-settings](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/bwsettings.png?raw=true)

* Geef de wallet een naam (bvb 'Relai')
* Bekijk je back-up via `Exporteren / Back-up maken`. Dit zijn de woorden die we reeds op papier hebben

![bluewallet-walletsettings](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/bwwalletsettings.png?raw=true)

Je kan op het saldo drukken om de weergave te veranderen van BTC naar EUR of naar [sats](definities.md#satoshi).

![bluewallet-walletdone](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/bwwalletdone.png?raw=true)


### Maak een nieuwe wallet aan in Blue Wallet
Via Relai kan je eenvoudig bitcoin kopen. Maar de wallet van Relai is niet echt handig. Er ontbreekt veel functionaliteit die we van een goeie wallet verwachten.[^2] Daarom gebruiken we een tweede wallet die beter voldoet aan onze eisen. In bovenstaand deel hebben we reeds de app van Blue Wallet gedownload. Nu maken we een nieuwe portemonnee aan en nemen we opnieuw een back-up van onze *seed* van die portemonnee.

[^2]: Relai gebruikt slechts 1 adres van jouw wallet. Dit is geen goeie gewoonte en slecht voor je privacy. Een bitcoin wallet kan een quasi-oneindig aantal adressen afleiden van jouw *seed*. Het is beter om telkens een nieuw adres af te leiden. Daarnaast biedt Blue Wallet extra opties zoals replace-by-fee (RBF) en coin-selection. Later leren we meer over deze begrippen.

Druk opnieuw op  `Voeg nu toe`. Geef de wallet een naam (bvb. 'Sparen') en kies het type van de wallet. We kiezen de eerste optie in de lijst (`Bitcoin`). Druk vervolgens op `Aanmaken`.

![bluewallet-nieuwewallet](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/bw-nieuwewallet.png?raw=true)

Noteer de 12 woorden die getoond worden op het scherm **op papier**. Bewaar dit op een veilige plaats.

![bluewallet-seed](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/bwseed.png?raw=true)

In de volgende stap gaan we aan de slag met onze wallets en doen we zelf een eerste transactie. Wil je nog meer informatie over wallets? Neem dan een kijkje in de [veelgestelde vragen over wallets](faq.md#bitcoin-wallets)

------

[Terug naar overzicht](overzicht.md) --
[Verder gaan](stap3.md)

------
