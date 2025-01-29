# WEPprojectCs346

## Introduction Product Management System (PMS) 

- This project is a CRUD-based Product Management System (PMS) designed for managing product data efficiently. It allows users to create, read, update, and delete (CRUD) product records, including details such as price, ads, taxes, discounts, and category.

- The system was built using MongoDB as a database, with a Node.js and Express.js backend to handle API requests. The frontend is powered by HTML, CSS, and JavaScript, making it a fully dynamic and interactive web application.


## Features
- Add Products – Users can input product details and save them to the database.
- View Products – Displays a table of all stored products dynamically fetched from MongoDB.
- Edit Products – Allows users to update existing product information.
- Delete Single Product – Removes a product from the database and updates the UI.
- Delete All Products – Clears the entire product list with one click.
- Search Functionality – Search by title or category to filter products in real-time.
- Automatic Calculations – The system dynamically calculates the total price based on taxes, ads, and discounts.


## You need:
- Database (MongoDB)

## Installation
- To install and run this project - install dependencies using npm and then start your server:
```
$ npm install
$ npm start
```
- To see your data in the server go to http://localhost:5000/api/products
- To see the web page go to index.html and open it
