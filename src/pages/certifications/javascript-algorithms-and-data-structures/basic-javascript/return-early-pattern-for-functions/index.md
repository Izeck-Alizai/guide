---
title: Return Early Pattern for Functions
---
## Return Early Pattern for Functions

This is a stub. <a href='https://github.com/freecodecamp/guides/tree/master/src/pages/certifications/javascript-algorithms-and-data-structures/basic-javascript/return-early-pattern-for-functions/index.md' target='_blank' rel='nofollow'>Help our community expand it</a>.

<a href='https://github.com/freecodecamp/guides/blob/master/README.md' target='_blank' rel='nofollow'>This quick style guide will help ensure your pull request gets accepted</a>.

<!-- The article goes here, in GitHub-flavored Markdown. Feel free to add YouTube videos, images, and CodePen/JSBin embeds  -->

Edited by: Ahmed Ishaq Alizai @isaac_alixai <br/> (If there are errors or this is not the way it was supposed to be done, then please, by all means, fix it. Thank you!)

## Return Early Pattern for Functions
When a return statement is reached, the execution of the current function stops and control returns to the calling location.

#### Example
    function myFun()
    {
    console.log("Hello");
    return "World";
    console.log("byebye");
    }
    myFun();
    
The above outputs "Hello" to the console, returns "World", but "byebye" is never output, because the function exits at the return statement.

Modify the function abTest so that if a or b are less than 0 the function will immediately exit with a value of undefined.

### Hint 1
Remember that undefined is a keyword, not a string.

### Hint 2
For you to understand and code easily, you can use Else...If statements in your code.
try to solve the problem now

# Spoiler alert!
Solution ahead!

#### Code Solution:
    function abTest(a, b)
    {
      if(a < 0 || b < 0)
      {
        return undefined;   //Not displaying "undefined" as output
      }
      else if(a == 2 && b == 2)
      {
        return 8;
      }
      else if(a == 2 && b == 8)
      {
        return 18;
      }
      else if(a == 3 && b == 3)
      {
        return 12;
      }
      else
      {
        return "Invalid";
      }
    }
    console.log(abTest(2, 2));
    console.log(abTest(-2, 2));
    console.log(abTest(2, -2));
    console.log(abTest(2, 8));
    console.log(abTest(3, 3));
