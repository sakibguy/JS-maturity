Data Types & Variables
----------------------
Learn to represent real-world data using JavaScript variables, and distinguish between the different data types in the language.

Keynotes
--------
1. Intro to Data Types
2. Numbers
3. Comments
   - Comments are often used to clarify and document non-obvious code. It's good practice to include code comments to improve code readability.
4. Quiz: First Expression (2-1)
5. Strings
   - [front-end](http://udacity.github.io/frontend-nanodegree-styleguide/javascript.html) nanodegree
6. String Concatenation 
   - What do you think will happen when you type "Hello" + 5*10 into the console?
   - implicit type coercion: You've just discovered some peculiar behavior in JavaScript. It’s called implicit type coercion and it's a feature of JavaScript. JavaScript multiplies the 5*10 to become 50 and then changes the number 50 into the string "50", so you're adding together the same data type. This then gets combined with the string "Hello". You'll learn more about why this happens later in this lesson.
7. [Variables](https://classroom.udacity.com/courses/ud803/lessons/74007e2e-2a0a-4de3-a8a6-5c2ec4275773/concepts/d38fbf76-c43a-47dd-b031-b20397d6c283): Google's JavaScript StyleGuide [here](https://google.github.io/styleguide/jsguide.html), [all](https://github.com/sakib-rahman-bangladesh/styleguide)
   - The postLiked variable has a descriptive name about what it represents
8. Quiz: Converting Temperatures (2-2)
9. **TODO:** [String Index](https://classroom.udacity.com/courses/ud803/lessons/74007e2e-2a0a-4de3-a8a6-5c2ec4275773/concepts/397a5635-43bd-42d1-b181-179b2c902f67) done
10. **Escaping Strings:** To use quotes inside a string ``` \ ```
    - If you forget to use the backslash to escape characters, then the JavaScript engine can misinterpret your strings. ``` "The man whispered, "please speak to me."" ``` 
     - By using the backslash to escape characters, the JavaScript engine can understand the meaning of your strings.
```"The man whispered, \"please speak to me.\"" ```
     - **Special characters**
Quotes aren’t the only special characters that need to be escaped, there’s actually [quite a few](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#Using_special_characters_in_strings). However, to keep it simple, here’s a list of some common special characters in JavaScript.
       - newline \n and tab \t, are unique because they add additional whitespace to your Strings. A newline character will add a line break and a tab character will advance your line to the next [tab stop](https://en.wikipedia.org/wiki/Tab_stop).
       - QUIZ QUESTION: Select the string that returns the following output: 
         ``` "The file located at "C:\\Desktop\My Documents\Roster\names.txt" contains the names on the roster." ```
       - Right answer is: ```"The file located at \"C:\\\\Desktop\\My Documents\\Roster\\names.txt\" contains the names on the roster."```
11. **Comparing Strings**
      - Comparing strings: Another way to work with strings is by comparing them. You've seen the comparison operators == and != when you compared numbers for equality. You can also use them with strings! For example, let’s compare the string "Yes" to "yes". ```"Yes" == "yes"``` Returns: false
      - When you run this in the console, it returns false. Why is that? "Yes" and "yes" are the same string, right? Well not quite.
      - Case-sensitive: When you compare strings, case matters. While both string use the same letters (and those letters appear in the same order), the first letter in the first string is a capital Y while the first letter in the second string is a lowercase y. ``` 'Y' != 'y' ``` Returns: true
      - [QUIZ QUESTION](https://classroom.udacity.com/courses/ud803/lessons/74007e2e-2a0a-4de3-a8a6-5c2ec4275773/concepts/3c9feefc-71f8-4d03-97a2-97f9386a53fb): Enter each expression into the console. Check the ones that evaluate to true.
      - When checking if a string is "greater than" or "less than" another string, JavaScript compares individual characters using a numerical value. Each character is assigned a numerical value that essentially corresponds to the character's location in an [ASCII](https://www.ascii-code.com/) table
12. Quiz: Favorite Food (2-3)
13. Quiz: [String Equality](https://classroom.udacity.com/courses/ud803/lessons/74007e2e-2a0a-4de3-a8a6-5c2ec4275773/concepts/1094e5d1-4986-42e5-9777-fa43d269ec81) for All (2-4)
14. Quiz: [All Tied Up](https://classroom.udacity.com/courses/ud803/lessons/74007e2e-2a0a-4de3-a8a6-5c2ec4275773/concepts/5a82b56c-8c1e-40e4-acc9-cc396fbfb439) (2-5)
15. Quiz: [Yosa Buson](https://classroom.udacity.com/courses/ud803/lessons/74007e2e-2a0a-4de3-a8a6-5c2ec4275773/concepts/69fa04db-4a01-443b-89f5-e60626379ef9) (2-6): ```var haiku = "Blowing from the west\n" + "Fallen leaves gather\n" + "In the east."; console.log(haiku);```
16. **TODO:** [Booleans](https://classroom.udacity.com/courses/ud803/lessons/74007e2e-2a0a-4de3-a8a6-5c2ec4275773/concepts/de395b73-8bbc-4d13-85bb-9d3f75141ecd) Next goal
      
17. Quiz: Facebook Post (2-7)
18. Null, Undefined, and NaN
19. Equality
    1. Implicit type coercion: JavaScript is known as a loosely typed language.
       - Basically, this means that when you’re writing JavaScript code, you do not need to specify data types. Instead, when your code is interpreted by the JavaScript engine it will **automatically be converted** into the "appropriate" data type. This is called implicit type coercion. It’s behavior like this which makes JavaScript unique from other programming languages, but it can lead to some quirky behavior when doing operations and comparisons on mixed data types.
        - **DEFINITION:** A strongly typed language is a programming language that is more likely **<i>to generate errors if data does not closely match an expected type</i>**. Because JavaScript is loosely typed, you don’t need to specify data types; however, this **<i>can lead to errors that are hard to diagnose</i>** due to implicit type coercion.
        - When you use the == or != operators, JavaScript first converts each value to the same type (if they’re not already the same type); this is why it's called **"type coercion"!** This is often not the behavior you want, and **it’s actually considered bad practice to use the == and != operators when comparing values for equality.**
    2. Strict equality
       - Instead, in JavaScript it’s better to use strict equality to see if numbers, strings, or booleans, etc. are identical in type and value without doing the type conversion first. To perform a strict comparison, simply add an additional equals sign = to the end of the == and != operators. "1" === 1 Returns: false; This returns false because the string "1" is not the same type and value as the number 1. 0 === false, Returns: false; This returns false because the number 0 is not the same type and value as the boolean false.
20. Quiz: Semicolons! (2-8)
21. Quiz: What's my Name? (2-9)
22. Quiz: Out to Dinner (2-10)
23. Quiz: Mad Libs (2-11)
24. Quiz: One Awesome Message (2-12)
25. Lesson 2 Summary
