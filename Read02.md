### Components, Classes and Callbacks 

"Components" can also mean a specific technical approach to doing so, like a React component or a Vanilla JS component.

## Applying Atomic Design
# [Part 1](https://medium.com/backticks-tildes/visually-breaking-down-ui-components-using-atomic-design-part-1-476e1ddd73ca)
> * Atomic Design Methodology
> * [Familiarity with Atomic Design terms](https://atomicdesign.bradfrost.com/chapter-2/)
> * Start big and work your way down
>   * Split the page design into large sections — Organisms
>   * Next, divide your Organisms into Molecules, Look out for sections that are repeated frequently
>   * hen, Extract your atoms from the Molecules. Remember elements that can’t be broken up any further 

# [Part 2](https://medium.com/backticks-tildes/visually-breaking-down-ui-components-using-atomic-design-and-building-with-react-part-2-20eb8aabab4b)
> * A folder structure should follow a consistent pattern, to allow you (and other people) browse through the files quickly and easily
> * Start small and work your way up
>   * When visually breaking down a design into components, we start big and work our way down. On the other hand, when building these components with code, it is preferable to do the exact opposite. Build the smaller components first and then use them to compose the larger ones.
>   * For components to be reusable and composable, you have to make them as small and as independent as possible
> * What this covers: 
>   * We split the page design visually into components
>   * Next, we structured our folder to follow a consistent pattern
>   * Then, we built out the components starting from the atoms, and we worked our way up to the organisms.
 
# [More Examples](https://theiconic.tech/the-art-of-transforming-ui-features-into-components-e86de5560fd7)
> * We’re not designing pages, we’re designing systems of components.
> * Similarly, interfaces are made up of smaller components. This means we can break entire interfaces down into fundamental building blocks and work up from there. That’s the basic gist of atomic design.
>   * the developer is wasting time by re-implementing patterns you already have
>   * the developer is contributing to the inflation of your stylesheets by adding the same styles again and again out of lack of awareness that they already exist
>   * the developer will notice that his styles interfere with other styles and will add a surplus of css overrides to force his component into shape
>   * the developer will not notice that his styles interfere with other styles and will break the barstool in the other bar

# [Step 1 only of Thinking in React](https://reactjs.org/docs/thinking-in-react.html)
> * Start With A Mock
> * Step 1: Break The UI Into A Component Hierarchy
>   * The first thing you’ll want to do is to draw boxes around every component (and subcomponent) in the mock and give them all names.
>       * Their Photoshop layer names may end up being the names of your React components!
>   *  single responsibility principle, that is, a component should ideally only do one thing.
>   * Now that we’ve identified the components in our mock, let’s arrange them into a hierarchy.


# [UI Components by Design](https://www.thoughtworks.com/insights/blog/ui-components-design)
> * Express design as working components
>   * “Components let you split the UI into independent, reusable pieces, and think about each piece in isolation".
> * Convergence of language
>   * What’s new is the emergence of a common language between designers and developers
> * Two Types of Components​
>   * Foundation Components are the primary expression of the design language of the system. They’re the defining parts of the experience, and very targeted in scope. They ensure a consistent underlying interface. UI Developers on the design team will build them.
>   * Application Components are specific to one of the applications being built, and not seen as a defining, foundational part of the UI. They’re usually larger in scope, and almost always composed of one or many Foundation Components. Some Application Components may eventually transition into Foundation Components. The application teams will build them.
> * Isolate and elaborate
> * Build
> * Integrate and Learn
> * Treat Foundation Components as a product

## Callbacks

# [What are JavaScript Callbacks?](https://www.sitepoint.com/callbacks-javascript/)
> * What Is a Callback? - 
>   * Simply put: A callback is a function that is to be executed after another function (normally asynchronous) has finished executing — hence the name ‘call back’.
>   * More complexly put: In JavaScript, functions are objects. Because of this, functions can take functions as arguments, and can be returned by other functions. Functions that do this are called higher-order functions. Any function that is passed as an argument and subsequently called by the function that receives it, is called a callback function.
> * Why Do We Need Callbacks?
>   * JavaScript is an event driven language. This means that instead of waiting for a response before moving on, JavaScript will keep executing while listening for other events.
> * Create a Callback (see article for specific examples)

# [JavaScript Callback Functions](https://www.dashingd3js.com/lessons/javascript-callback-functions)
> * 
> * 
> * 
> * 
> * 
> * 
> * 
> * 
> * 
> * 
>   * 
> * 
> * 
> * 
>   * 
>   * 
>   * 
>   * 
>       * 
>       * 
>       * 
>       * 
>       * 
>   * 
>   * 
>   * 

# []()
> * 
> * 
> * 
> * 
> * 
> * 
> * 
> * 
> * 
> * 

# []()
> * 
> * 
> * 
> * 
> * 
> * 
> * 
> * 
> * 
> * 

## Review: Classes
# []()
> * 
> * 
> * 
> * 
> * 
> * 
> * 
> * 
> * 
> * 

# []()
> * 
> * 
> * 
> * 
> * 
> * 
> * 
> * 
> * 
> * 

## Review: this
# []()
> * 
> * 
> * 
> * 
> * 
> * 
> * 
> * 
> * 
> * 
