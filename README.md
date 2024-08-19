<h1> Ordered Calculator Using Stack Method </h1>
A calculator that has an order of operations using the stack method that receives the input from the user and extracts the operands and operators, performs calculations by using a stack to arrange the operations, and finally gives out the results on the screen. The order that is used to simplify expressions is called the order of operations, by following this order, we can solve all the problems using PEMDAS which stands for:

P – Parentheses 
E - Exponents
M - Multiplication
D - Division
A - Addition
S - Subtraction



| **Command**       | **Description**                                                                                   |
| ----------------- | ------------------------------------------------------------------------------------------------- |
| `isOperator`      | Returns `true` if the user input is one of the valid operators (`+`, `-`, `*`, `/`).            |
| `getPrecedence`   | Assigns precedence levels to operators to determine their order of evaluation. Higher precedence operators are evaluated before lower precedence ones. |
| `processOperator` | Defines variables `OP1` and `OP2`. Check if the stack is empty using `isEmpty()`. If empty, display "Expression error" and set `error` to `true`. If not empty, assigns top stack values to `a` and `b`, computes the result based on the operator, and pushes the result back to the stack. |
| `processInput`    | Creates a `String` array for the expression. Iterates through tokens pushes numbers to the value stack, handles operators and parentheses, checks for unbalanced parentheses errors, and processes the operator stack to print the result if no errors are found. |
| `Main`            | Prompts the user to input an expression, creates a `FullCalculator` object, and calls `processInput` to evaluate the expression and display the result. |
| `stack<Character>`| A stack used to handle operators and parentheses.                                                |
| `stack<Double>`   | A stack used to handle numeric values during computation.                                         |
| **Notes on Stack Usage** | Uses `push()`, `pop()`, and `isEmpty()` methods for stack operations. `Peek()` is used instead of `top`. |
