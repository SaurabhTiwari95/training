# Training
##  JavaScript Tutorial Udemy

```
//booleans with true or false statements
var initreal= true;
var initfun = false;
var initSpicy = "true"
```
```
//booleans with if statements
var areYouAwake = true
if (areYouAwake ==true){
console.log("Glad you are awake")
}

var areYouAwake=false

if(areYouAwake == false){
console.log("Wake Up")
}

var areYouAwake=false

if(areYouAwake!=true){
console.log("Wake Up")
}
```
## Lecture 39
 // Activity Truth and Dare
 ```
  var answer = prompt("Do you like cheese Type Y or N")
var isItTrue

if (answer == "Y") {
    isItTrue = true
    console.log("Answer is " + isItTrue)
} else if (answer == "N") {
    isItTrue = false
    console.log("Answer is " + isItTrue)
} else {
    console.log("I don't understand")
 }
 ```

 ## Lecture 40
 // Values of an array
 ```
 var container =[]
 var first ="test"
 var second ="test2"
 var third ="test3"
  var people =["test","test1","test2"]
  
  // arrays are the index starting with 0
  var stuff = [1,2,3,"test",true]
 ```
  
### POP and PUSH
 var container = ["red","blue","yellow","green"]
### Syntax
container.pop()= pops the elements from the given array
container.push("element")= pushes the elements in the array

## Lecture 42
## Shift and Unshift
var container = ["red","blue","yellow","green"]
### Syntax
container.shift()
container.unshift("element")

### Difference between POP/PUSH & SHIFT/UNSHIFT
 POP & PUSH manipulates the **last element** of the array while the 
 SHIFT & UNSHIFT manipulates the **first element** of the array
 
### Lectuer 42 Changing the Specific elements of the Array
 It can be used to change the values of the specific elements and also to add new elements in the array.
var container = ["red","blue","yellow","green"]
container[0]
container[0]="white"
### SPLICE & SLICE
 var container = ["red","blue","yellow","green"]
 container.splice(0,0,"black")
### Syntax
array.splice(index, howmany, item1, ....., itemX)

```
 container.splice(0,0,"black") 
//adds black in the front of the array
container.splice(0,1)
//remove the first element
container.splice(0,1,"black")
//remove the first element and insert black

```
 var container = ["red","blue","yellow","green"]
 var newContainer = container.slice(3)
#### Lecture 45 Activity

 ```
 var things = []
 var answer
answer = prompt("What is your first favourite thing ??")
things.push(answer)

answer = prompt("What is your second favourite thing ??")
things.push(answer)

answer = prompt("What is your third favourite thing ??")
things.push(answer)

console.log(things)

 ```
### Assignment 4
```
 var questions = []
var book
book = prompt("What is your favourite book0 ??")
questions.push(book) 

book = prompt("What is your favourite book1 ??")
questions.push(book) 

book = prompt("What is your favourite book2 ??")
questions.push(book) 

book = prompt("What is your favourite book3 ??")
questions.push(book) 

book = prompt("What is your favourite book4 ??")
questions.push(book) 

book = prompt("What is your favourite book5 ??")
questions.unshift(book)/* unshift prints the last element in the beginning*/
questions.pop()/*removes the last element of the array*/
console.log(questions)/*prints the*/
```

#### OUTPUT
```
Array (5) [ test6,test1,test2,test3,test4 ] 

```
###  Lecture 46 For Loops
 ```
 // for Loop
 // for(starting place;condition;incrementer)
 for(var i=1;i<10;i++){
   console.log(i)
 } 
for (var i=1;i<5;i++){
 console.log("Hello" +i)
}
 ```

### Lecture 47 Infinite Loop
 ```
 for(var i=1;ii<10;i--){
  console.log(i)
 }

 ```
### Lecture 48 For Loop with an If Condition
```
 for (var i = 1; i < 5; i++) {
    if (i == 1) {
        console.log("Hello")
    } else if (i == 2) {
        console.log("Bye")
    } else if (i == 3) {
        console.log("Hello Again!!")
    } else if(i == 4) {
        console.log("Bye byeeeeeeeeee")
    }
}
````
#### OUTPUT
```
Hello
Bye
Hello Again!!
Bye byeeeeeeeeee
```
### Lecture 49 Breaking the For Loop
```
for(var i=1;i<10;i++)
// console.log(i)
if(i==5){
 break
}else
{
 console.log(i)
}
```
### Lecture 50 - For loop With an Array 
```
 var things = [1,2,"hello","bye"]
 for(var i=1;i<5;i++)
 {
  console.log(things[i])
  }
```
#### OUTPUT
```
2
hello
bye
```
### Lecture 51 Activity

```
var answer = prompt("Type Yes or NO")
        var answers = ["YES", "NO"]
        var responses = ["You said YES", " You said NO", "You did not follow instructions"]
        for (var i = 0; i < 2; i++) {
            if((answer != answers[0])&&(answer != answers[1]))
            {
                console.log(responses[2])
                break;
            } else if (answer == answers[i]) {
                console.log(responses[i])
            }
        }    

```
### Lecture 52 For Loop in a For Loop
```
//This is called a Nested For Loop
       var numbers = [1, 2, 3, 4, 5]
            var letters = ["a", "b", "c"]
            for (var i = 0; i < 5; i++) {
                console.log(numbers[i])
                for (var j = 0; j < 3; j++) {
                    console.log(letters[j])
                }
            }
```            
### OUTPUT
```
1
a
b
c
2
a
b
c
3
a
b
c
4
a
b
c
5
a
b
c
```

### Lecture 53 Activity Square

```
var square = ""
        for (var i = 0; i < 5; i++) {
            for (var j = 0; j < 5; j++) {
                square = square + "*"
            }
            square = square + "\n"
        }
        console.log(square)
```
### OUTPUT
```
*****
*****
*****
*****
*****
``` 
 ```
 var square = ""
        for (var i = 0; i < 5; i++) {
            for (var j = 0; j < 5; j++) {
                square = square + "ival =" + i+" "+ "ival =" +j
            }
            square = square + "*" + "\n"
        }
        console.log(square)
```
 ### Lecture 54 While Loop
 ```
 var i = 0;
while (i < 5){
console.log(i)
 i++
}
 ```
### DoWhile Loop
```
var i=0
do{
 console.log(i)
 i++
}while(i < 5)

```
 ### Lecture 56 For Vs While Vs Do While loop
```
 
 for(var i=0;i<5;i++){
  console.log(i)
 }


var i=0
while(i < 5){
 console.log(i)
 i++
}

var i=0
do{
 console.log(i)
 i++
}while(i < 5)

```
### Lecture 57 Switch Statements
```
var favfood = "Pasta!!"
  if(favfood=="pizza"){
   console.log("Pizza!!")
  }
if(favfood=="pasta"){
   console.log("Pasta!!")
  }
else{
   console.log("favfood!!")
  }
```
 ```
 var favfood = "pasta"
            switch (favfood) {
                case "pizza":
                    console.log("Pizza!")
                    break
                case "pasta":
                    console.log("Pasta!!")
                    break
                default:
                    console.log(favfood);
            }

 ```
 #### Assignment 
 ```
 var favColor = "red"
    switch (favColor) {
        case "blue":
            console.log("Violets are blue !!")
            break
        case "red":
            console.log("Roses are red !!")
            break
        default:
            console.log("Sugar is sweet !!")
    }
 ```
## Section 14
#### Lecture 58 & 59 Functions basics 
 ```
 const message = function () {
        console.log("Hello Function")
    }
    message() 
 ```
 ```
    function message() {
        console.log("Bye Function")
    }
    message()
```
```
    function newMessage() {
        console.log(1)
        console.log(2)
        console.log(3)
    }
    newMessage()
    newMessage()
```
 ** function can return data which means when we excute the function the function 
    gives us the value which then,can be used for something else**
```     
        function getMessage() {
        return "Hello Test"
    }
    //getMessage()
    console.log(getMessage())
```
```
function getNumber() {
        return 1
    }
    console.log(getNumber())
