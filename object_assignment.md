# Object Exercises
Jonathan Erquinigo
1. Log the cats species.
```js
 let cat = {
   genus: 'Felis',
   species: 'Catus'
}
```

let cat = {
  genus: 'Felis',
  species: 'Catus'
}

console.log(cat["species"])

2. Add a color quality to the cat from the previous question.

let cat = {
  genus: 'Felis',
  species: 'Catus'
  color: 'brown'
}

console.log(cat["species"])

3. How do you check if our cat object has the property texture?

let cat = {
  genus: 'Felis',
  species: 'Catus'
  color: 'brown'
}

console.log(cat["texture"])

4. Loop through the following object and log all of directors.
``` js
let films = [
 {
   name: 'Psycho',
   director: 'Alfred Hitchcock',
   released: 1960
 }, {
   name: 'Citizen Kane',
   director: 'Orson Welles',
   released: 1941
 }, {
   name: 'The Usual Suspects',
   director: 'Bryan Singer',
   released: 1995
 }
]


let films = [
 {
   name: 'Psycho',
   director: 'Alfred Hitchcock',   // 0
   released: 1960
 }, {
   name: 'Citizen Kane',
   director: 'Orson Welles',      // 1
   released: 1941
 }, {
   name: 'The Usual Suspects',
   director: 'Bryan Singer',     //2
   released: 1995
 }
]
let filmDirec = [];
for(let i = 0; i < films.length; i++){
  filmDirec.push(films[i].director)
  console.log(filmDirec)

}

```
5. What will this code log?
```js
let p1 = {
  name: 'Joe'
}

let p2 = {
  name: 'Joe'
}

console.log(p1 === p2)

it will log false

```


#### Recipe

* Create an object to hold information on your favorite recipe. It should have the following properties: `name`, `servings`, and `ingredients` (an array).
* Create a loop that logs the recipe information, so it looks like:

```javascript
name: Mole
servings: 2
ingredients: cinnamon, cumin, cocoa
```

let favRecipe = [
{
name: "lasagna",
serving: 1,
ingredients: ["pasta", "TomatoSauce","cheese"]

}
]
//console.log(favRecipe[0].ingredients[1]);

let favIngred = [];
for(let i = 0; i < favRecipe.length; i++){
favIngred.push(favRecipe[i].ingredients)
}
console.log(favIngred)

#### getProps
Write a code block that takes an object variable and logs all the keys as an array.
let dailyItems = {

person:["keys", "phone", "wallet"],
meals:["breakfast", "lunch","dinner"],
bathroom:["toilet paper", "toothpaste","toothbrush"]

}

let dailyKeys = Object.keys(dailyItems)
//console.log(dailyItems[0].meals[2])
console.log(dailyKeys)

#### getValues
Write a code block that takes an object variable and logs all the values as an array.


let dailyItems = {

person:["keys", "phone", "wallet"],
meals:["breakfast", "lunch","dinner"],
bathroom:["toilet paper", "toothpaste","toothbrush"]

}

let dailyKeys = Object.values(dailyItems)
//console.log(dailyItems[0].meals[2])
console.log(dailyKeys)

#### getObjLength
Write a code block the logs the number of properties an object has.

let getObjLength = {
  name: "Jonathan",
  school: "pursuit",
  location: "queens"
}


let objKeys = Object.keys(getObjLength).length

console.log(objKeys)



#### WatchList
Create an array of films, where each film has the following properties: title, director, and a boolean indicating if you started watching it.
Create a code block that iterates over the array and logs whether the film was watched or not. If it was watched, log a string like

`You already watched "Wonder Woman" directed by Patty Jenkins`
and if not, log

`You still need to watch "Wonder Woman" by director Patty Jenkins. `

let films = [
  {
title: "The Shining",
director: "Director1",
Boolean: true

},

{
  title: "Ready Player One",
  director: "Director2",
  Boolean: false
},

]

let watchedFilms = [];
for(let i = 0; i < films.length; i++){
  watchedFilms.push(films[i].Boolean)
  //console.log(watchedFilms[i])

  if(watchedFilms[i] === true){
console.log("You already watched " + films[i].title + " directed by " + films[i].director);

//favIngred.push(favRecipe[i].ingredient
  }else if(watchedFilms[i] === true){
console.log("You already watched " + films[i].title + " directed by " + films[i].director);
  }
}



#### characterCount
Write a block of code that takes a string varaible and counts the occurance of each character in the string. Use an object to keep track of the counts.

let str = "HelloWorld"
let empObj = {}
for(let i = 0; i < str.length; i++){
//console.log(str[i])
if(empObj[str[i]] === undefined){
  empObj[str[i]] = 1
}else{
empObj[str[i]] += 1
}
}
console.log(empObj)
