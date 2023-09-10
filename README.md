## Quadratic Equation Solver

This script builds a quadratic equation solver GUI that takes input coefficients (a, b, and c) from the user, solves the quadratic equation, and displays the roots along with the type of roots (real or complex) in a label widget.


---

The Required Modules For The Files To Be Executed Are :

1. Tkinter Module - Make a GUI for a program.


_To install tkinter, run the following in command prompt :_


```python
    pip install tk
```

2. Math Module - It is a built in module, for arthmetic operations.
3. CMath Module - It is a built in module, for complex arthmetic operations.

---

_The Breakdown Of Code Is Given Below :_


> 1. The first step is to import the required modules and libraries for building the GUI and performing mathematical calculations. In this code, the `tkinter` module is imported for creating the graphical user interface, and the `cmath` and `math` modules are imported for handling complex numbers and mathematical calculations, respectively.
>    
> 2. The code defines a function named `solve_quadratic(a, b, c)` to solve the quadratic equation. This function takes three parameters representing the coefficients of the quadratic equation (a, b, and c). It calculates the discriminant (d) using the formula `b**2 - 4*a*c`. Then, it calculates the two roots of the quadratic equation using the quadratic formula and returns them.
> 
> 3. The code defines a function named `on_button_click()` which is called when the "Solve" button is clicked. Inside this function, it retrieves the values entered in the input fields for coefficients a, b, and c. It then recalculates the discriminant `d` using the formula `b**2 - 4*a*c`.
> 
> 4. Based on the value of the discriminant `d`, the code determines the type of roots: real or complex. If `d` is greater than 0, it means the equation has real roots. It calls the `solve_quadratic(a, b, c)` function to calculate the roots and converts the roots into a string (sroot). The label widget is updated with the roots and the type of roots is set as "Roots: Real".
>       If `d` is less than 0, it means the equation has complex roots. In this case, it defines another function named `solve_complex_quadratic(a, b, c)` which calculates the complex roots using the `cmath` module. The label widget is updated with the complex roots and the type of roots is set as "Roots: Non-Real".
> 
> 5. The code creates a GUI window using the `tkinter` module and sets its dimensions and title. It creates various elements such as labels, entry fields, buttons, and frames using the tkinter methods like `Label()`, `Entry()`, `Button()`, etc. These elements are then organized and arranged in the window using grid layout (`grid()`) and pack layout (`pack()`) methods. The GUI window is displayed by calling the `mainloop()` method.
