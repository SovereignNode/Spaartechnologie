---
layout: page
title: Definities
show_in_menu: true
disable_anchors: true
---


### adres
Een bitcoin adres kan verschillende vormen aannemen:
* bc1qwgscp3mjhkscwkemmwex6x9ycs4t4qukkguxy4
* 147SwRQdpCfj5p8PnfsXV2SsVVpVcz3aPq
* 3BYdu2CfJ8sHaDV4p8xFmrvsfhxKQcbn3g

Net zoals je anderen vraagt om een email te versturen naar jouw emailadres, vraag je anderen om hun bitcoin te versturen naar een van jouw bitcoin adressen.

### blockchain
Een lijst van gevalideerde [`blokken`](definities.md#blok) die allemaal gelinkt zijn aan hun voorganger tot en met de eerste [`genesis-blok`](definities.md#genesis-blok) van [`Satoshi Nakamoto`](definities.md#satoshi-nakamoto) in 2009. De [`blokchain`](definities.md#blockchain) is een ketting van blokken (een blokketen). Het is een publiek grootboek dat een kopie bijhoudt van alle bitcoin transacties sinds het ontstaan van het netwerk. [`Miners`](definities.md#miners) concurreren met elkaar om blokken te produceren waarvoor ze transactiekosten en bloksubsidies ontvangen. Iedere succesvolle blok wordt met cryptografie gelinkt aan de vorige blok.

### blok
Een groepering van transacties die gemarkeerd wordt met een tijdstempel en een vingerafdruk van de vorige blok. De blokhoofding wordt gehashed om een proof-of-work te produceren waarmee de transacties gevalideerd worden. Gevalideerde blokken worden toegevoegd aan de blockchain (blokketen) via consensus op het netwerk.

### geheime sleutel
Een geheim getal waarmee bitcoins kunnen uitgegeven worden vanaf het publiek adres dat overeenkomt met de geheime sleutel.

### genesis blok
De eerste blok in de blockchain die gebruikt werd om het netwerk te initialiseren.

### hash
Een digitale vingerafdruk van een bepaalde binaire input.

### miner
Een miner is een node op het netwerk die valide proof-of-work oplossingen zoekt voor nieuwe blokken. Dit doet een miner door herhaaldelijk te hashen tot een juiste oplossing wordt gevonden.

### moeilijkheidsgraad
Een instelling op het netwerk die bepaald hoeveel computatie vereist is om een proof-of-work te produceren.

### open-source
De software van Bitcoin is open-source of open-broncode. Dit betekent dat iedereen kan lezen hoe het programma werkt. Dit is in tegenstelling tot closed-source of gesloten-broncode waarvan gebruikers niet kunnen achterhalen wat de software precies doet.

### peer-to-peer
Een peer-to-peer netwerk is een netwerk waar alle leden rechtstreeks met elkaar verbinden. Dit is in tegenstelling tot een netwerk waar iedereen met een centrale server verbindt zoals Facebook of Twitter.

### proof-of-work
Een stukje data dat een significante berekening vraagt om te bekomen. In Bitcoin moeten miners een numerieke oplossing vinden van een SHA256 algoritme dat aan een bepaalde vereiste op het netwerk voldoet, de moeilijkheidsgraad.

### satoshi
Een satoshi is de kleinste denominatie van een bitcoin die op de blockchain kan staan. Het is equivalent met 0.00000001 bitcoin en werd vernoemd naar de ontwerper van Bitcoin, Satoshi Nakamoto.

### Satoshi Nakamoto
Satoshi Nakamoto is de naam die gebruikt werd door de persoon (of personen) die Bitcoin ontwierpen en de eerste implementatie ontwikkelden. In 2008 werd op online mailing-lijst door een anonieme entiteit genaamd [`Satoshi Nakamoto`](definities.md#satoshi-nakamoto) de [`Bitcoin whitepaper`](https://bitcoin.org/bitcoin.pdf) gedeeld. Als onderdeel van deze implementatie ontwierpen zij de eerste blockchain databank. Met dit proces waren ze de eerste om het dubbel-uitgavenprobleem op te lossen voor digitaal geld. Hun echte identiteit blijft onbekend. Satoshi verdween in 2011 en is sindsdien niet meer online gezien. Daarna werkten honderden ontwikkelaars verder aan het Bitcoin protocol waarvan de broncode volledig open en vrij beschikbaar is ([`open-source`](definities.md#open-source)).

### transactie
In simpele verwoording is een transactie een transfer van bitcoin van een adres naar een ander. Meer precies is een transactie een ondertekende structuur van data die een expressie is van een transfer van waarde. Transacties worden uitgestuurd over het netwerk, ontvangen door miners en meegenomen in blokken waardoor ze permanent op de blokchain komen te staan.

### unspent transaction output (UTXO)
Een UTXO is een ongespendeerde output die nog kan uitgegeven worden als input in een nieuwe transactie.

### wallet
Een wallet is software die al jouw bitcoin adressen en geheime sleutels beheert. Je gebruikt een wallet om jouw bitcoin te ontvangen, te versturen en te bekijken.
