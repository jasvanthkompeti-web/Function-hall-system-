# ROYAL FUNCTION HALL — END-TO-END APPLICATION

## Technology
Frontend: HTML5 + CSS3 + JavaScript
Node: static frontend server + API gateway
Java: HTTP backend
JDBC: database access
MySQL: persistent database

## Full flow
Register/Login
 -> Halls
 -> Chairs/Tables/Decoration
 -> Veg/Non-Veg food
 -> Cart
 -> Checkout
 -> Demo payment method
 -> Java JDBC
 -> MySQL
 -> My Bookings
 -> Admin Dashboard

## Requirements
Install:
1. JDK 17+
2. Node.js
3. MySQL 8+
4. MySQL Connector/J JAR

Put `mysql-connector-j-*.jar` in this folder.

## Configure
Open BookingServer.java and change:
DB_USER="root";
DB_PASS="root";
to your MySQL credentials.

## Run Java backend
Windows:
javac BookingServer.java
java -cp ".;mysql-connector-j-9.4.0.jar" BookingServer

Linux/Mac:
javac BookingServer.java
java -cp ".:mysql-connector-j-9.4.0.jar" BookingServer

## Run Node
Open a second terminal:
node server.js

Open:
http://localhost:3000

## Admin
Open:
http://localhost:3000/admin.html

## Important
The payment options are DEMO payment methods. No real money is charged.
For a production application, integrate a real payment gateway, HTTPS, proper password hashing/salt, sessions/JWT, validation and authorization.

## Files
index.html
halls.html
food.html
cart.html
checkout.html
login.html
bookings.html
admin.html
style.css
app.js
server.js
BookingServer.java
schema.sql
package.json
README.md
