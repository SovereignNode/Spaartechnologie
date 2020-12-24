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
Een bitcoin transactie werkt volgens het principe van dubbel-boekhouden. Iedere transactie bevat `inputs` en `outputs`. De inputs debiteren een specifiek adres met bitcoin op. Aan de andere kant van de transactie staan outputs die dan weer adressen crediteren met bitcoin. De som van de inputs is niet gelijk aan de som van de outputs. Het verschil is de transactiekost die miners ontvangen.

| input   | waarde   | output   | waarde   |
|:-----   | :-----   | :-----   | :-----   |
| input 1 | 0.10 BTC | output 1 | 0.10 BTC |
| input 2 | 0.30 BTC | output 2 | 0.20 BTC |
|         |          | output 3 | 0.08 BTC |
|         |          |          |          |
| **totaal**  | **0.40 BTC** | **totaal**   | **0.38 BTC** |


~~~
transactiekost = inputs - outputs = 0.02 BTC
~~~

De inputs die in een transactie worden uitgegeven bevatten een handtekening van de sleutels van hun eigenaar. Zo'n digitale handtekening kan door iedereen op het netwerk eenvoudig gecontroleerd worden. De handtekening hoef je niet zelf te maken. Dit doet de software voor jou.

Veel bitcoin transacties zullen wisselgeld bevatten als output. De inputs kunnen namelijk niet gedeeld worden. Wanneer je in de winkel met een biljet van €20 betaalt voor een product van €5 dan krijg je €15 terug. Hetzelfde geldt voor bitcoin transacties. Gebruik je een input van 1BTC voor een betaling van 0.1BTC dan gebruik je de volledige input van 1BTC en stuur je 0.9BTC terug naar een adres van jezelf (min transactiekost).

| input   | waarde   | output   | waarde   |
|:-----   | :-----   | :-----   | :-----   |
| input 1 | 1.0  BTC | output 1 | 0.10 BTC |
|         |          | output 2 | 0.898 BTC |
|         |          |          |          |
| **totaal**  | **1.0 BTC** | **totaal**   | **0.998 BTC** |


~~~
transactiekost = inputs - outputs = 0.002 BTC
~~~

Samenvattend, sturen transacties waarde van transactie-inputs naar transactie-outputs. De gebruikte inputs zijn outputs van een vorige transactie en laten zien van waar het geld komt. De transactie-outputs van de transactie toont de nieuwe bestemming voor het geld en kan eventueel wisselgeld bevatten. De nieuw aangemaakte outputs kunnen vervolgens opnieuw gebruikt worden in een volgende transactie. Outputs die nog niet opnieuw uitgegeven werden noemen we [*Unspent Transaction Outputs*](definities.md#unspent-transaction-output) (UTXO's). Het saldo van jouw wallet toont dus de som van UTXO's op adressen waar jij de sleutels van beheert.

## Stuur bitcoin naar je spaarrekening

Open Blue Wallet en navigeer naar je spaarrekening. Kies `Ontvang` en druk op het adres dat getoond wordt. Het adres wordt gekopieerd naar het klembord. Een adres ziet er als volgt uit:

~~~
bc1qun4eca6h3yrl2ss483frzz8jk6pgrmh2frlfj3
~~~

Open de rekening van Relai binnen de Blue Wallet app. Kies vervolgens `Verstuur` en plak het adres in de voorziene ruimte.[^1]

[^1]: blijf drukken in de ruimte voor het adres en kies `Plakken` of `Paste`.

We kiezen het bedrag om te versturen. Tik rechtsboven op de drie puntjes en selecteer `Gebruik volledige saldo`.

![bluewallet-send](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/bw-send.png?raw=true)

Kies een notitie (die enkel voor jezelf is en niet wordt meegestuurd in de transactie). Het kan nuttig zijn om de oorsprong van de bitcoin te noteren (bvb. 'Van Relai').

Vervolgens kiezen we een transactiekost of *fee*. De ruimte in blokken is beperkt. Hoe hoger de fee die je betaalt, hoe sneller de miners jouw transactie zullen kiezen om aan de ketting toe te voegen. Echter, aangezien we naar onze eigen rekening sturen, hebben we geen haast. Druk op het groene vak en kies een lage fee.

![bluewallet-send-fee](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/bw-send-fee.png?raw=true)

Druk op `Volgende`. Je krijg nog een overzicht van de transactie. Kies `Nu verzenden` om de transactie te versturen naar het netwerk. Je krijgt een bevestiging en kan op `Klaar` drukken.

![bluewallet-send-confirm](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/bw-send-confirm.png?raw=true)

Het kan even duren voor je wallet de inkomende transactie herkent. Voorlopig blijf je saldo van je spaarrekening op 0 staan. Wanneer miners de transactie in een blok plaatsen zal het bedrag verhoogd worden. Tot die tijd geeft je wallet enkel de transactie met als kenmerk `In afwachting`. Even geduld...

![bluewallet-send-done](https://github.com/SovereignNode/Spaartechnologie/blob/master/documentation/images/bw-send-done.png?raw=true)

Gefeliciteerd! Je hebt zonet je eerste bitcoin transactie verstuurd. Om te begrijpen wat er nu precies gebeurt met deze transactie moeten we iets dieper ingaan op de verschillende rollen die de leden op het netwerk vervullen.

## Transactiekosten, mempools, miners en blokken



------

[Terug naar overzicht](overzicht.md) --
[Verder gaan](stap4.md)