```
### Lecture 60 Activity Passing the Buck
```
    function getCost() {
        //cost of Oranges
        return 5
    }
    console.log(" Five Oranges Cost about $" + getCost())
```
```
function getNumber(){
    return 5
}
console.log(getNumber() + 5)
```
```
function getSomething(){
    return getNumber()+5
}
console.log(getSomething())
```
```
function getNumber() {
        return 5
    }
    function getSomething() {
        return getNumber() + 5
    }
    console.log(getSomething())
```
### Lecture 61 Parameter and Arguments
 **Parameters** are the placeholders inside the function declaration.
 **Arguments** are the actual values which we pass into the function.
```
     function message11(message1, message2) {
        console.log(message1)
        console.log(message2)
    }
    message11("message1","message2")
```
 ### Lecture 62 Activity Area of a rectangle
```
 function rectangle(width,height) {
     var area = width * height
     return area
 }
 rectangle(5,10)
```
 ##### OUTPUT 
 ```
 50 
```
### Lecture 63 Constants
 **constants** means that,once it's set it can not be changed.
  ```
  const something = "test"
  something
  ```
##### OUTPUT
```
test
 ```
 **for arrrays constants we can change some of the elements of the array but not the whole array**
 ### Lecture 64 Variable Scopes
 ```
    var num = 1
    function thing() {
        num = 2
        console.log("function:" + num)
    }
    thing()
    console.log("OutSide function:" + num)
```
##### OUTPUT
```
function:2
OutSide function:2
```
```
var num = 1
    function thing() {
        num = 2
        var num2 = 2
        console.log("function:" + num2)
    }
    thing()
    console.log("OutSide function:" + num2)
// num2 is declared locally so it can not be called outside of the
// function,if called it will show an error(undefined)
```
##### OUTPUT
```
function:2
Reference Error { "num2 is not defined" }
```
```
//let num = 1
    function thing() {
        num = 2
        var num2 = 2
        console.log("function:" + num2)
    }
    thing()
    console.log("OutSide function:" + num2)
```
##### OUTPUT
```
function:2
Reference Error { "num2 is not defined" }
```
**var and let are both used for variable declaration in javascript but the 
 difference between them is that var is ***function scoped*** and let is ***block scoped***. 
 **It can be said that a variable declared with var is defined throughout the program 
 as compared to let.**
```
   //let num = 1
    if (1 == 1) {
        var num = 1
        console.log(" Inside If Statement: " + num)  
    }
    console.log("outside IF Statement:" + num)
```
##### OUTPUT
```
Inside If Statement: 1
outside IF Statement:1
```
```
if (1 == 1) {
        let num = 1
        console.log(" Inside If Statement: " + num)  
    }
    console.log("outside IF Statement:" + num)
```
##### OUTPUT
```
Inside If Statement: 1
Reference Error { "num is not defined" }
```
### Lecture 65 Assignment
```
        var amount = prompt("Enter the amount")
        var price = prompt("Enter the price")
        if (amount > price) {
            var change = amount - price
            console.log("You change due is $" + change)
        } else if (amount < price)
            {
                var change = price - amount
                console.log("You still owe $" + change)
            } else {
            console.log("You gave the exact amount")
        }
```
### Lecture 65 Object Basics
```
let person={
    firstName : "Test",
    faceColor: "Blue",
    favNumber: "6",
    isMarried: true,
    children: ["child1","child2"],
    thing:{
        name:"Object",
        color:"Yellow"
    }
}
```
##### OUTPUT
```
person
  { children:(2),faceColor:Blue,favNumber:6,firstName:Test,isMarried:true,… }
console.log(person.firstName)
  Test

console.log(person.children)
  (2)[ child1,child2 ]

console.log(person.children[1])
  child2

console.log(person.children[0])
  child1

person.thing.name
  Object
person.thing.color
  Yellow

```
##### OUTPUT
```
console.log(person["firstName"])
Test

console.log(person["children"][0])
child1

console.log(person["thing"])
{ color:Yellow,name:Object }
```
### Lecture 66 Activity Family Tree
```
var family = {
    father:{
        firstName:"FFather",
        lastName:"LFather",
        isAlive: false
    },
    mother:{
        firstName:"FMother",
        lastName:"LMother",
        isAlive: false
    },
    children:[{
        firstName:"FChildren",
        lastName:"LChildren",
        isAlive: true
    }],
    butler:{
        firstName:"FButler",
        lastName:"LButler",
        isAlive: true
    },
    isRich: true
}

```
##### OUTPUT
```
console.log(family.isRich)
true

console.log(family.mother.firstName)
FMother

