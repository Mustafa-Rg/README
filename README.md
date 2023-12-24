# Personal sales manager
#### Video Demo:  https://youtu.be/GWB7tcf7SzY?si=aOgtElGSFgIgClFp
#### Description:
This web app’s job is to handle the sales, products and buyers (custumers) to store, and output them and it is created using HTML, CSS, Javascript, Python (Flask) and SQL.

### Project Structure and Components
#### Python Files:
##### app.py: This is the backend file for the web app. It contains 9 routes:
###### /: The home route that returns home.html. It doesn't have any functionality because JavaScript is used for the home page.
###### /login: It compares the hashed password typed in login.html with the hash stored in project.db.
###### /logout: It simply clears the session.
###### /add_buyer: Takes input from add_buyer.html and stores it in the "buyers" table in project.db.
###### /add_product: Takes input from add_product.html and stores it in the "products" table in project.db.
###### /add_purchase: Takes input from add_purchase.html and stores every detail about the purchase in the "sales" table in project.db.
###### /data, /pros, and /sales: Their job is to send data to script files.


