# Java Script

While it is most well-known as the scripting language for Web pages,adds interactivity to your website , in the behavior of responses when buttons are pressed and it was invented by Brendan Eich.

With more experience, we'll be able to create games, animated 2D and 3D graphics

### 1. Assignment Operators

Assignment operators are used to assign values to variables. The most common assignment operator is the equal sign (=). For example, `x = 5` assigns the value 5 to the variable x.

### 2. Arithmetic Operators

Arithmetic operators are used to perform mathematical operations on numeric values. The most common arithmetic operators are addition (+), subtraction (-), multiplication (*), and division (/). For example, `x + y` adds the values of x and y together.

### 3. Comparison Operators

Comparison operators are used to compare values. The most common comparison operators are equal to (==), not equal to (!=), greater than (>), less than (<), greater than or equal to (>=), and less than or equal to (<=). For example, `x > y` returns true if x is greater than y.

### 4. Logical Operators

Logical operators are used to combine multiple conditions. The most common logical operators are and (&&), or (||), and not (!). For example, `x > 5 && y < 10` returns true if x is greater than 5 and y is less than 10.

### 5. String Operators

String operators are used to concatenate strings. The most common string operator is the plus sign (+). For example, `"Hello " + "World"` concatenates the two strings together.

These operators are essential to programming in JavaScript, as they allow developers to manipulate values and control program flow.

JavaScript is a programming language that is used primarily for web development. It is a high-level, dynamic, and interpreted language that is supported by all modern web browsers. JavaScript is used to create interactive web pages, dynamic user interfaces, and responsive mobile applications.

JavaScript can be used for a variety of tasks, including:

JavaScript has two categories of data types: primitive and non-primitive.

**JavaScript Objects**

In JavaScript, an object is a collection of properties, where each property has a name and a value. The value of a property can be a primitive value (such as a number or string) or another object. Objects can also have methods, which are functions that are associated with the object.

Objects in JavaScript are created using object literals, which are enclosed in curly braces `{}`. Here is an example of an object literal:

```
let person = {
  name: "John",
  age: 30,
  address: {
    street: "123 Main St",
    city: "Anytown",
    state: "CA"
  },
  sayHello: function() {
    console.log("Hello, my name is " + this.name);
  }
};

```

In this example, `person` is an object with four properties: `name`, `age`, `address`, and `sayHello`. The `address` property is itself an object with three properties: `street`, `city`, and `state`. The `sayHello` property is a method that logs a message to the console.

Objects can also be created using constructor functions, which are defined using the `function` keyword. Constructor functions are used to create objects with similar properties and methods. Here is an example:

```
function Person(name, age) {
  this.name = name;
  this.age = age;

  this.sayHello = function() {
    console.log("Hello, name is " + this.name);
  }
}

let john = new Person("John", 30);

```

In this example, `Person` is a constructor function that takes two arguments (`name` and `age`) and creates a new object with those properties. The `sayHello` method is defined inside the constructor function and is added to each new object that is created. The `new` keyword is used to create a new object from the `Person` constructor function.

Objects in JavaScript are dynamic, which means that properties can be added or removed from an object at any time. Properties can also be accessed using dot notation (`object.property`) or bracket notation (`object["property"]`). Methods can be called using dot notation and parentheses (`object.method()`).

In summary, objects in JavaScript are collections of properties and methods, and can be created using object literals or constructor functions. Objects are dynamic and can have properties added or removed at any time.

### Primitive Data Types

Primitive data types are the most basic data types in JavaScript. They include:

- **number**: This data type represents numeric values, such as `5` or `3.14`.
- **string**: This data type represents textual values, such as `"Hello"` or `'World'`.
- **boolean**: This data type represents logical values, such as `true` or `false`.
- **undefined**: This data type represents a variable that has not been assigned a value.
- **null**: This data type represents a variable that has been explicitly assigned a value of `null`.
- **symbol**: This data type represents a unique identifier.

