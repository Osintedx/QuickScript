# QuickScript Programming Language

QuickScript is a modern, lightweight programming language designed for simplicity and productivity. It combines the best features of JavaScript-like syntax with powerful functional programming capabilities and built-in async/await support.

## Features

- 🚀 **Simple, Clean Syntax**: JavaScript-like syntax that's easy to learn
- 🔄 **Async/Await Support**: Built-in support for asynchronous programming
- 🌐 **HTTP Client**: Native HTTP operations for API interactions
- 🧮 **Functional Programming**: First-class functions, map, filter, reduce
- 📦 **Modern Features**: Classes, modules, and array operations
- 🔍 **Type Inference**: Smart type system without explicit annotations
- 🛠️ **Built-in Tools**: Rich standard library with common utilities

## Installation

```bash
npm install -g quickscript
```

## Quick Start

```qs
// Hello World
print("Hello, World!");

// Functions
func add(a, b) {
    return a + b;
}

// Arrays and functional programming
let numbers = [1, 2, 3, 4, 5];
let doubled = map(numbers, func(n) {
    return n * 2;
});

// HTTP requests
func getTodos() {
    let response = get("https://api.example.com/todos");
    print(response.data);
}

// Classes
class Person {
    func constructor(name) {
        this.name = name;
    }
    
    func greet() {
        print("Hello, " + this.name);
    }
}
```

## Core Features

### Variables and Types
- Dynamic typing
- Let declarations
- Basic types: numbers, strings, booleans, arrays, objects

### Functions
- First-class functions
- Anonymous functions
- Arrow function syntax
- Async functions

### Control Flow
- If/else statements
- Loops and iterations
- Pattern matching
- Error handling

### Built-in Libraries
- HTTP client
- Array operations
- Math utilities
- String manipulation
- JSON handling

## Examples

### HTTP Request
```qs
func fetchUser(id) {
    let response = get("https://api.example.com/users/" + id);
    if (response.status == 200) {
        print("User:", response.data);
    }
}
```

### Array Operations
```qs
let numbers = [1, 2, 3, 4, 5];
let sum = reduce(numbers, func(acc, n) { 
    return acc + n; 
}, 0);
```

### Classes and Objects
```qs
class Calculator {
    func add(a, b) { return a + b; }
    func subtract(a, b) { return a - b; }
}
```

## Contributing

Contributions are welcome! See our [Contributing Guide](CONTRIBUTING.md) for details.

## License

MIT License - See [LICENSE](LICENSE) for details.
