Travel Tracker Project README
Description
This is a simple web application built with Node.js and Express that allows users to track the countries they have visited. Users can input a country name, and if it exists in the database, it will be added to their visited countries list. The application uses PostgreSQL as its database to store information about countries and visited countries.

Prerequisites
Before running this application, ensure you have the following installed on your system:

Node.js
PostgreSQL
Installation
Clone this repository to your local machine:
bash
Copy code
git clone <repository_url>
Navigate to the project directory:
bash
Copy code
cd <project_directory>
Install dependencies using npm:
Copy code
npm install
Database Setup
Ensure PostgreSQL is installed and running on your system.
Create a new database named World in PostgreSQL.
Import the SQL file world.sql into the World database. This file contains tables and sample data for countries.
Configuration
Open the index.js file.
Modify the PostgreSQL connection settings in the db object to match your PostgreSQL setup:
user: PostgreSQL username
host: PostgreSQL host (default is localhost)
database: Name of the PostgreSQL database (World)
password: PostgreSQL password
port: PostgreSQL port (default is 5432)
Usage
Start the application:
sql
Copy code
npm start
Open your web browser and go to http://localhost:3000 to access the application.
Enter a country name in the input field and click the "Add" button to add it to your visited countries list.
The list of visited countries will be displayed on the homepage.
Features
Add countries to the visited list.
Error handling for non-existent country names or already visited countries.
Technologies Used
Node.js
Express.js
PostgreSQL
EJS (Embedded JavaScript) for templating
body-parser middleware for parsing incoming request bodies
