What is JavaScript?
-------------------
Learn the history of JavaScript and start writing your code immediately using the JavaScript console.

Keynotes
--------
1. [Intro to JS](https://classroom.udacity.com/courses/ud803/lessons/e98aae00-9563-4fca-b91c-a4e79ca79c27/concepts/921085c8-9e58-4c26-a729-f1406b49b504)
   - **JS based platforms | Source of app:** web, robotics, game(unity), code editor 
2. TODO: [JS demo](https://classroom.udacity.com/courses/ud803/lessons/e98aae00-9563-4fca-b91c-a4e79ca79c27/concepts/0f5b4af1-c639-4cf1-85e7-933f31ad823a), **Done**
3. Lesson 1 Summary
   - Browser built-in js engine
   - JS console: print string + executes lines of js code on the fly inside browser
   - Added styles and animation through JS
     - Open the [following site](https://daringfireball.net/projects/markdown/) in a new tab and in that tab also open up developer tools. Then paste the following code:
     ``` document.getElementsByTagName("h1")[0].style.color = "#ff0000";```
   - Styling elements on the page is great, but you could also do that by just modifying the CSS. What makes JavaScript so special in this case? Refresh the page, then paste this line of code in the JavaScript console.
```
document.body.addEventListener('click', function () {
     var myParent = document.getElementById("Banner"); 
     var myImage = document.createElement("img");
     myImage.src = 'https://thecatapi.com/api/images/get?format=src&type=gif';
     myParent.appendChild(myImage);
     myImage.style.marginLeft = "160px";
});
```
If you’re confused because nothing happened. Don’t worry. Click somewhere on the page.
