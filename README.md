# Supermarket Inventory Management System

![Interface screenshot of supermarket inventory management system](doc/mockup/mockup.jpg)

This Python script offers a comprehensive solution for managing supermarket inventory. Utilizing the `openpyxl` library for Excel operations and `colorama` for enhanced terminal output, this script enables users to perform a variety of inventory management tasks. Key features include adding, updating, deleting items, searching items by name or category, and providing low stock alerts and expiration date warnings.

## Features

### General
- **Display Inventory**: View the entire inventory with details like item name, category, price, expiration date, and quantity.
![Screenshot showing inventory list with item details](doc/features/01-inventory.jpg)

- **Inventory Summary**: Get a summary of the inventory, including total items and quantities.

![Image of inventory summary with total items and quantities](doc/features/07-summary.jpg)
- **Low Stock Alert**: Receive alerts for items with low stock.

![Alert screen for low stock items](doc/features/08-low-stock.jpg)

- **Expiration Date Warning**: Get warnings for items nearing their expiration date.
![Warning screen for items nearing expiration](doc/features/09-date.jpg)

### Interactive Features with 'Cancel' Option
In several functions, users have the flexibility to exit the process at any time by typing "cancel". This feature is available in:
- **Add Item**: Add new items to the inventory. Type 'cancel' at any input prompt to exit.
![Interface for adding new inventory items](doc/features/02-add.jpg)

- **Update Item Details**: Modify existing item details. Type 'cancel' at any input prompt to exit.
![Screen for modifying inventory item details](doc/features/03-update.jpg)

- **Delete Item**: Remove items from the inventory. Includes a YES/NO confirmation prompt to prevent accidental deletions. Type 'cancel' to exit the prompt.
![Confirmation screen for deleting inventory items](doc/features/04-delete.jpg)

- **Search for an Item**: Look up items by name. Type 'cancel' to exit the search.
![Item search interface screenshot](doc/features/05-search-item.jpg)

- **Search by Category**: Find items based on their category. Type 'cancel' to exit the search.
![Category search interface in inventory system](doc/features/06-search-category.jpg)

## Installation

1. Clone the repository:
   ```bash
   git clone [URL to your repository]
   ```
2. Install the required packages:
   ```bash
   pip install openpyxl colorama
   ```

## Usage

Run the script using Python:
```bash
python inventory_management.py
```

You will be prompted to authenticate before accessing the inventory management functionalities.

## User stories
- As a store manager, I want to view the entire inventory so that I can have a clear understanding of all items available in the store.

- As a store clerk, I want to add new items to the inventory system quickly, ensuring that all recent purchases are tracked and accounted for.

- As an inventory manager, I want to update item details in the inventory to ensure all information is current and accurate, including prices, categories, and quantities.

- As a store owner, I want to delete items from the inventory system that are no longer available or have been discontinued.

- As a store supervisor, I want to search for items by name to find specific products quickly and check their details like price, quantity, and expiration date.

- As a stock manager, I want to search inventory by category so that I can get a better overview of items grouped under a specific category.

- As a store manager, I need to view a summary of the inventory to get insights into the total number of items, total quantity, and category-wise distribution.

- As a store assistant, I want to receive alerts for items with low stock, ensuring timely restocking and preventing stockouts.

- As a quality control officer, I want to get warnings for items nearing their expiration date to manage inventory rotation and reduce waste.

- As a new employee, I want to access the system using my credentials to ensure security and track my inventory management activities.

## Authentication

For trial purposes, you can log in using the username `user1` and the password `password1`. The script uses a simple authentication system with predefined usernames and passwords. Update the `authenticate_user` function to modify or extend the authentication logic.

![Login screen with username and password fields](doc/aut/username-password.jpg)
![Screen displaying successful login message](doc/aut/aut-successful.jpg)
![Screen showing login failure message](doc/aut/aut-failed.jpg)

## Validation
![Screenshot of validation](doc/check/validation.jpg)

## Data Storage

The inventory data is stored in an Excel file (`inventory.xlsx`). Ensure this file exists in the same directory as the script, or modify the `file_name` variable in the script to point to the correct file location.

## Customization

You can customize the script by modifying the source code to better fit your specific inventory management needs.

## Contributions

Contributions to this project are welcome. Please open an issue or submit a pull request with your proposed changes.

## Credits

Developed by Igor Dinuzzi.
