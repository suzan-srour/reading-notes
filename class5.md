
# Deep in React

**What is the single responsibility principle and how does it apply to components?**

 single responsibility principle, that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

**What does it mean to build a ‘static’ version of your application?**
build components that reuse other components and pass data using props. props are a way of passing data from parent to child.the . State is reserved only for interactivity, that is, data that changes over time.

**Once you have a static application, what do you need to add?**
You can build top-down or bottom-up. That is, you can either start with building the components higher up in the hierarchy (i.e. starting with FilterableProductTable) or with the ones lower in it (ProductRow). In simpler examples, it’s usually easier to go top-down, and on larger projects, it’s easier to go bottom-up and write tests as you build.

**What are the three questions you can ask to determine if something is state?**
1-Is it passed in from a parent via props? If so, it probably isn’t state.
2-Does it remain unchanged over time? If so, it probably isn’t state.
3-Can you compute it based on any other state or props in your component? If so, it isn’t state.

**How can you identify where state needs to live?**

Identify every component that renders something based on that state.
Find a common owner component (a single component above all the components that need the state in the hierarchy).
Either the common owner or another component higher up in the hierarchy should own the state.
If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

****************************************************

## Higher-Order Functions

**What is a “higher-order function”?**
 higher-order functions allow us to abstract over actions, not just values

**Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?**
return m => m > n;
 it compare the old value with the new and if the new value is greater than the old one return true .

# Explain how either map or reduce operates with regards to higherorder function

Map >>take function with item ,index return a new array without declartion for new array , it takes the array and update the value in the place

Reduce >> The parameters to reduce are, apart from the array, a combining function and a start value. This function is a little less straightforward than filter and map
