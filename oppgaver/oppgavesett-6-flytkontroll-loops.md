# Oppgavesett 6: Flytkontroll, loops

## Oppgave 1

#### for-løkke

```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

#### while-løkke

```javascript
let i = 0;
while (i < 5) {
  console.log(i);
  i++;
}
```

#### do-while-løkke

```javascript
let i = 0;
do {
  console.log(i);
  i++;
} while (i < 5);
```

#### For-inn-løkke

```javascript
const obj = { a: 1, b: 2, c: 3 };
for (const key in obj) {
  console.log(`${key}: ${obj[key]}`);
}
```

#### For-off-løkke

```javascript
const arr = [1, 2, 3, 4, 5];
for (const element of arr) {
  console.log(element);
}
```

## Oppgave 2

```javascript
const navneliste = ['Geir', 'Espen', 'Ellen', 'Erik', 'Lars', 'Gunnar', 'Oda', 'Nina', 'Tine', 'Henrik', 'Agnethe'];

for (const navn of navneliste) {
  console.log(`${navn} har ${navn.length} bokstaver.`);
}
```

<details>

<summary>Oppgave 2 output [log]</summary>

{% code title="Oppgave 2 output" %}
```
[log] Geir har 4 bokstaver.
[log] Espen har 5 bokstaver.
[log] Ellen har 5 bokstaver.
[log] Erik har 4 bokstaver.
[log] Lars har 4 bokstaver.
[log] Gunnar har 6 bokstaver.
[log] Oda har 3 bokstaver.
[log] Nina har 4 bokstaver.
[log] Tine har 4 bokstaver.
[log] Henrik har 6 bokstaver.
[log] Agnethe har 7 bokstaver.

```
{% endcode %}

</details>

Jeg valgte for-of-løkken fordi den er enklere å lese og mer egnet når du trenger å gå gjennom elementene i en array.

## Oppgave 3

```javascript
const navneliste = ['Geir', 'Espen', 'Ellen', 'Erik', 'Lars', 'Gunnar', 'Oda', 'Nina', 'Tine', 'Henrik', 'Agnethe'];

const nyNavneliste = [];

for (let i = navneliste.length - 1; i >= 0; i--) {
    nyNavneliste.push(navneliste[i]);
}

console.log(nyNavneliste);
```

{% code title="Oppgave 3 output" %}
```
['Agnethe', 'Henrik', 'Tine', 'Nina', 'Oda', 'Gunnar', 'Lars', 'Erik', 'Ellen', 'Espen', 'Geir'
```
{% endcode %}

## Oppgave 4

```javascript
function reduceToOddNumber(number) {
  if (typeof(number) == 'number') {
    while (number % 2 === 0) {
      number = number / 2;
    }
  }
  return number;
}
```

## Oppgave 5

De to løkkene som ikke ble brukt  er **for-in** og **do-while**.

{% hint style="info" %}
**for-in**-løkken ble ikke brukt.
{% endhint %}

{% hint style="info" %}
**do-while**-løkken kunne ha blitt brukt i oppgave 4, men jeg valgte en **while**-løkke fordi det virket enklere mot oppgaven.
{% endhint %}
