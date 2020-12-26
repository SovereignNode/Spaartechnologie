---
layout: page
title: Stap 3 - Begrijpen hoe transacties werken
show_in_menu: false
disable_anchors: true
---
## Principes
* Een bitcoin transactie is tekst die met het netwerk gedeeld wordt
* De transactie vertelt het netwerk dat de eigenaar van de sleutels de overdracht van bitcoins autoriseerd
* Om een transactie te versturen betaal je een vergoeding aan miners
* Een transactie is pas bevestigd indien een miner ze toevoegt aan een blok

## Hoe werkt een transactie?
Een bitcoin transactie werkt volgens het principe van dubbel-boekhouden. Iedere transactie bevat `inputs` en `outputs`. De inputs debiteren een specifiek adres met bitcoin op. Aan de andere kant van de transactie staan outputs die dan weer adressen crediteren met bitcoin. De som van de inputs is niet gelijk aan de som van de outputs. Het verschil is een vergoeding of *fee* die miners ontvangen.

| input   | waarde   | output   | waarde   |
|:-----   | :-----   | :-----   | :-----   |
| input 1 | 0.10 BTC | output 1 | 0.10 BTC |
| input 2 | 0.30 BTC | output 2 | 0.20 BTC |
|         |          | output 3 | 0.08 BTC |
|         |          |          |          |
| **totaal** | **0.40 BTC** | **totaal**  | **0.38 BTC** |
|         |          |  **fee**   |   **0.02 BTC**       |


De inputs die in een transactie worden uitgegeven bevatten een handtekening van de sleutels van hun eigenaar. Zo'n digitale handtekening kan door iedereen op het netwerk eenvoudig gecontroleerd worden. De handtekening hoef je niet zelf te maken. Dit doet de software voor jou.

Veel bitcoin transacties zullen wisselgeld bevatten als output. De inputs kunnen namelijk niet gedeeld worden. Wanneer je in de winkel met een biljet van €20 betaalt voor een product van €5 dan krijg je €15 terug. Hetzelfde geldt voor bitcoin transacties. Gebruik je een input van 1 BTC voor een betaling van 0.1 BTC dan gebruik je de volledige input van 1 BTC en stuur je 0.9 BTC terug naar een adres van jezelf (min fee).

| input      | waarde      | output     | waarde        |
|:-----      | :-----      | :-----     | :-----        |
| input 1    | 1.0  BTC    | output 1   | 0.10 BTC      |
|            |             | output 2   | 0.898 BTC     |
|            |             |            |               |
| **totaal** | **1.0 BTC** | **totaal** | **0.998 BTC** |
|            |             | **fee**    | **0.002 BTC** |

