# 100 Days Of Code - Log

## Goal:
1. Finish Web Developer Bootcamp
2. Flatiron School Bootcamp Prep
  - Ruby Fundamentals
  - JavaScript
3. Read JavaScript & jQuery by Jon Duckett


## Day 1: July 13, 2017

**Today's Progress:** I worked through ten JavaScript Basics Control Flow exercises on Web Developer Bootcamp. I relearned what while loops are and worked through some exercises. I also learned that I can very quickly break my computer with an infinite loop! :skull:

**Thoughts:** I'm feeling good! I struggled a few times with modulo % because I generally suck at math but I thought it was cool that you can write loops in different ways and have them output odd/even numbers. The indexOf() method was cool too. I like that Colt Steele brings up methods that we have to google during the exercises. It makes the work challenging, as if you're in an actual production environment. So I feel good! Makes my googling skills stronger!

![image](http://i66.tinypic.com/2q84oig.png)
![image](http://i64.tinypic.com/v4rxxt.png)

###### Learned some cool ways to write a program with user inputs
![image](http://i63.tinypic.com/9k6o2v.png)

## Day 2: July 14, 2017

**Today's Progress:** I completed the Intro to For Loops exercises on Web Developer Bootcamp. It was similar to the while loops exercises. I also finished JavaScript Functions tutorials and exercises, which covered functions syntax, arguments, and return.

**Thoughts:** Colt Steele's exercises are great. He teaches you how to google information if you don't know something so I've been trying master this skill; it'll be useful in the long run. I was frustrated with figuring out how to get a function to return a factorial of a number so I worked on it for a little bit, did some googling, and plugged in a few things and realized it worked! I needed the problem solution explanation though to understand why this is how the function returned a factorial.

```
function factorial(num) {
  // define a result variable
  var result = 1;
  for(var i = 2; i <= num; i++){
    result *= i;
  }
  //return the result variable
  return result;
}
```

## Day 3: July 15, 2017

**Today's Progress:** I worked through scopes and higher order functions on Web Developer Bootcamp. I learned about passing function into other functions. I also applied to be an editor for Medium so I worked through the edit challenge from Quincy Larson.

**Thoughts:** I think higher order functions are a bit confusing. I played around with it for a little bit to create my own and it's cool but I want to see how they work in an actual running app/production website.

![image](http://i68.tinypic.com/jutzqx.png)

## Day 4: July 16, 2017

**Today's Progress:** I worked through Introduction to Arrays on Web Developer Bootcamp. Went over some built-in methods such as push(), pop(), shift(), unshift(), indexOf, and slice().

**Thoughts:** This lesson was a nice refresher because I remembered these methods from doing Flatiron's Bootcamp Prep program. I was able to create my own exercises and use these methods in them so today was a good day!

## Day 5: July 17, 2017

**Today's Progress:** I applied to Medium to be a volunteer editor so even though I wasn't actively coding, I took the time to read over the guidelines for the position and read an article on Arduino - which I thought was super interesting.

**Thoughts:** I struggled editing the article because I haven't edited something in so long. However, it was interesting reading a tech article and learning some of the terminology. I'm going to give it another shot tomorrow and submit it to Quincy.

## Day 6: July 18, 2017

**Today's Progress:** I worked on Arrays To Do List part one on Web Developer Bootcamp.

**Thoughts:** Part one of the arrays To Do List code along - I felt like I didn't grasp much from the lesson because I was confused. It's nice to see his thought process in these code alongs but I wish he'd let us do some of the challenges on our own so it forces us to learn.

## Day 7: July 19, 2017

**Today's Progress:** I worked on Array Iteration today and a little bit of Part Two of the To Do List Code Along. I learned how to iterate through arrays using for loops and forEach. My focus was on the forEach() function.

**Thoughts:** I struggled understanding how to use forEach(). I know that it iterates through an array but I was still struggling with the passing functions within functions. So I looked it up on MDN and decided I'd try out a few things with my code:

1. I didn't understand why the first parameter is just a placeholder for the currentValue.
2. When Colt Steele wanted to add an index, I didn't get that either until I realized that the second parameter represents the index in a forEach().
3. The third parameter is the array that the forEach() is being applied to.

I used all the parameters because I was curious what they would do (a snippet of my code):

```
if(input === "list") {
  toDoList.forEach(function(todo, i, toDoList) {
    console.log(i + ": " + todo + toDoList);
  });

```

And this is what I ended up with:

![image](http://i68.tinypic.com/1236ttx.pngx)

I know that in the exercise, we were supposed to print the list out AS A LIST with its index #'s. I wasn't grasping how the forEach just *knew* to print the index of the array. Although the code above looked very ugly when I applied all three parameters, I understand how the forEach() method works! YAY.

## Day 8: July 20, 2017

**Today's Progress:** Worked on Part Two of the To Do List Code Along. My goal was to finish the entire Array section by now but that didn't go as planned because I did some external research on what each method does and took extra time to try to understand it.

**Thoughts:** So my JavaScript prompt kept loading before my HTML loaded even though my ```<script>``` tag was at the bottom of the ```<body>``` tag. I couldn't open my console to view my list because the ```prompt``` wouldn't stop showing up. This was definitely one of my least favorite exercises in the class. However - I learned about

```
window.onload = function() {
}
```

I wanted to understand what would make my HTML page load before my JavaScript. Even though it didn't really work, I now know there is another solution!

## Day 9: July 21, 2017

**Today's Progress:** I worked on the Array Problem Set but decided I'd focus on just the first problem - printReverse() - and spent some time on that.

**Thoughts:** I struggled with this one! I spent a couple of hours trying to figure it out. What I came up with was this:

![image](http://i63.tinypic.com/2j4djfd.png)
(there is a typo in it. artists.length is supposed to be array.length)

So this kept printing an empty array. I tried changing around the .reverse() method and printing different things but I got frustrated eventually so I slept on it. I don't want to look at the solution right away so I'm going to spend some time on it tomorrow!

## Day 10: July 23, 2017

**Today's Progress:** Finished the Array Problem Set. I spent time working on each problem while also trying to understand what I did. I worked on isUniform(), sumArray(), and max() on Web Developer Bootcamp.

**Thoughts:** I know that knowing how to do research and googling things is part of the industry so I utilize Stack Overflow quite a bit but I feel like I've been pretty good at finding/plugging things into my code and somehow, making it work - it almost feels like it's cheating??? Is this normal?!

So I worked on **isUniform()** and this is what I did:

```
function isUniform(array) {
  for(var i = 0; i < array.length -1; i++) {
    if(array[i] !== array[i+1]) {
      return false
    }
  }
  return true
}
```

**Colt Steele**:

```
function isUniform(arr) {
  var first = arr[0];
  for(var i = 1; i < arr.length; i++){
    if(arr[i] !== first) {
      return false;
    }
  }
  return true;
}
```

I honestly have no idea what I did and why it worked but I understood the second one a lot more because I know that I needed to keep track of the first element and if it's not equal to the first then return false. I understand the logic a lot more in the solution than what I attempted to do.


**sumArray()**: I used a for loop in this one and Colt Steele's solution used a forEach. I still don't feel comfortable using forEach, nor do I know when to use them. Does this get better the more you use them in daily applications?

**My code:**

```
function sumArray(num) {
  var result = 0;
  for(var i = 0; i < num.length; i++) {
    result += num[i];
  }
  return result;
}
```

**Colt Steele:**

```
function sumArray(arr) {
  var total = 0;
  arr.forEach(function(element){
    total += element;
  });
  return total;
}
```

And then in the last exercise, **max()**, where the function is supposed to look for the maximum number in an array, I was close!

**This is what I did:**
```
function max(arr) {
  var max = 0;
  for(var i = 0; i < arr.length; i++) {
    if(arr[i] > max) {
      max = arr[i];
    }
  }
  return max;
}
```

Where I messed up was that my variable wasn't equaled to ``` var max = arr[0] ``` I know that once I start using these methods more, I'll understand how/why they work the way they work.


## Day 11: July 24, 2017

**Today's Progress:** I moved on from arrays to objects. Completed three lessons on Web Developer Bootcamp in addition to using MDN to practice writing my own objects.

**Thoughts:** I feel good about this. So I know the basic structure of an object ``` var someObj = { key: value } ``` which is a data structure that holds information. I liked the dictionary analogy given. These lessons were a bit tedious/refreshers because I remember objects from previous tutorials. I think they are a lot more fun to write than arrays and a lot less confusing to access.

## Day 12: July 25, 2017

**Today's Progress:** I learned about objects within arrays and arrays within objects and completed the Movie Database exercise.

**Thoughts:** This was confusing! It didn't help that my motivation level today was very low. I wish that the instructor would use for loops instead of ```forEach()```. I'm still confused about how to use ```forEach()``` - it's scary! - but I guess I should practice exercises using it and see if they work. The lessons that involve code alongs are usually boring for me because I feel like I'm just watching tutorials. But I got through objects, so yay!

## Day 13: July 26, 2017

**Today's Progress:** Learned about JS Methods - putting functions inside of objects and the keyword ```this```. Also practiced more of ```forEach()```. I tried writing the Movie Database exercise with a ```for loop``` and failed miserably.

**Thoughts:** I spent about 2 hours writing the Movie Database exercise using a ```for loop```. I struggled and couldn't figure out what I was doing right/wrong so I decided to eventually move on from it. I'm going to pick it back up again and play around with it but for now I moved on to Web Developer Bootcamp lessons on JS Methods and learning about the keyword ```this```.

## Day 14: July 27, 2017

**Today's Progress:** I STARTED DOM MANIPULATION TODAY! This is exciting because this is where I got stuck last time and "gave up" because I didn't have any knowledge in HTML/CSS. I spent time learning about selectors.

**Thoughts:** I feel great! Selectors were a completely foreign language to me when I first started learning about the DOM. Now that I've come back to it, I understand it and I think it's so interesting. I learned about the 5 selectors:

```getElementById
getElementsByClassName
getElementsByTagName
querySelector
querySelectorAll
```

These are pretty self explanatory now because I know what ID, Class, Tags, and CSS-style elements are. When I first looked at the DOM, I freaked out and questioned taking this entire path because I was so stuck and my fear kicked in. Now that I know a little bit more, I understand it. I did pretty well on the exercise too. However, when I was doing some google research, I know that writing code like this ```document.querySelector("div.user-panel.main input[name='login']");``` is going to be difficult and I'm going to need time to learn.

## Day 15: July 28, 2017

**Today's Progress:** I worked on The DOM style manipulation, text and content, and attributes. I haven't gotten to build anything yet but I played around with the DOM code:

```var body = document.querySelector("body");
var isPurple = false;

setInterval(function() {
  if(isPurple) {
    body.style.background = "white";
  } else {
    body.style.background = "#9841f4";
  }
  isPurple = !isPurple;
}, 1000);

var tag = document.getElementById("highlight");
tag.style.color = "blue";
tag.style.border = "10px solid red";
tag.style.fontSize = "70px";
tag.style.background = "yellow";
tag.style.marginTop = "200px";
```

**Thoughts:** I'm not sure how I feel! I have so many questions and I also feel like I wouldn't know where to begin if I was given a problem...but who knows? So I learned about the separation of concerns where **HTML** is the structure, **Javascript** is the behavior and **CSS** is the presentation. If we have a CSS style sheet, what's the point of style manipulation? Is it to add interactivity? It's essentially the same thing as a style sheet? Wouldn't it override some of the CSS styles if we use style manipulation? Is it just a form of problem-solving?

## Day 16: July 29, 2017

**Today's Progress:** I spent an hour doing the Google Code Along and playing around with the DOM methods.

**Thoughts:** I thought this was cool! I see how these methods can be used for debugging. I can't wait to learn about interactivity!

## Day 17: July 30, 2017

**Today's Progress:** Coded for an hour - learned about ```addEventListener``` and then played around with the Color Toggle game on Web Dev Bootcamp.

**Thoughts:** Feeling good! I understood that I needed to start my code off with ```var button = document.querySelector("button");``` to select the ```<button></button>``` element and then I added the event listener by writing

``button.addEventListener("click", function() {
     document.body.style.background = "#9841f4";
});
``

After that I didn't know what to do so I played around with ```setInterval()``` and ```if/else``` statements but wasn't able to make it work so I had to watch the solution video. Definitely need more practice.

## Day 18: July 31, 2017

**Today's Progress:** I worked on the Score Keeper Game for a couple of hours. I did my own thing and added some CSS styling so that I can practice some CSS!

**Thoughts:** This was SO fckin' cool! But it was a challenge. When Colt Steele explains the methods and logic, it doesn't seem so hard. But when I have to do it myself...on my own...without any hand holding...that's where I get stuck and I know it can take me HOURS to do a simple task. And that's the scary part because what if I don't get it???!! Although I do believe these code-alongs help you develop a programmer thought-process. This is what I did to my game - yes I could have made it prettier but I wanted to move on to the next lesson.

![image](http://i63.tinypic.com/x3sfu1.png)

## Day 19: August 1, 2017

**Today's Progress:** Other Types of Events: To Do List/ Counting Events Exercise - JavaScript and jQuery

**Thoughts:**

## Day 20: August 2, 2017

**Today's Progress:**

**Thoughts:**

## Day 21: August 3, 2017

**Today's Progress:**

**Thoughts:**

## Day 22: August 4, 2017

**Today's Progress:**

**Thoughts:**

## Day 23: August 5, 2017

**Today's Progress:**

**Thoughts:**

## Day 24: August 6, 2017

**Today's Progress:**

**Thoughts:**

## Day 25: August 7, 2017

**Today's Progress:**

**Thoughts:**
