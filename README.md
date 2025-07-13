# Dice-Game
We all have played Dice-Game in our life offline/online where numbers lies from 1-6 and on each toss their comes a random number.
So, i thought why not build it online and check out my luck while playing it.

## Basic Instruction to follow
1. The game involves two players: Player1 and Player2
2. Player1 plays with dice1 and Player2 plays with dice2
3. Whosoever gets the highest number, when the dice is tossed, wins the game.
4. But, if both gets the same number then it's a draw.

## Tech Stack Used
+ HTML : basic structure for the website
+ CSS : styling the diffenet components in website
+ JavaScript + D0M : to access and manipulate the document's structure, style and content.

## DOM Methods() : Methods Used in Project
It will return the first element within the document that matches the specified CSS selector (as a input, it takes elements, class of element, it's id and can also combine the selectors).
here, it refers to the the first element with the ".img" class and will return it.
```
document.querySelector(".img")
```
SetAtrribute working on setting the attributs and it generally takes two inputs, the attribute we want to change and what we want to change it to.
here, it takes attribute "href" as value1 and "link to change into" 
```
document.querySelector(".img").SetAttribute("href", "https://meet.google.com/landing")
```
It will allow the maipulation of the HTML content within an element. Can be used to retrieve and set HTML content of an element.
here, i have used to change the text content of "h1" element.
```
document.querySelector("h1").innerHTML = "text to change into"
```
## WokFlow of Project
+ Generation of Random Numbers for Both Players
  using the Math.random() method and setting it's range 1-6, the random numbers (randomNumber1 & randomNumber2) will be generated for each players, whenever their specified dice is tossed.
+ Setting Attribute of each number
  Each number generated will be associated with their specified image using the setAttribute method.
+ Setting the necessary conditions
  randomNumber1 comes out to be greater than ranndomNumber2 --> player1 wins
  randomNumber2 comes out to be greater than ranndomNumber1 --> player2 wins
  randomNumber 1 comes out to be equal to randomNumber2 --> draw

