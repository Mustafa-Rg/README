# Personal sales manager
#### Video Demo:  https://youtu.be/GWB7tcf7SzY?si=aOgtElGSFgIgClFp
#### Description:
This web app’s job is to handle the sales, products and buyers (custumers) to store, and output them and it is created using HTML, CSS, Javascript, Python (Flask) and SQL.

### Project Structure and Components:
#### Python Files:

app.py: This is the backend file for the web app. It contains 9 routes:

/: The home route that returns home.html. It doesn't have any functionality because JavaScript is used for the home page.

/login: It compares the hashed password typed in login.html with the hash stored in project.db.

/logout: It simply clears the session.

/add_buyer: Takes input from add_buyer.html and stores it in the "buyers" table in project.db.

/add_product: Takes input from add_product.html and stores it in the "products" table in project.db.

/add_purchase: Takes input from add_purchase.html and stores every detail about the purchase in the "sales" table in project.db.

/data, /pros, and /sales: Their job is to send data to script files.

#### Database: 

project.db: This is a database file (SQLite) that includes four tables:

"buyers": Stores buyer information.

"products": Stores product information.

"sales": Stores details about each purchase.

"pass": Stores the hash of the password "Project".

#### HTML Files (stored in the "templates" directory):

home.html: Home page of the web app. It displays a table with product details, including price, quantity sold, and total earnings for each product. It also provides the total earnings of all products combined at the end.

login.html: Login page for authentication.

add_buyer.html: Form for adding buyer information.

add_product.html: Form for adding product information.

add_purchase.html: Form for adding purchase details.

base.html: This the main layout for the web app.

apology.html: When an error occurs it shows the type of the error.

#### JavaScript Files (stored in the "static" directory):

homesScript.js: This JavaScript file is specific to home.html. It retrieves data from the "sales" and "pros" routes and uses functions to output a table in home.html with product details, including price, quantity sold, and total earnings. It also calculates the total earnings of all products combined.

purchaseScript.js: This JavaScript file is specific to add_purchase.html. It retrieves data from the "pros" and "data" routes and provides interactivity to the page. It enables search functionality for selecting buyers and products.

script.js: This JavaScript file is applied to all HTML files. Its main function is to make the navbar items active when used.

#### CSS File (stored in the "static" directory):

styles.css: This file styles all the pages. It is not very complicated, and it uses black and white colors for a cool aesthetic.





