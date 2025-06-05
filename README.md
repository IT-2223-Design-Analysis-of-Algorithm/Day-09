# Day-09

# 📘 MATLAB Function Collection – README

This script demonstrates different types of MATLAB functions with examples of:
- No input/output
- Single and multiple inputs/outputs
- Interactive input handling
- Inline factorial logic

---

## 🔹 1. getPi – No Input, One Output
```matlab
function piValue = getPi()
    piValue = 3.1416;
end
```
Returns an approximate value of π.  
**Usage:** `val = getPi();`

---

## 🔹 2. addNumbers – Two Inputs, One Output
```matlab
function sum = addNumbers(a, b)
    sum = a + b;
end
```
Adds two numbers.  
**Usage:** `result = addNumbers(5, 10);`

---

## 🔹 3. Factorial Calculation – Inline Script
```matlab
x = input('Enter the number: ');
fact = 1;
for i = 1:x
    fact = fact * i;
end
disp(['Factorial: ', num2str(fact)]);
```
Takes user input and prints the factorial.

---

## 🔹 4. greeting – Input Only, No Output
```matlab
function greeting(name)
    disp(['Hello ', name]);
end
```
Displays a greeting message.  
**Usage:** `greeting('Alice');`

---

## 🔹 5. operations – Two Inputs, Multiple Outputs
```matlab
function [sum, sub, mul, div] = operations(x, y)
    sum = x + y;
    sub = x - y;
    mul = x * y;
    div = x / y;
end
```
Performs all four basic operations.  
**Usage:**
```matlab
[sum, sub, mul, div] = operations(20, 10);
```
🔸 If you use `operations(20, 10)` without brackets, only the sum is returned.

---

## ✅ Summary Table

| Function      | Inputs | Outputs     | Description                        |
|---------------|--------|-------------|------------------------------------|
| `getPi`       | None   | π value     | Returns a constant value           |
| `addNumbers`  | 2      | 1 (sum)     | Adds two numbers                   |
| Factorial     | 1      | 1 (factorial) | Calculates factorial from input   |
| `greeting`    | 1      | None        | Displays greeting message          |
| `operations`  | 2      | 4 (sum,sub,mul,div) | All basic arithmetic ops    |
