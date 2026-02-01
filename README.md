
# Prompt Engneering

## Projects  
### Loveable 
# P_1: Meter Reading Save & Calculate
#### No. 1 Prompt
You need a meter reading tracking system with the following columns in a table:
#### Date
- Meter Name
- Previous Reading
- Present Reading
- Total (Present – Previous) → Calculated column
- Description
- Actions (Edit, Delete, etc.)
#### Core Features:

- CRUD operations (Create, Read, Update, Delete entries)
- Automatic calculation of Total
- Data persistence (save to database)
- Web interface to view/add/edit data

### No. 2 Prompt
#### Prompt 1: 
System Design & Tech Stack Suggestion
“I need to build a meter reading tracking web app with CRUD functionality. Required table columns: Date, Meter Name, Previous Reading, Present Reading, Total (calculated), Description, Actions. Data must be saved persistently.
Suggest a simple full-stack tech stack for a beginner-friendly implementation, and outline the database schema.”

Expected output:

Recommended: HTML/CSS/JS (frontend) + Node.js/Express + SQLite or Python Flask + SQLite

Schema: Table meter_readings with columns matching your requirements plus an id primary key.

#### Prompt 2:
Generate HTML/CSS for Table UI
“Create a clean, responsive HTML page with a table that has these columns: Date, Meter Name, Previous Reading, Present Reading, Total, Description, Actions.
Include a form above the table to add new meter readings. Style it with modern CSS (flexbox/grid). Use a placeholder for the ‘Total’ column since it will be calculated automatically.”

Expected output:

HTML form with input fields for each column except Total and Actions.

Table with sample rows, Edit/Delete buttons in Actions column.

CSS for styling.

#### Prompt 3:
Generate JavaScript for Frontend Logic
“Write JavaScript to:

Handle form submission to add a new row to the table.

Calculate ‘Total’ automatically as Present Reading minus Previous Reading.

Implement ‘Edit’ and ‘Delete’ buttons in each row (Edit should populate the form).

Store data in browser’s localStorage as a fallback (optional, for demo).

Validate inputs (Present > Previous, numbers only for readings).”

Expected output:

addRow(), editRow(), deleteRow() functions.

Calculate total on input change.

Data saved to localStorage.

#### Prompt 4:
Backend API Endpoints
“Using Node.js and Express, create REST API endpoints for:

GET /readings → returns all meter readings

POST /readings → creates a new reading

PUT /readings/:id → updates a reading

DELETE /readings/:id → deletes a reading

Use SQLite database with a table meter_readings containing: id, date, meter_name, prev_reading, pres_reading, description.
The ‘total’ should be calculated in the backend when returning data.”

Expected output:

Express server code with SQLite setup using sqlite3 or better-sqlite3.

CRUD routes with SQL queries.

#### Prompt 5:
Connect Frontend to Backend
“Modify the earlier JavaScript to:

Fetch data from GET /readings on page load and populate the table.

On form submit, send POST request to /readings with JSON data.

On Edit, send PUT request; on Delete, send DELETE request.

Update UI after successful API response.”

Expected output:

Use fetch() for API calls.

### Async functions to handle CRUD operations.

#### No.3.
Additional Prompt Engineering Tips for Your Project
For complex validation:
“Write a function to validate meter readings: Present must be >= Previous, date not in future, meter name not empty.”

For printing/exporting:
“Add a button to export the table data as CSV with columns: Date, Meter Name, Previous, Present, Total, Description.”

For user authentication (if needed later):
“Extend the system to support multiple users with login. Each user sees only their meter entries.”

For deployment:
“How to deploy this full-stack app on Vercel/Railway/Render step-by-step?”

#### No.4.
Complete Prompt to Get Started Quickly
Here’s an all-in-one prompt you can give to an AI coding assistant:

“Build a complete single-page meter reading tracking web app with a SQLite backend.
Frontend: HTML table with columns [Date, Meter Name, Previous Reading, Present Reading, Total (auto-calculated), Description, Actions(Edit/Delete)]. Include an add form above the table. Style it neatly with CSS.
Backend: Node.js + Express with REST API for CRUD. Use SQLite table meter_readings (id, date, meter_name, prev_reading, pres_reading, description). Calculate ‘total’ in backend when sending data.
Integration: Frontend uses fetch() to call backend APIs.
Provide full code files (HTML, CSS, JS, server.js, package.json, database setup) in a structured way.”
## 🔗 Links
[![Website](https://img.shields.io/badge/my_website-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://id-preview--85409a5a-087b-4497-b857-bdf427764cd1.lovable.app/)

