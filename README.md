# DesmosProject
ICS project
Input → Tokenization → Parsing (Postfix) → Evaluation → Data Output → Plotting
Capabilities

* Expression parsing with correct operator precedence and associativity
* Support for standard mathematical operators: +  -  *  /  ^
* Built-in functions:
* Trigonometric: sin, cos, tan
* Inverse trig: asin, acos, atan
* Exponential / logarithmic: exp, ln, log, log2
* Roots: sqrt, cbrt
* Constants: pi, e
* Implicit multiplication handling (e.g., 2x, xsin(x), 3(x+1))
* Numerical evaluation over configurable ranges
* Export of computed points for external visualization

Architecture

The system is divided into three independent layers:

1. Tokenization

Converts raw input strings into structured tokens (numbers, operators, functions, variables).

2. Parsing

Implements the Shunting Yard Algorithm to convert infix expressions into postfix (RPN) form.

3. Evaluation

Evaluates the postfix expression for a sequence of x values and generates (x, y) pairs.

4. Visualization

A separate Python script (plot.py) reads generated data and renders graphs using matplotlib.
