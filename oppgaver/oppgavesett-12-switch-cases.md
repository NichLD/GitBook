# Page

## Oppgave1

```javascript
const expr = '4';
switch (expr) {
  case '1':
    console.log('Brukeren startet programmet');
    break;
  case '2':
    console.log('Brukeren vil gjøre en utskrift')
    break
  case '3':
    console.log('Brukeren vil avslutte programmet');
    break;
  default:
    console.log('Error')
}
```

***

## Oppgave 2

```javascript
function RegnUt(num1, operator, num2) {
  switch (operator) {
    case "+":
      return num1 + num2
    case "-":
        return num1 - num2;
    case "*":
        return num1 * num2;
    case "/":
        return num1 / num2;
    default:
      return "Syntax error"
  }
}

const result = RegnUt(5, "+", 10)
console.log(result) // 15
```
