# Project-Software-engineering

### Backend :
The backend is a RESTful API built with Express.js. It provides endpoints for managing data related to "bankers" and "customers". It also includes a health-check route for confirming that the server is running.

for the endpoints :
- /api/bankers : Serves data related to bankers.
  Returns a JSON array of banker objects, each containing properties like name, ID, role, etc.
- /api/customers : Similar to bankers, this endpoint would serve customer-related data.
- /health : Simple GET endpoint for checking server health. Returns : {"message": "Server is healthy!"}

The server listens on port 3000 and is accessible locally at http://localhost:3000

### Frontend : 
The frontend is a basic HTML/JavaScript page using Axios for AJAX requests to the backend API. It populates a table with data from the /api/bankers endpoint upon page load.

for the features :
- Fetches banker data from the backend.
- Displays the data in a dynamically created HTML table.
- Displays an error message if the API call fails.

for the main web page :
- Header: "Bankers Management Dashboard" (a simple title at the top).
- Table: Below the header, there's a table with the following structure:
    Columns: Depends on the properties of banker objects (e.g., Name, ID, Role).
    Rows: Populated dynamically from the API response.
  
for the error Display :
If the API call fails, a red alert box with the message "Error fetching data. Please try again later." appears.

### User's guide :
#### Step 1 : start the backend
On node.js :
Test the connection to the database
    node testConnection.js
Start the backend server
    node app.js
Verify that the server is running :
    Open a browser and go to http : //localhost:3000/health.
    You should see the message : "Server is healthy!"

#### step 2 start the frontend
on node.js :
Install a lightweight HTTP server
    npm install -g http-server
    http-server
Once the server starts, you will see a URL (e.g., http://localhost:8080).
Open this URL in your browser to view the frontend application.

