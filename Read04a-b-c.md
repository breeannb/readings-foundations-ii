# Read 04a: URL Search Params, URL Hash, & Hash Change Event

## [MDN URLSearchParams built-in class](https://developer.mozilla.org/en-US/docs/Web/API/URLSearchParams)
> * Not going to add much here, the article is very self explanatory, definitely want to keep it for future reference (probably tomorrow)


## [toString(https://developer.mozilla.org/en-US/docs/Web/API/URLSearchParams/toString) returns query string]()
> * The toString() method of the URLSearchParams interface returns a query string suitable for use in a URL.


## [Built-in Location Object](https://developer.mozilla.org/en-US/docs/Web/API/Location)
> * The Location interface represents the location (URL) of the object it is linked to. Changes done on it are reflected on the object it relates to. Both the Document and Window interface have such a linked Location, accessible via Document.location and Window.location respectively.


## [Built-in Location Object](https://developer.mozilla.org/en-US/docs/Web/API/Window/hashchange_event)
> * The hashchange event is fired when the fragment identifier of the URL has changed (the part of the URL beginning with and following the # symbol).


# Read 04b: URL Search Params, URL Hash, & Hash Change Event

## [RegExr](https://regexr.com/)

## [Regex Tutorial](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)
> * data validation (for example check if a time string i well-formed)
> *data scraping (especially web scraping, find all pages that contain a certain set of words eventually in a specific order)
> * data wrangling (transform data from “raw” to another format)
> * string parsing (for example catch all URL GET parameters, capture text inside a set of parenthesis)
> * string replacement (for example, even during a code session using a common IDE to translate a Java or C# class in the respective JSON object — replace “;” with “,” make it lowercase, avoid type declaration, etc.)
> * yntax highlightning, file renaming, packet sniffing and many other applications involving strings (where data need not be textual)

## [Regex 101](https://regex101.com/)
Tutorial 

# Read 04c: Read 04c: Asynchronous JavaScript, Promises, and fetch

## [On Callbacks](https://flaviocopes.com/javascript-callbacks/)
> * JavaScript is synchronous by default, and is single threaded. This means that code cannot create new threads and run in parallel. Find out what asynchronous code means and how it looks like
> * Asynchronous means that things can happen independently of the main program flow.
> * Programs internally use interrupts, a signal that’s emitted to the processor to gain the attention of the system.
> * JavaScript is synchronous by default and is single threaded. This means that code cannot create new threads and run in parallel.
> * Callbacks - You can’t know when a user is going to click a button, so what you do is, you define an event handler for the click event. This event handler accepts a function, which will be called when the event is triggered:
> * A callback is a simple function that’s passed as a value to another function, and will only be executed when the event happens. We can do this because JavaScript has first-class functions, which can be assigned to variables and passed around to other functions (called higher-order functions)

## [Understanding JavaScript Promises](https://flaviocopes.com/javascript-promises/)
> * Promises are one way to deal with asynchronous code in JavaScript, without writing too many callbacks in your code.
> * A promise is commonly defined as a proxy for a value that will eventually become available.
> * Async functions use the promises API as their building block, so understanding them is fundamental even if in newer code you’ll likely use async functions instead of promises.
> * Once a promise has been called, it will start in pending state. This means that the caller function continues the execution, while it waits for the promise to do its own processing, and give the caller function some feedback.
> * At this point, the caller function waits for it to either return the promise in a resolved state, or in a rejected state, but the function continues its execution while the promise does it work.


## [MDN on Asynchronous](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous/Promises)

## [Intro](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous/Introducing)

## [Promises](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous/Promises)


## [Using Promises](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Using_promises)
## [Javascript Promises and Fetch for beginners](https://www.youtube.com/watch?v=IHjzyhjKxtc)
## [JavaScript Promises in Sixteen Minutes](https://medium.com/quick-code/javascript-promises-in-twenty-minutes-3aac5b65b887)
## [All articles JavaScript Promises: An introduction](https://web.dev/promises/)
## [Using Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch)
## [That data looks so fetching on you: Understanding the JS Fetch API](https://itnext.io/that-data-looks-so-fetching-on-you-understanding-the-js-fetch-api-880eae0c8d25)