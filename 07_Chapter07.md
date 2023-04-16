# JavaScript Mastery: Conquering Data Structures Algorithms for Technical Programming Interviews

## Chapter 7: How to Handle Null and Undefined Values

Welcome back, my fellow code enthusiasts! In the last chapter, we learned all about managing time and dates in JavaScript. Today, we're diving into the complex world of null and undefined values. 

Our special guest for this chapter is none other than Kyle Simpson, an esteemed expert in the field of JavaScript with over 20 years of experience. Kyle will be sharing with us his expert insights and best practices for handling null and undefined values.

Null and undefined values can be a recurring nightmare for developers. Even the slightest misstep can lead to unexpected errors and crashes. It's crucial to understand how to properly handle and manipulate these values to ensure your code is robust and reliable.

In this chapter, we will be covering:

- The differences between null and undefined values
- How to safely check for null and undefined values
- Practical use cases of handling null and undefined values
- Best practices for avoiding common pitfalls with null and undefined values

With Kyle's expert guidance and our comprehensive code examples, you'll be well on your way to mastering this challenging topic. Let's dive in!
# JavaScript Mastery: Conquering Data Structures Algorithms for Technical Programming Interviews

## Chapter 7: How to Handle Null and Undefined Values

Welcome back to JavaScript Mastery! In our last chapter, special guest Kyle Simpson taught us all about managing time and dates in JavaScript. Today, Kyle is back to guide us through the tricky world of null and undefined values.

## The Real Housewives of Code County: Nulls and Undefines

In this episode, our Real Housewives cast is deep in code mode, but they run into a big issue. Tammy is getting an error saying that her variable is undefined, even though she thinks she's defined it. The other housewives jump in to help her out.

**Sue:** Tammy, it sounds like you've got a situation here with undefined values. 

**Tammy:** I know, I just can't figure out where I went wrong. 

**Kyle:** Well Tammy, one important thing to remember is that undefined indicates a variable has been declared, but has not yet been assigned a value. Null, on the other hand, is a value that represents the intentional absence of any object value.

**Jane:** So how do we check if a variable is undefined or null? 

**Kyle:** Great question, Jane! You can use the triple equals operator (**===**) to check a variable against undefined, and the double equals operator (**==**) to check against null. 

**Sue:** And what happens if we try to access a property of an object that is undefined or null? 

**Kyle:** If you try to access a property of an object that is undefined or null, you'll get a TypeError. To avoid this, you can use the optional chaining operator (**?.**) introduced in ES2020.

**Tammy:** Okay, I think I understand. But can you give us some examples of how to handle null and undefined? 

## The Resolution

After Kyle's explanation and code examples, the housewives are ready to tackle null and undefined values like pros.

**Kyle:** Sure thing, Tammy! Here's an example of how to check if a variable is undefined and provide a default value if it is:

```
function testUndefined(myValue) {
  if (myValue === undefined) {
    myValue = 'default value';
  }
  return myValue;
}

console.log(testUndefined()); // 'default value'
```

**Sue:** I see! So if we pass in an undefined value for **myValue**, the function will return the default 'default value' instead.

**Kyle:** Exactly, Sue. And here's an example of using the optional chaining operator to safely access properties of an object:

```
const myObject = {
  property1: {
    subProperty: 'value'
   }
};

console.log(myObject.property1.subProperty); // 'value'
console.log(myObject.property2?.subProperty); // undefined
```

**Jane:** Oh wow, I can see how that could save a lot of headaches when working with nested objects.

**Kyle:** That's right Jane. Always remember to handle null and undefined values with care and caution, and use the proper techniques to avoid errors in your code.

With Kyle's expert guidance and some practice in handling null and undefined values, our Real Housewives cast can now confidently tackle any code issue they come across. Stay tuned for the next episode, where we'll dive into even more challenging topics in JavaScript Mastery!
# JavaScript Mastery: Conquering Data Structures Algorithms for Technical Programming Interviews

## Chapter 7: How to Handle Null and Undefined Values

When working with variables that could potentially be null or undefined, it's important to know how to properly check for and handle these values. In this chapter, special guest Kyle Simpson shared with us his expert insights on how to avoid common pitfalls and write robust code.

### The Code

One common technique for handling undefined values is to check with the strict equality operator (**===**) and provide a default value if the variable is indeed undefined. Here's an example function that demonstrates this technique:

```javascript
function testUndefined(myValue) {
  if (myValue === undefined) {
    myValue = 'default value';
  }
  return myValue;
}

console.log(testUndefined()); // 'default value'
```

In this example, the `testUndefined` function takes in one parameter, `myValue`, and checks if it is strictly equal to undefined. If it is, the function assigns a default value of `'default value'` to `myValue`. The function then returns the value of `myValue`.

Another technique that Kyle introduced is using the optional chaining operator (**?.**) to safely access properties of an object, even if one of the intermediate properties is null or undefined. Here's an example demonstrating this:

```javascript
const myObject = {
  property1: {
    subProperty: 'value'
   }
};

console.log(myObject.property1.subProperty); // 'value'
console.log(myObject.property2?.subProperty); // undefined
```

In this example, we have an object `myObject` with a property `property1` that contains another property `subProperty`. We can safely access `subProperty` by chaining the dot notation to access `property1` and finally `subProperty`. The second `console.log` demonstrates using the optional chaining operator to access a non-existent property `property2` and then `subProperty`. The result of this is `undefined`. 

These are just a couple of examples of how to handle null and undefined values in your code. By following Kyle's expert guidance and practicing proper coding techniques, you can write reliable and robust code that can handle any potential issues with null and undefined values.


[Next Chapter](08_Chapter08.md)