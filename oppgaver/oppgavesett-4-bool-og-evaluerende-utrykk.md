# Oppgavesett 4: bool og evaluerende utrykk

## Oppgave 1

a) `console.log(1 === 1)` - Utskrift: `true` \
b) `console.log(1 === 2)` - Utskrift: `false` \
c) `console.log(3 == 3)` - Utskrift: `true` \
d) `console.log(2 == 3)` - Utskrift: `false`

## Oppgave 2

a) `console.log(1 == '1')` - Utskrift: `true` \
b) `console.log(2 === '2')` - Utskrift: `false`&#x20;

{% hint style="info" %}
Forskjellen mellom `==` og `===` er at `===` også sammenligner datatyper, mens `==` utfører en løsere sammenligning ved å konvertere datatyper
{% endhint %}

## Oppgave 3

a) `console.log(1 == 1 && 2 == 2)` - Utskrift: `true` \
b) `console.log(1 === '1' && 2 === 2)` - Utskrift: `false` \
c) `console.log(1 === 1 && '2' === 2)` - Utskrift: `false` \
d) `console.log(1 == '1' && 2 == '2')` - Utskrift: `false`

## Oppgave 4

a) `console.log(1 === '1' || 2 === 2)` - Utskrift: `true` \
b) `console.log(2 == '2' || 1 === '1')` - Utskrift: `true` \
c) `console.log(2 === 2 || 1 === 1 || 3 === '3')` - Utskrift: `true`

## Oppgave 5

a) `console.log(1 !== 1)` - Utskrift: `false` \
b) `console.log(2 !== 1)` - Utskrift: `true` \
c) `console.log(2 !== 1 && 1 === 1)` - Utskrift: `false` \
d) `console.log(2 !== '2' && 1 === '1' || 2 == '2')` - Utskrift: `true`
