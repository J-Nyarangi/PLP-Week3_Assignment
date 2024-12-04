# PLP-Week3_Assignment Price Calculator
# Discount Calculator

This program calculates the final price of an item after applying a discount percentage if the discount is 20% or more. It takes user input for the original price and discount percentage and performs the necessary calculations.

---

## Features
- **Discount Validation**: Applies the discount only if it is 20% or more.
- **User Interaction**: Prompts the user to input the original price and discount percentage.
- **Dynamic Calculation**: Computes the discounted price or retains the original price based on the discount criteria.

---

## Requirements
- **Python 3.x**: Ensure Python is installed on your system.

---

## How It Works
1. **Input**: The program asks the user to provide:
   - The original price of the item.
   - The discount percentage.
2. **Logic**: 
   - If the discount percentage is 20% or more, the discount is applied.
   - Otherwise, the original price remains unchanged.
3. **Output**: 
   - Displays the final price after the discount, or
   - Informs the user that no discount was applied.

---

## Code Explanation

### Function: `calculate_discount(price, discount_percent)`
- **Parameters**:
  - `price`: The original price of the item (float).
  - `discount_percent`: The discount percentage (float).
- **Logic**:
  - If `discount_percent >= 20`, calculate the discounted price using the formula:
    \[
    \text{final\_price} = \text{price} - (\text{price} \times \frac{\text{discount\_percent}}{100})
    \]
  - Otherwise, return the original price.

### User Interaction
- Prompts the user for:
  - Original price (`original_price`).
  - Discount percentage (`discount_percent`).
- Calls `calculate_discount` to compute the final price.

### Output
- If a discount is applied, it prints:
  ```
  The final price after applying the discount is: <final_price>
  ```
- If no discount is applied, it prints:
  ```
  No discount applied. The original price is: <original_price>
  ```

---

## How to Run
1. Save the code to a file (e.g., `discount_calculator.py`).
2. Open a terminal and navigate to the file's location.
3. Run the program:
   ```
   python discount_calculator.py
   ```
4. Follow the prompts to input the original price and discount percentage.

---

## Example
**Input**:
```
Enter the original price of the item: 100
Enter the discount percentage: 25
```
**Output**:
```
The final price after applying the discount is: 75.0
```

**Input**:
```
Enter the original price of the item: 100
Enter the discount percentage: 15
```
**Output**:
```
No discount applied. The original price is: 100.0
```
