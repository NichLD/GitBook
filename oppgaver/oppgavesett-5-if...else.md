# Oppgavesett 5: if...else

## Oppgave 1

```javascript
function sjekkType(parameter) {
    if (typeof parameter === 'string') {
        console.log("STRING STRING STRING!");
    } else {
        console.log("Dette er ikke en String i det hele tatt");
    }
}

// Test med argumenter
sjekkType(1);    // Dette er ikke en String i det hele tatt
sjekkType('1');  // STRING STRING STRING!
sjekkType('Navn');  // STRING STRING STRING!
```

***

## Oppgave 2

```javascript
function sjekkTypeAvArgumenter(arg1, arg2) {
    if (typeof arg1 === typeof arg2) {
        console.log("Argumentene du brukte er av samme type!");
    } else {
        console.log("Argumentene du brukte er IKKE av samme type!");
    }
}

// Test med argumenter
sjekkTypeAvArgumenter('en', 1);  // Argumentene du brukte er IKKE av samme type!
sjekkTypeAvArgumenter(1, 1);    // Argumentene du brukte er av samme type!
sjekkTypeAvArgumenter(2, 3);    // Argumentene du brukte er IKKE av samme type!
sjekkTypeAvArgumenter('2', '3');  // Argumentene du brukte er av samme type!
sjekkTypeAvArgumenter(2, '3');    // Argumentene du brukte er IKKE av samme type!
```

***

## Oppgave 3

```javascript
function sjekkParametere(param1, param2, param3) {
    if ((typeof param1 === typeof param2) || (typeof param3 === 'number' && param3 > 5)) {
        console.log("Det er to parametere av samme type her, ELLER så er det tall som er høyere enn FEM!!!");
    } else {
        console.log('FAIL!');
    }
}

// Test med argumenter
sjekkParametere('abc', 'def', 7);  // Det er to parametere av samme type her, ELLER så er det tall som er høyere enn FEM!!!
sjekkParametere(2, 'xyz', 3);     // FAIL!

```

***

## Oppgave 4

```javascript
function sjekkArrayType(arr) {
    if (Array.isArray(arr)) {
        let antallTall = 0;
        let antallOrd = 0;

        arr.forEach(element => {
            if (typeof element === 'number') {
                antallTall++;
            } else if (typeof element === 'string') {
                antallOrd++;
            }
        });

        console.log(`Arrayen inneholder ${antallTall} tall og ${antallOrd} ord!`);
    } else {
        console.log("Dette er ikke en array!");
    }
}

// Test med argument
sjekkArrayType([1, 'two', 3, 'four']);  // Arrayen inneholder 2 tall og 2 ord!
sjekkArrayType("Dette er ikke en array");  // Dette er ikke en array!
```

***
