# Functional Programming Spreadsheet

## Introduction

Welcome to the **Functional Programming Spreadsheet** project! This application is a web-based tool that mimics the functionality of a basic spreadsheet, allowing users to input, calculate, and manipulate data using formulas and functions. It leverages the power of JavaScript's functional programming paradigm to create a dynamic and efficient user experience.

Whether you're performing basic arithmetic, calculating averages, or working with ranges of cells, this spreadsheet application provides a clean and intuitive interface to manage your data.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Usage](#usage)
  - [Entering Formulas](#entering-formulas)
  - [Supported Functions](#supported-functions)
  - [Handling Cell Ranges](#handling-cell-ranges)
  - [CSS Customization](#css-customization)
- [Example Formulas](#example-formulas)
- [License](#license)
- [Contributing](#contributing)



This project is a simple spreadsheet-like web application that utilizes functional programming concepts in JavaScript. It allows users to input formulas, perform arithmetic operations, and manipulate ranges of cells.

## Features

- **Basic Arithmetic Operations**: Supports addition, subtraction, multiplication, and division.
- **Range Handling**: Expand ranges of cells and apply functions across them.
- **Dynamic Cell Updates**: Automatically updates cell values based on input formulas.
- **Flashy CSS**: Modern, vibrant UI with smooth animations and interactive elements.

## Usage

### Entering Formulas

- To perform operations in a cell, type `=` followed by your formula.
- For example, to sum two numbers in cells A1 and B1, enter `=SUM(A1, B1)` in the desired cell.
- Formulas can involve basic arithmetic operations, cell references, or built-in functions.

### Supported Functions

The spreadsheet supports a variety of built-in functions, including:

- **`SUM(nums)`**: Returns the sum of the given numbers or range.
  - Example: `=SUM(A1:A5)` will sum the values in cells A1 through A5.

- **`AVERAGE(nums)`**: Calculates the average of the provided numbers or range.
  - Example: `=AVERAGE(A1, B1, C1)` will return the average of the values in A1, B1, and C1.

- **`MEDIAN(nums)`**: Finds the median of the given numbers or range.
  - Example: `=MEDIAN(A1:A5)` will return the median value from cells A1 through A5.

- **`INCREMENT(nums)`**: Increments each value in the specified range or list by 1.
  - Example: `=INCREMENT(A1:A5)` will return the values in A1 through A5, each incremented by 1.

- **`RANDOM([x, y])`**: Generates a random number starting from the smaller of the first two numbers and ending just before their sum.
  - Example: `=RANDOM([2, 5])` could return a random number between 2 and 6.

- **`NODUPES(nums)`**: Removes duplicate values from the given range or list.
  - Example: `=NODUPES(A1:A5)` will return the unique values from A1 through A5.

### Handling Cell Ranges

- You can specify a range of cells using a colon `:` between the starting and ending cell references.
  - Example: To sum the values from A1 to A5, you would enter `=SUM(A1:A5)`.

- Formulas can also mix individual cells and ranges.
  - Example: `=SUM(A1, B2:B5)` will sum the value in A1 with the sum of the values in cells B2 through B5.

### CSS Customization

The spreadsheet comes with a default CSS file that styles the layout and appearance of the grid. You can customize the look and feel of the application by modifying the `styles.css` file.

- **Background Color**: Change the grid or label background color to match your design preference.
- **Grid Layout**: Adjust the `grid-template-columns` and `grid-template-rows` properties to change the size of the cells.
- **Animations**: Add or modify animations to make the spreadsheet more interactive.


## Example Formulas

### Basic Arithmetic

- **Addition**: `=A1 + B1` adds the values in cells A1 and B1.
- **Subtraction**: `=A1 - B1` subtracts the value in cell B1 from A1.
- **Multiplication**: `=A1 * B1` multiplies the values in cells A1 and B1.
- **Division**: `=A1 / B1` divides the value in A1 by the value in B1.

### Using Built-in Functions

- **Sum of a Range**: `=SUM(A1:A5)` adds all the values in cells A1 through A5.
- **Average of a Range**: `=AVERAGE(A1:A5)` calculates the average of the values in cells A1 through A5.
- **Median of a Range**: `=MEDIAN(A1:A5)` finds the median value of the range A1 through A5.
- **Incrementing Values**: `=INCREMENT(A1:A5)` increments each value in cells A1 through A5 by 1.
- **Random Number**: `=RANDOM([2, 5])` generates a random number between 2 and 6.

### Complex Formulas

- **Combining Functions**: `=SUM(A1:A5) / COUNT(A1:A5)` calculates the average by dividing the sum of A1 to A5 by the count of cells in the range.
- **Nested Functions**: `=MEDIAN(SUM(A1, B1), SUM(C1, D1))` sums A1 and B1, sums C1 and D1, and then returns the median of these two sums.

## Advanced Features

### Formula Parsing and Evaluation

The spreadsheet supports advanced formula parsing with the following features:

- **High Precedence Handling**: The spreadsheet handles multiplication and division before addition and subtraction, similar to standard mathematical precedence.
- **Custom Functions**: You can create your own functions and add them to the `spreadsheetFunctions` object.

### Extending Functionality

- You can extend the spreadsheet by adding new functions to the `spreadsheetFunctions` object.
  - Example: Add a custom function to calculate the variance of a range.

### Debugging Tips

- If your formula isn't working as expected, make sure it's correctly formatted.
- Use `console.log()` in the JavaScript file to debug custom functions.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Contributing

Contributions are welcome! If you'd like to contribute, please fork the repository and create a pull request with your changes. For major changes, please open an issue first to discuss what you would like to change.