Samenvattend, sturen transacties waarde van transactie-inputs naar transactie-outputs. De gebruikte inputs zijn outputs van een vorige transactie en laten zien van waar het geld komt. De transactie-outputs van de transactie toont de nieuwe bestemming voor het geld en kan eventueel wisselgeld bevatten. De nieuw aangemaakte outputs kunnen vervolgens opnieuw gebruikt worden in een volgende transactie. Outputs die nog niet opnieuw uitgegeven werden noemen we [*Unspent Transaction Outputs*](definities.md#unspent-transaction-output) (UTXO's). Het saldo van jouw wallet toont dus de som van UTXO's op adressen waar jij de sleutels van beheert.

## Stuur bitcoin naar je spaarrekening

Open Blue Wallet en navigeer naar je spaarrekening. Kies `Ontvang` en druk op het adres dat getoond wordt. Het adres wordt gekopieerd naar het klembord. Een adres ziet er als volgt uit:

~~~
bc1qun4eca6h3yrl2ss483frzz8jk6pgrmh2frlfj3
~~~

Open de rekening van Relai binnen de Blue Wallet app. Kies vervolgens `Verstuur` en plak het adres in de voorziene ruimte. We kiezen het bedrag om te versturen. Tik rechtsboven op de drie puntjes en selecteer `Gebruik volledige saldo`.

![bluewallet-send](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/bw-send.png?raw=true)

Kies een notitie om zelf later de oorsprong van het geld te kunnen achterhalen (bvb. 'Van Relai').

Vervolgens kiezen we een *fee*. De ruimte in blokken is beperkt. Hoe hoger de fee die je betaalt, hoe sneller de miners jouw transactie zullen kiezen om in een afgewerkte blok te plaatsen. Aangezien we naar onze eigen rekening sturen, hebben we geen haast. Druk op het groene vak en kies een lage fee.

![bluewallet-send-fee](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/bw-send-fee.png?raw=true)

Druk op `Volgende`. Je krijg nog een overzicht van de transactie. Kies `Nu verzenden` om de transactie te versturen naar het netwerk. Je krijgt een bevestiging en kan op `Klaar` drukken.

![bluewallet-send-confirm](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/bw-send-confirm.png?raw=true)

Het kan even duren voor je wallet de inkomende transactie herkent. Voorlopig blijft het saldo van je spaarrekening op 0 staan. Wanneer miners de transactie in een blok plaatsen zal het bedrag verhoogd worden. Tot die tijd geeft je wallet enkel de transactie met als kenmerk `In afwachting`. Even geduld...

![bluewallet-send-done](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/bw-send-done.png?raw=true)

Gefeliciteerd! Je hebt zonet je eerste bitcoin transactie verstuurd. Om te begrijpen wat er nu precies gebeurt met deze transactie moeten we iets dieper ingaan op de verschillende rollen die de leden op het netwerk vervullen.

## Fee's, mempools, miners en blokken

Waneer je de details van de onbevestigde transactie bekijkt kan je een transactie-ID terugvinden. Deze *Txid* kan je opzoeken in een [*block explorer*](faq.md#wat-is-een-block-explorer). We gebruiken [mempool.space](https://mempool.space/nl/){:target="_blank"}.

Bovenstaande transactie kan je [hier](https://mempool.space/nl/tx/bc5a6570e677d4614c648e4e82c7984ff205ed80e85fc27dae848addf41cd974) bekijken. Wanneer je vanuit je wallet een transactie verstuurt dan komt dit terecht in een pot met onbevestigde transacties. Dit noemen we de [*mempool*](definities.md#mempool). Op enkele seconden tijd wordt de transactie naar alle uithoeken op de wereld gestuurd. Iedereen die een zogenaamde Bitcoin [*node*](faq.md#wat-is-een-node) draait, ontvangt dit en stuurt het door naar andere *nodes*. Er is dus niet één mempool maar wel heel veel verschillende mempools.

Sommige van deze *nodes* zijn tegelijk ook *miners*. De miners concurreren met elkaar om de oplossing te vinden op een puzzel die hen toelaat om een nieuwe blok te maken. De [moeilijkheidgraad](definities.md#moeilijkheidsgraad) van de puzzel wordt om de 2016 blokken aangepast zodat er gemiddeld iedere 10 minuten een nieuwe blok wordt gevonden. We komen later terug op deze puzzel maar voorlopig volstaat om te begrijpen dat ongeveer iedere 10 minuten een miner een nieuwe blok mag toevoegen aan de blockchain. De winnaar kiest de transacties met de hoogste *fee's* en propt de blok vol. De ruimte in zo'n blok is ongeveer 1 megabyte. De winnaar stuurt zijn oplossing naar de rest van het netwerk die de oplossing op hun beurt makkelijk kunnen controleren. Indien de miner een blok stuurde die door de andere leden van het netwerk geaccepteerd wordt, ontvangt hij een *bloksubsidie* en alle transactiekosten. De wedstrijd start vervolgens opnieuw.

Bovenstaande, onbevestigde transactie ziet er als volgt uit:

![unconfirmedtx](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/mempool-unconfirmedtx.png?raw=true)

We zien dat:
* de transactie in totaal 215 bytes groot is
* een vergoeding van 1,4 sats per vByte betaalt aan de miners
* de fee in totaal 192 sats is (0.00000192 BTC)

Nieuwe blokken zullen eerst transacties kiezen die een hogere fee bieden. Tijdens weekends is het doorgaans wat minder druk op het netwerk en werken de miners hun achterstand weg.

Daarnaast toont de [*block explorer*](faq.md#wat-is-een-block-explorer) ons ook de inputs en de outputs. In dit geval is er maar 1 input en 1 output.

De input is mijn adres van Relai:
~~~
3E1cSyzCQ8s4j4xJCeCU4qKRh558FuFTqZ
~~~

De output is mijn adres van de spaarrekening in Blue Wallet:
~~~
bc1qun4eca6h3yrl2ss483frzz8jk6pgrmh2frlfj3
~~~

Bitcoin adressen komen in verschillende types. In dit geval is het adrestype van Relai niet gelijk aan het adrestype van onze spaarrekening.

Tot slot, bekijken we nog eens wat er in een blok zit. De blokken worden aangeduid met een *blokhoogte*. [Hier](https://mempool.space/nl/block/00000000000000000001ec5cf589abfeed744046f30bbc715885b090ca6fff15) vind je blok 662805.

![block](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/mempool-block.png?raw=true)

In totaal ontvang de miner 7,17 BTC aan beloning. Dit bedrag bestaat uit 6,25 BTC *bloksubsidie* en 0,92 BTC aan *fee's*. De eerste transactie in iedere blok bevat de *coinbase-transactie*. Deze transactie ontgint de nieuwe bitcoin en stuurt ze naar een adres van de miner. Alle andere transacties zijn van gebruikers die bitcoin willen versturen en daar vaak een hoge *fee* voor over hebben.

## Transactie versnellen
Met Blue Wallet is het mogelijk om een transactie sneller te laten bevestigen. Je stuurt dan een nieuwe transactie met een iets hogere fee. Deze tweede transactie stuurt het geld van je eerste adres (dat nog niet bevestigd is) naar een nieuw adres in jouw wallet. Druk op de transactie die nog `In afwachting` is en kies voor `Bump fee`. Selecteer een gepaste transactiekost en kies `Creëer`. In het volgende scherm druk je op `Nu verzenden`.

![bw-rbf](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/bw-rbf.png?raw=true)
![bw-rbf-fee](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/bw-rbf-fee.png?raw=true)
![bw-rbf-confirm](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/bw-rbf-confirm.png?raw=true)
![bw-rbf-show](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/bw-rbf-show.png?raw=true)

We kunnen opnieuw controleren op [mempool.space](https://mempool.space/nl/) hoe de status van onze transactie is.

![mempool-rbf](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/mempool-rbf.png?raw=true)

De transactie werd bevestigd in een blok en staat op een [nieuw adres](https://mempool.space/nl/address/bc1q726u37zg6dpgzcjrqufj2pc7eahhjfxppm9eqw) waar onze wallet ook de sleutels van beheert. Het eerste adres ontving de bitcoin en stuurde ze onmiddellijk opnieuw uit.

------

[Terug naar overzicht](overzicht.md) --
[Verder gaan](stap4.md)
