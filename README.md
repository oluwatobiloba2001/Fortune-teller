# Random Fortune Generator

This project is a simple JavaScript program that generates a random fortune from a predefined list of fortunes. It uses the `Math.random()` method to create a random number and assigns the corresponding fortune to the `selectedFortune` variable based on the generated number.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Usage](#usage)
- [How It Works](#how-it-works)
- [Code Walkthrough](#code-walkthrough)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The Random Fortune Generator is a beginner-friendly JavaScript project that demonstrates:
- Random number generation.
- Conditional logic with `if-else` statements.
- Assignment of values based on dynamic conditions.

## Features

- Generates a random fortune based on a set of predefined fortunes.
- Ensures each fortune is equally likely to be selected.
- Outputs the random number and the selected fortune.

## Usage

1. Copy the code into a JavaScript environment (e.g., Node.js, browser console, or online JavaScript editor).
2. Run the code to generate a random fortune.

## How It Works

1. Five fortunes are predefined as string variables (`fortune1` to `fortune5`).
2. A random number between 1 and 5 is generated using `Math.random()` and assigned to `randomNumber`.
3. Conditional logic (`if-else`) is used to select the appropriate fortune based on the value of `randomNumber`.
4. The program outputs the random number and the selected fortune.

## Code Walkthrough

### Defining the Fortunes

```javascript
const fortune1 = "Your cat will look very cuddly today.";
const fortune2 = "The weather will be nice tomorrow.";
const fortune3 = "Be cautious of your new neighbors.";
const fortune4 = "You will find a new hobby soon.";
const fortune5 = "It would be wise to avoid the color red today.";
```

Five unique fortunes are stored as string variables.

### Generating the Random Number

```javascript
const randomNumber = Math.round(Math.random() * (5 - 1)) + 1;
```

- `Math.random()` generates a pseudo-random number between 0 and 1.
- It is scaled and rounded to create an integer between 1 and 5.

### Selecting the Fortune

```javascript
let selectedFortune;
if (randomNumber === 1) {
  selectedFortune = fortune1;
} else if (randomNumber === 2) {
  selectedFortune = fortune2;
} else if (randomNumber === 3) {
  selectedFortune = fortune3;
} else if (randomNumber === 4) {
  selectedFortune = fortune4;
} else {
  selectedFortune = fortune5;
}
```

Conditional logic assigns the correct fortune to the `selectedFortune` variable.

### Outputting the Result

```javascript
console.log(randomNumber);
console.log(selectedFortune);
```

The random number and selected fortune are displayed in the console.

## Example Output

```
4
You will find a new hobby soon.
```

## Contributing

If you’d like to add more fortunes or improve the logic, feel free to fork this repository and submit a pull request.

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute this project as needed.

---

**Enjoy discovering your random fortune!**
