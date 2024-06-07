# 10 ARRAY METHODS

1. **push**
   - **What it does:** *Adds a new toy to the end of the box.*

   - **Example:**

```javascript
         let toyBox = ['car', 'doll'];
     toyBox.push('ball');
     console.log(toyBox); // ['car', 'doll', 'ball']
```
**Explanation:** You had a car and a doll, then you added a ball at the end.

2. **pop**
   - **What it does:** *Takes the last toy out of the box.*
   - **Example:**

```javascript
         let toyBox = ['car', 'doll', 'ball'];
     let lastToy = toyBox.pop();
     console.log(lastToy); // 'ball'
     console.log(toyBox); // ['car', 'doll']
 ```    
**Explanation:** You took the ball out of the box, leaving the car and doll.

3. **unshift**
   - **What it does:** *Adds a new toy to the beginning of the box.*
   - **Example:**

```javascript
         let toyBox = ['car', 'doll'];
     toyBox.unshift('teddy bear');
     console.log(toyBox); // ['teddy bear', 'car', 'doll']
 ```    
**Explanation:** You put the teddy bear at the very start of the toys.

4. **shift**
   - **What it does:** *Takes the first toy out of the box.*
   - **Example:**

```javascript
         let toyBox = ['teddy bear', 'car', 'doll'];
     let firstToy = toyBox.shift();
     console.log(firstToy); // 'teddy bear'
     console.log(toyBox); // ['car', 'doll']
```     
**Explanation:** You took the teddy bear out, so now you have the car and doll left.

5. **length**
   - **What it does:** *Tells you how many toys are in the box.*
   - **Example:**

```javascript
         let toyBox = ['car', 'doll', 'ball'];
     console.log(toyBox.length); // 3
```    
**Explanation:** You counted the toys and found out there are three.

6. **forEach**
   - **What it does:** *Plays with each toy one by one.*
   - **Example:**

```javascript
         let toyBox = ['car', 'doll', 'ball'];
     toyBox.forEach(function(toy) {
       console.log('Playing with ' + toy);
     });
```    
**Explanation:** You played with the car, then the doll, and then the ball.

7. **map**
   - **What it does:** *Makes a new box with new toys by changing each toy in some way.*
   - **Example:**

```javascript
         let toyBox = ['car', 'doll', 'ball'];
     let bigToys = toyBox.map(function(toy) {
       return 'big ' + toy;
     });
     console.log(bigToys); // ['big car', 'big doll', 'big ball']
```     
**Explanation:** You made each toy bigger and put them in a new box.

8. **filter**
   - **What it does:** *Makes a new box with only some toys, based on a rule.*
   - **Example:**

```javascript
         let toyBox = ['car', 'doll', 'ball', 'truck'];
     let smallToys = toyBox.filter(function(toy) {
       return toy.length <= 4;
     });
     console.log(smallToys); // ['car', 'ball']
```    
**Explanation:** You kept only the small toys (car and ball) and made a new box for them.

9. **find**
   - **What it does:** *Finds the first toy that matches a rule.*
   - **Example:**

```javascript
         let toyBox = ['car', 'doll', 'ball', 'truck'];
     let foundToy = toyBox.find(function(toy) {
       return toy === 'doll';
     });
     console.log(foundToy); // 'doll'
```    
**Explanation:** You looked for the doll and found it.

10. **join**
    - **What it does:** *Makes a string by joining all the toys with a special string.*
    - **Example:**

```javascript
           let toyBox = ['car', 'doll', 'ball'];
      let toyString = toyBox.join(', ');
      console.log(toyString); // 'car, doll, ball'
```     
**Explanation:** You took all the toys and put them together with a comma and a space in between each toy, making a long string of toys.


# 10 STRING METHODS

1. **concat**
   - **What it does:** *Joins two or more strings together.*
   - **Example:**

```javascript
         let str1 = 'Hello';
     let str2 = 'World';
     let result = str1.concat(' ', str2);
     console.log(result); // 'Hello World'
```

**Explanation:** You took 'Hello' and 'World', and put them together to make 'Hello World'.

2. **slice**
   - **What it does:** *Cuts out a piece of the string and returns it.*
   - **Example:**

```javascript
         let str = 'JavaScript';
     let result = str.slice(0, 4);
     console.log(result); // 'Java'
```
**Explanation:** You cut out the first four letters of 'JavaScript' to get 'Java'.

3. **toUpperCase**
   - **What it does:** *Changes all letters in a string to uppercase.*
   - **Example:**

```javascript
         let str = 'hello';
     let result = str.toUpperCase();
     console.log(result); // 'HELLO'
```

**Explanation:** You made all the letters in 'hello' BIG to get 'HELLO'.

4. **toLowerCase**
   - **What it does:** *Changes all letters in a string to lowercase.*
   - **Example:**

```javascript
         let str = 'WORLD';
     let result = str.toLowerCase();
     console.log(result); // 'world'
```

**Explanation:** You made all the letters in 'WORLD' small to get 'world'.


5. **indexOf**
   - **What it does:** *Finds the position of a specific letter or word in a string.*
   - **Example:**

```javascript
         let str = 'Hello, World!';
     let position = str.indexOf('World');
     console.log(position); // 7
```