console.log(family.children)
{ firstName:FChildren,isAlive:true,lastname:LChildren 

console.log(family.children[0].lastname)
LChildren

```
### Lecture 67 Methods
```
    var library={
    book:"JavaScript is fun",
    checkout:function(){
     console.log("You have checked out the box")
     }
    }

```
##### OUTPUT
```
library.checkout()
You have checked out the box

```
```
var library={
    book:"JavaScript is fun",
    checkout:function(){
        //console.log("You have checked out the book" + library.book)
        console.log("You have checked out the book" + this.book)
    },
    checkIn: function(number){
        console.log("You have checkedIN" + number + "books")
    }
}

```
**"this" refers to the owner of the object, here library is the owner of the object**

##### OUTPUT
```
library.checkout()
You have checked out the bookJavaScript is fun

library.checkIn(5)
You have checkedIN5books
```
### Lecture 68 Assigning New Values
```
let person={
    firstName : "Test",
    faceColor: "Blue",
    favNumber: "6",
    isMarried: true,
    children: ["child1","child2"],
    thing:{
        name:"Object",
        color:"Yellow"
    }
}
// Assign new Value to the firstName of the array element

person.firstName = "Bob"

person.children[0]="Kid1"
```
##### OUTPUT
```
Object {
children:Array(2)
faceColor:Blue
favNumber:6
firstName:Bob
isMarried:true
thing:Object
}

```
```
Object {
children:(2)[
Kid1
child2
]
faceColor:Blue
favNumber:6
firstName:Bob
isMarried:true
thing:Object
}

```
### Lecture 69 Assignment: Restaurant Menu
```
Assignment is to build a simple object that contains multiple properties and functions.
Here are the things that should be included:

1. An object named "restaurantMenu"
2. Properties that contains
    a. The name of the restaurant
    b. The items that the restaurant sells which includes the names and prices. Price can just be a number. Limit this to 5 items.
    c. A method that lists out all the menu items with their prices via an alert.
    d. A method that allows the user to select which menu item that the user wants to order via a prompt. 
       Simply alert the menu item back to the user.

```
##### [Bind() Method](https://www.codingame.com/playgrounds/9799/learn-solve-call-apply-and-bind-methods-in-javascript)

```

```

### Section 16
#### Lecture 69 [JSON Data](https://jsonlint.com/)

   **JSON : JavaScript Object Notation
           - it is a file format for what people use for data,
           - multiple languages use this file format**
           - **JSON can be used as the data stored in a variable**

```
{
    firstName : "Test" // This is an OBJECT
    "firstName" : "Test" // This is a JSON
} 

```
- Key need to be wrapped in the double quotes
- No function is allowed as values in the JSON
 
 #### Lecture 70 JSON Path
 ```
 // Pretty Print or Pretty JSON
 
 var school = {
        "name": "Learning U",
        "classes": [
            {
                "title": "Test is fun",
                "teacher": "Test1",
                "courseId": "A122",
                "credits": 2
            },
            {
                "title": "test2 is good",
                "teacher": "Test2",
                "courseId": "B123",
                "credits": "4"
            },
            {
                "title": "Test3 is great",
                "teacher": "Test3",
                "courseId": "C123",
                "credits": "5"
            }
        ]
    }
 
 ```
##### OUTPUT
```
school.name
Learning U

school.classes
Array (3)[
{
courseId:A122
credits:2
teacher:Test1
title:Test is fun
}
{
courseId:B123
credits:4
teacher:Test2
title:test2 is good
}
{
courseId:C123
credits:5
teacher:Test3
title:Test3 is great
}
]
```
```
// Minified Json(It comes in one line)

{"name":"Learning U","classes":[{"title":"Test is fun","teacher":"Test1","courseId":"A122","credits":2},{"title":"test2 is good","teacher":"Test2","courseId":"B123","credits":"4"},{"title":"Test3 is great","teacher":"Test3","courseId":"C123","credits":"5"}]}

```
##### OUTPUT

```
Object{
        classes: Array(3)[
            Object {
            courseId: A122
            credits: 2
            teacher: Test1
            title: Test is fun
        }
        Object {
            courseId: B123
            credits: 4
            teacher: Test2
            title: test2 is good
        }
        Object {
            courseId: C123
            credits: 5
            teacher: Test3
            title: Test3 is great
        }
            ]
        name: "Learning U"
    }
    
```
### Lecture 71 [Minified](https://codebeautify.org/jsonminifier) VS Pretty JSON
### Assignment 
```
Your assignment is to take a large piece of JSON data and find different values for that data.
Use the https://pokeapi.co/ website.
You will see a "Try it now" section. Inside the text field it should have "pokemon/ditto/".
If you don't see data below the label "Resource for ditto", you will need to click the blue "submit" button.
At the bottom of the section where the data is presented there is a small checkbox labeled "View raw JSON". Check it.
Now take the data and paste it into your editor. Assign a variable name for it.
I recommend that you minify this before you put it into the console.
Now using the data that you have I want you to find the following values.

All the abilities
The base experience
The height
The url for the item "metal-powder"
All the sprites
The different stat names
The slot for the types
The weight
The first version_group_details

```
```
var pokemon =
 { "abilities": [{ "ability": { "name": "imposter", "url": "https://pokeapi.co/api/v2/ability/150/" }, "is_hidden": true, "slot": 3 }, { "ability": { "name": "limber", "url": "https://pokeapi.co/api/v2/ability/7/" }, "is_hidden": false, "slot": 1 }], "base_experience": 101, "forms": [{ "name": "ditto", "url": "https://pokeapi.co/api/v2/pokemon-form/132/" }], "game_indices": [{ "game_index": 132, "version": { "name": "white-2", "url": "https://pokeapi.co/api/v2/version/22/" } }, { "game_index": 132, "version": { "name": "black-2", "url": "https://pokeapi.co/api/v2/version/21/" } }, { "game_index": 132, "version": { "name": "white", "url": "https://pokeapi.co/api/v2/version/18/" } }, { "game_index": 132, "version": { "name": "black", "url": "https://pokeapi.co/api/v2/version/17/" } }, { "game_index": 132, "version": { "name": "soulsilver", "url": "https://pokeapi.co/api/v2/version/16/" } }, { "game_index": 132, "version": { "name": "heartgold", "url": "https://pokeapi.co/api/v2/version/15/" } }, { "game_index": 132, "version": { "name": "platinum", "url": "https://pokeapi.co/api/v2/version/14/" } }, { "game_index": 132, "version": { "name": "pearl", "url": "https://pokeapi.co/api/v2/version/13/" } }, { "game_index": 132, "version": { "name": "diamond", "url": "https://pokeapi.co/api/v2/version/12/" } }, { "game_index": 132, "version": { "name": "leafgreen", "url": "https://pokeapi.co/api/v2/version/11/" } }, { "game_index": 132, "version": { "name": "firered", "url": "https://pokeapi.co/api/v2/version/10/" } }, { "game_index": 132, "version": { "name": "emerald", "url": "https://pokeapi.co/api/v2/version/9/" } }, { "game_index": 132, "version": { "name": "sapphire", "url": "https://pokeapi.co/api/v2/version/8/" } }, { "game_index": 132, "version": { "name": "ruby", "url": "https://pokeapi.co/api/v2/version/7/" } }, { "game_index": 132, "version": { "name": "crystal", "url": "https://pokeapi.co/api/v2/version/6/" } }, { "game_index": 132, "version": { "name": "silver", "url": "https://pokeapi.co/api/v2/version/5/" } }, { "game_index": 132, "version": { "name": "gold", "url": "https://pokeapi.co/api/v2/version/4/" } }, { "game_index": 76, "version": { "name": "yellow", "url": "https://pokeapi.co/api/v2/version/3/" } }, { "game_index": 76, "version": { "name": "blue", "url": "https://pokeapi.co/api/v2/version/2/" } }, { "game_index": 76, "version": { "name": "red", "url": "https://pokeapi.co/api/v2/version/1/" } }], "height": 3, "held_items": [{ "item": { "name": "metal-powder", "url": "https://pokeapi.co/api/v2/item/234/" }, "version_details": [{ "rarity": 5, "version": { "name": "ultra-sun", "url": "https://pokeapi.co/api/v2/version/29/" } }, { "rarity": 5, "version": { "name": "moon", "url": "https://pokeapi.co/api/v2/version/28/" } }, { "rarity": 5, "version": { "name": "y", "url": "https://pokeapi.co/api/v2/version/24/" } }, { "rarity": 5, "version": { "name": "x", "url": "https://pokeapi.co/api/v2/version/23/" } }, { "rarity": 5, "version": { "name": "white-2", "url": "https://pokeapi.co/api/v2/version/22/" } }, { "rarity": 5, "version": { "name": "black-2", "url": "https://pokeapi.co/api/v2/version/21/" } }, { "rarity": 5, "version": { "name": "white", "url": "https://pokeapi.co/api/v2/version/18/" } }, { "rarity": 5, "version": { "name": "black", "url": "https://pokeapi.co/api/v2/version/17/" } }, { "rarity": 5, "version": { "name": "soulsilver", "url": "https://pokeapi.co/api/v2/version/16/" } }, { "rarity": 5, "version": { "name": "heartgold", "url": "https://pokeapi.co/api/v2/version/15/" } }, { "rarity": 5, "version": { "name": "platinum", "url": "https://pokeapi.co/api/v2/version/14/" } }, { "rarity": 5, "version": { "name": "pearl", "url": "https://pokeapi.co/api/v2/version/13/" } }, { "rarity": 5, "version": { "name": "diamond", "url": "https://pokeapi.co/api/v2/version/12/" } }, { "rarity": 5, "version": { "name": "leafgreen", "url": "https://pokeapi.co/api/v2/version/11/" } }, { "rarity": 5, "version": { "name": "firered", "url": "https://pokeapi.co/api/v2/version/10/" } }, { "rarity": 5, "version": { "name": "emerald", "url": "https://pokeapi.co/api/v2/version/9/" } }, { "rarity": 5, "version": { "name": "sapphire", "url": "https://pokeapi.co/api/v2/version/8/" } }, { "rarity": 5, "version": { "name": "ruby", "url": "https://pokeapi.co/api/v2/version/7/" } }] }, { "item": { "name": "quick-powder", "url": "https://pokeapi.co/api/v2/item/251/" }, "version_details": [{ "rarity": 50, "version": { "name": "ultra-sun", "url": "https://pokeapi.co/api/v2/version/29/" } }, { "rarity": 50, "version": { "name": "moon", "url": "https://pokeapi.co/api/v2/version/28/" } }, { "rarity": 50, "version": { "name": "y", "url": "https://pokeapi.co/api/v2/version/24/" } }, { "rarity": 50, "version": { "name": "x", "url": "https://pokeapi.co/api/v2/version/23/" } }, { "rarity": 50, "version": { "name": "white-2", "url": "https://pokeapi.co/api/v2/version/22/" } }, { "rarity": 50, "version": { "name": "black-2", "url": "https://pokeapi.co/api/v2/version/21/" } }, { "rarity": 50, "version": { "name": "white", "url": "https://pokeapi.co/api/v2/version/18/" } }, { "rarity": 50, "version": { "name": "black", "url": "https://pokeapi.co/api/v2/version/17/" } }, { "rarity": 50, "version": { "name": "soulsilver", "url": "https://pokeapi.co/api/v2/version/16/" } }, { "rarity": 50, "version": { "name": "heartgold", "url": "https://pokeapi.co/api/v2/version/15/" } }, { "rarity": 50, "version": { "name": "platinum", "url": "https://pokeapi.co/api/v2/version/14/" } }, { "rarity": 50, "version": { "name": "pearl", "url": "https://pokeapi.co/api/v2/version/13/" } }, { "rarity": 50, "version": { "name": "diamond", "url": "https://pokeapi.co/api/v2/version/12/" } }] }], "id": 132, "is_default": true, "location_area_encounters": "https://pokeapi.co/api/v2/pokemon/132/encounters", "moves": [{ "move": { "name": "transform", "url": "https://pokeapi.co/api/v2/move/144/" }, "version_group_details": [{ "level_learned_at": 1, "move_learn_method": { "name": "level-up", "url": "https://pokeapi.co/api/v2/move-learn-method/1/" }, "version_group": { "name": "ultra-sun-ultra-moon", "url": "https://pokeapi.co/api/v2/version-group/18/" } }, { "level_learned_at": 1, "move_learn_method": { "name": "level-up", "url": "https://pokeapi.co/api/v2/move-learn-method/1/" }, "version_group": { "name": "sun-moon", "url": "https://pokeapi.co/api/v2/version-group/17/" } }, { "level_learned_at": 1, "move_learn_method": { "name": "level-up", "url": "https://pokeapi.co/api/v2/move-learn-method/1/" }, "version_group": { "name": "omega-ruby-alpha-sapphire", "url": "https://pokeapi.co/api/v2/version-group/16/" } }, { "level_learned_at": 1, "move_learn_method": { "name": "level-up", "url": "https://pokeapi.co/api/v2/move-learn-method/1/" }, "version_group": { "name": "x-y", "url": "https://pokeapi.co/api/v2/version-group/15/" } }, { "level_learned_at": 1, "move_learn_method": { "name": "level-up", "url": "https://pokeapi.co/api/v2/move-learn-method/1/" }, "version_group": { "name": "black-2-white-2", "url": "https://pokeapi.co/api/v2/version-group/14/" } }, { "level_learned_at": 1, "move_learn_method": { "name": "level-up", "url": "https://pokeapi.co/api/v2/move-learn-method/1/" }, "version_group": { "name": "xd", "url": "https://pokeapi.co/api/v2/version-group/13/" } }, { "level_learned_at": 1, "move_learn_method": { "name": "level-up", "url": "https://pokeapi.co/api/v2/move-learn-method/1/" }, "version_group": { "name": "colosseum", "url": "https://pokeapi.co/api/v2/version-group/12/" } }, { "level_learned_at": 1, "move_learn_method": { "name": "level-up", "url": "https://pokeapi.co/api/v2/move-learn-method/1/" }, "version_group": { "name": "black-white", "url": "https://pokeapi.co/api/v2/version-group/11/" } }, { "level_learned_at": 1, "move_learn_method": { "name": "level-up", "url": "https://pokeapi.co/api/v2/move-learn-method/1/" }, "version_group": { "name": "heartgold-soulsilver", "url": "https://pokeapi.co/api/v2/version-group/10/" } }, { "level_learned_at": 1, "move_learn_method": { "name": "level-up", "url": "https://pokeapi.co/api/v2/move-learn-method/1/" }, "version_group": { "name": "platinum", "url": "https://pokeapi.co/api/v2/version-group/9/" } }, { "level_learned_at": 1, "move_learn_method": { "name": "level-up", "url": "https://pokeapi.co/api/v2/move-learn-method/1/" }, "version_group": { "name": "diamond-pearl", "url": "https://pokeapi.co/api/v2/version-group/8/" } }, { "level_learned_at": 1, "move_learn_method": { "name": "level-up", "url": "https://pokeapi.co/api/v2/move-learn-method/1/" }, "version_group": { "name": "firered-leafgreen", "url": "https://pokeapi.co/api/v2/version-group/7/" } }, { "level_learned_at": 1, "move_learn_method": { "name": "level-up", "url": "https://pokeapi.co/api/v2/move-learn-method/1/" }, "version_group": { "name": "emerald", "url": "https://pokeapi.co/api/v2/version-group/6/" } }, { "level_learned_at": 1, "move_learn_method": { "name": "level-up", "url": "https://pokeapi.co/api/v2/move-learn-method/1/" }, "version_group": { "name": "ruby-sapphire", "url": "https://pokeapi.co/api/v2/version-group/5/" } }, { "level_learned_at": 1, "move_learn_method": { "name": "level-up", "url": "https://pokeapi.co/api/v2/move-learn-method/1/" }, "version_group": { "name": "crystal", "url": "https://pokeapi.co/api/v2/version-group/4/" } }, { "level_learned_at": 1, "move_learn_method": { "name": "level-up", "url": "https://pokeapi.co/api/v2/move-learn-method/1/" }, "version_group": { "name": "gold-silver", "url": "https://pokeapi.co/api/v2/version-group/3/" } }, { "level_learned_at": 1, "move_learn_method": { "name": "level-up", "url": "https://pokeapi.co/api/v2/move-learn-method/1/" }, "version_group": { "name": "yellow", "url": "https://pokeapi.co/api/v2/version-group/2/" } }, { "level_learned_at": 1, "move_learn_method": { "name": "level-up", "url": "https://pokeapi.co/api/v2/move-learn-method/1/" }, "version_group": { "name": "red-blue", "url": "https://pokeapi.co/api/v2/version-group/1/" } }] }], "name": "ditto", "order": 197, "species": { "name": "ditto", "url": "https://pokeapi.co/api/v2/pokemon-species/132/" }, "sprites": { "back_default": "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/back/132.png", "back_female": null, "back_shiny": "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/back/shiny/132.png", "back_shiny_female": null, "front_default": "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/132.png", "front_female": null, "front_shiny": "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/shiny/132.png", "front_shiny_female": null }, "stats": [{ "base_stat": 48, "effort": 0, "stat": { "name": "speed", "url": "https://pokeapi.co/api/v2/stat/6/" } }, { "base_stat": 48, "effort": 0, "stat": { "name": "special-defense", "url": "https://pokeapi.co/api/v2/stat/5/" } }, { "base_stat": 48, "effort": 0, "stat": { "name": "special-attack", "url": "https://pokeapi.co/api/v2/stat/4/" } }, { "base_stat": 48, "effort": 0, "stat": { "name": "defense", "url": "https://pokeapi.co/api/v2/stat/3/" } }, { "base_stat": 48, "effort": 0, "stat": { "name": "attack", "url": "https://pokeapi.co/api/v2/stat/2/" } }, { "base_stat": 48, "effort": 1, "stat": { "name": "hp", "url": "https://pokeapi.co/api/v2/stat/1/" } }], "types": [{ "slot": 1, "type": { "name": "normal", "url": "https://pokeapi.co/api/v2/type/1/" } }], "weight": 40 }

```
```
{
  "abilities": [
    {
      "ability": {
        "name": "imposter",
        "url": "https://pokeapi.co/api/v2/ability/150/"
      },
      "is_hidden": true,
      "slot": 3
    },
    {
      "ability": {
        "name": "limber",
        "url": "https://pokeapi.co/api/v2/ability/7/"
      },
      "is_hidden": false,
      "slot": 1
    }
  ],
  "base_experience": 101,
  "forms": [
    {
      "name": "ditto",
      "url": "https://pokeapi.co/api/v2/pokemon-form/132/"
    }
  ],
  "game_indices": [
    {
      "game_index": 132,
      "version": {
        "name": "white-2",
        "url": "https://pokeapi.co/api/v2/version/22/"
      }
    },
    {
      "game_index": 132,
      "version": {
        "name": "black-2",
        "url": "https://pokeapi.co/api/v2/version/21/"
      }
    },
    {
      "game_index": 132,
      "version": {
        "name": "white",
        "url": "https://pokeapi.co/api/v2/version/18/"
      }
    },
    {
      "game_index": 132,
      "version": {
        "name": "black",
        "url": "https://pokeapi.co/api/v2/version/17/"
      }
    },
    {
      "game_index": 132,
      "version": {
        "name": "soulsilver",
        "url": "https://pokeapi.co/api/v2/version/16/"
      }
    },
    {
      "game_index": 132,
      "version": {
        "name": "heartgold",
        "url": "https://pokeapi.co/api/v2/version/15/"
      }
    },
    {
      "game_index": 132,
      "version": {
        "name": "platinum",
        "url": "https://pokeapi.co/api/v2/version/14/"
      }
    },
    {
      "game_index": 132,
      "version": {
        "name": "pearl",
        "url": "https://pokeapi.co/api/v2/version/13/"
      }
    },
    {
      "game_index": 132,
      "version": {
        "name": "diamond",
        "url": "https://pokeapi.co/api/v2/version/12/"
      }
    },
    {
      "game_index": 132,
      "version": {
        "name": "leafgreen",
        "url": "https://pokeapi.co/api/v2/version/11/"
      }
    },
    {
      "game_index": 132,
      "version": {
        "name": "firered",
        "url": "https://pokeapi.co/api/v2/version/10/"
      }
    },
    {
      "game_index": 132,
      "version": {
        "name": "emerald",
        "url": "https://pokeapi.co/api/v2/version/9/"
      }
    },
    {
      "game_index": 132,
      "version": {
        "name": "sapphire",
        "url": "https://pokeapi.co/api/v2/version/8/"
      }
    },
    {
      "game_index": 132,
      "version": {
        "name": "ruby",
        "url": "https://pokeapi.co/api/v2/version/7/"
      }
    },
    {
      "game_index": 132,
      "version": {
        "name": "crystal",
        "url": "https://pokeapi.co/api/v2/version/6/"
      }
    },
    {
      "game_index": 132,
      "version": {
        "name": "silver",
        "url": "https://pokeapi.co/api/v2/version/5/"
      }
    },
    {
      "game_index": 132,
      "version": {
        "name": "gold",
        "url": "https://pokeapi.co/api/v2/version/4/"
      }
    },
    {
      "game_index": 76,
      "version": {
        "name": "yellow",
        "url": "https://pokeapi.co/api/v2/version/3/"
      }
    },
    {
      "game_index": 76,
      "version": {
        "name": "blue",
        "url": "https://pokeapi.co/api/v2/version/2/"
      }
    },
    {
      "game_index": 76,
      "version": {
        "name": "red",
        "url": "https://pokeapi.co/api/v2/version/1/"
      }
    }
  ],
  "height": 3,
  "held_items": [
    {
      "item": {
        "name": "metal-powder",
        "url": "https://pokeapi.co/api/v2/item/234/"
      },
      "version_details": [
        {
          "rarity": 5,
          "version": {
            "name": "ultra-sun",
            "url": "https://pokeapi.co/api/v2/version/29/"
          }
        },
        {
          "rarity": 5,
          "version": {
            "name": "moon",
            "url": "https://pokeapi.co/api/v2/version/28/"
          }
        },
        {
          "rarity": 5,
          "version": {
            "name": "y",
            "url": "https://pokeapi.co/api/v2/version/24/"
          }
        },
        {
          "rarity": 5,
          "version": {
            "name": "x",
            "url": "https://pokeapi.co/api/v2/version/23/"
          }
        },
        {
          "rarity": 5,
          "version": {
            "name": "white-2",
            "url": "https://pokeapi.co/api/v2/version/22/"
          }
        },
        {
          "rarity": 5,
          "version": {
            "name": "black-2",
            "url": "https://pokeapi.co/api/v2/version/21/"
          }
        },
        {
          "rarity": 5,
          "version": {
            "name": "white",
            "url": "https://pokeapi.co/api/v2/version/18/"
          }
        },
        {
          "rarity": 5,
          "version": {
            "name": "black",
            "url": "https://pokeapi.co/api/v2/version/17/"
          }
        },
        {
          "rarity": 5,
          "version": {
            "name": "soulsilver",
            "url": "https://pokeapi.co/api/v2/version/16/"
          }
        },
        {
          "rarity": 5,
          "version": {
            "name": "heartgold",
            "url": "https://pokeapi.co/api/v2/version/15/"
          }
        },
        {
          "rarity": 5,
          "version": {
            "name": "platinum",
            "url": "https://pokeapi.co/api/v2/version/14/"
          }
        },
        {
          "rarity": 5,
          "version": {
            "name": "pearl",
            "url": "https://pokeapi.co/api/v2/version/13/"
          }
        },
        {
          "rarity": 5,
          "version": {
            "name": "diamond",
            "url": "https://pokeapi.co/api/v2/version/12/"
          }
        },
        {
          "rarity": 5,
          "version": {
            "name": "leafgreen",
            "url": "https://pokeapi.co/api/v2/version/11/"
          }
        },
        {
          "rarity": 5,
          "version": {
            "name": "firered",
            "url": "https://pokeapi.co/api/v2/version/10/"
          }
        },
        {
          "rarity": 5,
          "version": {
            "name": "emerald",
            "url": "https://pokeapi.co/api/v2/version/9/"
          }
        },
        {
          "rarity": 5,
          "version": {
            "name": "sapphire",
            "url": "https://pokeapi.co/api/v2/version/8/"
          }
        },
        {
          "rarity": 5,
          "version": {
            "name": "ruby",
            "url": "https://pokeapi.co/api/v2/version/7/"
          }
        }
      ]
    },
    {
      "item": {
        "name": "quick-powder",
        "url": "https://pokeapi.co/api/v2/item/251/"
      },
      "version_details": [
        {
          "rarity": 50,
          "version": {
            "name": "ultra-sun",
            "url": "https://pokeapi.co/api/v2/version/29/"
          }
        },
        {
          "rarity": 50,
          "version": {
            "name": "moon",
            "url": "https://pokeapi.co/api/v2/version/28/"
          }
        },
        {
          "rarity": 50,
          "version": {
            "name": "y",
            "url": "https://pokeapi.co/api/v2/version/24/"
          }
        },
        {
          "rarity": 50,
          "version": {
            "name": "x",
            "url": "https://pokeapi.co/api/v2/version/23/"
          }
        },
        {
          "rarity": 50,
          "version": {
            "name": "white-2",
            "url": "https://pokeapi.co/api/v2/version/22/"
          }
        },
        {
          "rarity": 50,
          "version": {
            "name": "black-2",
            "url": "https://pokeapi.co/api/v2/version/21/"
          }
        },
        {
          "rarity": 50,
          "version": {
            "name": "white",
            "url": "https://pokeapi.co/api/v2/version/18/"
          }
        },
        {
          "rarity": 50,
          "version": {
            "name": "black",
            "url": "https://pokeapi.co/api/v2/version/17/"
          }
        },
        {
          "rarity": 50,
          "version": {
            "name": "soulsilver",
            "url": "https://pokeapi.co/api/v2/version/16/"
          }
        },
        {
          "rarity": 50,
          "version": {
            "name": "heartgold",
            "url": "https://pokeapi.co/api/v2/version/15/"
          }
        },
        {
          "rarity": 50,
          "version": {
            "name": "platinum",
            "url": "https://pokeapi.co/api/v2/version/14/"
          }
        },
        {
          "rarity": 50,
          "version": {
            "name": "pearl",
            "url": "https://pokeapi.co/api/v2/version/13/"
          }
        },
        {
          "rarity": 50,
          "version": {
            "name": "diamond",
            "url": "https://pokeapi.co/api/v2/version/12/"
          }
        }
      ]
    }
  ],
  "id": 132,
  "is_default": true,
  "location_area_encounters": "https://pokeapi.co/api/v2/pokemon/132/encounters",
  "moves": [
    {
      "move": {
        "name": "transform",
        "url": "https://pokeapi.co/api/v2/move/144/"
      },
      "version_group_details": [
        {
          "level_learned_at": 1,
          "move_learn_method": {
            "name": "level-up",
            "url": "https://pokeapi.co/api/v2/move-learn-method/1/"
          },
          "version_group": {
            "name": "ultra-sun-ultra-moon",
            "url": "https://pokeapi.co/api/v2/version-group/18/"
          }
        },
        {
          "level_learned_at": 1,
          "move_learn_method": {
            "name": "level-up",
            "url": "https://pokeapi.co/api/v2/move-learn-method/1/"
          },
          "version_group": {
            "name": "sun-moon",
            "url": "https://pokeapi.co/api/v2/version-group/17/"
          }
        },
        {
          "level_learned_at": 1,
          "move_learn_method": {
            "name": "level-up",
            "url": "https://pokeapi.co/api/v2/move-learn-method/1/"
          },
          "version_group": {
            "name": "omega-ruby-alpha-sapphire",
            "url": "https://pokeapi.co/api/v2/version-group/16/"
          }
        },
        {
          "level_learned_at": 1,
          "move_learn_method": {
            "name": "level-up",
            "url": "https://pokeapi.co/api/v2/move-learn-method/1/"
          },
          "version_group": {
            "name": "x-y",
            "url": "https://pokeapi.co/api/v2/version-group/15/"
          }
        },
        {
          "level_learned_at": 1,
          "move_learn_method": {
            "name": "level-up",
            "url": "https://pokeapi.co/api/v2/move-learn-method/1/"
          },
          "version_group": {
            "name": "black-2-white-2",
            "url": "https://pokeapi.co/api/v2/version-group/14/"
          }
        },
        {
          "level_learned_at": 1,
          "move_learn_method": {
            "name": "level-up",
            "url": "https://pokeapi.co/api/v2/move-learn-method/1/"
          },
          "version_group": {
            "name": "xd",
            "url": "https://pokeapi.co/api/v2/version-group/13/"
          }
        },
        {
          "level_learned_at": 1,
          "move_learn_method": {
            "name": "level-up",
            "url": "https://pokeapi.co/api/v2/move-learn-method/1/"
          },
          "version_group": {
            "name": "colosseum",
            "url": "https://pokeapi.co/api/v2/version-group/12/"
          }
        },
        {
          "level_learned_at": 1,
          "move_learn_method": {
            "name": "level-up",
            "url": "https://pokeapi.co/api/v2/move-learn-method/1/"
          },
          "version_group": {
            "name": "black-white",
            "url": "https://pokeapi.co/api/v2/version-group/11/"
          }
        },
        {
          "level_learned_at": 1,
          "move_learn_method": {
            "name": "level-up",
            "url": "https://pokeapi.co/api/v2/move-learn-method/1/"
          },
          "version_group": {
            "name": "heartgold-soulsilver",
            "url": "https://pokeapi.co/api/v2/version-group/10/"
          }
        },
        {
          "level_learned_at": 1,
          "move_learn_method": {
            "name": "level-up",
            "url": "https://pokeapi.co/api/v2/move-learn-method/1/"
          },
          "version_group": {
            "name": "platinum",
            "url": "https://pokeapi.co/api/v2/version-group/9/"
          }
        },
        {
          "level_learned_at": 1,
          "move_learn_method": {
            "name": "level-up",
            "url": "https://pokeapi.co/api/v2/move-learn-method/1/"
          },
          "version_group": {
            "name": "diamond-pearl",
            "url": "https://pokeapi.co/api/v2/version-group/8/"
          }
        },
        {
          "level_learned_at": 1,
          "move_learn_method": {
            "name": "level-up",
            "url": "https://pokeapi.co/api/v2/move-learn-method/1/"
          },
          "version_group": {
            "name": "firered-leafgreen",
            "url": "https://pokeapi.co/api/v2/version-group/7/"
          }
        },
        {
          "level_learned_at": 1,
          "move_learn_method": {
            "name": "level-up",
            "url": "https://pokeapi.co/api/v2/move-learn-method/1/"
          },
          "version_group": {
            "name": "emerald",
            "url": "https://pokeapi.co/api/v2/version-group/6/"
          }
        },
        {
          "level_learned_at": 1,
          "move_learn_method": {
            "name": "level-up",
            "url": "https://pokeapi.co/api/v2/move-learn-method/1/"
          },
          "version_group": {
            "name": "ruby-sapphire",
            "url": "https://pokeapi.co/api/v2/version-group/5/"
          }
        },
        {
          "level_learned_at": 1,
          "move_learn_method": {
            "name": "level-up",
            "url": "https://pokeapi.co/api/v2/move-learn-method/1/"
          },
          "version_group": {
            "name": "crystal",
            "url": "https://pokeapi.co/api/v2/version-group/4/"
          }
        },
        {
          "level_learned_at": 1,
          "move_learn_method": {
            "name": "level-up",
            "url": "https://pokeapi.co/api/v2/move-learn-method/1/"
          },
          "version_group": {
            "name": "gold-silver",
            "url": "https://pokeapi.co/api/v2/version-group/3/"
          }
        },
        {
          "level_learned_at": 1,
          "move_learn_method": {
            "name": "level-up",
            "url": "https://pokeapi.co/api/v2/move-learn-method/1/"
          },
          "version_group": {
            "name": "yellow",
            "url": "https://pokeapi.co/api/v2/version-group/2/"
          }
        },
        {
          "level_learned_at": 1,
          "move_learn_method": {
            "name": "level-up",
            "url": "https://pokeapi.co/api/v2/move-learn-method/1/"
          },
          "version_group": {
            "name": "red-blue",
            "url": "https://pokeapi.co/api/v2/version-group/1/"
          }
        }
      ]
    }
  ],
  "name": "ditto",
  "order": 197,
  "species": {
    "name": "ditto",
    "url": "https://pokeapi.co/api/v2/pokemon-species/132/"
  },
  "sprites": {
    "back_default": "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/back/132.png",
    "back_female": null,
    "back_shiny": "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/back/shiny/132.png",
    "back_shiny_female": null,
    "front_default": "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/132.png",
    "front_female": null,
    "front_shiny": "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/shiny/132.png",
    "front_shiny_female": null
  },
  "stats": [
    {
      "base_stat": 48,
      "effort": 0,
      "stat": {
        "name": "speed",
        "url": "https://pokeapi.co/api/v2/stat/6/"
      }
    },
    {
      "base_stat": 48,
      "effort": 0,
      "stat": {
        "name": "special-defense",
        "url": "https://pokeapi.co/api/v2/stat/5/"
      }
    },
    {
      "base_stat": 48,
      "effort": 0,
      "stat": {
        "name": "special-attack",
        "url": "https://pokeapi.co/api/v2/stat/4/"
      }
    },
    {
      "base_stat": 48,
      "effort": 0,
      "stat": {
        "name": "defense",
        "url": "https://pokeapi.co/api/v2/stat/3/"
      }
    },
    {
      "base_stat": 48,
      "effort": 0,
      "stat": {
        "name": "attack",
        "url": "https://pokeapi.co/api/v2/stat/2/"
      }
    },
    {
      "base_stat": 48,
      "effort": 1,
      "stat": {
        "name": "hp",
        "url": "https://pokeapi.co/api/v2/stat/1/"
      }
    }
  ],
  "types": [
    {
      "slot": 1,
      "type": {
        "name": "normal",
        "url": "https://pokeapi.co/api/v2/type/1/"
      }
    }
  ],
  "weight": 40
}

```
##### OUTPUT

```
1.All the abilities
 pokemon.abilities
2.pokemon.base_experience
 The base experience
3.The height
 pokemon.height
4.The url for the item "metal-powder"
 pokemon.held_items[0].item.url
5.All the sprites
 pokemon.sprites
6.The different stat names
 pokemon.types[0].slot
7.The slot for the types
 pokemon.weight
8.The weight
 pokemon.weight
9.The first version_group_details
 pokemon.moves[0].version_group_details[0]



```
#### Section 16 - String Methods
##### Lecture 72 Getting the String Length
```
var thing = "Hello There !!"
thing.length
```
**Space is also counted as character**
 ##### OUTPUT 
 ```
 14
 
 ```
 ##### Lecture 73 Indexes and Searching
 
 ```
 // Using Indexes and Searching
var sentence = "I say Hello and You say Hello "

// First Sentence of string
sentence.indexOf("Hello")

// last sentence of string
sentence.lastIndexOf("Hello")
 
 ```
**Diffference** between Index and lastIndexOf is 
 
 - indexOf : gives the first occurence of the matching string
 - lastIndexOf : searches the whole string until it finds the last one  
 - search : gives the first occurence of the matching string

```
    // Using Indexes and Searching
    var sentence = "I say Hello and You say Hello"
    
    // First Sentence of string
    sentence.indexOf("Hello")

    // last sentence of string
    sentence.lastIndexOf("Hello")

    // search
    sentence.search("Hello")

```
```
var sentence = "I say Hello and You say Hello"

sentence.lastIndexOf("Hello")
24

sentence.indexOf("Hello")
6

sentence.search("I")
0

sentence.search("and")
12
```

#### Lecture 74 Taking a Slice,substring and substr
 ```
var str = "Happy ,Excited ,Calm"
var sl = str.slice(7,14)
console.log(sl)
```
- **Slice takes a copy or a part of the original string and then return it,so that we can store it into a new variable.**
- **It doesn't change the original string which means the vlue of the original string will remain same.**
- **It goes from left to right.**
 - **The text direction flow can also be changed.Which adds the -ve place values**
- **Substring does not allow the negative values.**
- **slice() works like substring() with a few different behaviors.**

  ***What they have in common between SLICE and SUBSTRING***
- If start equals stop: returns an empty string
- If stop is omitted: extracts characters to the end of the string
- If either argument is greater than the string's length, the string's length will be used instead.
  
  ***Distinctions of substring():***
- If start > stop, then substring will swap those 2 arguments.
- If either argument is negative or is NaN, it is treated as if it were 0.

  ***Distinctions of slice():***
- If start > stop, slice() will return the empty string. ("")
- If start is negative: sets char from the end of string, exactly like substr() in Firefox. This behavior is  observed in both Firefox and IE.
- If stop is negative: sets stop to: string.length – Math.abs(stop) (original value), except bounded at 0 (thus, Math.max(0, string.length + stop)) 


###### **SYNTAX**
```
datatype NewDataName = OriginalStringVariable.slice(Starting Index,Ending Index )
```
```
var str = "Happy ,Excited ,Calm"

var sl = str.slice(7,14)
console.log(sl)
  Excited

sl = str.slice(7)
console.log(sl)
  Excited ,Calm

sl=str.slice(-13,-6)
console.log(sl)
  Excited

sl=str.slice(-13)// to change the direction from L2R to R2L 
console.log(sl)
  Excited ,Calm
 ```
 
```
 var str = "Happy ,Excited ,Calm"
 var sb = str.substring(7,14)
 console.log(sb)

 sb = str.substring(7)
 console.log(sb) 
```
```
Excited

Excited ,Calm
```
#### Lecture 75 Replacing Content
 ```
    var str =  "I have turkey for lunch and turkey for dinner"
    var lunch = str.replace("turkey","pasta")
    console.log(lunch)
    lunch = str.replace("TURKEY","pasta")
 ```
 // this is case sensitive method
// but if we don't want to be case sensitive(case insensitive) below is the query to avoid this
```
    lunch = str.replace(/Turkey/i,"pasta")// to make it case insensitive
    lunch = str.replace(/Turkey/gi,"Maggi")// to make it case insensitive and global
    console.log(lunch)
```
// g - global replaces all the instances of the occurences that we want to replace

#### Lecture 76 Converting to Upper,Lower and Trimming
```
    var word ="Happy"
    var upperword = word.toUpperCase()
    console.log(upperword)

    var word = "HAPPY"
    var lowerword = word.toLowerCase()
    console.log(lowerword)

    var sentence = " Hello World! "
    var cln = sentence.trim()
    console.log(cln)
```
##### OUTPUT
```
HAPPY // UpperCase
happy // LowerCase
Hello World! //trim()
```
#### Lecture 77 Converting a string to an array

```
var str = "1,2,3,4,5"
var arr = str.split(",")
arr

// OUTPUT

Array (5)[
 0: 1
 1: 2
 2: 3
 3: 4
 4: 5
]

var str = "1,2,3,4,5"
var arr = str.split(" ")
arr

// OUTPUT

Array (1)[
 0: 1,2,3,4,5
]

var str = "1 2 3 4 5"
var arr = str.split(" ")
arr

// OUTPUT
Array (5)[
 0: 1
 1: 2
 2: 3
 3: 4
 4: 5
]

var str = "12345"
var arr = str.split(" ")
arr

// OUTPUT

Array (1)[
0: 12345
]

var str = "12345"
var arr = str.split("")
arr

// OUTPUT

Array (5)[
 0: 1
 1: 2
 2: 3
 3: 4
 4: 5
]

var str = "I have a test"
var arr = str.split(" ")
arr

// OUTPUT

(4)[
 0: "I"
 1: "have"
 2: "a"
 3: "test"
]
```

#### Lecture 78 Converting a string to a number

```
var num = "5"
     var newnum = Number(num)
     newnum = Number("5.5")

// OUTPUT

5.5
```
```
var num = "5"
     var newnum = Number(num)
     newnum = Number("0.5")
// OUTPUT

0.5
```
```
var num = "5"
     var newnum = Number(num)
     newnum = Number(" 5.5 ")

// OUTPUT

5.5
```
**The AlphaNumeric parameter gives the NULL value**
```
var num = "5"
     var newnum = Number(num)
     newnum = Number("t5")

// OUTPUT

NaN
```
```
var num = ""
num = parseFloat("0.5")

// OUTPUT

0.5


var num = ""
num = parseFloat(" t5 ")

// OUTPUT

NaN

```
#### Lecture 79 Assignment
```
Find all instances of the word "cheeseburgers", and replace it with the word "hamburgers". Be sure to note the casing of the word.

Find all instances of the word "bun", and capitalize all the letters.
  story.split("bun").length 
  //Above script give the count of the word "bun" in the stroy string

Then I want you to provide the following information using string methods.

How many characters are in the story?

How many words are in the story?

If you are curious where the story came from, check our http://cheeseburgeripsum.com.

```
```
var story = "Cheeseburgers come in all kinds of manifestations, but we want them in and around our mouth no matter what. Slide those smashed patties with the gently caramelized meat fat between a toasted brioche bun and pass it over. You fall in love with the cheeseburger itself but the journey ain’t half bad either. They’re the childhood friend that knows your highest highs and lowest lows. They’ve been with you through thick and thin and they’re the best at keeping secrets. Whether it’s dressed up or informal, cheeseburgers have your back. Sometimes we lose sight of what really matters in life. There’s something to be said for a gourmet brie and truffle burger paired with parmesan frites, but don’t let that make you forget about the ol’ faithful with American cheddar and a squishy bun. Lettuce remind you that cheeseburgers come in all forms - bun intended. Pop quiz: what’s the greatest thing to happen to your mind, body, and soul in recent history? A cheeseburger, obviously. Cheeseburgers know that what you want can also be what you need."

```
#### OUTPUT and SOLUTIONS
```
var story1 = story.replace(/hamburgers/gi,"cheeseburgers")
```
```
story1
"cheeseburgers come in all kinds of manifestations, but we want them in and around our mouth no matter what. Slide those smashed patties with the gently caramelized meat fat between a toasted brioche bun and pass it over. You fall in love with the cheeseburger itself but the journey ain’t half bad either. They’re the childhood friend that knows your highest highs and lowest lows. They’ve been with you through thick and thin and they’re the best at keeping secrets. Whether it’s dressed up or informal, cheeseburgers have your back. Sometimes we lose sight of what really matters in life. There’s something to be said for a gourmet brie and truffle burger paired with parmesan frites, but don’t let that make you forget about the ol’ faithful with American cheddar and a squishy bun. Lettuce remind you that cheeseburgers come in all forms - bun intended. Pop quiz: what’s the greatest thing to happen to your mind, body, and soul in recent history? A cheeseburger, obviously. cheeseburgers know that what you want can also be what you need."
```
```
story.replace(/bun/g ,"bun".toUpperCase())
```
```
hamburgers come in all kinds of manifestations, but we want them in and around our mouth no matter what. Slide those smashed patties with the gently caramelized meat fat between a toasted brioche BUN and pass it over. You fall in love with the cheeseburger itself but the journey ain’t half bad either. They’re the childhood friend that knows your highest highs and lowest lows. They’ve been with you through thick and thin and they’re the best at keeping secrets. Whether it’s dressed up or informal, hamburgers have your back. Sometimes we lose sight of what really matters in life. There’s something to be said for a gourmet brie and truffle burger paired with parmesan frites, but don’t let that make you forget about the ol’ faithful with American cheddar and a squishy BUN. Lettuce remind you that hamburgers come in all forms - BUN intended. Pop quiz: what’s the greatest thing to happen to your mind, body, and soul in recent history? A cheeseburger, obviously. hamburgers know that what you want can also be what you need.
```
```
//String Length

story.length
1031

// Counting the number of words using split method in JavaScript

story.split(" ").length
178
```

#### Lecture 79 - Converting A number to a String

```
var num = 1234
var str
str = num.toString()
 "1234"
str
 "1234"
num
 1234
(123).toString()
 "123"
(123.5).toString()
 "123.5"
 
```

#### Lecture 80 - Exponents and Working with Decimals
###### Syntax
```
number.toExponential(decimal places)
```
###### Examples

```
var x =5.566
x
 5.566

x.toExponential(2)
 5.57e+0

x.toExponential()
 5.566e+0

x.toExponential(5)
 5.56600e+0

var x=5.566
x.toFixed(2)
 5.57

var x =5.6666
x.toPrecision(2)
 5.7

```
##### Lecture 80 Not A Number
##### Lecture 81 Math Object
```
Math()
Math.PI [Value of PI]
Math.round(argument) [round up/down the value of the given argument]
Math.pow(base value,exponential value) [gives the value of the power]
Math.sqrt(argument) [gives the value of the square root]
Math.cell(4.4) 
 5 // cell feature will give the round up value
Math.floor[4.7]
 4 //will restrict to round down the value
Math.min(1,2,3,4,5,6,7) // gives the minimum value
Math.max(1,2,3,4,5,6,7) // gives the maximum value
Math.random() // gives a random number between 0 and 1
```

##### Lecture 83 Array Length
```
var arr = [1, 2, 3, 4, 5]
arr.length

5
```
```
##### OUTPUT
5
length is not a method but a property of an array
```
##### Lecture 84 Converting an array to a string
```
var arr =["hi","Bye","Morning","Hello"]
arr.toString()
 "hi,Bye,Morning,Hello"

var arr =["hi","Bye","Morning","Hello"]
arr.join(" | ")
 "hi | Bye | Morning | Hello"
```
#### Lecture 85 Merging Arrays
 
 ```
  var arr1 = [1,2,3,4]
    var arr2 = [5,6,7,8]
newArr = arr1.concat(arr2)

Array (8)[ 1,2,3,4,5,6,7,8 ]

var arr1 = [1,2,3,4]
    var arr2 = [5,6,7,8]
newArr = arr2.concat(arr1)

Array (8)[ 5,6,7,8,1,2,3,4 ]
 
 ```
#### Lecture 86 Sorting of a String Array
```
 var arr = ["b","a","c"]
   arr.sort()

Array (3)[ a,b,c ]

   var arr = ["c","a","b"]
   arr.reverse()

Array (3)[ "b","a","c" ]

```
```
  var arr = ["b","a","c"]
  arr.sort()
  arr.reverse()
  
Array (3)[ "c","b","a" ]


```

**Reverse function takes the whole array and just flips it and prints it backward so in order to print it in a sorted reverse order,
we should first sort the array string and then reverse it**

#### Lecture 87 Sorting of a Number Array
sort() function does not work good with the numbers because it deals with a character like a string

#### Lecture 88 Array forEach and Map
 forEach doesn,t return anything and the map method returns an array

```
var num = [1,2,3,4,5]
   num.forEach(test)
   function test(value,index,array) {
     console.log(index + ": " + value + "\n")
   }
   
0: 1
1: 2
2: 3
3: 4
4: 5
```
```
var num = [1,2,3,4,5]
   num.forEach(test)
   function test(value,index,array) {
     console.log(index + ": " + value + "\n" + array)
   }

0: 1
1,2,3,4,5
1: 2
1,2,3,4,5
2: 3
1,2,3,4,5
3: 4
1,2,3,4,5
4: 5
1,2,3,4,5
```
```
var num = [1,2,3,4,5]
   num.forEach(test)
   function test(value,index,array) {
     console.log(index + ": " + value + " & " + array[index] + "\n" )
   }
   
0: 1 & 1
1: 2 & 2
2: 3 & 3
3: 4 & 4
4: 5 & 5
```
```
var num = [1,2,3,4,5]
   var newNum
   newNum = num.map(test)
   function test(value, index ,array){
     newNum = index + ": " + value + " & " +array[index] + "\n"
     return newNum
   }
   
Array (5)[
0: "0: 1 & 1↵"
1: "1: 2 & 2↵"
2: "2: 3 & 3↵"
3: "3: 4 & 4↵"
4: "4: 5 & 5↵"
]
```
```
var num = [1, 2, 3, 4 ,5]
var newNum = ""
num.forEach(test)
function test(value, index, array){
  newNum = newNum + index + " : " + value + " & " + array[index] + "\n"
}
undefined
newNum
"0 : 1 & 1
1 : 2 & 2
2 : 3 & 3
3 : 4 & 4
4 : 5 & 5
"
```
#### Lecture 89 Array Filter
 It is callback function which takes a value index and the array 
 
```
 var num = [1, 5, 10, 11, 12, 15]
 var even = num.filter(isEven)
 function isEven(value,index,array){
 return value % 2 == 0
}

even

Array (2)[
0: 10
1: 12
]
```
#### Lecture 90 Date Basics
Date is a snapshot of the moment in time

```
var newDate = new Date()
newDate
Mon Jan 13 2020 11:03:11 GMT+0530 (India Standard Time)

var newDate = new Date()
newDate
Mon Jan 13 2020 11:03:21 GMT+0530 (India Standard Time)
```
#### Lecture 91 Getting Parts of a Date

```
newDate.getUTCFullYear()
2020

newDate.getUTCMonth()
0
//Month starts with zero(0)

newDate.getUTCDay()
1

newDate.getDate()
13

newDate.getHours()
11

var today = newDate.getMonth() +  "-" + newDate.getDate() + " - " + newDate.getFullYear()

today

"0-13 - 2020"

newDate.getHours()
11

newDate.getUTCMinutes()
45

newDate.getMinutes()
15

newDate.getMilliseconds()
884

newDate
Mon Jan 13 2020 11:15:17 GMT+0530 (India Standard Time)

```
#### Lecture 92 Setting new Dates
```
Mon Jan 13 2020 11:15:17 GMT+0530 (India Standard Time)
var newDate = new Date()

Mon Jan 13 2020 11:21:40 GMT+0530 (India Standard Time)
newDate.setFullYear(2021)
1610517100685

newDate
Wed Jan 13 2021 11:21:40 GMT+0530 (India Standard Time)
```
#### Lecture 93 Running JavaScript from a WebPage
 JavaScript executes from top to bottom
 
#### Lecture 94 Minified JavaScript// minified JavaScript
 ```
 // Normal JavaScript
 
 var thing = "Hello world"
 document.getElementById("sample").innerHTML = thing

// Minified JavaScript
 var thing="Hello world";document.getElementById("sample").innerHTML=thing;

 // it is like the minified JSON and it is just a way of conserving space

```
##### Lecture 95 The DOM(Document Object Model)

```
The use of the dom fr javascript is to access the elements of the HTML
with the DOM JavaScript can change all the elements on the page, it also can react to HTML events
```

##### Lecture 96 Finding Elements

##### Lecture 97 Relationships
```
Parent - child - Sibling - relationship
```

##### Lecture 98 Changing HTML
inner HTML is going to change the contents inside the HTML

```
  - getElementById
  - document.createElement
  - appendChild
  - insertBefore
  - removeChild
```

##### Lecture 99 Changing Style
```
document.getElementById("ElementName").style.color = "blue"
document.getElementById("ElementName").style.border = "1px black solid"
```
##### Lecture 100 JavaScript Events Intro
##### Lecture 101 Events

