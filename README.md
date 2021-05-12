# ArrayAssignment

map - take 1 array and convert into a new array. Creates a new array populated with the result of calling a provided function on every element in the calling array

Example 1:

const codes = [
{name: "Javascript"},
{name: "Node"},
{name: "HTML"},
{name: "CSS"},
{name: "Python"}
]

const codeNames = codes.map((item) => {
return item.name;
})

console.log(codeNames);

Example 2:

const rappers = [
{name: "Dababy", Birthname: "Jonathan Lyndale Kirk"},
{name: "Lil Durk", Birthname: "Durk Derrick Banks"},
{name: "Pooh Sheisty", Birthname: "Lontrell Dennell Williams, Jr."},
{name: "Chance The Rapper", Birthname: "Chancelor Johnathan Bennett"},
{name: "Megan Thee Stallion", Birthname: "Megan Jovon Ruth Pete"}
]

const Rap = rappers.map((item) => {
return item.Birthname;
})

console.log(Rap);

Example 3:

const items = [
{name: 'Bike', price: 50},
{name: 'Apple iwatch', price: 300},
{name: 'Ipad mini', price: 400}
]

const itemNames = items.map((item) => {
return item.price;
})

console.log(itemNames);

reduce - takes in 4 methods which are accumulator, current value, current index, and source array. It executes a reducer function on each element of the array, resulting in a single output value.

Example 1:

let arr = [1,3,5,7,8];

let result = arr.reduce((sum, current) => sum + current, 0);

console.log(result);

Example 2:

let price = [13,17,52,33];

const total = price.reduce((currentTotal, item) => {
return item.price + currentTotal;
},0)

console.log(total);

Example 3:

let num = [1,2,3,4,5,6]

num.reduce((sum,current) => sum + current);

filter - executes a callback function on each element in an array Returns a new array after calling on an existing array

Example 1:

const supplies = [
{name: "notebook", price: 15},
{name: "ruler", price: 6},
{name: "pencils", price: 4},
{name: "pens", price: 5}
]

const filt = supplies.filter((item) => {
return item.price <=5;
})

console.log(filt);

Example 2:

const name = [
{name: "Jennifer", ID: 1},
{name: "Danielle", ID: 2},
{name: "Katie", ID: 3},
{name: "Bradley", ID: 4}
]

const school = name.filter((item) => {
return item.ID<3;
})

console.log(school);

Example 3:

const num1 = [1,2,3,4,5,6,7,8];

const number = num1.filter((item) => {
return item.num1<3
})

console.log(number);

forEach - allows to run a function for every element of the array. Executes a provided function once for each array and the same code for each array

Example 1:

["apple","orange","strawberry", "peach"].forEach(alert);

Example 2:

const foods = [
{name: "Burger", price: 10},
{name: "fries", price: 12}
]

foods.forEach((item) => {
console.log(item.price);
})

Example 2:

["Bilbo", "Gandalf", "Nazgul"].forEach((item, index, array) => {
alert(${item} is at index ${index} in ${array});
});

sort - sorts an array in place.

Example 1:

const names = ["James","Debra","Brandon","Parker","Nancy"];

console.log(names.sort())

Example 2:

const number = [7,18,4,6,100,50,30];

console.log(number.sort());

Example 3:

const fruits = ["Banana","Apple","strawberry","peach","lemon"]

console.log(fruits.sort());

slice - Returns a shallow copy of a portion of an array into a new array object selected from start to end.

Example 1:

const arr = [1,2,3,4,5,6,7];

console.log(arr.slice(2,5));

Example 2:

const names = ["Terri","Brandon","Jared","Jennifer"]

console.log(names.slice(2,4),"Lindsay","Ryan");

Example 3:

const rap = ["Dababy","Lil durk","lil baby","Pooh Sheisty","Chance the rapper","Megan thee Stallion"]

console.log(rap.slice(3,5));

pop - extracts item from the end. Removes item

Example 1:

const food = ["burger","fries","hotdog","pizza"]

food.pop();

console.log(food);

Example 2:

const rap = ["Dababy","Lil durk","Chance the rapper","Megan thee stallion","lil baby"];

rap.pop();

console.log(rap)

Example 3:

const num = [1,2,3,4,5,6,7];

num.pop();

console.log(num);

shift - extracts an item from the beginning. removes an item from the beginning

Example 1:

const toys = ["Minni mouse","Mickey mouse","Pokemon","Fidget spinner"]

toys.shift();

console.log(toys);

Example 2:

const rapNames = ["Lil mosey","lil durk","lil baby","pooh sheisty","cardi b"]

rapNames.shift();

console.log(rapNames);

Example 3:

const fruits = ['Pear','Apple',"peaches"];

fruits.shift();

console.log(fruits);

push - Adds an item to the end;

Example 1:

const products = ["Computers","Ipad","Playstation 5"];

products.push("Iphone");

console.log(products);

Example 2:

const ID = [1,2,3,4,5];

ID.push(6);

console.log(ID);

Example 3:

const Iphone = ["Iphone 8plus","Iphone 11","Iphone x"]

Iphone.push("Iphone 12")

console.log(Iphone)

unshift - adds an item to the beginning

Example 1:

const music = ["Billie Eilish","Meran Morris","Lizzo","Ariana Grande"]

music.unshift("Lil Nas X")

console.log(music);

Example 2:

const NBA = ["Knicks","Nets","Milwaukee"]

NBA.unshift("Pelicans")

NBA.unshift("Clippers")

console.log(NBA);

includes - takes in a single argument in an array. looks for item starting from index from, returns true if found. Uses item and from parameter

Example 1:

const arr = ["Lil Nas X","Megan Thee Stallion"]

console.log(arr.includes("Lil Nas X"));

Example 2:

console.log(arr.includes("Chance the Rapper"));

Example 3:

console.log(arr.includes("Lil Nas X","Chance The Rapper"));

indexOf - returns the first index at which a given element can be found in the array, or -1 if is not present.

Example 1:

const people = ["Brandon", "Jennifer","Casey","Jack"]

console.log(people.indexOf("Brandon"));

Example 2:

console.log(people.indexOf("Jack"))

Example 3:

console.log(people.indexOf(9));

Every - checks every items to see if its true. Some checks some number returns a boolean value

Example 1:

const items = [
{name: "Laptop", price: 400},
{name: "Ipad", price: 450},
{name: "Iwatch", price: 500},
{name: "Dell", price: 700}
]

const products = items.every((item) => {
return item.price <=800;
})

console.log(products);

Example 2:

const products = items.every((item) => {
return item.price <= 500
})

console.log(products);
