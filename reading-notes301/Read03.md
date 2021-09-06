# Spread Operator
The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.  

 ### What is the spread operator?
  
InJavaScript, spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments

### What is ... used for?
Spread operator to the rescue! It looks similar to rest parameters, also using ..., but does quite the opposite.
also can do the next: 
- Copying an array
- Concatenating or combining arrays
- Using Math functions
- Using an array as arguments
- Adding an item to a list
- Adding to state in React
- Combining objects
- Converting NodeList to an array

## the spread operator and older browsers
When programming to support Internet Explorer and browsers on older mobile devices, the spread operator is not going to work.

## A note about copying by reference
One of the benefits of using the spread operator is that it will create a new reference to its primitive values, copying them.
That means that changes to the original array will not affect the copied array, which is what would happen if the array had been linked to the original with the assignment operator =:
## Watch out for the deeply-nested Gotcha!
Onthe other hand, when JavaScript objects including arrays are deeply nested, the spread operator only copies the first level with a new reference, but the deeper values are still linked together.

# Lists and Keys
Given the code below, we use the map() function to take an array of numbers and double their values. We assign the new array returned by map() to the variable doubled and log it:

    const numbers = [1, 2, 3, 4, 5];
    const doubled = numbers.map((number) => number * 2);
    console.log(doubled);
This code logs [2, 4, 6, 8, 10] to the console.

In React, transforming arrays into lists of elements is nearly identical.

**Rendering Multiple Components**
You can build collections of elements and include them in JSX using curly braces {}.

Below, we loop through the numbers array using the JavaScript map() function. We return a


**Basic List Component**
Usually you would render lists inside a component.

We can refactor the previous example into a component that accepts an array of numbers and outputs a list of elements.

    function NumberList(props) {
    const numbers = props.numbers;
    const listItems = numbers.map((number) =>
    < li>{number}< /li>
     );
    return (
      < ul>{listItems}< /ul>
     );
    }

    const numbers = [1, 2, 3, 4, 5];
    ReactDOM.render(
    <NumberList numbers={numbers} />,
     document.getElementById('root')
    );  