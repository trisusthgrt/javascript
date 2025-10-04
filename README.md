Contents

[What is JavaScript ? 2](#_Toc209523883)

[Applications of JavaScript 2](#_Toc209523884)

[Why Learn JavaScript? 3](#_Toc209523885)

[Execution environment (Browser, Node.js) 3](#_Toc209523886)

[Var vs let vs const 4](#_Toc209523887)

[Data Types 4](#_Toc209523888)

[**Type Conversion & Coercion** (== vs ===) 8](#_Toc209523889)

[JavaScript Operators 9](#_Toc209523890)

[JavaScript Operators: typeof, instanceof, delete, in 13](#_Toc209523891)

[NAN: 16](#_Toc209523892)

[**Comparing objects:** 18](#_Toc209523893)

[JavaScript Comparison & Type Cheat Sheet 20](#_Toc209523894)

[Control flow 25](#_Toc209523895)

[Functions 30](#_Toc209523896)

[Object : 37](#_Toc209523897)

[Array methods: 39](#_Toc209523898)

[Closures & Scope 39](#_Toc209523899)

[What is Hoisting? 45](#_Toc209523900)

[Asynchronous JavaScript 47](#_Toc209523901)

[Event Handling 52](#_Toc209523902)

[ES6+ Features 55](#_Toc209523903)

[Advanced Objects 60](#_Toc209523904)

[JavaScript Internals 66](#_Toc209523905)

[Error Handling 71](#_Toc209523906)

[**Browser APIs** 74](#_Toc209523907)

[JavaScript Patterns 76](#_Toc209523908)

[**JavaScript in Practice** 84](#_Toc209523909)

[Modern Topics (Advanced) 87](#_Toc209523910)

[Interview-Favourite Questions: 90](#_Toc209523911)

JavaScript

### What is JavaScript ?

JavaScript is a programming language used to create dynamic content for websites. It is a lightweight, cross-platform, and single-threaded programming language(Only **one instruction/task runs at a time** in the main thread.). It's an interpreted language that executes code line by line, providing more flexibility**.**

**Client Side:** On the client side, JavaScript works along with HTML and CSS. HTML adds structure to a web page, CSS styles it, and JavaScript brings it to life by allowing users to interact with elements on the page, such as actions on clicking buttons, filling out forms, and showing animations. JavaScript on the client side is directly executed in the user's browser.

**Server Side**: On the Server side (on Web Servers), JavaScript is used to access databases, file handling, and security features to send responses**,** to browsers.

### Applications of JavaScript

JavaScript is a versatile language that powers various applications, from web development to mobile apps, making it an essential tool for modern programming.

*   [**Web Development**](https://www.geeksforgeeks.org/web-tech/web-technology/): JavaScript is widely used in web development to create interactive and dynamic websites. Frameworks like React and Angular make front-end development faster, while Node.js is used for building server-side applications.
*   [**Mobile App Development**](https://www.geeksforgeeks.org/blogs/top-javascript-frameworks-for-mobile-apps-development/): JavaScript helps in developing mobile apps using frameworks like React Native, allowing developers to build cross-platform apps for both iOS and Android.
*   [**Game Development**](https://www.geeksforgeeks.org/blogs/top-javascript-frameworks-libraries-for-building-games/): JavaScript is also used for creating browser-based games with libraries like Phaser, making it easy to develop 2D games that run directly in the browser.
*   [**Server-Side Development**](https://www.geeksforgeeks.org/javascript/javascript-backend-basics/): With Node.js, JavaScript is used for server-side programming, enabling developers to build scalable applications and APIs, especially for real-time features like chat systems.
*   [**Scripting & Automation**](https://www.geeksforgeeks.org/javascript/what-is-scripting/): JavaScript is ideal for automating web-related tasks like form validation and data manipulation, improving efficiency and reducing manual work.
*   [**Web Scraping**](https://www.geeksforgeeks.org/node-js/what-is-web-scraping-in-node-js/): JavaScript, along with libraries like [Puppeteer](https://www.geeksforgeeks.org/node-js/npm-puppeteer/), is used to extract information from websites for data analysis or research, making it useful for web scraping tasks.
*   [**IoT (Internet of Things)**](https://www.geeksforgeeks.org/javascript/javascript-for-iot/): JavaScript is used to control devices and sensors in IoT projects, allowing developers to build smart systems with frameworks like Johnny-Five.

[**Real-Time Applications**](https://www.geeksforgeeks.org/blogs/how-to-implement-real-time-features-in-your-web-app-with-example/): JavaScript powers real-time applications, such as live chats or notifications, using technologies like WebSockets and Socket.io for instant communication between users and servers.

### Why Learn JavaScript?

*   Core language for web development, enabling dynamic and interactive features in websites with fewer lines of code.
*   Highly in demand, offering many job opportunities in Frontend, Backend (Node.js), and Full Stack Development.
*   Supports powerful frameworks and libraries like React, Angular, Vue.js, Node.js, and Express.js, widely used in modern web applications.
*   Object-oriented and event-driven language, ideal for building scalable and responsive applications.
*   Cross-platform and runs directly in all modern web browsers without the need for installation.
*   Major companies like Google, Facebook, and Amazon use JavaScript in their tech stacks.

### Execution environment (Browser, Node.js)

JavaScript can be executed in two primary environments: the browser and Node.js. While both execute JavaScript, their environments and capabilities differ significantly.

Browser Execution Environment:

*   **Purpose:** 

Primarily designed for client-side scripting, enabling interactive and dynamic web experiences within a web browser.

*   **Core Components:** 

Includes the JavaScript engine (e.g., V8 in Chrome, SpiderMonkey in Firefox), the Document Object Model (DOM) for manipulating web page content, and Web APIs (e.g., fetch for network requests, localStorage for client-side storage, setTimeout for timing).

*   **Access:** 

Limited to the browser's sandbox for security reasons, preventing direct access to the user's file system or operating system.

*   **Example Use Cases:** 

Front-end development, manipulating HTML and CSS, handling user interactions, making API calls to servers, building single-page applications.

Node.js Execution Environment:

*   **Purpose:** 

A JavaScript runtime environment that allows executing JavaScript code outside of a web browser, typically for server-side development and command-line tools.

*   **Core Components:** 

Built on the same V8 JavaScript engine as Chrome, but provides different APIs and modules for server-side functionalities (e.g., fs for file system operations, http for creating web servers, path for path manipulation).

*   **Access:** 

Has full access to the underlying operating system and file system, enabling server-side logic, database interactions, and system-level tasks.

*   **Example Use Cases:** 

Building web servers and APIs, creating command-line tools, developing real-time applications (e.g., chat applications), backend services, microservices.

### Var vs let vs const

[https://www.geeksforgeeks.org/javascript/difference-between-var-let-and-const-keywords-in-javascript/](https://www.geeksforgeeks.org/javascript/difference-between-var-let-and-const-keywords-in-javascript/)

### Data Types

JavaScript data types are **divided into two main categories**: **Primitive** and **Non-Primitive** (Reference Types).

**1) Primitive Data Types**

Primitive values are **immutable** (cannot be changed) and are **passed by value**. Each variable stores its **own copy**.

**List of Primitives**

1.  **String**
    *   Textual data.
    *   Enclosed in single quotes ' ', double quotes " ", or backticks \` \` (template literals).
    *   Examples:
    *   let name = "Sushobhan";
    *   let greeting = \`Hello, ${name}!\`;
    *   Features:
        *   Strings are **immutable**.
        *   String methods like toUpperCase() return a new string.
2.  **Number**
    *   Represents integers and floating-point numbers.
    *   JavaScript has **one numeric type** (no int/float distinction).
    *   Examples:
    *   let age = 25;
    *   let pi = 3.14159;
    *   Special numeric values:
        *   Infinity, -Infinity, NaN (Not a Number)
    *   console.log(1 / 0); // Infinity
    *   console.log("a" \* 2); // NaN
3.  **Boolean**
    *   Represents logical values: true or false.
    *   Example:
    *   let isLoggedIn = true;
    *   let hasAccess = false;
4.  **Null**
    *   Represents **intentional absence of any value**.
    *   Type of null is interesting:
    *   let data = null;
    *   console.log(typeof data); // "object" (quirk)
    *   Use when you want to explicitly indicate “no value.”
5.  **Undefined**
    *   Default value of a variable **declared but not assigned**.
    *   Example:
    *   let x;
    *   console.log(x); // undefined
    *   undefined vs null: undefined = not initialized, null = intentionally empty.
6.  **BigInt**
    *   Represents **integers larger than 2^53 - 1** (safe integer limit in JS).
    *   Created by appending n to number or BigInt() function.
    *   Example:
    *   let bigNumber = 123456789012345678901234567890n;
    *   let anotherBig = BigInt("123456789012345678901234567890");
7.  **Symbol**
    *   Represents **unique identifiers**, often used as object keys.
    *   Every symbol is unique, even if descriptions are same.
    *   Example:
    *   const sym1 = Symbol("id");
    *   const sym2 = Symbol("id");
    *   console.log(sym1 === sym2); // false

**2) Non-Primitive (Reference) Data Types**

Reference types store **a reference (memory address) to the actual value**, not the value itself. Changes to the object/array affect all references pointing to it.

**List of Non-Primitives**

1.  **Object**
    *   Collection of key-value pairs.
    *   Can store mixed types.
    *   Example:
    *   let user = {
    *   name: "Sushobhan",
    *   age: 25,
    *   isAdmin: true
    *   };
    *   console.log(user.name); // Sushobhan
    *   Objects are **mutable**.
2.  **Array**
    *   Ordered list of elements.
    *   Elements can be any type (including arrays/objects).
    *   Example:
    *   let numbers = \[1, 2, 3, 4\];
    *   let mixed = \["hello", 42, true, null\];
    *   Arrays are **mutable**:
    *   numbers.push(5); // numbers = \[1,2,3,4,5\]
3.  **Function**
    *   Functions are **first-class objects**.
    *   Can be assigned to variables, passed as arguments, or returned from other functions.
    *   Example:
    *   function greet(name) {
    *   return \`Hello, ${name}!\`;
    *   }
    *   const sayHi = greet;
    *   console.log(sayHi("Sushobhan")); // Hello, Sushobhan!

**3) Key Differences: Primitive vs Non-Primitive**

| Feature | Primitive | Non-Primitive (Reference) |
| --- | --- | --- |
| Storage | Direct value | Reference (pointer) |
| Mutability | Immutable | Mutable |
| Comparison (==/===) | Compared by value | Compared by reference |
| Example | number, string, boolean | object, array, function |
| Copy behavior | Copy value to new var | Copy reference, same object |

**Example to explain in interviews:**

// Primitive

let a = 10;

let b = a;

b = 20;

console.log(a); // 10 (original unchanged)

// Non-primitive

let obj1 = { name: "Alice" };

let obj2 = obj1;

obj2.name = "Bob";

console.log(obj1.name); // Bob (original changed)

**4) Tips / Interview Tricky Points**

1.  typeof null → "object" (historical JS bug)
2.  Arrays are objects: typeof \[\] → "object", but Array.isArray(\[\]) → true
3.  Functions are objects: can have properties
4.  Symbols are unique even with same description
5.  BigInt operations: cannot mix with Number directly:

let x = 1n;

let y = 2;

// x + y → TypeError

### Type Conversion & Coercion (== vs ===)

Type coercion is the implicit, automatic conversion of a value's data type during operations, while type conversion is the general process, which can be either implicit (coercion) or explicit (manual), such as using a function or constructor. In JavaScript, == performs loose equality, which involves type coercion before comparison, whereas === performs strict equality, checking both value and type without coercion.  

Type Conversion (Explicit)

*   **Intentional:** The programmer explicitly instructs the conversion from one data type to another. 
*   **Manual:** Achieved by using built-in functions, constructors, or casting operators. 
*   **Example:** In Python, int("5") converts the string "5" to the integer 5. 

Type Coercion (Implicit)

*   **Automatic:** The conversion happens automatically without explicit instruction from the programmer. 
*   **Context-Driven:** Occurs during mixed-mode operations, like adding a string to a number. 
*   **Example:** In JavaScript, '3' + 6 results in "36" because the number 6 is coerced into a string to be concatenated with the string "3". 

\== vs. === in JavaScript 

*   \== (Loose Equality): 

Compares two values after performing type coercion if they are of different types.

*   *   **Example:** '5' == 5 evaluates to true because the string '5' is coerced to the number 5 for comparison.
*   \=== (Strict Equality): 

Compares two values without performing any type coercion.

*   *   **Example:** '5' === 5 evaluates to false because the string '5' and the number 5 are of different types, even though their values are the same.

### JavaScript Operators

Operators are symbols that perform operations on **operands** (variables or values).

**1) Arithmetic Operators**

Used for numeric calculations.

| Operator | Description | Example | Output |
| --- | --- | --- | --- |
| + | Addition / string concatenation | 5 + 3 / 'Hi' + 'JS' | 8 / 'HiJS' |
| - | Subtraction | 5 - 3 | 2 |
| * | Multiplication | 5 * 3 | 15 |
| / | Division | 6 / 3 | 2 |
| % | Modulus (remainder) | 7 % 3 | 1 |
| ** | Exponentiation | 2 ** 3 | 8 |
| ++ | Increment | let a = 5; a++; | 6 |
| -- | Decrement | let a = 5; a--; | 4 |

**Tricky points / interview highlights:**

*   \+ can **concatenate strings**: '5' + 3 → '53'
*   \-, \*, / auto-convert strings to numbers: '5' - 3 → 2
*   Pre-increment vs post-increment:

let a = 5;

console.log(++a); // 6 (increments before evaluation)

console.log(a++); // 6 (returns then increments)

**2) Comparison Operators**

Compare two values and return a **boolean** (true or false).

| Operator | Description | Example | Output |
| --- | --- | --- | --- |
| == | Equal (type coercion) | '5' == 5 | true |
| === | Strict equal (no type coercion) | '5' === 5 | false |
| != | Not equal (type coercion) | '5' != 6 | true |
| !== | Strict not equal | '5' !== 5 | true |
| > | Greater than | 5 > 3 | true |
| < | Less than | 3 < 5 | true |
| >= | Greater or equal | 5 >= 5 | true |
| <= | Less or equal | 5 <= 3 | false |

**Tricky points / interview highlights:**

*   Always prefer **\=== / !==** to avoid type coercion surprises.
*   '0' == false → true, but '0' === false → false.
*   NaN comparisons: NaN === NaN → false (use Number.isNaN()).

**3) Logical Operators**

Used to combine **boolean expressions**.

| Operator | Description | Example | Output |
| --- | --- | --- | --- |
| && | Logical AND | true && false | false |
| ` |  | ` | Logical OR |
| ! | Logical NOT | !true | false |

**Tricky points / interview highlights:**

*   JavaScript uses **short-circuit evaluation**:

let x = 0;

let y = x || 10; // 10 (x is falsy)

let z = x && 10; // 0 (x is falsy)

*   Non-boolean values are coerced:
    *   0, '', null, undefined, NaN → falsy
    *   Everything else → truthy

**4) Ternary Operator (? :)**

A **shortcut for if-else** statements.

**Syntax:**

condition ? exprIfTrue : exprIfFalse

**Example:**

let age = 18;

let canVote = (age >= 18) ? "Yes" : "No";

console.log(canVote); // "Yes"

**Tricky points / interview highlights:**

*   Can be nested, but readability suffers:

let result = score > 90 ? "A" : score > 75 ? "B" : "C";

*   Returns a value; can assign directly to a variable.

**5) Bitwise Operators**

Operate on numbers at the **binary level**. Usually asked for low-level JS understanding.

| Operator | Description | Example | Binary Explanation |
| --- | --- | --- | --- |
| & | AND | 5 & 3 → 1 | 0101 & 0011 = 0001 |
| ` | ` | OR | `5 |
| ^ | XOR | 5 ^ 3 → 6 | 0101 ^ 0011 = 0110 |
| ~ | NOT | ~5 → -6 | flips bits, two’s complement |
| << | Left shift | 5 << 1 → 10 | 0101 << 1 = 1010 |
| >> | Right shift | 5 >> 1 → 2 | 0101 >> 1 = 0010 |
| >>> | Zero-fill right shift | -5 >>> 1 → 2147483645 | fills with 0 |

**Tricky points / interview highlights:**

*   Bitwise operators convert operands to **32-bit signed integers**.
*   Useful for low-level programming, masks, flags.
*   ~x is equivalent to -(x+1) — commonly asked trick.

**6) Other operator types often mentioned in interviews**

1.  **Assignment Operators**

let a = 10;

a += 5; // a = 15

a -= 3; // a = 12

a \*= 2; // a = 24

1.  **String / Template Literals**

*   \+ can concatenate strings:

let name = "Sushobhan";

let greeting = "Hello " + name;

*   Template literal:

let greeting2 = \`Hello ${name}\`;

1.  **Unary Operators**

*   typeof, void, delete, + (convert to number), - (negate)

typeof 42; // "number"

\+ "42"; // 42 (number)

\- "42"; // -42

**7) Common interview pitfalls / questions**

1.  '5' + 3 → '53' (string concatenation)
2.  '5' - 3 → 2 (type coercion to number)
3.  true + false → 1 (true=1, false=0)
4.  !!value → converts any value to boolean
5.  x = y && z → y falsy? returns y, else returns z

### JavaScript Operators: typeof, instanceof, delete, in

**1) typeof Operator**

**Purpose:** Returns a **string** indicating the type of a variable or value.

**Syntax:**

typeof operand

**Examples:**

typeof 42; // "number"

typeof "hello"; // "string"

typeof true; // "boolean"

typeof undefined; // "undefined"

typeof null; // "object" (quirky JS historical bug)

typeof Symbol(); // "symbol"

typeof 123n; // "bigint"

typeof {}; // "object"

typeof \[\]; // "object" (arrays are objects)

typeof function(){}; // "function"

**Interview tips / quirks:**

*   typeof null === "object" (legacy JS bug).
*   Use Array.isArray() to check arrays, because typeof \[\] === "object".
*   Safe type check for variables that may not exist:

if (typeof someVar !== 'undefined') { ... }

**2) instanceof Operator**

**Purpose:** Checks if an object **is an instance of a particular constructor or class**. Returns true or false.

**Syntax:**

object instanceof Constructor

**Examples:**

const arr = \[1, 2, 3\];

console.log(arr instanceof Array); // true

console.log(arr instanceof Object); // true

console.log(arr instanceof String); // false

function Person(name){ this.name = name; }

const p = new Person("Sushobhan");

console.log(p instanceof Person); // true

console.log(p instanceof Object); // true

**Interview tips / quirks:**

*   Works for **objects and custom classes**, not primitives directly:

5 instanceof Number; // false

new Number(5) instanceof Number; // true

*   Good to use for **type-checking objects**, classes, or custom constructors.

**3) delete Operator**

**Purpose:** Deletes a **property from an object**. Returns true if deletion succeeds or has no effect.

**Syntax:**

delete object.property

delete object\['property'\]

**Examples:**

const obj = { name: "Sushobhan", age: 25 };

delete obj.age;

console.log(obj); // { name: "Sushobhan" }

const arr = \[1, 2, 3\];

delete arr\[1\];

console.log(arr); // \[1, empty, 3\]

**Key points / quirks:**

*   Does **not delete variables declared with var, let, or const**:

var x = 10;

delete x; // false

*   Use delete mainly for **object properties**.
*   For arrays, it leaves a **hole**; splice() is preferred to remove elements.

**4) in Operator**

**Purpose:** Checks whether an **object has a specific property** (own or inherited). Returns true or false.

**Syntax:**

'property' in object

**Examples:**

const obj = { name: "Sushobhan", age: 25 };

console.log('name' in obj); // true

console.log('salary' in obj); // false

// inherited properties

console.log('toString' in obj); // true, inherited from Object.prototype

const arr = \[1, 2, 3\];

console.log(1 in arr); // true (index 1 exists)

console.log(5 in arr); // false

**Key points / quirks:**

*   Checks **both own and inherited properties**.
*   To check **own property only**, use obj.hasOwnProperty('prop').

**5) Quick Summary Table**

| Operator | Purpose / Returns | Example | Output / Notes |
| --- | --- | --- | --- |
| typeof | Returns type as string | typeof 42 | "number" |
| instanceof | Checks if object is instance of constructor | [] instanceof Array | true |
| delete | Deletes a property from an object | delete obj.age | true / property removed |
| in | Checks if property exists in object (own or inherited) | 'name' in obj | true |

**6) Interview-ready points**

*   typeof null → "object" (quirk)
*   typeof \[\] → "object" → use Array.isArray()
*   instanceof works with objects/classes, not primitives directly
*   delete cannot delete variables declared with var, let, const
*   in checks for **own + inherited properties**, unlike hasOwnProperty

### NAN:

**1) What is NaN?**

*   NaN stands for **“Not-a-Number”**.
*   It is a **special numeric value** representing an **invalid number operation**.
*   **Type:** number
*   Examples of producing NaN:

let a = "hello" / 2; // NaN, cannot divide string by number

let b = parseInt("abc"); // NaN, invalid integer conversion

let c = 0 / 0; // NaN, undefined math operation

**2) Type of NaN**

console.log(typeof NaN); // "number"

**Explanation:**

*   NaN is technically a **number value** in JavaScript.
*   Quirk: even though it means “Not a Number”, typeof NaN is "number" because JavaScript’s type system considers it a special numeric value.

**3) Key Characteristics of NaN**

1.  **NaN is unique**: it is the only value in JS that is **not equal to itself**.

console.log(NaN === NaN); // false

console.log(NaN == NaN); // false

*   To check for NaN, use **Number.isNaN()** (ES6):

console.log(Number.isNaN(NaN)); // true

console.log(Number.isNaN("hello")); // false (correct, unlike global isNaN)

*   **isNaN() vs Number.isNaN()**:

isNaN("hello"); // true (global isNaN coerces to number first)

Number.isNaN("hello"); // false (strict check)

1.  **NaN propagates**: any arithmetic operation with NaN results in NaN:

console.log(NaN + 5); // NaN

console.log(NaN \* 10); // NaN

1.  **NaN is part of Number type**:

console.log(Number.NaN); // NaN

**4) Common interview questions / traps**

1.  **Q:** What is typeof NaN?  
    **A:** "number" — because it’s a special numeric value.
2.  **Q:** How to check if a value is NaN?  
    **A:** Use Number.isNaN(value) — safe check without type coercion.
3.  **Q:** Why is NaN === NaN false?  
    **A:** By definition in IEEE-754 (floating point standard), NaN is **not equal to anything**, including itself.
4.  **Q:** Difference between isNaN() and Number.isNaN()?  
    **A:**
    *   isNaN() coerces the value to number first, may give **true for non-number strings**.
    *   Number.isNaN() checks **strictly if the value is the NaN value**.

**5) Examples in practice**

console.log("10" / 2); // 5

console.log("hello" / 2); // NaN

console.log(typeof NaN); // "number"

console.log(NaN === NaN); // false

console.log(Number.isNaN(NaN)); // true

console.log(Number.isNaN("hello")); // false

### Comparing objects:

**1) Comparing objects with ===**

*   **Objects in JavaScript are reference types**.
*   When you do:

const obj1 = { name: "Sushobhan" };

const obj2 = { name: "Sushobhan" };

console.log(obj1 === obj2);

**Output:**

false

**Why:**

*   obj1 and obj2 **store references** to objects in memory.
*   Even if the **contents/properties are identical**, they are **different objects in memory**.
*   \=== checks **reference equality** for objects, not structural equality.

**2) When would === be true?**

const obj1 = { name: "Sushobhan" };

const obj2 = obj1; // same reference

console.log(obj1 === obj2); // true

*   Here, obj2 **points to the same object** as obj1.
*   Any change via obj2 will reflect in obj1 because they share the same reference:

obj2.age = 25;

console.log(obj1.age); // 25

**3) Comparing object contents (deep equality)**

*   \=== **cannot compare contents**.
*   To compare objects by **value**, you can use:

const obj1 = { name: "Sushobhan" };

const obj2 = { name: "Sushobhan" };

// Method 1: JSON.stringify

console.log(JSON.stringify(obj1) === JSON.stringify(obj2)); // true

// Method 2: Deep comparison (lodash)

\_.isEqual(obj1, obj2); // true

**4) Quick interview-ready points**

1.  \=== compares **references for objects**, not their contents.
2.  Two objects with the same properties are **not equal** unless they refer to the **same memory location**.
3.  For primitives (number, string, boolean) === compares **value**.
4.  To check equality of object contents, use **deep comparison**.

**Summary Table:**

| Comparison Type | === Result | Explanation |
| --- | --- | --- |
| Primitives | true if values are same | Values compared directly |
| Objects | true if same reference | References must be identical |
| Arrays | same as objects | References compared, not elements |

**Example:**

let a = 5, b = 5;

console.log(a === b); // true (primitives)

let arr1 = \[1,2\], arr2 = \[1,2\];

console.log(arr1 === arr2); // false (different references)

let arr3 = arr1;

console.log(arr1 === arr3); // true (same reference)

### JavaScript Comparison & Type Cheat Sheet

**1) Primitives vs Reference Types**

| Type | Examples | Equality Behavior | Notes / Quirks |
| --- | --- | --- | --- |
| Number | 5, 3.14, Infinity, NaN | === compares values directly | NaN !== NaN (use Number.isNaN()) |
| String | "abc", 'hello', \hi`` | === compares values directly | Template literals support ${} |
| Boolean | true, false | === compares values directly | — |
| Null | null | Only equal to null (===) | typeof null === "object" (quirk) |
| Undefined | undefined | Only equal to undefined (===) | — |
| BigInt | 123n | === compares numeric value | Cannot mix with Number (1n + 1 → TypeError) |
| Symbol | Symbol("id") | Unique, even with same description | Used as object keys |

**Primitive behavior:** Immutable, stored by value, === compares value.

**2) Reference Types (Objects / Arrays / Functions)**

| Type | Examples | Equality Behavior | Notes / Quirks |
| --- | --- | --- | --- |
| Object | {a:1, b:2} | === compares references only | Deep equality requires JSON or library |
| Array | [1,2,3] | === compares references only | Arrays are objects |
| Function | function(){} | === compares references only | Functions are objects, can have properties |

**Example:**

let obj1 = {name:"A"};

let obj2 = {name:"A"};

console.log(obj1 === obj2); // false

let obj3 = obj1;

console.log(obj1 === obj3); // true

**3) == vs ===**

| Operator | Description | Example | Output |
| --- | --- | --- | --- |
| == | Loose equality (type coercion) | '5' == 5 | true |
| === | Strict equality (no coercion) | '5' === 5 | false |
| != | Loose not equal | '5' != 6 | true |
| !== | Strict not equal | '5' !== 5 | true |

**Interview tip:** Always use === / !== to avoid unexpected type coercion.

**4) Special values comparisons**

| Value | Behavior |
| --- | --- |
| NaN | NaN !== NaN, use Number.isNaN() to check |
| null & undefined | null == undefined → true, null === undefined → false |
| Objects | Different objects with same properties → === false |
| Arrays | [1,2] === [1,2] → false |
| Functions | Different instances → === false |

**Examples:**

console.log(NaN === NaN); // false

console.log(Number.isNaN(NaN)); // true

console.log(null == undefined); // true

console.log(null === undefined); // false

console.log(\[1,2\] === \[1,2\]); // false

**5) typeof Operator**

| Operand | typeof Output |
| --- | --- |
| Number / NaN / Infinity | "number" |
| String | "string" |
| Boolean | "boolean" |
| Null | "object" (quirk) |
| Undefined | "undefined" |
| BigInt | "bigint" |
| Symbol | "symbol" |
| Object | "object" |
| Array | "object" (use Array.isArray()) |
| Function | "function" |

**6) instanceof Operator**

*   Checks if an object is an **instance of a class or constructor**.

\[\] instanceof Array; // true

\[\] instanceof Object; // true

({}) instanceof Object; // true

5 instanceof Number; // false

new Number(5) instanceof Number; // true

**7) in Operator**

*   Checks if **property exists in object** (own + inherited).

const obj = {name:"A"};

'name' in obj; // true

'toString' in obj; // true (inherited)

**8) delete Operator**

*   Deletes **object properties**, cannot delete variables declared with var/let/const.

let obj = {a:1};

delete obj.a; // true

console.log(obj); // {}

*   delete leaves **holes in arrays**, use splice() to remove.

**9) Practical Interview Tips / Gotchas**

1.  **NaN quirks**:
    *   NaN !== NaN, check using Number.isNaN()
2.  **null vs undefined**:
    *   null == undefined → true
    *   null === undefined → false
3.  **Objects & arrays equality**:
    *   Only same reference is equal (===)
4.  **typeof null** → "object"
5.  **Array detection**: Array.isArray(\[\]) → true
6.  **Loose vs strict equality**:
    *   '5' == 5 → true, '5' === 5 → false
7.  **instanceof vs typeof**:
    *   typeof → type string, instanceof → object/class check

**10) Quick Example Table**

| Expression | Result | Explanation |
| --- | --- | --- |
| 5 === 5 | true | primitives, same value |
| '5' == 5 | true | loose equality converts string to number |
| NaN === NaN | false | NaN never equals itself |
| null == undefined | true | loose equality |
| [1,2] === [1,2] | false | different references |
| obj1 = {}; obj2 = obj1; obj1 === obj2 | true | same reference |
| typeof null | "object" | JS historical bug |
| Array.isArray([]) | true | check array |
| [] instanceof Array | true | array is instance of Array |

### Control flow

Control flow is the order in which a program executes its instructions. By default, this is a linear top-to-bottom sequence, but control flow statements, including conditionals, loops, and exception handlers, alter this sequence to create dynamic and responsive programs. 

**Conditional statements: if, else, and switch**

These statements execute different blocks of code based on whether a condition is true or false. 

**if statement**

The if statement is the most basic conditional. The code block inside the if statement runs only if its condition evaluates to true. 

javascript

const age = 20;

if (age >= 18) {

console.log("You are an adult.");

}

Use code with caution.

**if...else statement**

The if...else statement provides a fallback option. If the if condition is false, the code block inside the else statement is executed. 

javascript

const age = 16;

if (age >= 18) {

console.log("You are an adult.");

} else {

console.log("You are a minor.");

}

Use code with caution.

**if...else if...else statement**

You can chain multiple if statements together to test multiple conditions in order. The first condition that evaluates to true will execute its block, and subsequent else if and else blocks will be ignored. 

javascript

const temperature = 25;

if (temperature > 30) {

console.log("It's hot.");

} else if (temperature >= 20) {

console.log("It's warm.");

} else {

console.log("It's cold.");

}

Use code with caution.

**switch statement**

The switch statement evaluates a single expression and compares its value to multiple potential case values. It is often more readable than a long chain of if...else if statements. 

*   The break keyword is essential for preventing "fall-through," where code continues to execute into the next case.
*   The default keyword specifies code to run if no other case matches. 

javascript

const day = "Wednesday";

switch (day) {

case "Monday":

console.log("Start of the week.");

break;

case "Friday":

console.log("End of the workweek.");

break;

default:

console.log("It's a regular day.");

break;

}

Use code with caution.

**Loops: for, while, do-while, for...in, for...of**

Loops repeat a block of code until a certain condition is met. 

**for loop**

The for loop is used when you know in advance how many times you want to iterate. Its structure includes an initialization, a condition, and a final expression. 

javascript

for (let i = 0; i < 3; i++) {

console.log(\`Loop iteration ${i}\`);

}

Use code with caution.

**while loop**

A while loop executes a block of code as long as its condition remains true. The condition is checked _before_ each iteration. 

javascript

let count = 0;

while (count < 3) {

console.log(\`Count is ${count}\`);

count++;

}

Use code with caution.

**do-while loop**

The do-while loop is similar to the while loop, but it guarantees the code block will execute at least once before checking the condition. 

javascript

let count = 5;

do {

console.log(\`Count is ${count}\`);

count++;

} while (count < 3); _// This will still run once, printing "Count is 5"._

Use code with caution.

**for...in loop**

This loop iterates over the _enumerable properties_ of an object. It is useful for iterating through object keys. 

javascript

const person = { name: "Alice", age: 30 };

for (const key in person) {

console.log(\`${key}: ${person\[key\]}\`);

}

Use code with caution.

**for...of loop**

This loop iterates over the _values_ of an iterable object, such as an array, map, or string. 

javascript

const colors = \["red", "green", "blue"\];

for (const color of colors) {

console.log(color);

}

Use code with caution.

**break vs. continue**

These are jump statements used to alter the flow of a loop. 

**break**

*   **Purpose:** The break statement terminates the entire loop immediately and transfers control to the statement following the loop.
*   **Use case:** Useful for exiting a loop prematurely when a specific condition is met, such as finding a target item in a search. 

javascript

for (let i = 0; i < 5; i++) {

if (i === 3) {

break; _// Stops the loop completely._

}

console.log(i); _// Prints 0, 1, 2._

}

Use code with caution.

**continue**

*   **Purpose:** The continue statement skips the rest of the code in the _current iteration_ and jumps to the next iteration of the loop.
*   **Use case:** Useful for skipping certain values or conditions and continuing the loop, such as processing every item in a list except for a few. 

javascript

for (let i = 0; i < 5; i++) {

if (i === 3) {

continue; _// Skips printing 3._

}

console.log(i); _// Prints 0, 1, 2, 4._

}

Use code with caution.

**try...catch...finally**

This construct is used for exception handling, allowing you to manage runtime errors and prevent your program from crashing. 

**try block**

The try block contains the code that you want to monitor for errors. If an exception (error) occurs, the code execution immediately stops and moves to the catch block. 

**catch block**

The catch block is executed only if an error occurs in the try block. It receives the error object, which can be used to get information about the exception, such as the error message. 

**finally block**

The finally block is optional, but if present, its code is **always** executed, regardless of whether an exception was thrown or not. It is typically used for cleanup tasks, such as closing files or database connections. 

javascript

try {

_// Code that may cause an error_

let result = someUndefinedVariable + 1;

} catch (error) {

_// This code runs if there is an error_

console.error("An error occurred:", error.message);

} finally {

_// This code always runs_

console.log("Execution finished.");

}

### Functions

**Function declaration vs. expression**

| Feature | Function Declaration | Function Expression |
| --- | --- | --- |
| Hoisting | Hoisted to the top of their scope, so you can call them before they are defined in the code. | Not hoisted. You must define a function expression before you call it; otherwise, it will throw an error. |
| Syntax | Starts with the function keyword, followed by the function name, parentheses for parameters, and curly braces for the body.function greet(name) { return 'Hello, ' + name; } | Created as part of an expression and is often anonymous (without a name). It can be assigned to a variable.const greet = function(name) { return 'Hello, ' + name; }; |
| Use Case | Ideal for general-purpose functions that are widely used in a program. It's often the preferred method for declaring functions for readability. | Better for creating functions that are only needed once, such as callbacks for event listeners or within an Immediately Invoked Function Expression (IIFE). |
| Debugging | The function name is useful for stack traces when debugging. | Anonymous functions may have less informative stack traces, though modern browsers often infer the function's name from the variable it's assigned to. |

**Arrow functions**

Introduced in ES6, arrow functions provide a shorter syntax for writing function expressions and have a different behavior for the this keyword. 

*   **Concise syntax:** The syntax (param1, param2) => { ... } is more compact than a traditional function expression. For single-parameter functions, the parentheses can be omitted, e.g., param => { ... }. For single-line functions that implicitly return a value, you can omit the curly braces and return keyword, e.g., (a, b) => a + b.
*   **No this binding:** Unlike regular functions, arrow functions do not have their own this value. Instead, this is lexically bound, meaning it inherits the this value from the enclosing scope where the function was defined.
*   **Cannot be constructors:** Arrow functions cannot be used with the new keyword to create new objects.
*   **No arguments object:** Arrow functions do not have their own arguments object, but you can access the arguments of the surrounding function. 

**Default parameters**

Default parameters allow you to initialize a parameter with a default value if no value or undefined is passed in for that argument. This simplifies function definitions and avoids repetitive manual checks for missing arguments. 

javascript

function greet(name = 'Guest') {

console.log(\`Hello, ${name}!\`);

}

greet('Alice'); _// Output: Hello, Alice!_

greet(); _// Output: Hello, Guest!_

Use code with caution.

**Rest & spread operators**

The rest and spread operators both use the three-dot syntax (...), but they have opposite functions. 

| Feature | Rest Operator (...) | Spread Operator (...) |
| --- | --- | --- |
| Purpose | Gathers multiple arguments into a single array. Used in function parameter lists and destructuring assignments. | Expands an iterable (like an array, string, or object) into individual elements. |
| Use Case | Gathering function arguments: Used to accept an indefinite number of arguments into a function.function sum(...numbers) { return numbers.reduce((acc, num) => acc + num, 0); } | Combining arrays: Merges elements from multiple arrays.const combined = [...arr1, ...arr2];Cloning arrays/objects: Creates a shallow copy.const clone = [...original];Passing arguments: Spreads an array's elements as individual arguments into a function call.Math.max(...numbers); |
| Context | Appears in a function's parameter list or during destructuring. | Appears in array literals, object literals, and function calls. |

**Higher-order functions**

A higher-order function is a function that either takes one or more functions as arguments or returns a function as its result. They are a cornerstone of functional programming in JavaScript. 

**Examples of built-in higher-order functions:**

*   **Array.prototype.map():** Takes a callback function and returns a new array with the results of calling the function on every element.
*   **Array.prototype.filter():** Takes a callback function and returns a new array containing only the elements for which the callback returns true.
*   **Array.prototype.reduce():** Takes a reducer function and returns a single value by executing the function on each element of the array. 

**Example of a custom higher-order function:**

javascript

function operateOnNumbers(operation) {

return (a, b) => operation(a, b);

}

const add = operateOnNumbers((x, y) => x + y);

console.log(add(5, 3)); _// 8_

Use code with caution.

**IIFE (Immediately Invoked Function Expression)**

An IIFE is a function that runs as soon as it is defined. Its primary purpose is to create a private scope for variables to prevent them from polluting the global namespace. 

javascript

(function() {

const message = "This variable is private.";

console.log(message);

})(); _// The function is immediately invoked_

_// console.log(message); // This would result in a ReferenceError_

Use code with caution.

**this keyword behavior**

The value of this is not fixed and depends on how a function is called, also known as its "call-site". 

**Global context**

*   **Non-strict mode:** When this is used in the global scope (outside of any function), it refers to the global object. In a web browser, this is the window object.
*   **Strict mode:** In strict mode, this in the global context is undefined. 

**Object methods**

When a function is called as a method of an object (e.g., obj.method()), this refers to the object itself. 

javascript

const person = {

name: 'John',

greet() {

console.log(\`Hello, my name is ${this.name}.\`);

}

};

person.greet(); _// \`this\` refers to \`person\`, outputting: "Hello, my name is John."_

Use code with caution.

**Arrow functions**

Arrow functions do not have their own this binding. They inherit the this value from their enclosing lexical (parent) scope at the time they are defined. This makes them useful for callbacks inside object methods, where the this context needs to be preserved. 

javascript

const person = {

name: 'John',

greet() {

_// \`this\` here refers to \`person\`_

setTimeout(() => {

_// \`this\` in the arrow function is inherited from \`greet()\`_

console.log(\`Hello, my name is ${this.name}.\`);

}, 100);

}

};

person.greet(); _// \`this\` refers to \`person\`, outputting: "Hello, my name is John."_

Use code with caution.

**Classes**

Inside a class, the this keyword behaves predictably.

*   **Constructor:** Inside a class constructor, this refers to the new instance of the class being created.
*   **Methods:** For a regular class method, this refers to the instance of the class.
*   **Method binding:** A common pitfall is that when you pass a class method as a callback, its this context is lost. To fix this, you can bind the method to the instance in the constructor. 

javascript

class Player {

constructor(name) {

this.name = name;

}

_// Regular method_

sayName() {

console.log(this.name);

}

_// Arrow function method (lexically bound)_

sayNameArrow = () => {

console.log(this.name);

}

}

const player1 = new Player('Alice');

const sayNameCallback = player1.sayName;

player1.sayName(); _// Outputs: Alice_

sayNameCallback(); _// Outputs: undefined (lost \`this\` context)_

player1.sayNameArrow(); _// Outputs: Alice (\`this\` is preserved)_

first class function in javascript

In JavaScript, a 

**first-class function** is one that is treated like any other variable or value. This means functions are "first-class citizens," and you can do anything with a function that you can do with other data types like strings or numbers. 

**What you can do with first-class functions**

1.  **Assign to a variable**: You can assign a function (including an anonymous function) to a variable. The variable then holds the function's definition and can be used to invoke it.

javascript

const sayHi = function() {

console.log("Hi there!");

};

sayHi(); _// Outputs: Hi there!_

Use code with caution.

1.  **Pass as an argument**: A function can be passed as an argument to another function. The function being passed is often called a "callback" function. This is the basis for many common JavaScript patterns, such as event listeners and array methods.

javascript

function logMessage(messageFunction) {

console.log(messageFunction());

}

const createGreeting = () => "Hello!";

logMessage(createGreeting); _// Pass \`createGreeting\` as a callback_

_// Outputs: Hello!_

Use code with caution.

1.  **Return from another function**: A function can return another function as its result. This is a core concept that enables higher-order functions and closures.

javascript

function createMultiplier(multiplier) {

return function(number) {

return number \* multiplier;

};

}

const double = createMultiplier(2);

console.log(double(5)); _// The returned function is invoked_

_// Outputs: 10_

Use code with caution.

1.  **Store in data structures**: You can store functions inside other data structures, such as arrays or objects, allowing for dynamic and flexible management of functionality.

javascript

const operations = {

add: (a, b) => a + b,

subtract: (a, b) => a - b

};

console.log(operations.add(10, 5)); _// Access the function from the object_

_// Outputs: 15_

Use code with caution.

**First-class functions vs. higher-order functions**

It's important to distinguish between first-class functions and higher-order functions. 

*   **First-class function**: A characteristic of a language where functions are treated like values. **In JavaScript, all functions are first-class functions**.
*   **Higher-order function**: A specific type of function that either takes one or more functions as arguments or returns a function as its result. 

The ability of a language to have first-class functions is what makes it possible to create higher-order functions. For example, Array.prototype.map() is a higher-order function because it accepts another function as an argument, and this is only possible because JavaScript's functions are first-class. 

### Object :

**Object creation**

**Object literals**

This is the simplest and most common way to create an object. It involves defining key-value pairs inside curly braces {}. 

javascript

const person = {

name: 'John',

age: 30,

greet() {

console.log(\`Hello, my name is ${this.name}\`);

}

};

Use code with caution.

**new Object()**

This is a more verbose and less common way to create a generic object. 

javascript

const person = new Object();

person.name = 'John';

person.age = 30;

person.greet = function() {

console.log(\`Hello, my name is ${this.name}\`);

};

Use code with caution.

**Object.create(prototype)**

This method creates a new object using an existing object as its prototype. It provides more control over the prototype chain and allows for prototypal inheritance. 

javascript

const carPrototype = {

drive() {

console.log('Vroom!');

}

};

const myCar = Object.create(carPrototype);

myCar.make = 'Honda';

myCar.drive(); _// 'Vroom!'_

### Array methods:

[https://www.geeksforgeeks.org/javascript/what-are-the-important-array-methods-of-javascript/](https://www.geeksforgeeks.org/javascript/what-are-the-important-array-methods-of-javascript/)

### Closures & Scope

**Closures & Scope in JavaScript**

**Scope: The accessibility of variables**

In JavaScript, scope determines where variables are accessible. 

*   **Global scope:** Variables declared outside of any function or block are in the global scope. They can be accessed from anywhere in the code.
*   **Function (local) scope:** Variables declared with var inside a function are local to that function. They are not accessible from outside the function.
*   **Block scope:** Introduced with ES6, variables declared with let and const within a block of code (e.g., inside an if statement or for loop) are only accessible within that block. 

**Lexical scope**

Lexical scope, also known as static scope, means that the scope of a variable is determined at the time of its creation in the source code. In simpler terms, a function's scope is determined by where it is written, not where it is called. 

Example:

javascript

let globalVar = "I am global";

function outerFunction() {

let outerVar = "I am outer";

function innerFunction() {

let innerVar = "I am inner";

console.log(globalVar); _// Accessible (Global Scope)_

console.log(outerVar); _// Accessible (Outer Function Scope)_

console.log(innerVar); _// Accessible (Own Scope)_

}

innerFunction();

}

outerFunction();

Use code with caution.

In this example, innerFunction has access to its own variables, plus those from its parent (outerFunction) and the global scope. 

**Closures**

**Definition of a closure**

A closure is the combination of a function bundled together with references to its surrounding state (the lexical environment). In other words, a closure allows an inner function to access the variables and parameters of an outer function, even after the outer function has finished executing. 

Example:

javascript

function createCounter() {

let count = 0; _// The 'count' variable is part of the closure_

return function() {

count++;

console.log(count);

};

}

const myCounter = createCounter(); _// The outer function has finished running._

myCounter(); _// 1_

myCounter(); _// 2_

myCounter(); _// 3_

Use code with caution.

In this example, myCounter is a function returned by createCounter. Even though createCounter has finished, the returned function "remembers" the count variable from its parent's lexical scope. 

**Use cases for closures**

*   **Encapsulation and private variables:** Closures can create private variables and methods that are not directly accessible from outside the function, hiding the internal state of an object.

javascript

function createBankAccount(initialBalance) {

let balance = initialBalance; _// Private variable_

return {

deposit: function(amount) {

balance += amount;

},

getBalance: function() {

return balance;

}

};

}

const account = createBankAccount(100);

account.deposit(50);

console.log(account.getBalance()); _// 150_

console.log(account.balance); _// undefined (cannot access private variable)_

Use code with caution.

*   **Memoization:** Closures can be used to cache the results of expensive function calls to avoid recomputing them.

javascript

function memoizedAddition() {

const cache = {};

return function(n) {

if (n in cache) {

console.log('Fetching from cache...');

return cache\[n\];

} else {

console.log('Calculating result...');

const result = n + 10;

cache\[n\] = result;

return result;

}

};

}

const add = memoizedAddition();

add(5); _// Calculates result... returns 15_

add(5); _// Fetches from cache... returns 15_

Use code with caution.

*   **Event handling:** Closures are frequently used in event handlers to maintain a reference to a specific piece of data.

javascript

function createButtonHandler(id) {

return function() {

console.log(\`Button with ID ${id} was clicked.\`);

};

}

const button1 = createButtonHandler('btn-1');

const button2 = createButtonHandler('btn-2');

_// Attach event listeners..._

_// button1() -> logs "Button with ID btn-1 was clicked."_

_// button2() -> logs "Button with ID btn-2 was clicked."_

Use code with caution.

**Practical closure questions in JS**

**Question 1: What will be the output of the following code?**

javascript

function buildFunctions() {

var arr = \[\];

for (var i = 0; i < 3; i++) {

arr.push(function() {

console.log(i);

});

}

return arr;

}

var fs = buildFunctions();

fs\[0\]();

fs\[1\]();

fs\[2\]();

Use code with caution.

**Answer:** The output will be 3, 3, 3. This is because the var keyword is function-scoped, not block-scoped. All three functions in the array share the same i from the outer for loop. By the time the functions are executed, the loop has already completed, and i has a final value of 3. 

**Question 2: How would you fix the previous example to get the expected output (0, 1, 2)?**

javascript

_// Using a closure inside the loop_

function buildFunctionsWithClosure() {

var arr = \[\];

for (var i = 0; i < 3; i++) {

(function(j) {

arr.push(function() {

console.log(j);

});

})(i);

}

return arr;

}

_// Or using 'let' which is block-scoped_

function buildFunctionsWithLet() {

var arr = \[\];

for (let i = 0; i < 3; i++) {

arr.push(function() {

console.log(i);

});

}

return arr;

}

var fs2 = buildFunctionsWithClosure();

fs2\[0\](); _// 0_

fs2\[1\](); _// 1_

fs2\[2\](); _// 2_

var fs3 = buildFunctionsWithLet();

fs3\[0\](); _// 0_

fs3\[1\](); _// 1_

fs3\[2\](); _// 2_

### What is Hoisting?

Hoisting is JavaScript’s behavior of **moving declarations to the top of their scope (global/function/block)** during the compile phase.  
👉 But only the **declaration** is hoisted, not the initialization.

**1\. Variable Hoisting**

**a) var hoisting**

*   **Declarations are hoisted, initialized with undefined.**
*   They become available throughout the entire function/global scope even before their declaration.

console.log(a); // undefined (not error, because 'a' is hoisted)

var a = 10;

console.log(a); // 10

Internally, JS treats it like:

var a; // declaration hoisted

console.log(a); // undefined

a = 10; // initialization remains in place

console.log(a); // 10

➡️ var is **function-scoped**, not block-scoped.

**b) let and const hoisting**

*   **Declarations are hoisted, but not initialized.**
*   They are in a **Temporal Dead Zone (TDZ)** from the start of the block until their declaration is executed.
*   Accessing them before declaration → **ReferenceError**.

console.log(b); // ❌ ReferenceError (TDZ)

let b = 20;

console.log(c); // ❌ ReferenceError (TDZ)

const c = 30;

Key differences:

*   var → hoisted & initialized to undefined.
*   let/const → hoisted but stay in TDZ until declared.
*   const must also be initialized at the time of declaration.

**2\. Function Hoisting**

**a) Function Declarations**

*   Fully hoisted (both name & body).
*   Can call the function **before its definition**.

greet(); // ✅ "Hello!"

function greet() {

console.log("Hello!");

}

Internally:

function greet() { console.log("Hello!"); }

greet();

**b) Function Expressions**

*   **Only the variable name is hoisted, not the function assignment.**
*   Acts like variables (var, let, const).

sayHi(); // ❌ TypeError (if var), or ReferenceError (if let/const)

var sayHi = function () {

console.log("Hi!");

};

Why?

*   var sayHi is hoisted → initialized as undefined.
*   At call time, sayHi is undefined (not callable).
*   If let/const used → ReferenceError due to TDZ.

### Asynchronous JavaScript

**Asynchronous JavaScript** allows certain operations to be performed without blocking the main execution thread. Instead of waiting for a long-running task (like a network request or a timer) to finish, the JavaScript engine can continue with other code. This is managed by the **event loop**. 

**Callbacks (Callback Hell)**

*   **What they are:** Functions passed as arguments to another function, which are then executed when the task is complete. Asynchronous callbacks are handled by external environments like the browser or Node.js through Web APIs.
*   **Callback Hell:** A situation where multiple nested callbacks are required for sequential asynchronous operations, resulting in code that is difficult to read, maintain, and debug. The deeply indented code resembles a "pyramid of doom". 

**Example of Callback Hell:**

javascript

getData(function(data) {

processData(data, function(processedData) {

updateUI(processedData, function() {

console.log('Update finished!');

});

});

});

Use code with caution.

**Modern asynchronous patterns: Promises and async/await**

**Promises**

A Promise is a JavaScript object that represents the eventual completion (or failure) of an asynchronous operation and its resulting value. 

*   **States:** A promise can be in one of three states:
    *   **pending**: The initial state. The operation has not yet completed.
    *   **fulfilled**: The operation completed successfully.
    *   **rejected**: The operation failed.
*   **Handling promises:** The .then(), .catch(), and .finally() methods are used to "consume" a promise.
    *   **.then(onFulfilled, onRejected)**: Registers callbacks to receive the promise's resolved value or rejection reason. It returns a new promise, enabling **promise chaining**.
    *   **.catch(onRejected)**: A shorthand for .then(null, onRejected) used specifically for handling rejections.
    *   **.finally(onFinally)**: Registers a callback that is invoked when the promise is settled (either fulfilled or rejected). It's useful for cleanup tasks. 

**Example of Promise Chaining:**

javascript

fetch('https://api.example.com/data')

.then(response => response.json())

.then(data => {

console.log('Data fetched:', data);

})

.catch(error => {

console.error('Failed to fetch data:', error);

})

.finally(() => {

console.log('Fetch request completed.');

});

Use code with caution.

**async/await**

Introduced in ES2017, async/await is syntactic sugar built on top of promises that provides a cleaner, more readable way to handle asynchronous code. 

*   **async keyword**: Preceded by async, a function will always return a promise. Any non-promise value is automatically wrapped in a resolved promise.
*   **await keyword**: Pauses the execution of an async function until a promise is settled (resolved or rejected). The resolved value is then returned, or the rejected error is thrown.
*   **Error handling**: In async/await, errors are handled with standard try...catch blocks. 

**Example of async/await:**

javascript

async function fetchData() {

try {

const response = await fetch('https://api.example.com/data');

const data = await response.json();

console.log('Data fetched:', data);

} catch (error) {

console.error('Failed to fetch data:', error);

} finally {

console.log('Request completed.');

}

}

fetchData();

Use code with caution.

**Promise concurrency methods**

These static methods on the Promise object allow managing multiple asynchronous tasks concurrently. 

| Method | Behavior | Use Case |
| --- | --- | --- |
| Promise.all(iterable) | Resolves when all promises resolve, rejects if any reject. | All operations must succeed. |
| Promise.race(iterable) | Settles (resolves or rejects) with the first promise that settles. | Get the fastest result. |
| Promise.any(iterable) | Resolves with the first promise that resolves, rejects only if all reject. | Get the first successful result. |
| Promise.allSettled(iterable) | Resolves when all promises settle, regardless of outcome. | Get results for all operations. |

**Event Loop**

**The JavaScript event loop is a crucial mechanism that allows a single-threaded language like JavaScript to perform non-blocking, asynchronous operations. This prevents time-consuming tasks, like fetching data from a server, from freezing the entire application, ensuring a responsive user experience.** 

**The event loop is a continuous cycle that monitors two key components: the call stack and the task queues.** 

**Event loop components**

*   **Call stack: This is where JavaScript tracks the execution of synchronous function calls. It follows a "Last-In, First-Out" (LIFO) principle, meaning the most recently added function is the first to be executed and removed. If the stack is busy with a long-running function, it's considered "blocked," and nothing else can execute.**
*   **Web APIs: Provided by the browser (or the runtime environment like Node.js), these are not part of the JavaScript engine itself. Web APIs handle asynchronous tasks, such as setTimeout(), fetch(), and DOM events, in the background. Once the task is complete, the associated callback function is placed into the appropriate task queue.**
*   **Task Queues: These are data structures that hold the callbacks for asynchronous operations, waiting to be moved to the call stack. There are two types:**
    *   **Macrotask Queue (or Callback Queue): Holds callbacks from tasks like setTimeout(), setInterval(), and DOM events. The event loop processes these one at a time.**
    *   **Microtask Queue: Has a higher priority than the macrotask queue. It holds callbacks from promises (.then(), .catch(), .finally()) and the queueMicrotask() API. The event loop processes all microtasks in the queue until it is empty before it handles the next macrotask.** 

**The event loop cycle**

1.  **Run synchronous code: When a script first runs, all synchronous code is executed and managed by the call stack.**
2.  **Offload asynchronous tasks: When an asynchronous function like setTimeout() or fetch() is encountered, it is passed to the relevant Web API. The browser or Node.js starts the operation in the background while the JavaScript engine continues executing synchronous code.**
3.  **Queue callbacks: When an asynchronous operation completes, its callback function is placed into either the macrotask or microtask queue, depending on the type of task.**
4.  **Process queues: The event loop continuously checks if the call stack is empty.**
5.  **Prioritize microtasks: If the call stack is empty, the event loop empties the entire microtask queue before it moves on.**
6.  **Handle macrotasks: After the microtask queue is clear, the event loop takes the first callback from the macrotask queue and pushes it onto the call stack for execution.**
7.  **Repeat: This process repeats. The call stack empties, the microtask queue is checked again, then a single task from the macrotask queue is run.** 

**Example: The event loop in action**

**Consider the following code snippet:**

**javascript**

**console.log('Start');**

**setTimeout(() => {**

**console.log('Timeout');**

**}, 0);**

**Promise.resolve().then(() => {**

**console.log('Promise');**

**});**

**console.log('End');**

**Use code with caution.**

**Here is the step-by-step execution:**

1.  **console.log('Start') is pushed to the call stack, executed, and popped off.**
2.  **setTimeout() is pushed to the call stack. The Web API starts a timer in the background, and the callback is added to the macrotask queue after 0ms. setTimeout() is popped off the stack.**
3.  **Promise.resolve().then() is pushed to the call stack. The .then() callback is placed in the microtask queue. The promise is popped off the stack.**
4.  **console.log('End') is pushed to the call stack, executed, and popped off.**
5.  **The call stack is now empty. The event loop checks the microtask queue first, finds the Promise callback, moves it to the call stack, and executes it. Promise is logged.**
6.  **The microtask queue is now empty. The event loop moves to the macrotask queue, finds the setTimeout callback, moves it to the call stack, and executes it. Timeout is logged.** 

**The final output is:**

**Start**

**End**

**Promise**

**Timeout**

**This example clearly demonstrates the priority given to the microtask queue over the macrotask queue.**

**Browser vs. Node.js event loops**

**While the core principles are the same, there are differences in implementation between browser and Node.js environments.** 

*   **Browser: The event loop prioritizes UI responsiveness. After processing microtasks, it handles a single macrotask before possibly updating the UI and starting the next cycle.**
*   **Node.js: The event loop has a more complex, six-phase model optimized for server-side I/O operations. It also includes additional microtask callbacks like process.nextTick(), which has a special, high-priority placement in the execution order.** 

**setTimeout, setInterval, clearTimeout, clearInterval**

These functions are used for scheduling function execution. 

*   **setTimeout(callback, delay)**: Executes a function once after a delay.
*   **setInterval(callback, delay)**: Executes a function repeatedly at intervals.
*   **clearTimeout(timeoutId)**: Cancels a setTimeout timer.
*   **clearInterval(intervalId)**: Cancels an setInterval timer. 

Note that setTimeout with a 0 delay doesn't run immediately but is queued after the call stack and microtasks are clear. 

### Event Handling

The core of event handling in the DOM involves detecting user interactions or browser events and running a JavaScript function in response. The browser processes events through a defined flow, and developers can control this process using methods like onclick, addEventListener, preventDefault, and stopPropagation. 

**onclick vs. addEventListener**

| Feature | onclick | addEventListener |
| --- | --- | --- |
| Method | Assigns a function to an element's onclick property. | Attaches an event listener method to an element. |
| Multiple Handlers | Only one onclick handler can be assigned per element per event type. A new assignment will overwrite the old one. | You can add multiple event handlers for the same event type on a single element. All will execute when the event fires. |
| Syntax | element.onclick = function() { ... } or directly in HTML: <button onclick="myFunction()">. | element.addEventListener('click', function() { ... }). |
| Event Flow | Only registers handlers during the event's bubbling phase. | Allows control over the event's phase (capturing or bubbling) via an optional third argument. |
| Recommendation | Not recommended for modern development due to its limitations, especially for complex applications. | The modern, flexible, and recommended approach for handling events. |

**Event bubbling and capturing**

Event propagation is the mechanism that defines the order in which an event is handled when nested elements have event listeners. The process consists of three phases: 

1.  **Capturing Phase:** The event travels from the window down through the DOM hierarchy to the target element. Listeners set to the capturing phase (capture: true) are executed during this descent.
2.  **Target Phase:** The event reaches its destination element and any listeners on the target itself are triggered.
3.  **Bubbling Phase:** By default, events "bubble" up from the target element back up to the window. Most event listeners, including onclick and addEventListener without the capture option, are executed during this phase. 

javascript

_// Example of capturing and bubbling_

const grandparent = document.getElementById('grandparent');

const parent = document.getElementById('parent');

const child = document.getElementById('child');

_// Capturing phase listener_

grandparent.addEventListener('click', () => {

console.log('Grandparent (Capturing)');

}, { capture: true });

_// Bubbling phase listener (default)_

parent.addEventListener('click', () => {

console.log('Parent (Bubbling)');

});

_// Event target listener_

child.addEventListener('click', () => {

console.log('Child (Target)');

});

_// If you click the 'child' element, the console output will be:_

_// Grandparent (Capturing)_

_// Child (Target)_

_// Parent (Bubbling)_

Use code with caution.

**Event delegation**

Event delegation is a powerful pattern that leverages event bubbling to manage events efficiently. Instead of attaching a separate event listener to each child element, you place a single listener on a common parent element. 

**How it works:**

1.  The event listener is attached to the parent element.
2.  When a user interacts with a child, the event bubbles up to the parent.
3.  The parent's listener function executes. Inside the function, you use the event.target property to identify which specific child element was originally clicked and take action based on it. 

**Benefits:**

*   **Performance:** Reduces memory usage by minimizing the number of event listeners, especially for large lists or tables.
*   **Dynamic Elements:** Automatically handles events for elements that are added or removed dynamically, without needing to re-attach listeners. 

**preventDefault() vs. stopPropagation()**

These two methods are often used within an event handler, but they serve very different purposes. 

|  | event.preventDefault() | event.stopPropagation() |
| --- | --- | --- |
| Purpose | Prevents the default browser action for a given event from happening. | Stops the event from propagating further up or down the DOM tree. |
| Use Case | Preventing a link (<a>) from navigating to a new page, stopping a checkbox from being toggled, or halting a form's submission. | Stopping a click on a nested element from also triggering the click handler on its parent. |
| Example | event.preventDefault(); | event.stopPropagation(); |
| Propagation | Does not stop event propagation (bubbling/capturing). The event will continue its journey through the DOM unless stopPropagation() is also called. | Does not prevent the default action. For example, a link click will still navigate unless preventDefault() is also called. |

### ES6+ Features

This overview covers several modern JavaScript (ES6 and later) features, detailing how they improve code clarity, reduce verbosity, and manage complexity. 

**let and const**

These keywords provide block-scoped variable declarations, replacing the older var, which is function-scoped and known for unpredictable behavior like hoisting. 

*   **let**: Declares a variable that can be reassigned. Its scope is limited to the block ({...}), and it is not accessible before its declaration.
*   **const**: Declares a constant that cannot be reassigned. It also has a block scope and must be initialized when declared. For objects and arrays declared with const, their contents can be mutated, but the variable cannot be pointed to a new object or array. 

javascript

_// let_

let count = 1;

if (true) {

let count = 2; _// Different variable, block-scoped_

console.log(count); _// Output: 2_

}

console.log(count); _// Output: 1_

_// const_

const PI = 3.14159;

_// PI = 3.14; // Throws TypeError_

const person = { name: 'Alice' };

person.name = 'Bob'; _// Allowed, mutates the object_

_// person = { name: 'Charlie' }; // Throws TypeError, cannot reassign_

Use code with caution.

**Template literals**

Introduced in ES6, template literals allow for more readable string interpolation and multi-line strings. They are enclosed in backticks ( ) and use the ${expression} syntax to embed variables or expressions. 

javascript

const name = 'Alice';

const age = 30;

_// Regular string concatenation_

const greetingOld = 'Hello, ' + name + '! You are ' + age + ' years old.';

_// Template literal for interpolation and multi-line support_

const greetingNew = \`Hello, ${name}!

You are ${age} years old.\`;

Use code with caution.

**Destructuring (object and array)**

Destructuring is an expression that makes it possible to unpack values from arrays or properties from objects into distinct variables. 

javascript

_// Array destructuring_

const fruits = \['apple', 'banana', 'cherry'\];

const \[first, second\] = fruits;

console.log(first); _// Output: 'apple'_

_// Object destructuring_

const user = { name: 'Alice', role: 'admin' };

const { name, role } = user;

console.log(name); _// Output: 'Alice'_

Use code with caution.

**Spread and rest operators**

The spread (...) and rest (...) operators use the same syntax but have opposite functions. 

*   **Spread operator**: Expands an iterable (like an array or string) into its individual elements. It is useful for creating copies, merging arrays, or passing array elements as arguments to a function.
*   **Rest operator**: Gathers remaining elements into a single array. It is used in function parameters or array destructuring to collect the "rest" of the arguments or items. 

javascript

_// Spread operator_

const arr1 = \[1, 2\];

const arr2 = \[3, 4\];

const combined = \[...arr1, ...arr2\];

console.log(combined); _// Output: \[1, 2, 3, 4\]_

_// Rest operator_

function logArguments(first, second, ...rest) {

console.log(rest);

}

logArguments(1, 2, 3, 4, 5); _// Output: \[3, 4, 5\]_

Use code with caution.

**Modules (import, export)**

ES6 introduced a native module system to better organize and reuse code. The import and export statements are used to share functions, objects, or variables across different JavaScript files. 

*   **export**: Used to make variables, functions, or classes available to other modules.
*   **import**: Used to access exported members from another module. 

**Default, named, and dynamic imports**

*   **Named imports/exports**: A module can have multiple named exports. The import name must match the export name (though it can be aliased).
*   **Default imports/exports**: A module can only have one default export. It can be imported with any name.
*   **Dynamic imports**: Allows modules to be loaded on demand, using import('path/to/module.js'). This returns a Promise that resolves to the module object, making it useful for code splitting. 

javascript

_// math.js_

export const pi = 3.14; _// Named export_

export default function add(a, b) {

return a + b;

} _// Default export_

_// main.js_

import sum, { pi } from './math.js'; _// Default and named import_

console.log(sum(5, 5)); _// Output: 10_

console.log(pi); _// Output: 3.14_

_// Dynamic import_

document.getElementById('myButton').addEventListener('click', () => {

import('./math.js').then((math) => {

console.log(math.default(10, 10)); _// Output: 20_

});

});

Use code with caution.

**Optional chaining (?.)**

This operator provides a safer way to access properties of a nested object without having to check if each intermediate property exists. It returns undefined if an element in the chain is null or undefined, instead of throwing an error. 

javascript

const user = {

address: {

city: 'New York'

}

};

_// Without optional chaining_

const city = user.address && user.address.city;

console.log(city); _// Output: 'New York'_

_// With optional chaining_

const zipcode = user.address?.zipcode;

console.log(zipcode); _// Output: undefined_

const nonExistentProperty = user.location?.country;

console.log(nonExistentProperty); _// Output: undefined_

Use code with caution.

**Nullish coalescing (??)**

The nullish coalescing operator is a logical operator that returns its right-hand side operand when its left-hand side operand is null or undefined. This is different from the logical OR operator (||), which returns the right-hand operand for _any_ falsy value (e.g., 0, "", false). 

javascript

const userInput = '';

const defaultName = 'Guest';

_// Using logical OR (||)_

const nameWithOr = userInput || defaultName;

console.log(nameWithOr); _// Output: 'Guest' (empty string is falsy)_

_// Using nullish coalescing (??)_

const nameWithNullish = userInput ?? defaultName;

console.log(nameWithNullish); _// Output: '' (empty string is not nullish)_

const nullValue = null;

const assignedValue = nullValue ?? 'Default';

console.log(assignedValue); _// Output: 'Default'_

Use code with caution.

### Advanced Objects

In JavaScript, advanced object-oriented programming relies on a set of powerful concepts for handling object creation, method binding, and property access. 

**this binding with call(), apply(), and bind()**

[https://www.geeksforgeeks.org/javascript/explain-call-apply-and-bind-methods-in-javascript/](https://www.geeksforgeeks.org/javascript/explain-call-apply-and-bind-methods-in-javascript/)

In JavaScript, the this keyword refers to the object executing the current function. These three methods provide explicit control over what this refers to when a function is called. 

| Method | Invocation | Argument format | Description |
| --- | --- | --- | --- |
| call() | Immediate | Comma-separated | Calls the function immediately with a specified this value and arguments passed individually. |
| apply() | Immediate | Array or array-like | Calls the function immediately with a specified this value and arguments provided as an array. |
| bind() | Deferred | Comma-separated | Returns a new function that has a permanent this context. The function must be invoked separately. |

**Example**

javascript

const person = {

name: 'John',

greet: function(greeting, punctuation) {

console.log(\`${greeting}, my name is ${this.name}${punctuation}\`);

}

};

const anotherPerson = {

name: 'Jane'

};

_// call()_

person.greet.call(anotherPerson, 'Hello', '!'); _// "Hello, my name is Jane!"_

_// apply()_

person.greet.apply(anotherPerson, \['Hi', '.'\]); _// "Hi, my name is Jane."_

_// bind()_

const greetJane = person.greet.bind(anotherPerson, 'Hola', '!');

greetJane(); _// "Hola, my name is Jane!"_

Use code with caution.

**Currying functions**

Currying is the process of transforming a function with multiple arguments into a sequence of functions, each taking a single argument. It is often used for creating specialized, reusable functions. 

**Example**

javascript

_// Non-curried function_

const add = (a, b, c) => a + b + c;

console.log(add(1, 2, 3)); _// 6_

_// Curried version_

const curriedAdd = (a) => (b) => (c) => a + b + c;

console.log(curriedAdd(1)(2)(3)); _// 6_

_// Partial application using currying_

const addTwo = curriedAdd(2);

const addTwoAndThree = addTwo(3);

console.log(addTwoAndThree(4)); _// 9_

Use code with caution.

**Constructor functions and the new keyword**

A constructor function is a regular function used to create multiple, similar objects. By convention, constructor functions are named with an initial capital letter. 

*   The new keyword automates four steps to create and return an object:
    1.  A new, empty object is created.
    2.  The new object's internal \[\[Prototype\]\] is set to the constructor function's prototype.
    3.  The this context is bound to the new object and the function is executed.
    4.  The new object is returned (unless the constructor returns a non-primitive value). 

**Example**

javascript

function Person(name, age) {

this.name = name;

this.age = age;

this.sayHello = function() {

console.log(\`Hello, my name is ${this.name}.\`);

};

}

const person1 = new Person('Alice', 30);

const person2 = new Person('Bob', 25);

person1.sayHello(); _// "Hello, my name is Alice."_

person2.sayHello(); _// "Hello, my name is Bob."_

Use code with caution.

**Classes and inheritance (extends, super)**

The class syntax, introduced in ES6, provides a more concise way to create constructor functions. It uses prototypal inheritance under the hood, but offers a cleaner, object-oriented syntax. 

*   **extends**: Used to create a subclass (child) that inherits properties and methods from a superclass (parent).
*   **super**: Used inside a subclass to access the superclass.
    *   **super()**: Calls the parent's constructor. This must be done before using this in the subclass constructor.
    *   **super.method()**: Calls a method from the parent class. 

**Example**

javascript

class Animal {

constructor(name) {

this.name = name;

}

speak() {

console.log(\`${this.name} makes a noise.\`);

}

}

class Dog extends Animal {

constructor(name, breed) {

super(name); _// Call the parent constructor_

this.breed = breed;

}

speak() {

super.speak(); _// Call the parent method_

console.log(\`${this.name} barks.\`);

}

}

const myDog = new Dog('Buddy', 'Golden Retriever');

myDog.speak();

_// Output:_

_// "Buddy makes a noise."_

_// "Buddy barks."_

Use code with caution.

**Static methods and properties**

Static methods and properties are defined on the class itself, not on instances of the class. This makes them ideal for creating utility functions or storing class-level configuration. 

*   Inside a static method, this refers to the class itself, not an instance.
*   You call them directly on the class name, e.g., MyClass.myStaticMethod(). 

**Example**

javascript

class MathUtils {

static PI = 3.14159;

static getArea(radius) {

return this.PI \* radius \* radius;

}

}

console.log(MathUtils.PI); _// 3.14159_

console.log(MathUtils.getArea(5)); _// 78.53975_

_// Attempting to call a static method on an instance will fail_

const utils = new MathUtils();

_// utils.getArea(5); // TypeError_

Use code with caution.

**Getters and setters**

Getters and setters are special methods that allow you to control access to object properties. They let you run custom logic when a property is retrieved or set, without requiring the user to call a method explicitly. 

*   **get**: Binds an object property to a function that will be called when that property is looked up. It is accessed like a property, not a function.
*   **set**: Binds an object property to a function to be called when there is an attempt to set that property. The setter must have exactly one parameter for the new value. 

**Example**

javascript

class User {

constructor(firstName, lastName) {

this.firstName = firstName;

this.lastName = lastName;

}

get fullName() {

return \`${this.firstName} ${this.lastName}\`;

}

set fullName(value) {

const parts = value.split(' ');

this.firstName = parts\[0\];

this.lastName = parts\[1\];

}

}

const user = new User('Alice', 'Smith');

console.log(user.fullName); _// Calls the getter: "Alice Smith"_

user.fullName = 'Bob Johnson'; _// Calls the setter_

console.log(user.firstName); _// "Bob"_

console.log(user.lastName); _// "Johnson"_

### JavaScript Internals

JavaScript's internals explain how the engine executes code, handles memory, and manages asynchronous tasks in its single-threaded environment. 

**Execution context**

An execution context is the environment where JavaScript code is evaluated and executed. It is created in two distinct phases. 

**1\. Creation phase**

This happens immediately when the JavaScript engine encounters code, before it is executed. 

*   **Global execution context (GEC):** For a JavaScript file, the engine creates a global object (like window in browsers or global in Node.js) and sets the value of this to point to it.
*   **Function execution context (FEC):** When a function is called, the engine creates a new, separate context. It's pushed onto the call stack, a LIFO (Last-In, First-Out) structure that keeps track of the currently executing functions.
*   **Memory allocation:** The engine scans the code and allocates memory for variables and functions.
    *   **Variables:** Variable declarations (using var, let, and const) are hoisted. With var, the variable is initialized to undefined. With let and const, the variable is uninitialized, entering the temporal dead zone (TDZ).
    *   **Functions:** Function declarations are completely hoisted, and their full function code is stored in memory. 

**2\. Execution phase**

After the creation phase, the engine executes the code line by line. 

*   **Assignments and function calls:** It assigns the real values to variables and executes the code within function calls.
*   **New execution contexts:** If a function call is encountered, a new function execution context is created and pushed onto the call stack.
*   **Stack management:** When a function's execution is complete, its context is popped off the call stack, and control returns to the parent context. When all code is executed, the GEC is also popped, and the stack is empty. 

**Memory allocation and garbage collection**

**Memory allocation**

The JavaScript engine uses two primary areas of memory: 

*   **Stack:** Used for static memory allocation. It stores primitive values (numbers, strings, booleans) and references (pointers) to objects. The size of these items is known at compile time.
*   **Heap:** Used for dynamic memory allocation. It stores reference types like objects, arrays, and functions. Memory is allocated on the heap as needed during runtime. 

**Garbage collection**

JavaScript automatically frees up memory that is no longer needed through a process called garbage collection. This is crucial for preventing memory leaks. 

*   **Reachability:** The main concept is "reachability." A value is considered reachable if it's accessible from a set of root values, such as the global object and the current function's local variables.
*   **Mark-and-sweep algorithm:** Modern JavaScript engines primarily use this algorithm, which works in two phases:
    *   **Mark:** The garbage collector starts from the root objects and traverses all reachable objects, "marking" them.
    *   **Sweep:** It then sweeps through memory and collects (removes) all unmarked objects.
*   **Circular references:** The mark-and-sweep algorithm can detect and collect objects that have circular references (e.g., object A references object B, and object B references object A) but are no longer reachable from any root. 

**Event loop mechanism**

As a single-threaded language, JavaScript uses an event loop to handle asynchronous operations without blocking the main execution thread. 

The event loop relies on several components:

*   **Call Stack:** Executes synchronous code.
*   **Web APIs:** Provided by the browser (e.g., setTimeout, fetch, DOM events), these handle asynchronous tasks in the background.
*   **Callback (Task) Queue:** Holds the callbacks of completed asynchronous tasks (like timers or DOM events) waiting to be executed.
*   **Microtask Queue:** A higher-priority queue for callbacks from promises (.then, .catch, .finally) and other microtasks. 

The event loop works as follows: 

1.  Continuously checks if the **Call Stack** is empty.
2.  If the Call Stack is empty, it checks the **Microtask Queue** and moves any pending microtasks to the Call Stack to be executed.
3.  After the Microtask Queue is empty, it checks the **Callback Queue** and moves the first pending callback to the Call Stack.
4.  This process repeats, ensuring that microtasks are always prioritized over regular tasks. 

**Shadowing and Temporal Dead Zone (TDZ)**

**Shadowing**

Variable shadowing occurs when a variable declared in a nested scope (e.g., inside a function or block) has the same name as a variable in a containing scope. 

*   **Effect:** The inner variable "shadows" or hides the outer variable. Any code inside the inner scope will only have access to the inner variable.
*   **With var, let, and const:**
    *   var is function-scoped, so it will shadow a global var within a function.
    *   let and const are block-scoped, so they will shadow an outer variable within a specific block (if statement, for loop). 

javascript

let myVar = "global";

function example() {

let myVar = "local"; _// 'local' shadows 'global' inside this function_

console.log(myVar); _// logs "local"_

}

example();

console.log(myVar); _// logs "global"_

Use code with caution.

**Temporal Dead Zone (TDZ)**

The TDZ is the period between the start of a block scope and the initialization of a let or const variable within that scope. 

*   **Cause:** Unlike var which is initialized with undefined upon hoisting, let and const are hoisted but remain uninitialized.
*   **Result:** Attempting to access a let or const variable within the TDZ results in a ReferenceError, preventing the bugs associated with accessing uninitialized variables. 

javascript

{ _// Start of the TDZ for \`myConst\`_

_// console.log(myConst); // ReferenceError: Cannot access 'myConst' before initialization_

const myConst = "value"; _// End of the TDZ_

console.log(myConst); _// logs "value"_

}

Use code with caution.

**Polyfills (for map, bind, reduce)**

A polyfill is a piece of code that adds modern functionality to older JavaScript environments that do not support it natively. You can write polyfills by extending the Array.prototype or Function.prototype. 

**Polyfill for Array.prototype.map()**

The map() method creates a new array by applying a function to each element of the original array. 

javascript

if (!Array.prototype.myMap) {

Array.prototype.myMap = function(callback) {

const result = \[\];

for (let i = 0; i < this.length; i++) {

result.push(callback(this\[i\], i, this));

}

return result;

};

}

Use code with caution.

**Polyfill for Function.prototype.bind()**

The bind() method creates a new function with the this keyword permanently set to the provided value. 

javascript

if (!Function.prototype.myBind) {

Function.prototype.myBind = function(scope, ...args) {

const originalFunction = this;

return function(...newArgs) {

return originalFunction.apply(scope, \[...args, ...newArgs\]);

};

};

}

Use code with caution.

**Polyfill for Array.prototype.reduce()**

The reduce() method executes a reducer function on each element of the array, resulting in a single output value. 

javascript

if (!Array.prototype.myReduce) {

Array.prototype.myReduce = function(callback, initialValue) {

let accumulator = initialValue;

for (let i = 0; i < this.length; i++) {

if (accumulator !== undefined) {

accumulator = callback(accumulator, this\[i\], i, this);

} else {

accumulator = this\[i\];

}

}

return accumulator;

};

}

### Error Handling

n JavaScript, different error types signal specific problems, from basic syntax issues to more complex runtime failures. You can also create and throw your own custom errors to provide more context during development and debugging. 

**Built-in error types**

**SyntaxError**

A SyntaxError is thrown when the JavaScript engine encounters code that does not follow the correct syntax of the language during the parsing phase. These errors typically cannot be caught with a standard try...catch block because they prevent the code from even beginning to execute. 

**Example:**

javascript

_// A SyntaxError caused by a missing parenthesis_

console.log("Hello World";

Use code with caution.

**Error message:**  
SyntaxError: missing ) after argument list 

**ReferenceError**

A ReferenceError occurs when you attempt to access a variable or an identifier that does not exist in the current scope or has not been initialized. 

**Example:**

javascript

_// A ReferenceError because 'myVariable' has not been declared_

console.log(myVariable);

Use code with caution.

**Error message:**  
ReferenceError: myVariable is not defined 

**TypeError**

A TypeError is thrown when an operation is performed on a value that is not of the expected type. This can happen when calling a method on an undefined variable or using an incompatible type with an operator. 

**Example:**

javascript

_// A TypeError because a number does not have a 'toUpperCase' method_

let myNum = 123;

myNum.toUpperCase();

Use code with caution.

**Error message:**  
TypeError: myNum.toUpperCase is not a function 

**Custom errors with throw**

You can create and throw your own custom errors using the throw statement. This is useful for signaling a specific issue in your application logic that standard error types may not cover. You can then use a try...catch block to handle it gracefully. 

The throw statement is often used with a new Error object. The Error object itself has several useful properties: message, name, and stack. 

**Error object properties**

*   **message**: A human-readable description of the error.
*   **name**: The name of the error. For the generic Error object, this is "Error," but it will be different for specific error types like "TypeError".
*   **stack**: A string detailing the function calls that led to the error, helping you trace the origin of the problem. 

**Example: Throwing and catching a custom error**

javascript

function validateAge(age) {

if (age < 0 || !Number.isInteger(age)) {

throw new Error("InvalidAgeError: Age must be a positive integer.");

}

console.log("Age is valid.");

}

try {

validateAge(-5);

} catch (e) {

console.log("Caught an error:");

console.log(\`Error Name: ${e.name}\`); _// Output: "Error" (default for custom error)_

console.log(\`Error Message: ${e.message}\`); _// Output: "InvalidAgeError: Age must be a positive integer."_

console.log(\`Error Stack: ${e.stack}\`); _// Output: Stack trace details_

}

Use code with caution.

**Creating custom error classes**

For more specific and maintainable custom errors, you can create a new class that extends the built-in Error class. 

**Example:**

javascript

_// Extend the built-in Error class_

class InvalidAgeError extends Error {

constructor(message) {

super(message); _// Call the parent constructor_

this.name = 'InvalidAgeError'; _// Set a custom name_

}

}

function validateAge(age) {

if (age < 0 || !Number.isInteger(age)) {

throw new InvalidAgeError("Age must be a positive integer.");

}

console.log("Age is valid.");

}

try {

validateAge(-5);

} catch (e) {

if (e instanceof InvalidAgeError) {

console.log("Caught a specific InvalidAgeError!");

console.log(\`Error Name: ${e.name}\`); _// Output: "InvalidAgeError"_

console.log(\`Error Message: ${e.message}\`); _// Output: "Age must be a positive integer."_

} else {

console.log("Caught a different kind of error.");

}

}

### Browser APIs

**localStorage and sessionStorage (Web Storage)** are browser APIs for storing key-value pairs of data on the client side. Unlike cookies, this data is not automatically sent with every HTTP request, making it suitable for larger datasets. 

| Feature | localStorage | sessionStorage |
| --- | --- | --- |
| Persistence | Data persists even after the browser is closed and reopened. It is cleared only when the user or script explicitly deletes it. | Data is cleared when the page session ends, typically when the browser tab or window is closed. It survives a page reload. |
| Scope | Available across all browser tabs from the same origin (domain). | Confined to the specific browser tab or window where it was created. |
| Capacity | Around 10MB across most browsers. | About 5MB across most browsers. |
| Use Case | Storing permanent user preferences, caching large chunks of API data, or remembering a user's logged-in status. | Storing temporary, session-specific data like form progress, shopping cart contents, or a multi-step process. |

**Cookies** are small pieces of text data sent from a web server to a browser and stored on the user's computer. 

*   They are sent automatically with every HTTP request to the server, making them useful for authentication, session management, and tracking users.
*   Cookies have a small storage capacity (approx. 4KB) and can be set with an expiration date.
*   Because they are included with every request, excessive use can negatively impact performance. 

**Fetch API (GET, POST requests)** is a modern, promise-based JavaScript interface for making network requests to get or send resources from a server. 

*   **GET requests** are used to retrieve data. They are initiated by a basic fetch(url) call and do not contain a body.
*   **POST requests** are used to send data to a server (e.g., submitting a form). They require a configuration object (init) specifying the method: 'POST' and include the data in the body option. 

**CORS (Cross-Origin Resource Sharing) basics** are a set of rules enforced by web browsers to allow or deny web pages from making requests to a different domain than the one that served the page. 

*   **Same-Origin Policy:** By default, web browsers prevent scripts from making requests to a different origin (a different domain, protocol, or port) to prevent malicious activity.
*   **How it works:** When a web page makes a cross-origin request, the browser sends an Origin header. The server must then respond with the correct Access-Control-Allow-Origin header to grant permission.
*   **Preflight Requests:** For complex requests (like POST with custom headers), the browser automatically sends a preflight OPTIONS request first to check with the server if the actual request is safe to send. 

**Geolocation API** allows a user's device to provide their geographic location to a web application. 

*   It is accessed via navigator.geolocation and uses methods like getCurrentPosition() to get a device's latitude and longitude.
*   For security, it requires explicit user permission, and the browser will prompt the user to allow or deny location access. 

**Notifications API** enables web pages to display desktop-style notifications to the user. 

*   Notifications appear outside the browser window and can alert users to new information, even if they are not actively on the page.
*   Like Geolocation, it requires a user's permission to send notifications. 

**Clipboard API** provides the ability to programmatically read from and write to the system clipboard. 

*   It uses promise-based, asynchronous methods like navigator.clipboard.readText() and navigator.clipboard.writeText('Some Text').
*   For security, access is protected, and writing to the clipboard typically requires a user gesture, like a button click. 

**setTimeout and setInterval** are functions for executing code at a scheduled time.

*   **setTimeout(function, delay):** Executes a function _once_ after a specified delay in milliseconds. You can use clearTimeout() with the returned ID to cancel it.
*   **setInterval(function, delay):** Executes a function repeatedly with a fixed time delay between each call. It continues indefinitely until you call clearInterval() with its returned ID. 

### JavaScript Patterns

**Module Pattern**

The Module pattern in JavaScript is a design pattern used to create encapsulated, reusable, and organized code by controlling public and private access to variables and functions. It helps prevent global scope pollution and promotes data privacy, similar to the concept of classes in other languages. 

**Key features:**

*   **Encapsulation:** Protects private variables and methods.
*   **Namespacing:** Prevents global scope pollution.
*   **Reusability:** Allows the module to be used in different parts of an application. 

For an example using an IIFE (Immediately-Invoked Function Expression), please see the referenced document. 

**Singleton Pattern**

The Singleton pattern ensures that a class has only one instance and provides a global access point to it. This is useful for centralized resources like configuration settings or a logging service, where only one instance is needed. 

**Key features:**

*   **Single instance:** Limits a class to a single object.
*   **Global access:** Provides a single point to access that instance.
*   **Lazy initialization:** Creates the instance only when needed. 

For an example using a class, please see the referenced document. 

**Factory Pattern**

The Factory pattern provides an interface for creating objects without revealing the creation logic to the user. It's helpful when you need to create various related objects, and the factory function decides which object to create based on input. 

**Key features:**

*   **Decoupling:** Separates object creation from the specific class.
*   **Flexibility:** Allows adding new object types easily.
*   **Centralized logic:** Simplifies managing the creation process. 

For an example, please see the referenced document. 

**Observer Pattern**

The Observer pattern (also known as Pub/Sub) creates a one-to-many relationship where a subject notifies its observers when its state changes. 

**Key features:**

*   **Loose coupling:** Observers and subjects are independent.
*   **Event-driven:** Suitable for handling events where multiple components react to the same event.
*   **Dynamic:** Observers can be added or removed anytime. 

For an example, please see the referenced document. 

**Debouncing and Throttling**

Debouncing and throttling control how often a function executes, especially for rapid events like typing or scrolling. 

**Debouncing**

Debouncing delays a function's execution until a certain time has passed without the event being triggered again. This ensures the function runs only once after a pause. A use case is making an API call for a search input only after the user stops typing for a moment. 

For an example implementation, please see the referenced document. 

**Throttling**

Throttling limits a function's execution to a maximum of once within a specified time frame. It executes at regular intervals, unlike debouncing, which waits for a pause. A use case is a window.resize or window.scroll event where you want to perform an action at most every 100ms. 

For an example implementation, please see the referenced document.

**1\. Module Pattern (with IIFE)**

// Module Pattern using IIFE

const CounterModule = (function () {

// Private variable

let count = 0;

// Private function

function log(message) {

console.log("Log:", message);

}

return {

// Public methods

increment() {

count++;

log(\`Incremented: ${count}\`);

},

decrement() {

count--;

log(\`Decremented: ${count}\`);

},

getCount() {

return count;

}

};

})();

// Usage

CounterModule.increment(); // Log: Incremented: 1

CounterModule.increment(); // Log: Incremented: 2

console.log(CounterModule.getCount()); // 2

🔑 Private stuff stays hidden in closure; only returned methods are public.

**2\. Singleton Pattern**

// Singleton using a class

class Singleton {

constructor(name) {

if (Singleton.instance) {

return Singleton.instance; // return existing instance

}

this.name = name;

Singleton.instance = this; // save instance

}

getName() {

return this.name;

}

}

// Usage

const s1 = new Singleton("First");

const s2 = new Singleton("Second");

console.log(s1.getName()); // First

console.log(s2.getName()); // First (same instance)

console.log(s1 === s2); // true

🔑 Only one instance exists across the app.

**3\. Factory Pattern**

// Factory Pattern

class Car {

constructor() {

this.type = "Car";

}

}

class Bike {

constructor() {

this.type = "Bike";

}

}

function VehicleFactory(vehicleType) {

if (vehicleType === "car") {

return new Car();

} else if (vehicleType === "bike") {

return new Bike();

}

}

// Usage

const v1 = VehicleFactory("car");

const v2 = VehicleFactory("bike");

console.log(v1.type); // Car

console.log(v2.type); // Bike

🔑 Creation logic is centralized, flexible for new types.

**4\. Observer Pattern (Pub/Sub)**

// Observer Pattern

class Subject {

constructor() {

this.observers = \[\];

}

subscribe(observerFn) {

this.observers.push(observerFn);

}

unsubscribe(observerFn) {

this.observers = this.observers.filter(fn => fn !== observerFn);

}

notify(data) {

this.observers.forEach(fn => fn(data));

}

}

// Usage

const subject = new Subject();

function logger(data) {

console.log("Logger:", data);

}

function alertUser(data) {

console.log("Alert:", data);

}

subject.subscribe(logger);

subject.subscribe(alertUser);

subject.notify("Event 1");

// Logger: Event 1

// Alert: Event 1

subject.unsubscribe(logger);

subject.notify("Event 2");

// Alert: Event 2

🔑 Many observers react when subject fires notify.

**5\. Debounce**

// Debounce function

function debounce(fn, delay) {

let timer;

return function (...args) {

clearTimeout(timer);

timer = setTimeout(() => fn.apply(this, args), delay);

};

}

// Usage: Run only after typing stops for 500ms

const handleSearch = debounce((query) => {

console.log("Searching for:", query);

}, 500);

// Simulating typing

handleSearch("H");

handleSearch("He");

handleSearch("Hel");

// Only last call ("Hel") executes after 500ms

🔑 Useful for input fields, API calls.

**6\. Throttle**

// Throttle function

function throttle(fn, limit) {

let lastCall = 0;

return function (...args) {

const now = Date.now();

if (now - lastCall >= limit) {

lastCall = now;

fn.apply(this, args);

}

};

}

// Usage: Allow execution at most every 1000ms

const handleScroll = throttle(() => {

console.log("Scroll event at", Date.now());

}, 1000);

// Simulating rapid scroll

setInterval(handleScroll, 200); // Logs only once every 1s

🔑 Useful for scroll/resize events.

### JavaScript in Practice

This practical guide explores key JavaScript concepts: deep vs. shallow copying, the nuances of == vs. ===, pass-by-value vs. pass-by-reference, and immutability. 

**Deep copy vs. shallow copy**

When copying an object or array, you create either a shallow copy or a deep copy. The main difference lies in how nested objects or arrays are handled. 

| Feature | Shallow Copy | Deep Copy |
| --- | --- | --- |
| Nested objects | Copies only the top-level properties. Nested objects share the same memory references as the original. | Creates a completely new object with new memory references for all nested objects, providing full independence from the original. |
| Modification | Changing a nested property in the copy will also affect the original object. | Changes to the deep copy, even in nested structures, do not affect the original object. |
| Performance | Faster and less memory-intensive, as it only copies the top level. | Slower and more memory-intensive due to the need to recursively copy all levels. |

**Copying methods**

| Method | Type of Copy | When to Use | Limitations |
| --- | --- | --- | --- |
| Spread syntax (...) | Shallow copy. | When your object or array is flat (has no nested objects/arrays), and for simple cases. | Fails on nested objects. If a nested object exists, it will still be a reference to the original. |
| Object.assign() | Shallow copy. | Similar to the spread syntax, for creating a new object from one or more sources. | Also only goes one level deep. |
| JSON.parse(JSON.stringify(obj)) | Deep copy. | For creating a quick deep copy of objects that only contain simple data types (numbers, strings, booleans, arrays, plain objects). | * Does not work with functions, undefined, Map, Set, BigInt, or circular references.* Serializes Date objects into strings. |
| structuredClone() | Deep copy. | The modern, recommended way for deep cloning. It is robust and handles a wide variety of data types, including circular references, Map, and Set. | Cannot clone functions. |

**\== vs. ===**

These operators both check for equality, but they handle different data types differently. 

*   **Loose Equality (==)**: This operator compares for equality after performing **type coercion** if the operands are of different types. This means it will automatically convert one type to match the other before making the comparison, which can lead to unexpected results.

javascript

console.log(5 == '5'); _// true (string '5' is coerced to number 5)_

console.log(0 == false); _// true (false is coerced to 0)_

console.log(null == undefined); _// true (a special case in loose equality)_

Use code with caution.

*   **Strict Equality (===)**: This operator compares for equality without performing any type coercion. For two values to be strictly equal, they must have both the same value **and** the same data type. This behavior is more predictable and is considered a best practice in most cases.

javascript

console.log(5 === '5'); _// false (different types)_

console.log(0 === false); _// false (different types)_

console.log(null === undefined); _// false (different types)_

Use code with caution.

**Best practice**: Use === and !== by default to avoid unexpected behavior caused by type coercion. The == operator should only be used when you explicitly want type coercion and understand its implications. 

**Pass-by-value vs. pass-by-reference**

JavaScript's behavior for passing function arguments depends on the data type. A key nuance is that JavaScript **never** passes by true reference. Instead, it passes object references **by value**. 

*   **Pass-by-value**: For **primitive data types** (string, number, boolean, null, undefined), a function receives a copy of the actual value. Changes to the variable inside the function do not affect the original variable outside the function.

javascript

let myNumber = 10;

function addFive(num) {

num += 5; _// Changes the local copy, not the original myNumber_

console.log('Inside function:', num); _// 15_

}

addFive(myNumber);

console.log('Outside function:', myNumber); _// 10 (Original is unchanged)_

Use code with caution.

*   **Pass-by-value (for references)**: For **non-primitive data types** (objects and arrays), JavaScript passes a copy of the reference (memory address), not the object itself. The function receives a reference that points to the same object in memory as the original. This allows the function to modify the original object's contents.

javascript

let myObject = { value: 10 };

function addFiveToValue(obj) {

obj.value += 5; _// Mutates the original object's property_

console.log('Inside function:', obj.value); _// 15_

}

addFiveToValue(myObject);

console.log('Outside function:', myObject.value); _// 15 (Original object is changed)_

Use code with caution.

However, if you reassign the entire object inside the function, the original reference is unaffected because you are only changing the local copy of the reference.

javascript

let myObject = { value: 10 };

function replaceObject(obj) {

obj = { value: 20 }; _// Reassigns the local 'obj' reference_

console.log('Inside function:', obj.value); _// 20_

}

replaceObject(myObject);

console.log('Outside function:', myObject.value); _// 10 (Original object is unchanged)_

Use code with caution.

### Modern Topics (Advanced)

**Generators and iterators**

  
In JavaScript, an iterator is an object that follows the iterator protocol, which means it must have a next() method. When called, next() returns an object with two properties: value (the next item in the sequence) and done (a boolean indicating if the sequence has finished). Many built-in types like Array and Map are iterable by default. 

Generators are functions that provide a more convenient and readable way to write iterators. 

*   They are defined using the function\* syntax.
*   The yield keyword is used inside a generator function to pause its execution and return a value.
*   When a generator function is called, it returns a special type of iterator called a generator object.
*   The next() method is then used to resume execution and retrieve the next value from the generator.
*   Generators are useful for creating custom iterators, handling infinite sequences, and simplifying asynchronous code. 

**Proxies and Reflect API**  
The Proxy and Reflect APIs were introduced in ES6 to provide powerful meta-programming capabilities. 

*   **Proxy:** An object that wraps a "target" object and defines custom behavior for fundamental operations like property lookup, assignment, and function invocation.
    *   It uses a handler object containing methods, known as "traps," which intercept operations.
    *   **Use cases:** Validation, logging, access control, and building reactive systems.
*   **Reflect:** A built-in object with static methods that correspond to the same fundamental operations as Proxy traps.
    *   It's not a function or constructor, so it can't be instantiated with new.
    *   It provides a way to invoke the default behavior for an operation, which is useful when combined with a Proxy to log an operation before executing its default behavior.
    *   This is generally cleaner and safer than applying the operation directly on the target object within the trap. 

**Symbols**  
Symbols are a primitive data type introduced in ES6 that represent a unique and immutable identifier. 

*   **Unique keys:** They are used to create unique property keys on objects that are guaranteed not to clash with other keys, including other Symbols.
*   **Privacy:** Symbols can be used to create pseudo-private properties in objects because they don't appear in for...in loops or Object.keys().
*   **"Well-known" symbols:** A set of built-in symbols (e.g., Symbol.iterator, Symbol.toStringTag) are used by JavaScript to expose internal language behaviors. 

**WeakMap and WeakSet**  
WeakMap and WeakSet are collections that differ from regular Map and Set by holding "weak" references to their objects. 

*   **Weak references and garbage collection:** If the only reference to an object is in a WeakMap or WeakSet, that object can be garbage-collected. This prevents memory leaks that can occur with regular maps and sets.
*   **WeakMap:** A collection of key-value pairs where the keys must be objects. When a key is garbage-collected, its corresponding value is automatically removed.
*   **WeakSet:** A collection of unique objects. When an object is garbage-collected, it is automatically removed from the set.
*   **Key limitations:** Neither WeakMap nor WeakSet are iterable and they do not have a size property. 

**BigInt**  
BigInt is a new numeric primitive data type that can represent integers of arbitrary size. 

*   **Overcoming limitations:** It addresses the limitation of JavaScript's standard Number type, which can only safely represent integers up to

![](data:image/gif;base64,R0lGODlhAQABAIAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==)

253−12 to the 53rd power minus 1

253−1

(Number.MAX\_SAFE\_INTEGER).

*   **Creating a BigInt:** You can create a BigInt by appending n to an integer literal (e.g., 100n) or by calling the BigInt() function.
*   **Usage rules:** Arithmetic operations with a BigInt require all operands to be BigInts; you cannot mix a BigInt and a regular Number. 

**Service workers and Web workers**  
Web and Service Workers are scripts that run in separate threads, allowing developers to offload tasks from the main thread to prevent performance issues and improve responsiveness. 

*   **Web Workers:**
    *   Used for running CPU-intensive scripts (e.g., heavy computations, data processing) without blocking the main UI thread.
    *   They have no access to the DOM and communicate with the main thread via postMessage().
*   **Service Workers:**
    *   Act as a programmable network proxy, intercepting and caching network requests.
    *   This enables features like offline access, push notifications, and background data synchronization.
    *   They operate independently of the web page and can be active even when the page is closed. 

### Interview-Favourite Questions:

This is a compilation of advanced JavaScript topics frequently covered in technical interviews. It includes common output-based questions, explanations of key concepts, and polyfill implementations to help demonstrate a deep understanding of the language. 

**Output-based tricky questions**

**Hoisting**

**Question:** What will be the output of the following code?

javascript

var a = 1;

function b() {

a = 10;

return;

function a() {}

}

b();

console.log(a);

Use code with caution.

**Answer:** The output will be 1.  
**Explanation:**

1.  Function declarations are fully hoisted to the top of their function scope. Inside b(), the declaration function a() {} is hoisted.
2.  The local function a() declaration shadows the outer var a = 1.
3.  The statement a = 10; inside b() assigns the value 10 to the local a, not the global a.
4.  The function b() returns, and the outer a remains unchanged. 

**Closures**

**Question:** What will be the output of the following code?

javascript

for (var i = 0; i < 3; i++) {

setTimeout(function() {

console.log(i);

}, 100);

}

Use code with caution.

**Answer:** The output will be 3, 3, 3.  
**Explanation:**

1.  The for loop, using var, does not create a new scope for each iteration. The variable i is function-scoped.
2.  The setTimeout callbacks are scheduled to run after the loop has completed.
3.  By the time the callbacks execute, the loop has already finished and i has a final value of 3. All three closures share the same i variable. 

**this**

**Question:** What will be the output of the following code?

javascript

var hero = {

\_name: 'John',

getSecretIdentity: function() {

return this.\_name;

}

};

var stoleSecretIdentity = hero.getSecretIdentity;

console.log(stoleSecretIdentity());

console.log(hero.getSecretIdentity());

Use code with caution.

**Answer:**

undefined

John

**Explanation:**

1.  The value of this depends on how a function is called.
2.  stoleSecretIdentity() is called as a standalone function in the global context, so this inside it refers to the global object (e.g., window or undefined in strict mode). Since \_name is not a property of the global object, the first call returns undefined.
3.  hero.getSecretIdentity() is called as a method of the hero object, so this correctly refers to hero. 

**Implement polyfills**

**Array.prototype.myMap()**

javascript

Array.prototype.myMap = function(callback) {

const result = \[\];

for (let i = 0; i < this.length; i++) {

result.push(callback(this\[i\], i, this));

}

return result;

};

Use code with caution.

**Array.prototype.myFilter()**

javascript

Array.prototype.myFilter = function(callback) {

const result = \[\];

for (let i = 0; i < this.length; i++) {

if (callback(this\[i\], i, this)) {

result.push(this\[i\]);

}

}

return result;

};

Use code with caution.

**Function.prototype.myBind()**

javascript

Function.prototype.myBind = function(context, ...args) {

const func = this;

return function(...newArgs) {

return func.apply(context, \[...args, ...newArgs\]);

};

};

Use code with caution.

**Explanation:**  
A polyfill is a piece of code that provides the functionality of a feature not supported by older browsers. These implementations extend the Array or Function prototypes to mimic the behavior of the native methods. 

**Promise chaining questions**

**Question:** What is the final output of this promise chain?

javascript

Promise.resolve(1)

.then(val => {

console.log(val);

return val + 1;

})

.then(val => {

console.log(val);

return Promise.reject('Error!');

})

.then(val => {

console.log('This will not run.');

return val + 1;

})

.catch(err => {

console.log(err);

return 10;

})

.then(val => {

console.log(val);

});

Use code with caution.

**Answer:**

1

2

Error!

10

**Explanation:**

1.  The first .then() logs 1 and returns 2, which is passed to the next .then().
2.  The second .then() logs 2 and returns a rejected promise.
3.  The rejected promise skips the next .then() and goes to the .catch().
4.  The .catch() logs the error message and returns a synchronous value, 10, which resolves the promise chain.
5.  The final .then() receives 10 and logs it. 

**Event loop + setTimeout vs. Promise.resolve() output order**

**Question:** What is the order of console logs?

javascript

console.log('Start');

setTimeout(() => console.log('Timeout 1'), 0);

Promise.resolve().then(() => {

console.log('Promise 1');

setTimeout(() => console.log('Timeout 2'), 0);

});

Promise.resolve().then(() => console.log('Promise 2'));

console.log('End');

Use code with caution.

**Answer:**

Start

End

Promise 1

Promise 2

Timeout 1

Timeout 2

**Explanation:**

1.  **Synchronous code:** Start and End are executed immediately.
2.  **Microtask Queue:** Promises are placed in the microtask queue. The event loop processes all microtasks before moving on to macrotasks. Promise 1 and Promise 2 are added to the microtask queue and executed in order.
3.  **Macrotask Queue:** setTimeout callbacks are placed in the macrotask queue. The event loop processes the macrotask queue after the call stack and microtask queue are empty. Timeout 1 is added to the macrotask queue first, and Timeout 2 is added later from within the Promise 1 microtask. The macrotasks are processed in the order they were queued. 

**call vs. apply vs. bind scenarios**

**Question:** Explain the difference between call, apply, and bind with a code example.  
**Answer:** All three methods change the value of this inside a function, but they differ in how they are invoked and how they handle arguments. 

javascript

const person = { name: 'Alice' };

function introduce(greeting, mood) {

console.log(\`${greeting}, my name is ${this.name} and I'm feeling ${mood}.\`);

}

_// call: Invokes the function immediately. Arguments are passed individually._

introduce.call(person, 'Hello', 'happy'); _// Output: Hello, my name is Alice and I'm feeling happy._

_// apply: Invokes the function immediately. Arguments are passed as an array._

introduce.apply(person, \['Hi', 'great'\]); _// Output: Hi, my name is Alice and I'm feeling great._

_// bind: Returns a new function with \`this\` permanently bound. It is not invoked immediately._

const introduceAlice = introduce.bind(person, 'Hey');

introduceAlice('tired'); _// Output: Hey, my name is Alice and I'm feeling tired._

Use code with caution.

**Debounce & throttle implementation**

**Debounce**

Delays function execution until a certain amount of time has passed since the last invocation. 

javascript

function debounce(func, delay) {

let timeoutId;

return function(...args) {

clearTimeout(timeoutId);

timeoutId = setTimeout(() => {

func.apply(this, args);

}, delay);

};

}

Use code with caution.

**Throttle**

Limits the rate at which a function is called. It executes at most once per a specified time interval. 

javascript

function throttle(func, limit) {

let inThrottle;

return function(...args) {

if (!inThrottle) {

func.apply(this, args);

inThrottle = true;

setTimeout(() => (inThrottle = false), limit);

}

};

}

Use code with caution.

**Explanation:** Debouncing is useful for events like window resizing or typing into a search box, where you only want the final result. Throttling is better for continuous events like scrolling or mouse movement, where a regular, but not excessive, event rate is desired. 

**Flatten nested arrays**

**Using recursion with reduce**

javascript

function flatten(arr) {

return arr.reduce((acc, item) => {

if (Array.isArray(item)) {

acc.push(...flatten(item));

} else {

acc.push(item);

}

return acc;

}, \[\]);

}

Use code with caution.

**Using Array.prototype.flat()**

Introduced in ES2019, flat() can flatten an array to a specified depth. 

javascript

const nestedArray = \[1, \[2, \[3, \[4\]\]\], 5\];

const flattened = nestedArray.flat(Infinity); _// Pass Infinity for any level of nesting_

console.log(flattened); _// Output: \[1, 2, 3, 4, 5\]_

Use code with caution.

**Explanation:** The recursive reduce approach is a classic manual implementation. The flat() method is the modern, more concise way to achieve the same result. 

**Deep vs. shallow clone implementation**

**Shallow clone:** Creates a new object, but nested objects still reference the same memory locations as the original. 

javascript

const original = { a: 1, b: { c: 2 } };

const shallowCopy = { ...original };

shallowCopy.b.c = 3;

console.log(original.b.c); _// Output: 3_

Use code with caution.

**Deep clone:** Creates a new object with no shared references, making the copy completely independent. 

**Using JSON.parse(JSON.stringify())**

This is a quick and common trick, but has limitations (e.g., doesn't handle functions, Dates, undefined). 

javascript

const original = { a: 1, b: { c: 2 } };

const deepCopy = JSON.parse(JSON.stringify(original));

deepCopy.b.c = 3;

console.log(original.b.c); _// Output: 2_

Use code with caution.

**Manual recursive implementation**

For a more robust solution, a recursive function is necessary. 

javascript

function deepClone(obj) {

if (obj === null || typeof obj !== 'object') {

return obj;

}

const copy = Array.isArray(obj) ? \[\] : {};

for (let key in obj) {

if (Object.prototype.hasOwnProperty.call(obj, key)) {

copy\[key\] = deepClone(obj\[key\]);

}

}

return copy;

}

Use code with caution.

**Explanation:** A deep clone is necessary when you need to make changes to a nested object without affecting the original. Shallow copies are faster but can cause unexpected side effects with nested data structures.
