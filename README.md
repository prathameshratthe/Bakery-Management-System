# Bakery Order Management System

## Overview

The Bakery Order Management System is a simple command-line application designed to help manage orders for a bakery. The system allows users to add, view, update, and save orders to an Excel file. This application is implemented using Python and the pandas library.

## Features

- **Add Order**: Add a new order by providing the customer name, item ordered, quantity, and the order date is automatically set to the current date.
- **View Orders**: Display all the orders in a tabular format.
- **Update Order**: Update an existing order's item and quantity based on the order ID.
- **Save to Excel**: Save all the orders to an Excel file named `bakery_orders.xlsx`.

## Installation

1. Clone the repository or download the code.
2. Ensure you have Python installed (preferably version 3.6 or higher).
3. Install the required library by running:
   ```sh
   pip install pandas
   ```

## Usage

1. Run the `bakery_order_management.py` file.
   ```sh
   python bakery_order_management.py
   ```
2. Follow the on-screen instructions to interact with the system:
   - **1. Add Order**: Add a new order.
   - **2. View Orders**: View all existing orders.
   - **3. Update Order**: Update an order using its order ID.
   - **4. Save to Excel**: Save all orders to an Excel file.
   - **5. Exit**: Exit the application.

## Code Explanation

### Class: BakeryOrderManagement

- **`__init__`**: Initializes an empty DataFrame to store orders.
- **`add_order`**: Prompts the user to input customer name, item ordered, and quantity, then adds the order to the DataFrame.
- **`view_orders`**: Displays the DataFrame containing all orders.
- **`update_order`**: Updates an existing order based on the order ID provided by the user.
- **`save_to_excel`**: Saves the DataFrame containing all orders to an Excel file.

### Main Loop

- The main loop continuously prompts the user to select an action (add, view, update, save, or exit) and calls the corresponding method of the `BakeryOrderManagement` class based on the user's choice.

## Example

```sh
1. Add Order
2. View Orders
3. Update Order
4. Save to Excel
5. Exit
Enter your choice: 1
Enter customer name: John Doe
Enter item ordered: Chocolate Cake
Enter quantity: 2
Order added successfully!

Enter your choice: 2
  Customer Name          Item  Quantity  Order Date
0      Prathamesh  Chocolate Cake     2  2024-07-17

Enter your choice: 4
Orders are saved to 'bakery_orders.xlsx'.
```

## License

This project is licensed under the MIT License.

---
Created by @prathameshratthe