**JavaScript classes**

In JavaScript, classes are a way to define objects with similar properties and methods. Classes are a relatively new feature in JavaScript, introduced in ECMAScript 6 (ES6).

A class is defined using the `class` keyword, followed by the name of the class. Here is an example of a class definition:

```
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  sayHello() {
    console.log("Hello, my name is " + this.name);
  }
}

```

In this example, `Person` is a class that has a constructor method and a `sayHello` method. The constructor method is used to create new objects with the `name` and `age` properties. The `sayHello` method is a simple method that logs a message to the console.

To create a new object from a class, the `new` keyword is used, followed by the name of the class and any arguments that are required by the constructor method. Here is an example:

```
let john = new Person("John", 30);

```

In this example, `john` is a new object created from the `Person` class, with the `name` property set to "John" and the `age` property set to .

Classes in JavaScript can also inherit properties and methods from other classes using the `extends` keyword. Here is an example:

```
class Student extends Person {
  constructor(name, age, grade) {
    super(name, age);
    this.grade = grade;
  }

  sayHello() {
    console.log("Hello, my name is " + this.name + " and I am in grade " + this.grade);
  }
}

```

In this example, `Student` is a subclass of `Person` that adds a `grade` property and overrides the `sayHello` method to include the grade.

In summary, classes in JavaScript are a way to define objects with similar properties and methods. Classes are defined using the `class` keyword, and objects are created using the `new` keyword. Classes can also inherit properties and methods from other classes using the `extends` keyword.

**JavaScript Functions**

In JavaScript, functions are a fundamental building block of the language. Functions are used to encapsulate a block of code that can be called and executed at any time. Functions can take arguments (input) and return values (output), making them a powerful tool for creating reusable code.

Functions in JavaScript can be defined in several ways. The most common way is using a function declaration, which uses the `function` keyword followed by the name of the function and a set of parentheses that contain any arguments. Here is an example:

```
function add(a, b) {
  return a + b;
}

```

In this example, `add` is a function that takes two arguments (`a` and `b`) and returns their sum.

Functions can also be defined using function expressions, which are similar to variable declarations. Here is an example:

```
let add = function(a, b) {
  return a + b;
};

```

In this example, `add` is a variable that is assigned a function expression that takes two arguments (`a` and `b`) and returns their sum.

Functions in JavaScript can also be defined using arrow functions, which are a shorthand syntax for function expressions. Here is an example:

```
let add = (a, b) => {
  return a + b;
};

```

In this example, `add` is a variable that is assigned an arrow function that takes two arguments (`a` and `b`) and returns their sum.

Functions in JavaScript can also be used as first-class objects, which means that they can be passed as arguments to other functions, returned as values from functions, and assigned to variables or properties. This makes functions a powerful tool for creating higher-order functions, which are functions that take other functions as arguments or return functions as values.

In summary, functions in JavaScript are a fundamental building block of the language, used to encapsulate a block of code that can be called and executed at any time. Functions can take arguments and return values, making them a powerful tool for creating reusable code. Functions can be defined using function declarations, function expressions, or arrow functions, and can be used as first-class objects.

**JavaScript Arrays**

In JavaScript, arrays are used to store collections of data, such as numbers, strings, or objects. Arrays are a fundamental data structure in JavaScript and are used extensively in programming.

Arrays in JavaScript are defined using square brackets `[]` and can contain any number of elements, separated by commas. Here is an example of an array:

```
let numbers = [1, 2, 3, 4, 5];

```

In this example, `numbers` is an array that contains five elements, each of which is a number.

Arrays in JavaScript are zero-indexed, which means that the first element in the array has an index of 0, the second element has an index of 1, and so on. Elements in an array can be accessed using their index, using square brackets `[]`. Here is an example:

```
let numbers = [1, 2, 3, 4, 5];
console.log(numbers[0]); // Output: 1
console.log(numbers[2]); // Output: 3

```

