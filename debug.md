Foundation of Debugging
-----------------------
1. Get Started with Debugging JavaScript in [Chrome DevTools](https://developers.google.com/web/tools/chrome-devtools/javascript/)
   - Step 1: BUG Reproduce the bug
   - Step 2: SPUI Get familiar with the Sources panel UI
     - File Navigator pane: Every file that the page requests is listed here
     - Code Editor pane: After selecting a file in the File Navigator pane, the contents of that file are displayed here.
     - JavaScript Debugging pane: Various tools for inspecting the page's JavaScript. If your DevTools window is wide, this pane is displayed to the right of the Code Editor pane.
    - Step 3: BREAKPOINT Pause the code with a breakpoint
       - A common method for debugging a problem like this is to insert a lot of console.log() statements into the code, in order to inspect values as the script executes. For example:
       ```
       function updateLabel() {
          var addend1 = getNumber1();
          console.log('addend1:', addend1);
          var addend2 = getNumber2();
          console.log('addend2:', addend2);
          var sum = addend1 + addend2;
          console.log('sum:', sum);
          label.textContent = addend1 + ' + ' + addend2 + ' = ' + sum;
       }
       ```
       - breakpoints can help you find and fix bugs faster than the console.log() method.
       - See [Pause Your Code With Breakpoints](https://developers.google.com/web/tools/chrome-devtools/javascript/breakpoints) to learn when and how to use each type.
