# README
Project Structure and Components:
Python Files:

app.py: This is the backend file for the web app, containing 9 routes:
"/": The home route that returns home.html and includes JavaScript functionality.
"/login": Compares the hashed password typed in login.html with the hash stored in project.db.
"/logout": Clears the session.
"/add_buyer": Takes input from add_buyer.html and stores it in the "buyers" table in project.db.
"/add_product": Takes input from add_product.html and stores it in the "products" table in project.db.
"/add_purchase": Takes input from add_purchase.html and stores the purchase details in the "sales" table in project.db.
"/data": Sends data to script files.
"/pros": Sends data to script files.
"/sales": Sends data to script files.
helpers.py: Copied from the Finance project, containing some functions used by app.py.
Database:

project.db: A SQLite database containing four tables:
"buyers": Stores buyer information.
"products": Stores product information.
"sales": Stores details about each purchase.
"pass": Stores the hash of the password "Project".
HTML Files (stored in the "templates" directory):

home.html: Home page of the web app, displays a table with product details and total earnings.
login.html: Login page for authentication.
add_buyer.html: Form for adding buyer information.
add_product.html: Form for adding product information.
add_purchase.html: Form for adding purchase details.
(Remaining HTML files not specified)
JavaScript Files (stored in the "static" directory):

homesScript.js: JavaScript file specific to home.html. Retrieves data from "sales" and "pros" routes to populate a table with product details and total earnings.
purchaseScript.js: JavaScript file specific to add_purchase.html. Retrieves data from "pros" and "data" routes to provide interactivity and search functionality for selecting buyers and products.
script.js: JavaScript file applied to all HTML files, responsible for making the navbar items active.
CSS File (stored in the "static" directory):

styles.css: Stylesheet that provides styling for all pages, predominantly in black and white.
