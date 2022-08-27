
# Form

**What is a ‘Controlled Component’?** An input form element whose value is controlled by React in this way is called a “controlled component”.

**Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.**

no ,Since the value attribute is set on our form element, the displayed value will always be this.state.value, making the React state the source of truth. Since handleChange runs on every keystroke to update the React state, the displayed value will update as the user types.
With a controlled component, the input’s value is always driven by the React state. While this means you have to type a bit more code, you can now pass the value to other UI elements too, or reset it from other event handlers

**How do we target what the user is entering if we have an event handler on an input field?**

 the input’s value is always driven by the React state. While this means you have to type a bit more code, you can now pass the value to other UI elements too, or reset it from other event handlers.

-------------------------------------------------------------------------------------------------------------------------------------------

## The Conditional (Ternary) Operator Explained

**Why would we use a ternary operator?**
 to shorten our if statment .

**Rewrite the following statement using a ternary statement**
if(x===y){
  console.log(true);
} else {
  console.log(false);
} ?

X===Y? console.log(true): console.log(false) ;
