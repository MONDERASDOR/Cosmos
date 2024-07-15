![Alt text](https://upload.wikimedia.org/wikipedia/commons/3/35/Cosmos_logo.png)

```markdown
# Cosmos 

Cosmos is a simple, custom programming language designed to demonstrate basic language features such as variables, arithmetic operations, loops, and function definitions. This language is built using Python and showcases how to create a lexer, parser, and evaluator for a custom syntax.

## Features

- **Variable Assignment**: Define and assign variables using `letCS`.
- **Arithmetic Operations**: Support for addition, subtraction, multiplication, and division.
- **Conditional Statements**: Use `ifCS` and `elseCS` for conditional logic.
- **Loops**: Support for `forCS` and `whileCS` loops.
- **Function Definitions**: Define and call functions using `functionCS`.
- **Print Statements**: Print output using `printCS`.

## Requirements

To run Cosmos, you need the following:

- **Python 3.x**: Ensure you have Python installed on your system. You can download it from [python.org](https://www.python.org/downloads/).

## Installation

1. **Clone the repository**:
   
   Cosmos isn't released yet but It will be officially released in this repository after a week. you can download it with git and use the simple tutorial down thare.Enjoy!

2. **Create and activate a virtual environment** (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. **Install dependencies** (if any):
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Create a Cosmos source file**:
   Create a file with the extension `.clang` (e.g., `test.clang`) and write your Cosmos code in it.

   Example `calculator.clang`:
   ```plaintext
   //CS Define addition function
   functionCS add(a, b) {
       return a + b;
   }

   //CS Define subtraction function
   functionCS subtract(a, b) {
       return a - b;
   }

   //CS Define multiplication function
   functionCS multiply(a, b) {
       return a * b;
   }

   //CS Define division function
   functionCS divide(a, b) {
       ifCS (b != 0) {
           return a / b;
       } elseCS {
           printCS("Error: Division by zero");
           return 0;
       }
   }

   //CS Use a loop to define repeated addition
   letCS sum = 0;
   forCS (letCS i = 0; i < 5; i = i + 1) {
       sum = add(sum, i);
   }
   printCS("Sum from 0 to 4: " + sum);

   //CS Perform arithmetic operations
   letCS result_add = add(10, 5);
   letCS result_subtract = subtract(10, 5);
   letCS result_multiply = multiply(10, 5);
   letCS result_divide = divide(10, 5);

   //CS Print results
   printCS("Addition: " + result_add);
   printCS("Subtraction: " + result_subtract);
   printCS("Multiplication: " + result_multiply);
   printCS("Division: " + result_divide);
   ```

2. **Run the Cosmos interpreter**:
   Execute the `main.py` script to interpret and run your Cosmos code:
   ```bash
   python main.py
   ```

   Ensure that the `main.py` script is in the same directory as your `.clang` file. The output will be printed to the console.

## Example

Here's an example of running the `calculator.clang` file:

```bash
python main.py
```

Output:
```plaintext
Sum from 0 to 4: 10
Addition: 15
Subtraction: 5
Multiplication: 50
Division: 2
```

## About the Creator

Cosmos was created by Monderasdor and enigma . The purpose of this project is to demonstrate how to build a simple programming language from scratch using Python. Feel free to contribute, fork, and modify the language as you see fit!

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
```
