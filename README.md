# BAMAZON

An Ebay-like store front using Node.js and MySQL.

## Getting Started

- Clone repo.
- Using Terminal or Gitbash, run 'npm install'
- Then run these commands:
    * Customer - 'node bamazonCustomer,js'
    * Manager - 'node bamazonManager.js'
    * Exective - 'node bamazonSupervisor.js'
- Run 'ctrl + c' to exit each mode

## Running the application

1. `bamazonCustomer.js`

    * Prints the products in the store.

    * Ask them the ID of the product they would like to buy

    * Asks for the quantity.

      * If there is a sufficient amount of the product in stock, it will return the total for that purchase.
      * However, if there is not enough of the product in stock, it will tell the user that there isn't enough of the product.
      * If the purchase goes through, it updates the stock quantity to reflect the purchase.
      * It will also update the product sales in the department table.

-----------------------

2. `bamazonManager.js`

    * Running this application will list a set of menu options:
        * View Products for Sale
        * View Low Inventory
        * Add to Inventory
        * Add New Product

    * If the manager selects `View Products for Sale`, it lists all of the products in the store including all of their details.

    * If the manager selects `View Low Inventory`, it'll list all the products with less than five items in its StockQuantity column.

    * If the manager selects `Add to Inventory`, it allows the manager to select a product and add inventory.

    * If the manager selects `Add New Product`, it allows the manager to add a new product to the store.


-----------------------

3. `bamazonSupervisor.js`

    *  Running this application will list a set of menu options:
        * View Product Sales by Department
        * Create New Department


    * If the manager selects `View Product Sales by Department`, it lists the Department Sales and calculates the total sales from the overhead cost and product sales.

    * If the manager selects `Create New Department`, it allows the manager to create a new department and input current overhead costs and product sales. If there are none, by default it will set at 0.


## Technologies used
- Node.js
- Inquire NPM Package (https://www.npmjs.com/package/inquirer)
- MySQL Workbench