In this example, the first element in the `numbers` array is accessed using `numbers[0]`, which returns the value `1`. The third element in the `numbers` array is accessed using `numbers[2]`, which returns the value `3`.

Arrays in JavaScript can also be modified by adding or removing elements. Elements can be added to the end of an array using the `push()` method, or to the beginning of an array using the `unshift()` method. Elements can be removed from the end of an array using the `pop()` method, or from the beginning of an array using the `shift()` method. Here is an example:

```
let numbers = [1, 2, 3, 4, 5];
numbers.push(6); // Add 6 to the end of the array
numbers.unshift(0); // Add 0 to the beginning of the array
numbers.pop(); // Remove the last element from the array
numbers.shift(); // Remove the first element from the array

```

In this example, the `push()` method is used to add the value `6` to the end of the `numbers` array, and the `unshift()` method is used to add the value `0` to the beginning of the `numbers` array. The `pop()` method is used to remove the last element from the `numbers` array, and the `shift()` method is used to remove the first element from the `numbers` array.

In summary, arrays in JavaScript are used to store collections of data and are defined using square brackets `[]`. Elements in an array can be accessed using their index, and arrays can be modified by adding or removing elements using methods such as `push()`, `unshift()`, `pop()`, and `shift()`.

### Non-Primitive Data Types

Non-primitive data types are more complex data types in JavaScript. They include:

- **object**: This data type represents a collection of key-value pairs, such as `{name: "John", age: 30}`.
- **array**: This data type represents a collection of values, such as `["apple", "banana", "orange"]`.
- **function**: This data type represents a block of code that can be called by name, such as `function add(x, y) { return x + y }`.

Understanding the differences between these data types is important for effective programming in JavaScript.

JavaScript is a programming language that is used primarily for web development. It is a high-level, dynamic, and interpreted language that is supported by all modern web browsers. JavaScript is used to create interactive web pages, dynamic user interfaces, and responsive mobile applications.

Examples of primitive data types:

```
let num = 5; // number
let str = "Hello World"; // string
let bool = true; // boolean
let undef; // undefined
let n = null; // null
let sym = Symbol("foo"); // symbol

```

Examples of non-primitive data types:

```
let obj = {name: "John", age: 30}; // object
let arr = ["apple", "banana", "orange"]; // array
let add = function(x, y) { return x + y }; // function

```

**JavaScript can be used for a variety of tasks, including:**

1. Client-side scripting

JavaScript is primarily used for client-side scripting, which is the process of creating scripts that run in a user's web browser. These scripts are used to add interactivity and dynamic functionality to web pages, such as validating forms, creating animations, and updating content without requiring a page refresh.

2. Server-side scripting

JavaScript can also be used for server-side scripting, which is the process of creating scripts that run on a web server. Server-side JavaScript is used to create dynamic web applications, such as chat applications, real-time collaboration tools, and social networking sites.

3. Mobile application development

JavaScript can also be used to develop mobile applications for iOS, Android, and other mobile platforms. There are several frameworks and tools available that allow developers to create cross-platform mobile applications using JavaScript, such as React Native and Ionic..

1. Client-side scripting

JavaScript is primarily used for client-side scripting, which is the process of creating scripts that run in a user's web browser. These scripts are used to add interactivity and dynamic functionality to web pages, such as validating forms, creating animations, and updating content without requiring a page refresh.

## 2. Server-side scripting

JavaScript can also be used for server-side scripting, which is the process of creating scripts that run on a web server. Server-side JavaScript is used to create dynamic web applications, such as chat applications, real-time collaboration tools, and social networking sites.

## 3. Mobile application development

JavaScript can also be used to develop mobile applications for iOS, Android, and other mobile platforms. There are several frameworks and tools available that allow developers to create cross-platform mobile applications using JavaScript, such as React Native and Ionic.
