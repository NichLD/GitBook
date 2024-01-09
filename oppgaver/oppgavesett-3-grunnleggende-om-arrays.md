# Oppgavesett 3: Grunnleggende om arrays

## Oppgave 1

a. Hensikten med en array er å lagre og organisere en samling av elementer under ett navn.

b. Arrays i Javascript er dynamiske og kan ha elementer av forskjellige typer

***

## Oppgave 2

{% code title="oppgave 2A" %}
```javascript
let enderIBy = [];
```
{% endcode %}

{% code title="oppgave 2B" %}
```javascript
enderIBy[0] = "Donald";
enderIBy[1] = "Dolly";
enderIBy[2] = "Ole";
enderIBy[3] = "Dole";
enderIBy[4] = "Doffen";
enderIBy[5] = "Fetter Anton";
enderIBy[6] = "Magica fra Tryll";
enderIBy[7] = "Petter smart"; // Vet ikke om det er en and en gang 
enderIBy[8] = "Elvira Kvakk";
enderIBy[9] = "Onkel Skrue";
```
{% endcode %}

{% code title="Oppgave 2C" %}
```javascript
console.log(enderIBy[2], enderIBy[5], enderIBy[8]);
```
{% endcode %}

{% code title="Output 2C" %}
```
[Log] Ole – "Fetter Anton" – "Elvira Kvakk"
```
{% endcode %}

***

## Oppgave 3

a) En index i en array er en numerisk verdi som representerer posisjonen til et element i arrayet.

b) Den første indexen i en array er alltid 0.

c) Den siste indexen i en array er alltid (array.length - 1).

d) Lengden på en array (array.length) angir antallet elementer i arrayet.

e) Sammenhengen mellom lengden og siste index er at den siste indexen alltid er ett mindre enn lengden på arrayet.

***

## Oppgave 4

a) `typeof` operatøren vil returnere "object" hvis den brukes på en array.

b) For å sjekke om en variabel er en array, kan du bruke `Array.isArray(variable)`.

{% code title="oppgave 4C" %}
```javascript
let EksempelArray = [];

function sjekkArray(argument) {
  if (Array.isArray(argument)) {
    console.log("Argumentet er en array");
  } else {
    console.log("Argumentet er ikke en array");
  }
}

print(sjekkArray(EksempelArray))
```
{% endcode %}

{% code title="output 4C" %}
```
[Log] Argumentet er en array
```
{% endcode %}
