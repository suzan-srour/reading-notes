
# React Docs - lists and keys

*What does.map() return?* used to iterate over an array and manipulate or change data items.

*If I want to loop through an array and display each value in JSX, how do I do that in React?* use map().

Each list item needs a unique  Key.

*What is the purpose of a key?* Keys help React identify which items have changed, are added, or are removed.

-------------------------------------------------------------------------------------------------------------------------

## The Spread Operator

*What is the spread operator?* (..) expand an iterable object into the list of arguments.
*List 4 things that the spread operator can do.>>*  spreads the array into separate arguments,Copying an array ,Concatenating or combining arrays , Using Math functions ,Using an array as arguments , Adding an item to a list .

*Give an example of using the spread operator to combine two arrays.*
const myArray = [ "S","U","Z","A","N"]
const yourArray = ["A","O","U","N"]
const ourArray = [...myArray,...yourArray]

*Give an example of using the spread operator to add a new item to an array.*
const fewFruit = ['🍏','🍊','🍌']
const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
console.log(fewMoreFruit)

*Give an example of using the spread operator to combine two objects into one.*

const objectOne = {hello: "🤪"}

const objectTwo = {world: "🐻"}

const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}

-------------------------------------------------------------------------------------------------------------------------

## Video

*In the video, what is the first step that the developer does to pass functions between components?* go to the state object and create the function in it's scope , and he use map
*In your own words, what does the increment function do?* update the counter depend on the name we pass
*How can you pass a method from a parent component into a child component?* this.props.method >> this .props.increment
*How does the child component invoke a method that was passed to it from a parent component?* this.increment
