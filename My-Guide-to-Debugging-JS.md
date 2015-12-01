#### MY GUIDE TO DEBUGGING JAVASCRIPT
You think you've created the perfect code - rich in its content, majestic in its simplicity - and then BAM!

`Error: TypeError: undefined`               

But how is this possible??! You spent hours on that thing and not only that, you double, triple *and* quadruple checked it. Sound familiar? Whether your JS journey started recently at zero or not, you may well empathise. During my short time in the coding game, bugs were, initially, purely a source of frustration and cursing the language for all its unhelpfulness. Since those early stages, the relationship between bugs and I has blossomed into a strange kind of love, for nowhere has the learning curve been more enlightening as in the process of __debugging__.

As is often the case, *Eloquent Java Script* hits the nail on the head and [Chapter 8](http://eloquentjavascript.net/08_error.html) is no exception. The first step to making friends with a bug: 
> Try to resist making random changes to the code. 

I found casting wildly with random code tweaks only furthered my incomprehension. 

Here's how I approach the situation:

1. Switch on the *strict mode* by typing `"strict mode"` into the top of a function body or file (see [EJS](http://eloquentjavascript.net/08_error.html) for detailed example). This will flush out any reading of accidentally created global objects and variables.

2. Use `alert();` to figure out *where* the bug is. Alerts only work with strings but are useful in narrowing down the problem area. Quite simply, an inserted alert which isn't displayed by the browser indicates a bug in the preceding code and vice versa. Watch out *for* using these in *for* loops, you may find your browser crashing!

3. Use `console.log();` to examine certain values at different stages of the code. This can provide important clues as to the bug's whereabouts.

You can practice your debugging skills on these Codewars kata:
-  Unexpected parsing (http://www.codewars.com/kata/unexpected-parsing)
-  Grasshopper - Debug (http://www.codewars.com/kata/grasshopper-debug)
-  Regex Failure - Bug Fixing #2 (http://www.codewars.com/kata/regex-failure-bug-fixing-number-2)
-  Honey to the Bee (http://www.codewars.com/kata/honey-to-the-bee)
-  "this" is an other problem (http://www.codewars.com/kata/this-is-an-other-problem)
-  Breaking search bad (http://www.codewars.com/kata/breaking-search-bad)

### No need to keep clicking it oldskool...
In the real world of web development, times have supposedly moved on for the better and now most browsers support their own tools for debugging. Arguably the most useful is the "Console" option since it shows, not only the error itself, but also the error's exact position! Instructions on how to access this feature are listed by browser [here](http://www.w3schools.com/js/js_debugging.asp). If you're using Chrome, just right click the page, inspect the element and find the "Console" tab on the far right of the menu after "Audits". 

### Further resources...
- For an interactive tour of Chrome's debugging features, this: (http://juliepagano.com/blog/2014/05/18/javascript-debugging-for-beginners/) is definitely a winner. 
- There's also a really interesting half hour tutorial: (https://www.youtube.com/watch?v=rcjUR4icvoQ) on lesser known debugging techniques in JS.
