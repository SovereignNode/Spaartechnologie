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
| input 1 | 0.10 BTC | output 2 | 0.10 BTC |
| input 2 | 0.30 BTC | output 2 | 0.20 BTC |
|         |          | output 2 | 0.08 BTC |
|         |          |          |          |
| **totaal**  | **0.40 BTC** | **totaal**   | **0.38 BTC** |


~~~
impliciete transactiekost = inputs - outputs = 0.02 BTC
~~~

De inputs die in een transactie worden uitgegeven bevatten een handtekening van de sleutels van hun eigenaar. Zo'n digitale handtekening kan door iedereen op het netwerk eenvoudig gecontroleerd worden. De handtekening hoef je niet zelf te maken. Dit doet de software voor jou.

Veel bitcoin transacties zullen wisselgeld bevatten als output. De inputs kunnen namelijk niet gedeeld worden. Wanneer je in de winkel met een biljet van €20 betaalt voor een product van €5 dan krijg je €15 terug. Hetzelfde geldt voor bitcoin transacties. Gebruik je een input van 1BTC voor een betaling van 0.1BTC dan gebruik je de volledige input van 1BTC en stuur je 0.9BTC terug naar een adres van jezelf (min transactiekost).

Samenvattend, sturen transacties waarde van transactie-inputs naar transactie-outputs. De gebruikte inputs zijn outputs van een vorige transactie en laten zien van waar het geld komt. De transactie-outputs van de transactie toont de nieuwe bestemming voor het geld en kan eventueel wisselgeld bevatten. De nieuw aangemaakte outputs kunnen vervolgens opnieuw gebruikt worden in een volgende transactie. Outputs die nog niet opnieuw uitgegeven werden noemen we [*Unspent Transaction Outputs*](definities.md#unspent-transaction-output) (UTXO's). Het saldo van jouw wallet toont dus de som van UTXO's op adressen waar jij de sleutels van beheert.

## Stuur bitcoin naar je spaarrekening

1. Open Relai en ga naar het tweede tabblad (met het Bitcoin logo).
2. Druk op 'send BTC' om jouw transactie voor te bereiden.
3. Kies 'BTC', 'slow' en druk op 'max' en bevestig met next.
4. Open BlueWallet en ga naar jouw Spaarpotje
5. Druk op 'receive'
6. Scan de QR-code of kopieer het adres. Indien beide wallets op hetzelfde toestel staan, kan je de QR-code niet gebruiken.
7. Plak het adres van de ontvanger in de Relai app. Opgelet: vóór het adres staat bitcoin:. Dit stuk moet je verwijderen zodat Relai het adres correct herkent. Druk op 'next'
8. **Controleer** nogmaals dat dit adres juist is en bevestig met 'confirm'. De transactie wordt nu verstuurd naar het netwerk.
10. In BlueWallet zie je de transactie reeds verschijnen. Let op: deze transactie werd nog niet bevestigd (conf: 0). Gemiddeld iedere 10 minuten wordt een nieuwe blok met transacties toegevoegd aan de ketting. De ruimte is beperkt dus hoe meer transactiekosten je betaalt, hoe sneller miners jouw transactie zullen toevoegen in de ketting van blokken. Je kan pas spreken van een bevestigde betaling wanneer je minstens 1 confirmatie hebt.
11. Druk op de transactie en ga naar details.
12. Voeg een notitie toe zodat je in de toekomst makkelijk herkent waar deze bitcoins vandaan kwamen. Druk op 'save'
Bitcoin is digitaal geld. De vraag wat geld precies is, kan niet simpel beantwoord worden. Al honderden jaren zijn we op zoek naar het antwoord en misschien is er zelfs geen correct antwoord. Maar de zoektocht op zich is zeker al de moeite waard. We spenderen vele jaren van ons leven aan werk om geld te verdienen en iedere transactie die we doen wordt geintermedieerd door geld. Toch kunnen we de vraag vaak moeilijk beantwoorden. Het loont de moeite om daar eens wat meer over na te denken.


------

[Terug naar overzicht](overzicht.md) --
[Verder gaan](stap4.md)
