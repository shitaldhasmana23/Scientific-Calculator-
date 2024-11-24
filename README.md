# Scientific-Calculator-

This Python script implements a scientific calculator with a graphical user interface (GUI) built using the ttkbootstrap library, which provides a modern and aesthetically pleasing look for Tkinter widgets. The calculator includes both basic and advanced functionalities, as well as enhancements like memory operations, keyboard input, and full-screen support.

Key Features
1- Basic Arithmetic:

    - Standard operations such as addition, subtraction, multiplication, and division.
    - Buttons for numerical input (0-9) and common symbols like . (decimal point), = (equals), ( and ) (parentheses).
2- Scientific Functions:

    - Buttons for advanced operations like sin, cos, tan, log, ln, x² (square), √x (square root), 1/x (reciprocal), and exponential functions (exp).
    - Constants like π (pi) and e (Euler's number).
3- Error Handling:

    - Ensures invalid expressions are caught and displays a clear error message (Invalid Expression).
4- Memory Operations:

    - MC (Memory Clear): Clears the stored memory value.
    - MR (Memory Recall): Recalls the stored memory value.
    - M+ (Memory Add): Adds the current value to the stored memory.
    - M- (Memory Subtract): Subtracts the current value from the stored memory.
5- Dynamic Layout:

    - Buttons dynamically adjust their size to fit the screen using grid configurations.
    - The 0 button spans two columns for better alignment and aesthetic balance.
6- Keyboard Input:

    - Users can input values and operators directly from the keyboard for convenience.
7- Full-Screen Support:

    - The application can toggle full-screen mode using the F11 key.
    - Exiting full-screen mode is possible using the Escape key.
8- Modern Styling:

    - Buttons and the entry box are styled with ttkbootstrap themes, providing a sleek and responsive design.
    - Different button categories (e.g., danger for C, success for =, primary for scientific functions) are styled accordingly.


.....Structure and Logic......


Initialization

- The main window (root) is initialized with the darkly theme from ttkbootstrap.
- The entry box is added at the top to display user inputs and results.
  
Functions

-- Core Functions:
 
    - clear(): Clears the entry field.
    - backspace(): Deletes the last character in the entry field.
    - append_char(char): Appends a character to the entry field, replacing 0 if it’s the first character.
    - evaluate_expression(): Evaluates the mathematical expression in the entry field using eval().
-- Special Operations:

    - calculate_special(func): Handles advanced operations (e.g., trigonometric functions, square root, logarithms).
-- Memory Functions:

    - Functions like memory_clear(), memory_recall(), memory_add(), and memory_subtract() manage a global variable (memory_value) for storing and recalling numbers.

Button Layout
-- Buttons are dynamically created and added to a grid layout using a list of tuples. Each tuple defines:
    - Button text, grid row, grid column, and optional rowspan/colspan for spanning multiple rows or columns.
-- Buttons are styled and mapped to their respective functions using lambda expressions.

Grid Configuration

-- The grid layout ensures that buttons are responsive and adjust to the window size.
    - Five columns and nine rows (including the entry box) are configured with equal weight for uniform resizing.

Full-Screen Behavior

  - F11 toggles full-screen mode for better visibility.
  - Escape exits full-screen mode.
    
Use Case

This calculator is ideal for users who need a versatile tool for both basic and scientific computations. The dynamic layout, modern design, and additional features like memory operations and keyboard support make it user-friendly and efficient for everyday use.
