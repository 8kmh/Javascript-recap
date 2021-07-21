# Les boucles en javascript

## La boucle **_for_**

L'instruction **_for_** crée une boucle composée de trois expressions optionnelles séparées par des points-virgules et encadrées entre des parenthèses qui sont suivies par une instruction (généralement une instruction de bloc) à éxécuter dans la boucle.

```js
for (i = 0; i < 10; i++) {
  console.log(i);
}

// résultat : 0 1 2 3 4 5 6 7 8 9
```

### Syntaxe

`for ([initialisation]; [condition]; [expression_finale]) instruction`

---

## La boucle **_while_**

L'instruction **_while_** permet de créer une boucle qui s'exécute tant qu'une condition de test est vérifié (age < 48 == true). La condition (age < 48) est évaluée avant d'exécuter l'instruction contenue dans la boucle (age++).

```js
let age = 5;

while (age < 48) {
  age++;
}

console.log(age);
// résultat : 48
```

### Syntaxe

`while (condition) instruction`

---

## La boucle **_for...in_**

L'instruction **_for...in_** permet d'itérer sur les propriétés énumérables d'un objet qui ne sont pas des symboles. Pour chaques propriété obtenue, on éxécute une instruction (ou plusieurs grâce à un bloc d'instructions).

```js
const weapons = ["épée", "masse", "hache", "arc"];

for (let weapon in weapons) {
  console.log(weapons[weapon]);
}

// résultat : épée, masse, hache, arc
```

### Syntaxe

`for (variable in objet) {instructions}`

---

## La boucle **_for...of_**

L'instruction **_for...of_** permer de créer une boucle Array qui parcourt un objet itérable (ce qui inclut les objets Array, Map, Set, String, TypedArray, l'objet arguments, etc.) et qui permet d'exécuter une ou plusieurs instructions pour la valeur de chaque propriété.

```js
const weapons = ["épée", "masse", "hache", "arc"];

for (let weapon of weapons) {
  console.log(weapon);
}

// résultat : épée, masse, hache, arc
```

### Syntaxe

`for (variable of iterable) {instructions}`

---

## La boucle **_Array.prototype.forEach_**

La méthode forEach() permet d'exécuter une fonction donnée sur chaque élément d'un tableau.

```js
const weapons = ["épée", "masse", "hache", "arc"];

weapons.forEach((weapon) => {
  console.log(weapon);
});

// résultat : épée, masse, hache, arc
```

### Syntaxe

`arr.forEach(callback);`
`arr.forEach(callback, thisArg);`
