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
9. **TODO:** [String Index](https://classroom.udacity.com/courses/ud803/lessons/74007e2e-2a0a-4de3-a8a6-5c2ec4275773/concepts/397a5635-43bd-42d1-b181-179b2c902f67) Next goal
10. Escaping Strings: To use quotes inside a string ``` \ ```
    - If you forget to use the backslash to escape characters, then the JavaScript engine can misinterpret your strings. ``` "The man whispered, "please speak to me."" ``` 
     - By using the backslash to escape characters, the JavaScript engine can understand the meaning of your strings.
```"The man whispered, \"please speak to me.\"" ```
     - **Special characters**
Quotes aren’t the only special characters that need to be escaped, there’s actually [quite a few](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#Using_special_characters_in_strings). However, to keep it simple, here’s a list of some common special characters in JavaScript.
       - newline \n and tab \t, are unique because they add additional whitespace to your Strings. A newline character will add a line break and a tab character will advance your line to the next [tab stop](https://en.wikipedia.org/wiki/Tab_stop).
       - QUIZ QUESTION: Select the string that returns the following output: 
         ``` "The file located at "C:\\Desktop\My Documents\Roster\names.txt" contains the names on the roster." ```
       - Right answer is: ```"The file located at \"C:\\\\Desktop\\My Documents\\Roster\\names.txt\" contains the names on the roster."```
11. Comparing Strings
12. Quiz: Favorite Food (2-3)
13. Quiz: String Equality for All (2-4)
14. Quiz: All Tied Up (2-5)
15. Quiz: Yosa Buson (2-6)
16. Booleans
17. Quiz: Facebook Post (2-7)
18. Null, Undefined, and NaN
19. Equality
20. Quiz: Semicolons! (2-8)
21. Quiz: What's my Name? (2-9)
22. Quiz: Out to Dinner (2-10)
23. Quiz: Mad Libs (2-11)
24. Quiz: One Awesome Message (2-12)
25. Lesson 2 Summary
