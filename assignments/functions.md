1. 🎖Write a function named calculateDogAge that:
  * [ ] Takes 1 argument: your puppy's age.
  * [ ] Calculates your dog's age based on the conversion rate of 1 human year to 7 dog years.
  * [ ] Outputs the result to the screen like so: "Your doggie is NN years old in dog years!"
  * [ ] Add an additional argument to the function that takes the conversion rate of human to dog years.

```js
// your code goes here

let age = prompt('enter the puppyAge',"");
let conversionRate = prompt ('enter the conversionRate');
function calculateDogAge(age, conversionRate){
  let dogAge = age * conversionRate ;
  alert(`Your doggie is ${dogAge} years old in dog years`);
}
calculateDogAge(age,conversionRate );

```

2. 🎖Write a function named calculateSupply that:
  * [ ] takes 2 arguments: age, amount per day.
  * [ ] calculates the amount consumed for rest of the life (based on a constant max age).
  * [ ] outputs the result to the screen like so: "You will need NN to last you until the ripe old age of X"
  * [ ] Accept floating point values for amount per day, and round the result to a round number.


  function 

```js
// your code goes here

function calculateSupply(age,amountPerDay){
let maxAge=80;
let restAge = maxAge - age;
let supply = restAge*365*amountPerDay;
alert(`You will need ${supply} kg to last you until the ripe old age of ${maxAge}`)
}
calculateSupply(15,2); // if present age is 15 year and consume 2 kg per day.   
```


3. 🎖Create a function called celsiusToFahrenheit:
  * [ ] Store a celsius temperature into a variable.
  * [ ] Convert it to fahrenheit and output "NN°C is NN°F".
  * [ ] Create a function called fahrenheitToCelsius:
  * [ ] Now store a fahrenheit temperature into a variable.
  * [ ] Convert it to celsius and output "NN°F is NN°C."

```js
// your code goes here

let temp= prompt('enter temperature in °C')
function celsiusToFahrenheit(temp) {
   let fTemp= (temp*9/5)+32;
   alert(`the temperature is ${fTemp} °F `);
}
celsiusToFahrenheit(temp);


let temp= prompt('enter temperature in °F')
function fahrenheitToCelsius(temp) {
   let cTemp= (temp-32)*5/9;
   alert(`the temperature is ${cTemp} °C `);
}
fahrenheitToCelsius(temp);


```
4. 🎖The function below returns true if the parameter age is greater than 18. Otherwise it asks for a confirmation and returns its result:

```js
function checkAge(age) {
  if (age > 18) {
    return true;
  } else {
    // ...
    return confirm("Did parents allow you?");
  }
}
```
  4.1 🎖Convert the above function using ternary operator.
  ```js
  // your code goes here
function checkAge(age) {
  return (age > 18) {
    return true;
  } else {
    // ...
    return confirm("Did parents allow you?");
  }
}


  ```

  4.2 🎖Convert the above function using `||` operator.
  ```js
  // your code goes here
  ```
Will the function work differently if else is removed like below?

```js
function checkAge(age) {
  if (age > 18) {
    return true;
  }
  // ...
  return confirm("Did parents allow you?");
}
```
Is there any difference in the behavior of these two variants? If there is what is that?


5. 🎖 Write a function pow(x,n) that returns x in power n.

  * [ ] Use prompt to take values for x and n, and then shows the result of pow(x,n) using alert.
  * [ ] In this task the function should support only natural values of n: integers greater then 1.

```js
// Your code goes here
function pow(x,n){
   if (n >= 1 && x >= 1) {
      return x**n;
   }
   else{
      alert("please the value of x & n greater than or equal to 1")
   }  
}
let result= pow(2,3);
alert(result);

// After writing code uncomment to check the answer.
// pow(3, 2); // 9
// pow(3, 3); // 27
// pow(1, 100); // 1
// pow(-31, 2); // "The number below 1 is not allowed"

6. 🎖Write a program that asks the user for a number n and gives them the possibility to choose between computing the sum and computing the product of 1,…,n. Return the result accordingly.

```js
// your code goes here

let n = prompt('enter the value', "");
let choice= prompt("enter your choice sum/product")
if (choice == "sum"){
   function sum(){
      let sum = 0;
      for (var i = 1; i <= n; i++) {   
         sum = sum + i;
      }
      return ("Sum = " + sum); 
   }
   let result= sum();
   alert(result);
} else{
   function product(){
      let product = 1;
      for (var i = 1; i <= n; i++) {   
         product = product * i;
      }
      return ("Product = " + product); 
   }
   let result= product();
   alert(result);
}

```
6. 🎖Write a program that asks the user for a number n using prompt and prints the sum of the numbers 1 to n

```js
// your code goes here

let n = prompt('enter the value', "");
function sum(){
  let sum = 0;
  for (var i = 1; i <= n; i++) {   
    sum = sum + i;
  }
    return ("Sum = " + sum); 
}

let result= sum();
  alert(result);


```
7. 🎖Modify the previous program such that only multiples of 5 or 7 are considered in the sum, e.g. n = 20 (5,7,10,14,15,20) 71

```js
// your code goes here

let n = prompt('enter the value', "");
function sum(){
  let sum = 0;
    for (let i = 1; i <= n; i++) {

    if (i % 5==0 || i%7==0) {
        sum = sum + i;
    }
    
  }
  return ("Sum = " + sum);
}
  let result= sum();
  alert(result);
```

8. 🎖Write a function `min` that takes two arguments and returns their minimum.

```js
// Your code here.


function min(x,y){
   if(x<y){
      console.log(x);
   } else{
      console.log(y)
   }
}
min (15,45);

console.log(min(0, 10));
// → 0
console.log(min(0, -10));
// → -10
```