**Explanation:** You found where 'World' starts in 'Hello, World!', and it's at position 7.


6. **replace**
   - **What it does:** *Replaces a part of the string with another part.*
   - **Example:**

```javascript
         let str = 'I like apples';
     let newStr = str.replace('apples', 'bananas');
     console.log(newStr); // 'I like bananas'
```     
**Explanation:** You changed 'apples' to 'bananas' in 'I like apples' to get 'I like bananas'.

7. **charAt**
   - **What it does:** *Returns the character at a specified index in a string.*
   - **Example:**

```javascript
         let str = 'Hello';
     let char = str.charAt(1);
     console.log(char); // 'e'
```

**Explanation:** You looked at the second letter in 'Hello' and found 'e'.

8. **split**
   - **What it does:** *Splits a string into an array of substrings based on a specified separator.*
   - **Example:**

```javascript
         let str = 'apple,banana,kiwi';
     let fruits = str.split(',');
     console.log(fruits); // ['apple', 'banana', 'kiwi']
```

**Explanation:** You took the string 'apple,banana,kiwi' and split it at every comma to get an array of fruits: ['apple', 'banana', 'kiwi'].

9. **startsWith**
   - **What it does:** *Checks if a string starts with a specific substring.*
   - **Example:**

```javascript
         let str = 'Hello, World!';
     let startsWithHello = str.startsWith('Hello');
     console.log(startsWithHello); // true
```

**Explanation:** You checked if 'Hello, World!' starts with 'Hello', and it does, so the answer is true.

10. **endsWith**
    - **What it does:** *Checks if a string ends with a specific substring.*
    - **Example:**

```javascript
           let str = 'Hello, World!';
      let endsWithWorld = str.endsWith('World!');
      console.log(endsWithWorld); // true
```

**Explanation:** You checked if 'Hello, World!' ends with 'World!', and it does, so the answer is true.

# 10 NUMBER METHODS

1. **parseInt()**
   - **What it does:** *Turns a string into a whole number.*
   - **Example:**

```javascript
         let number = parseInt("123");
     console.log(number); // 123
```
**Explanation:** Imagine you have the word "123" and you want it to be the number 123. parseInt helps you do that!


2. **parseFloat()**
   - **What it does:** *Turns a string into a number, including decimals.*
   - **Example:**

```javascript
         let number = parseFloat("123.45");
     console.log(number); // 123.45
```

**Explanation:** If you have "123.45" and you want it to be a number with the pointy part (decimal), parseFloat helps you with that.


3. **toFixed()**
   - **What it does:** *Rounds a number to a certain number of decimals and makes it a string.*
   - **Example:**

```javascript
         let number = 123.456;
     let roundedNumber = number.toFixed(2);
     console.log(roundedNumber); // "123.46"
```

**Explanation:** When you want to tell your friends that 123.456 is almost 123.46, toFixed(2) makes it look nice and round with 2 decimal places.

4. **Math.round()**
   - **What it does:** *Rounds a number to the nearest whole number.*
   - **Example:**
```javascript
         let number = Math.round(4.6);
     console.log(number); // 5
```

**Explanation:** If you have 4.6 and you want to make it a whole number, Math.round will say, "Hmm... that's closer to 5!"

5. **Math.ceil()**
   - **What it does:** *Rounds a number up to the next whole number.*
   - **Example:**

```javascript
         let number = Math.ceil(4.2);
     console.log(number); // 5
```
**Explanation:** If you have 4.2 and you want to always go up, Math.ceil will take you to 5.

6. **Math.floor()**
   - **What it does:** *Rounds a number down to the previous whole number.*
   - **Example:**

```javascript
         let number = Math.floor(4.8);
     console.log(number); // 4
```

**Explanation:** If you have 4.8 and you always want to go down, Math.floor will take you to 4.

7. **Math.max()**
   - **What it does:** *Finds the biggest number in a list of numbers.*
   - **Example:**

```javascript
         let maxNumber = Math.max(1, 3, 2);
     console.log(maxNumber); // 3
```

**Explanation:** Imagine you have 1, 3, and 2 and you want to know which one is the biggest. Math.max will tell you it's 3.

8. **Math.min()**
   - **What it does:** *Finds the smallest number in a list of numbers.*
   - **Example:**

```javascript
         let minNumber = Math.min(1, 3, 2);
     console.log(minNumber); // 1
```

**Explanation:** If you have 1, 3, and 2 and you want to know the smallest, Math.min will say it's 1.

9. **Math.random()**
   - **What it does:** *Gives you a random number between 0 and 1.*
   - **Example:**

```javascript
         let randomNumber = Math.random();
     console.log(randomNumber); // Could be 0.12345 or 0.6789 or any number between 0 and 1
```

**Explanation:** Think of it like a magic box that gives you different surprise numbers every time you open it!

10. **Number.isNaN()**
    - **What it does:** *Checks if a value is "Not a Number."*
    - **Example:**

```javascript
           let result = Number.isNaN(NaN);
      console.log(result); // true
      let result2 = Number.isNaN(123);
      console.log(result2); // false
```
          
**Explanation:** If you have something and you wonder, "Is this really a number?" Number.isNaN helps you check. If it's not a number, it will say "true."