# Read 03: Responsive Web Design

## [Shay Howe’s intro to RWD](https://learn.shayhowe.com/advanced-html-css/responsive-web-design/)
> * Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.
> * Responsive web design is focused around providing an intuitive and gratifying experience for everyone.
> * Responsive vs. Adaptive vs. Mobile
>   * Responsive generally means to react quickly and positively to any change, while adaptive means to be easily modified for a new purpose or situation, such as change.
>   * Mobile, on the other hand, generally means to build a separate website commonly on a new domain solely for mobile users. While this does occasionally have its place, it normally isn’t a great idea.
> * Flexible Layouts
>   * Responsive web design is broken down into three main components, including flexible layouts, media queries, and flexible media
>       * Flexible layouts, is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width.
>           * Flexible Grid
>       * Media queries were built as an extension to media types commonly found when targeting and including styles. Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation for example.
>           * Initializing Media Queries
>           * Logical Operators in Media Queries - Logical operators in media queries help build powerful expressions.

## [All About Floats](https://css-tricks.com/all-about-floats/)
> * Float is a CSS positioning property. To understand its purpose and origin, we can look to print design. In a print layout, images may be set into the page such that text wraps around them as needed. This is commonly and appropriately called “text wrap”.
> * Floated elements remain a part of the flow of the web page.
> * Absolutely positioned page elements are removed from the flow of the webpage, like when the text box in the print layout was told to ignore the page wrap.
> * Absolutely positioned page elements will not affect the position of other elements and other elements will not affect them, whether they touch each other or not.
> * There are four valid values for the float property. Left and Right float elements those directions respectively. None (the default) ensures the element will not float and Inherit which will assume the float value from that elements parent element.
> * Clearing the Float
>   * Float’s sister property is clear. An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float.
>   * Clear has four valid values as well. Both is most commonly used, which clears floats coming from either direction. Left and Right can be used to only clear the float from one direction respectively. None is the default, which is typically unnecessary unless removing a clear value from a cascade. Inherit would be the fifth, but is strangely not supported in Internet Explorer.
> * The Great Collapse
>   * One of the more bewildering things about working with floats is how they can affect the element that contains them (their “parent” element). If this parent element contained nothing but floated elements, the height of it would literally collapse to nothing.
> * Techniques for Clearing Floats
>   * The Empty Div Method
>       * ``` <div style="clear: both;"></div> ```
>       * The Overflow Method
>       * The Easy Clearing Method
> * Problems with Floats
>   * Pushdown is a symptom of an element inside a floated item being wider than the float itself (typically an image)
>   * Double Margin Bug
>   * 3px Jog
>   * Bottom Margin Bug


## [Don't Overthink It Grids](https://css-tricks.com/dont-overthink-it-grids/)
## [CSS Floats Explained By Riding An Escalator](https://www.freecodecamp.org/news/css-floats-explained-by-riding-an-escalator-57fa55232333/)
## [SMACSS Official Documentation](http://smacss.com/)
Skimmed over the two above, but wanted to link to come back to 