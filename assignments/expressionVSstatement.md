# Expression vs Statement

## Write down if the code is valid or not with reason.

1. What is the output or error of the code below.

```js
function add(a = 0, b = 0){
   return a + b;
 }
 let result = add(21,23);
 console.log(result); // 44
```

2. What is the output or error of the code below.

```js
function add(a = 0, b = 0) {
  return a + b;
}
let result = add(21,23);
 console.log(result); // 44
```

3. What is the output or error of the code below.

```js
function add(a = 0, b = 0) {
  return a + b;
}
add(21, 23); // 44
```

4. What is the output or error of the code below.

```js
function add(a = 0, b) {
  return a + b;
}
add(21); // Nan
```

5. What is the output or error of the code below.

```js
function add(a = 0, b = 0) {
  return a + b;
}
add(undefined, 21);//21
```

6. What is the output or error of the code below.

```js
function knowWhy(value) {
  if(value === 21){ // no  return
    return "Yes"; //semicolon must
  } else {
    return "No"; //semicolon must
  }
}
knowWhy(211); // "No"
```

7. What is the output or error of the code below.

```js
function knowWhy(value) {
  if(value === 21){   // no return with if statement
    return "Yes"; // semicolon must
  } else {
    return "No"; // semicolon must
  }
}
knowWhy(21); // "Yes"
```

8. What is the output or error of the code below.

```js
function isItIf(ifElse) {
  return ifElse;
}
isItIf(if(true)){ // if statement can't come , value is neede.
  console.log('Testing');
  }
```
