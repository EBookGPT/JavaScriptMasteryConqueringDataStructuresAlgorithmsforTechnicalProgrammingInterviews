# JavaScript Mastery: Conquering Data Structures Algorithms for Technical Programming Interviews

## Chapter 2: Object-Oriented Programming in JavaScript

Darlings, welcome back to our journey of mastering JavaScript for technical programming interviews! We hope you thoroughly enjoyed the previous chapter, "The Fundamentals of JavaScript Programming," where we reviewed the basic concepts and syntax of JavaScript. Now, it's time to kick things up a notch and dive into the exciting world of Object-Oriented Programming in JavaScript.

Object-Oriented Programming, or OOP for short, is a popular programming paradigm that uses the concept of objects to represent real-world entities. With OOP, we can organize our code into reusable and modular components, making it easier to write, debug, and maintain.

In this chapter, we will explore the foundational principles of OOP, such as encapsulation, inheritance, and polymorphism. We will also take a closer look at how JavaScript implements these principles and compare it to other programming languages such as Java and Python.

But wait, there's more! We will also cover some key data structures and algorithms used in OOP, such as linked lists, binary trees, and heaps. These topics are essential for technical programming interviews and will give you a competitive edge in the job market.

So, are you ready to take your JavaScript skills to the next level and become an OOP master? Let's get started!
# JavaScript Mastery: Conquering Data Structures Algorithms for Technical Programming Interviews

## Chapter 2: Object-Oriented Programming in JavaScript

### The Real Housewives of OOP

Welcome back, dear viewers, to another episode of The Real Housewives of OOP! In this episode, we'll dive into the concept of inheritance in Object-Oriented Programming.

Our resident JavaScript expert, Jane, is hosting a dinner party with her fellow housewives. As they sip on their glasses of wine, Jane explains to the group about how inheritance works in JavaScript. 

```javascript
class Animal {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  speak() {
    console.log(`${this.name} makes a noise.`);
  }
}

class Dog extends Animal {
  constructor(name, age, breed) {
    super(name, age);
    this.breed = breed;
  }

  speak() {
    console.log(`${this.name} barks.`);
  }
}

const fido = new Dog('Fido', 2, 'Golden Retriever');
console.log(fido.name); // Output: 'Fido'
fido.speak(); // Output: 'Fido barks.'
```

The other housewives are impressed by how JavaScript implements inheritance using the `extends` keyword and the `super()` function. They can see how this allows for efficient code reuse and easy maintenance.

But wait, drama unfolds as one of the housewives, Karen, pipes up and asks, "What happens if we have a situation where we need to modify a property of the parent class in the child class?"

Jane smiles, knowing this is a common issue in inheritance. She responds, "Ah, that's where polymorphism comes in! In JavaScript, we can use `super` to access the parent class's properties and then modify them in the child class like so:"

```javascript
class Animal {
  constructor(name, age) {
    this.name = name;
    this.age = age;
    this.type = 'animal';
  }

  speak() {
    console.log(`${this.name} makes a noise.`);
  }
}

class Dog extends Animal {
  constructor(name, age, breed) {
    super(name, age);
    this.breed = breed;
    this.type = 'dog';
  }

  speak() {
    console.log(`${this.name} barks.`);
    super.speak();
  }
}

const fido = new Dog('Fido', 2, 'Golden Retriever');
console.log(fido.type); // Output: 'dog'
fido.speak(); // Output: 'Fido barks.' 'Fido makes a noise.'
```

Karen is relieved and impressed with the solution. The other housewives nod their heads in agreement, knowing that polymorphism is a powerful tool that allows for code flexibility.

With this newfound knowledge, the housewives bid farewell to Jane and vow to practice their OOP skills in their own coding endeavors.

### Resolution

Well folks, that's all for this episode of The Real Housewives of OOP! Today, we learned about inheritance and polymorphism in JavaScript, and saw how they can be used to create reusable and modular code.

In the next chapter, we will take a closer look at some common data structures used in OOP, such as linked lists and binary trees. So, stay tuned and keep practicing your skills!
# JavaScript Mastery: Conquering Data Structures Algorithms for Technical Programming Interviews

## Chapter 2: Object-Oriented Programming in JavaScript

### Explanation of the Code

Welcome back, darlings! Let's take a closer look at the code Jane presented to The Real Housewives of OOP.

```javascript
class Animal {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  speak() {
    console.log(`${this.name} makes a noise.`);
  }
}

class Dog extends Animal {
  constructor(name, age, breed) {
    super(name, age);
    this.breed = breed;
  }

  speak() {
    console.log(`${this.name} barks.`);
  }
}

const fido = new Dog('Fido', 2, 'Golden Retriever');
console.log(fido.name); // Output: 'Fido'
fido.speak(); // Output: 'Fido barks.'
```

In this example, Jane creates two classes: `Animal` and `Dog`. `Animal` is the parent class, and `Dog` is the child class that inherits from `Animal` using the `extends` keyword.

The `constructor()` method is what initializes the properties of each class. In the `Animal` class, it takes in a `name` and `age` parameter and assigns them to the class properties `this.name` and `this.age`, respectively.

The `speak()` method is a common method to both classes. It uses interpolation to log out the name of the animal and a message about its noise.

In the `Dog` class, the `constructor()` method takes in an additional `breed` parameter, which is assigned to `this.breed`. The `super()` function is called to pass in the `name` and `age` parameters to the `Animal` class and assign them to their corresponding properties. 

Finally, the `speak()` method in `Dog` overrides the parent `speak()` method by logging out a message about barking.

When we create a new instance of `Dog` named `fido`, we pass in the arguments `'Fido'`, `2`, and `'Golden Retriever'`. `fido.name` outputs `'Fido'` and `fido.speak()` outputs `'Fido barks.'`.

In the second part of the episode, Karen had a question about modifying the parent class's properties in the child class. Jane demonstrated how to achieve this using polymorphism:

```javascript
class Animal {
  constructor(name, age) {
    this.name = name;
    this.age = age;
    this.type = 'animal';
  }

  speak() {
    console.log(`${this.name} makes a noise.`);
  }
}

class Dog extends Animal {
  constructor(name, age, breed) {
    super(name, age);
    this.breed = breed;
    this.type = 'dog';
  }

  speak() {
    console.log(`${this.name} barks.`);
    super.speak();
  }
}

const fido = new Dog('Fido', 2, 'Golden Retriever');
console.log(fido.type); // Output: 'dog'
fido.speak(); // Output: 'Fido barks.' 'Fido makes a noise.'
```

In this updated example, both classes have a `type` property. In the parent `Animal` class, `type` is assigned the value `'animal'`. In the child `Dog` class, `type` is reassigned the value `'dog'`.

In the `speak()` method of `Dog`, it logs out a message about barking and calls `super.speak()` to also log out the parent `speak()` method, which is `"makes a noise."`.

Finally, `fido.type` outputs `'dog'` and `fido.speak()` outputs both `"Fido barks."` and `"Fido makes a noise."`, demonstrating how polymorphism allows for flexible and dynamic code.


[Next Chapter](03_Chapter03.md)