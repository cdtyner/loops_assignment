# Loop Exercises

1. Write a `while` loop and a `for` loop that takes the variable "num" and logs all the numbers, descending, between "num" and 1.

```js

let num = 15
while(num >= 1){
  console.log(num)
  num--
}


for(num = 7; num >= 1; num--){
  console.log(num)
}

```
2. Write a `while` loop and a `for` loop that takes the variable "num", and iterates over all numbers from 0 to "num".
For each iteration, it will check if the current number is even or odd, and log that to the screen (e.g. "2 is even")

```js

let num = 0
while(num <= 10) {
if(num % 2 === 0){
  console.log(num + " is even." )
}else{
  console.log(num + " is odd.")
}
num++
}

for(num = 0; num <= 20; num++) {
  if(num % 2 === 0) {
    console.log(num + " is even.")
  }else{
    console.log(num + " is odd.")
 }
}


```



3. Write a `while` loop and a `for` loop that takes the variable "num" and iterates over all numbers from 0 to "num".
For each iteration of the loop, it will multiply the number by 9 and log the result (e.g. "2 * 9 = 18").

```js

let num = 0
while(num <= 5) {
 console.log(num * 9)
 num++
}


for(let num = 0; num <= 5; num++) {
  console.log(num * 9)
}

```
_Bonus_ think of another way to solve it.
  <details>
    <summary>
      Hint
    </summary>
    Find the final number and increment the loop by 9.
  </details>

  ```js


  ```

4. Write a loop that uses console.log to log all the numbers from 1 to 100, with two exceptions. For numbers divisible by 3, log "Fizz" instead of the number, and for numbers divisible by 5 (and not 3), log "Buzz" instead.

```js

for(let soda = 1; soda < 101; soda++) {
  if(soda % 3 === 0){
    console.log("Fizz");
  }else if(soda % 5 === 0){
    console.log("Buzz");
  }else{
    console.log(soda);
  }
}

```

5. Modify your program to log "FizzBuzz", for numbers that are divisible by both 3 and 5 (still log "Fizz" or "Buzz" for numbers divisible by only one of those).

```js

for(let soda = 0; soda < 101; soda++){
  if(soda % 5 === 0 && soda % 3 === 0){
    console.log("Fizzbuzz");
  }else if(soda % 3 === 0){
    console.log("Fizz")
  }else if(soda % 5 === 0){
    console.log("Buzz")
  }else{
    console.log(soda)
  }
}

```

Bonus:

1. Write a program that would log the lyrics of the song 99 Bottles of Beer. This is the first verse of the song:

99 bottles of beer on the wall,

99 bottles of beer.

Take one down, pass it around,

98 bottles of beer on the wall.

This verse is repeated, each time with one less bottle, until the number of bottles is 0. When the number of bottles is 2, the verse is:

2 bottles of beer on the wall,

2 bottles of beer.

Take one down, pass it around,

1 bottle of beer on the wall.

In the last line, the word bottles (plural), is  replaced with bottle (singular)

When the number of bottles is 1, the verse is:

```js


for(let i = 100; i >= 1; i--){
  if(i > 2) {
  console.log(i + " bottles of beer on the wall, " + i + " bottles of beer. Take one down, pass it around, " + (i - 1) + " bottles of beer on the wall.")
  }else if(i < 3 &&  i > 1){
  console.log(i + " bottles of beer on the wall, " + i + " bottles of beer. Take one down, pass it around, " + (i - 1) + " bottle of beer on the wall.")
  }else if(i < 2){
  console.log(i + " bottle of beer on the wall, " + i + " bottle of beer. Take one down, pass it around, no more bottles of beer on the wall.")
  }else{
    console.log(i)
  }
  }

```



2. Use the assignGrade function (given below). Write a function that logs each number from 60 - 100 along with its corresponding letter score.
Exp For each number from 81 to 90, log B, like so:

```js
81 - B
82 - B
83 - B
...
```

```js
function assignGrade(score) {
    if (score > 90) {
        return 'A';
    } else if (score > 80) {
        return 'B';
    } else if (score > 70) {
        return 'C';
    } else if (score > 65) {
        return 'D';
    } else {
        return 'F';
    };
};
```
