---
layout: page
title: Definities
show_in_menu: true
disable_anchors: true
---

## Stap 1
### seed
Een *seed* is een reeks van 12 of 24 willekeurig gekozen woorden die samen een wachtwoordzin vormen. De seed wordt aangemaakt wanneer je een nieuwe portemonnee opent. De seed wordt ook wel *mnemonic* of geheugensteun genoemd. Deze geheugensteun dient als de belangrijkste back-up van je volledige portemonnee en dient niet gedeeld te worden met anderen. Bewaar deze woorden veilig want iedereen die toegang heeft tot deze woorden kan je bitcoin stelen.

### wallet
Een wallet is software die al je bitcoin adressen en sleutels beheert en dienst doet als een portemonee voor je geld. Je gebruikt een wallet om bitcoin te ontvangen, te versturen en te bekijken.

## Stap 2
### blockchain
Een ketting van gevalideerde [blokken](definities.md#blok) die allemaal gelinkt zijn aan hun voorganger tot en met de [*genesis-blok*](definities.md#genesis-blok) van [Satoshi Nakamoto](definities.md#satoshi-nakamoto) in 2009. De blockchain is een ketting van blokken. Het is een publiek grootboek dat alle bitcoin transacties sinds het ontstaan van het netwerk bijhoudt.

<!-- [*Miners*](definities.md#miners) concurreren met elkaar om nieuwe blokken te produceren waarvoor ze transactiekosten en een bloksubsidies ontvangen. Iedere succesvolle blok wordt met cryptografie gelinkt aan de vorige blok. -->

### blok
Een blok is een groepering van bitcoin [transacties](definities.md#transacties) die een tijdstempel krijgen en een verwijzing naar de voorgaande blok bevatten. Door deze verwijzing naar de vorige blok vormt de opeenvolging van blokken een ketting die we de Bitcoin blockchain noemen.

<!-- De hoofding van een blok wordt gehashed om een proof-of-work te produceren waarmee de transacties gevalideerd worden. Gevalideerde blokken worden toegevoegd aan de blockchain via consensus op het netwerk. -->

### genesis blok
De eerste blok in de blockchain die gebruikt werd om het netwerk te lanceren.

### Satoshi Nakamoto
Satoshi Nakamoto is het pseudoniem dat gebruikt werd door de persoon (of personen) die Bitcoin ontwierpen en de eerste implementatie ontwikkelden. In 2008 werd op online mailing-lijst door een anonieme entiteit genaamd Satoshi Nakamoto de [*Bitcoin whitepaper*](https://bitcoin.org/bitcoin.pdf) gedeeld. Ze waren de eerste om het dubbel-uitgavenprobleem op te lossen voor digitaal geld. Hun echte identiteit blijft onbekend. Satoshi verdween in 2011 en is sindsdien niet meer online gezien. Daarna werkten honderden ontwikkelaars verder aan het Bitcoin protocol waarvan de broncode volledig open en vrij beschikbaar is ([*open-source*](definities.md#open-source)).

### open-source
De software van Bitcoin is *open-source* of open-broncode. Dit betekent dat iedereen kan lezen hoe het programma werkt. Dit is in tegenstelling tot *closed-source* of gesloten-broncode waarvan gebruikers niet kunnen achterhalen wat de software precies doet.

### transactie
In simpele verwoording is een transactie een transfer van bitcoin van één adres naar een ander. Meer precies is een transactie een ondertekende structuur van data die een expressie is van een transfer van waarde. Transacties worden uitgestuurd over het netwerk, ontvangen door andere leden op het netwerk en meegenomen in blokken waardoor ze permanent op de blockchain komen te staan.

### custodial
Een *custodial* wallet is een beheerde wallet. Een derde partij beheert de sleutels van je wallet. Met beheerde wallets kan veel complexiteit verborgen worden met als nadeel dat je niet meer de controle hebt over je geld. Beheerde wallets worden bijvoorbeeld aangeboden door beurzen of wisselkantoren. Houdt nooit grote hoeveelheden bitcoin in een beheerde wallet.

### non-custodial
Een *non-custodial* wallet of niet-beheerde wallet is een wallet waar jij volledige controle hebt over jouw geheime sleutels. Bitcoin werd ontworpen om gebruik te maken van geheime en publieke sleutels en dit blijft de beste manier om het netwerk te gebruiken. Gebruik altijd wallets die je toelaten om zelf jouw *seed* neer te schrijven bij het aanmaken van je wallet. Zo ben je vrij zeker dat je een non-custodial wallet gebruikt.

### satoshi
Een satoshi is de kleinste denominatie van een bitcoin die op de blockchain kan staan. Het is equivalent met 0.00000001 bitcoin en werd vernoemd naar de ontwerper van Bitcoin, Satoshi Nakamoto. Eén volledige bitcoin (1 BTC) komt dus overeen met 100 miljoen sats.

## Stap 3
### unspent transaction output
Een *unspent transaction output* (**UTXO**) is een ongespendeerde output die nog kan uitgegeven worden als input in een nieuwe [transactie](definities.md#transactie).

### adres
Een bitcoin adres kan verschillende vormen aannemen:
* bc1qwgscp3mjhkscwkemmwex6x9ycs4t4qukkguxy4
* 147SwRQdpCfj5p8PnfsXV2SsVVpVcz3aPq
* 3BYdu2CfJ8sHaDV4p8xFmrvsfhxKQcbn3g

Net zoals je anderen vraagt om een email te versturen naar jouw emailadres, kunnen anderen bitcoin versturen naar één van jouw adressen.

### miner
Een miner is een lid van het netwerk die geldige oplossingen zoekt op een wiskundig probleem. Om deze oplossing te vinden gebruiken miners elektriciteit. De winnaar van de wedstrijd mag een nieuwe blok toevoegen. In ruil voor deze berekeningen krijgen miners van het netwerk een beloning. Deze beloning bestaat uit een bloksubsidie en transactiefee's.

### geheime sleutel
Een geheim getal waarmee bitcoins kunnen uitgegeven worden vanaf het publiek adres dat overeenkomt met de geheime sleutel. Een geheime sleutel deel je nooit mee met anderen.

### block explorer
Een *block explorer* of blokverkenner is een website of applicatie die je toelaat om de details van een bepaalde blok op de blockchain te bekijken. Je vindt er data zoals aantal transacties in een blok, adres van de verzender, adres van de ontvanger, betaalde kosten, verstuurde hoeveelheid, de blokhoogte en de bloktijd.

### mempool
Een mempool is een pot met onbevestigde transacties (transacties die nog niet in een blok werden geplaatst). Miners kiezen transacties met de hoogste fee's om in een blok te stoppen wanneer ze een oplossing vinden voor de puzzel.

### node
Een node is een computer die de Bitcoin-software draait. Die computer is dan een knooppunt op het netwerk. Jouw persoonlijke node bevat je eigen kopie van de Bitcoin blockchain en dwingt de spelregels op het netwerk af. Je kan het best zien als een portaal naar het Bitcoin ecosysteem vergelijkbaar met een router die je toegang geeft tot het internet. Een node stuurt transacties uit naar het netwerk, verifieert dat de bitcoin die je ontvangt echt zijn en beschermt je privacy aangezien je van niemand anders afhankelijk bent om deel te nemen.

### coinbase
Een coinbase transactie is de eerste transactie in iedere blok. Deze transactie bevat de bloksubsidie en de som van de fee's van alle transacties in dat blok.

### moeilijkheidsgraad
Een instelling op het netwerk die bepaalt hoe moeilijk de puzzel is die opgelost moet worden door miners. Hoe meer miners actief zoeken naar de oplossing van de puzzels, hoe moeilijker de puzzel wordt. Hierdoor blijft het interval tussen de blokken altijd gemiddeld rond de 10 minuten. De moeilijkheidsgraad wordt iedere 2016 blokken aangepast.



<!-- ### proof-of-work
Een stukje data dat een significante berekening vraagt om te bekomen. In Bitcoin moeten miners een numerieke oplossing vinden van een SHA256 algoritme dat aan een bepaalde vereiste op het netwerk voldoet, de moeilijkheidsgraad.

### hash
Een digitale vingerafdruk van een bepaalde binaire input.

### peer-to-peer
Een peer-to-peer netwerk is een netwerk waar alle leden rechtstreeks met elkaar verbinden. Dit is in tegenstelling tot een netwerk waar iedereen met een centrale server verbindt zoals Facebook of Twitter. -->
