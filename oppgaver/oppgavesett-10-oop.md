# Oppgavesett 10: OOP

## Oppgave 1

```javascript
let elev1 = {
  fornavn: "Ola",
  etternavn: "Nordmann",
  Alder: 17
};

let elev2 = {
  fornavn: "Kari",
  etternavn: "Nordkvinne",
  Alder: 17
};

let elev3 = {
  fornavn: "Per",
  etternavn: "Hansen",
  Alder: 17
};

let elev4 = {
  fornavn: "Anne",
  etternavn: "Olsen",
  Alder: 17
};
```

## Oppgave 2

```javascript
function printStudent(student) {
  console.log(`Navn: ${student.fornavn} Etternavn: ${student.etternavn} Alder: ${student.Alder}`);
}

printStudent(elev1);
printStudent(elev2);
printStudent(elev3);
printStudent(elev4);
```

## Oppgave 3

```javascript
function carFactory(set, hp, model, type) {
  return {
    seter: set,
    hestekrefter: hp,
    modell: model,
    biltype: type
  };
}

let biler = [
  carFactory(5, 200, "Sedan", "Sedan"),
  carFactory(7, 250, "SUV", "SUV"),
  carFactory(5, 180, "Stasjonsvogn", "Stasjonsvogn"),
  carFactory(4, 220, "Coupe", "Coupe")
];

console.log(biler);
```

## Oppgave 4

```javascript
function carFactoryWithSerial(set, hp, model, type) {
  return {
    seter: set,
    hestekrefter: hp,
    modell: model,
    biltype: type,
    serienummer: generateSerial()
  };

  function generateSerial() {
    return Math.floor(Math.random() * 1000000);
  }
}

let bilerMedSerienummer = [
  carFactoryWithSerial(5, 200, "Sedan", "Sedan"),
  carFactoryWithSerial(7, 250, "SUV", "SUV"),
  carFactoryWithSerial(5, 180, "Stasjonsvogn", "Stasjonsvogn"),
  carFactoryWithSerial(4, 220, "Coupe", "Coupe")
];

console.log(bilerMedSerienummer);
```

## Oppgave 5

```javascript
function generateCarFactory(merke) {
  return function (set, hp, model, type) {
    return {
      seter: set,
      hestekrefter: hp,
      modell: model,
      biltype: type,
      merke: merke
    };
  };
}

let fordCarFactory = generateCarFactory("Ford");

let fordBiler = [
  fordCarFactory(5, 200, "Sedan", "Sedan"),
  fordCarFactory(7, 250, "SUV", "SUV"),
  fordCarFactory(5, 180, "Stasjonsvogn", "Stasjonsvogn"),
  fordCarFactory(4, 220, "Coupe", "Coupe")
];

console.log(fordBiler);
```
