# Coding Standard For Kioto UI

## LIFT coding style

Try and structure the app such that you can *Locate* code quickly, *Identify* the purpose of the code at a glance, keep the structure as *Flat* as possible, and *Try* to be DRY.

---

### Locate

Make locating code intuitive, fast and simple.

To work efficiently, we must be able to find files quickly, especially when we do not know (or do not remember) the file names.
Keeping related files near each other, in an intuitive location, saves time.
An appropriate and intuitive folder structure with descriptive names can make a world of difference to future you and the other people who will work with your code.

### Identify

Choose file names such that you instantly know what they contain and represent. Be descriptive(but not too much).

Keep the content of files to one component.

Avoid files with multiple components, multiple services, or a mixture of services and components.

### Flat

Keep the folder structure flat as much as possible.

Consider creating sub-folders(with appropriate logical grouping of files) when a folder reaches seven or more files.

### DRY

__Don't Repeat Yourself__

But avoid being so DRY that you sacrifice readability.

## Standard

### 1. Naming

 1. Use PascalCase for type names.
 2. Do not use "I" as a prefix for interface names.
 3. Use camelCase for function names.
 4. Use camelCase for property names and local variables.
 5. Use whole words(instead of abbreviations) in names when possible.
 6. Consider spelling `const` variables in lower camel case.
 7. Follow a pattern that describes the symbol's feature, then its type.
 8. __Don't__ use custom prefix for the selector of component. Use `app`
 9. Magic values (eg. numerical constants) must be formatted LIKE_THIS(upper snake case).

### 2. File content

 1. 1 file per logical component.
 2. Create a new service when a component starts being too complex.
 3. Put logic for data operations and interaction in a service.
 4. Consider limiting files to 300 lines of code.

### 3. Variable

 1. Use `undefined`. Do not use `null` except for API (Python use `null')
 2. `var` must NOT be used.

### 4. Documentation

 1. Use TSDoc style comments for functions, interfaces, enums, and classes.
 2. Document as much as possible.

### 5. Functions

 1. Try to limit functions to no more than 75 lines.

### 6. Strings

 1. Static strings must be declared using single quotes or backticks.
 2. Dynamic strings must be declared using ES6 template literals (backticks). Dynamic strings must not be declared using single- or double-quotes.
 3. Never use double-quotes.

### 7. General Constructs

 1. Do not use for..in statements; instead, use ts.forEach, ts.forEachKey and ts.forEachValue.
 2. Try to use ts.forEach, ts.map, and ts.filter instead of loops when it is not strongly inconvenient.

### 8. Style

 1. Use arrow function syntax for anonymous function expressions.
 2. Open curly braces always go on the same line as the start of the code block or property list.
 3. Use 4 spaces per indentation level. DO NOT USE TABS.
 4. `else` goes on a separate line from the closing curly brace.
 5. Always surround loops and conditionals' body with curly braces.

### 9. Inspiration

* [TypeScript - Coding Guidelines](https://github.com/Microsoft/TypeScript/wiki/Coding-guidelines)
* [Angular - Style Guide](https://angular.io/guide/styleguide)
* [ES6 - Coding Style](https://github.com/elierotenberg/coding-styles/blob/master/es6.md)

### Other

Run `ng lint` from time to time...

You can download the TSLint extension [Visual Studio Code](https://code.visualstudio.com/).
