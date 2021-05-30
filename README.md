# shorter-js 
a curated list for Javascript tricks & tips to write a shorter & cleaner code with Javascipt built-in features . 

> check the Laravel Version of this file [here](https://github.com/adnane-ka/shorter-lara) .

#### Arrays 
* Filter Unique Values .
* Remove Falsy Values From Arrays .
* Shorthand Way To Sort numbers arrays . 

#### Loops 
* Short Way to do For Loops

#### Other 
* Count Speed & Performance of an Algorithm 
* Every and some
* use this instead of string concatenation !
* Get rid of if conditions !
* Throw Console Errors !
* Get Query Params ! 
* Disable Right Click

---
## Arrays 

### Filter Unique Values
```js
const array = [1, 1, 2, 3, 5, 5, 1]
const unique = [...new Set(array)];

console.log(unique); // [1, 2, 3, 5]
```

### Remove Falsy Values From Arrays
```js 
// Falsy Values Are : undefined , null , NaN , 0 , empty strings , false
myArray.filter(Boolean);

```
### Shorthand Way To Sort numbers arrays 

```js
[0,10,4,9,123,54,1].sort((a,b) => a-b);
>>> [0, 1, 4, 9, 10, 54, 123]
```
---
## Loops 

### Short Way to do For Loops
```js
const names = ["Kio", "Rio", "Mac"];

// Old Version
for (let i = 0; i < names.length; i++) {
  const name = names[i];
  console.log(name);
}

// New Version
for (let name of names) console.log(name);
```

---
## Other 

### Count Speed & Performance of an Algorithm  
```js
const firstTime = performance.now();
something();
const secondTime = performance.now();
console.log(`The something function took ${secondTime - firstTime} milliseconds.`);
```

### Every and some
```js
const random_numbers = [ 13, 2, 37, 18, 5 ]
const more_random_numbers = [ 0, -1, 30, 22 ]

const isPositive = (number) => {
  return number > 0
}

random_numbers.every(isPositive); // returns true
more_random_numbers.every(isPositive); // returns false
```

### use this instead of string concatenation !
```js 
// instead of 
let messageConcat = 'Mr. ' + name + ' is from ' + place;

// you can 
let messageTemplateStr = `Mr. ${name} is from ${place}.`;
```

### Get rid of if conditions !
```js 
// instead of 
if (isPrime) {
    startWatching();
}

// you can 
isPrime && startWatching();
```

### Throw Console Errors !
```js 
let isRequired = () => {
    throw new Error('This is a required parameter.');
}
```

### Get Query Params ! 
```js 
let nyParam = new URLSearchParams(location.search).get('nyParam');
```

### Disable Right Click 
```html
<body oncontextmenu="return false">
    <div></div>
</body>
```
---


