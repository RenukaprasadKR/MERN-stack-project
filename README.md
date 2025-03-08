# Roxiler Systems - MERN Stack Developer Intern - Online Assessment Submission

## Overview
This project is a MERN stack-based assessment that involves creating backend APIs and a frontend interface for handling product transactions. The project fetches data from a third-party API, initializes a database, and provides various endpoints for transactions, statistics, and visualizations.

## Author
**Renukaprasad KR**

## Features
### Backend APIs
- **Initialize Database**: Fetch data from a third-party API and seed the database.
- **List Transactions**: Supports search, pagination, and filtering by month.
- **Statistics API**: Provides total sales amount, sold items, and unsold items for a given month.
- **Bar Chart API**: Returns the number of items in different price ranges for a selected month.
- **Pie Chart API**: Returns unique categories and the number of items per category.
- **Combined API**: Merges data from all the above APIs into a single response.

## Backend Task
### Data Source
- **Third-Party API URL**: [Product Transactions JSON](https://s3.amazonaws.com/roxiler.com/product_transaction.json)
- **Request Method**: GET
- **Response Format**: JSON

### API Requirements
1. **Initialize Database API**
   - Fetch data from the third-party API and initialize the database with seed data.
   - Use an efficient table/collection structure.

2. **List Transactions API**
   - Supports search and pagination.
   - Search parameters match against product title, description, and price.
   - Default pagination: page = 1, per page = 10.

3. **Statistics API**
   - Provides total sales amount, total number of sold items, and unsold items for the selected month.

4. **Bar Chart API**
   - Returns the number of items in different price ranges for a selected month.
   - Price Ranges:
     - 0 - 100
     - 101 - 200
     - 201 - 300
     - 301 - 400
     - 401 - 500
     - 501 - 600
     - 601 - 700
     - 701 - 800
     - 801 - 900
     - 901 and above

5. **Pie Chart API**
   - Returns unique categories and the number of items per category for a selected month.

6. **Combined API**
   - Fetches data from all three APIs and combines responses into a single JSON.

## Frontend Task
Using the created APIs, develop a web interface with the following features:

### Transactions Table
- Displays transaction records for the selected month.
- Search transactions by title, description, or price.
- Supports pagination (Next/Previous buttons).
- Default month selection: March.

### Transactions Statistics
- Displays total sales amount, total sold items, and total unsold items for the selected month.

### Transactions Bar Chart
- Displays the price range distribution of items for the selected month.

### Transactions Pie Chart
- Displays the category-based distribution of items for the selected month.

## Tech Stack
### Backend
- **Node.js**
- **Express.js**
- **MongoDB with Mongoose**
- **dotenv** (for environment variables)
- **cors** (for handling cross-origin requests)
- **axios** (for API calls)
- **nodemon** (for development auto-restart)

### Frontend
- **React.js**
- **TailwindCSS**
- **Chart.js** & **react-chartjs-2** (for visualizations)
- **@remixicon/react** (for icons)

## Setup Instructions
### Prerequisites
- Node.js and npm installed
- MongoDB running locally or a cloud-based MongoDB instance

### Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/RenukaprasadKR/MERN-stack-project.git
   cd MERN-stack-project
   ```

2. Install dependencies:
   ```sh
   npm install
   ```

3. Set up environment variables:
   - Create a `.env` file in the root directory.
   - Add the required variables:
     ```env
     MONGODB_URI=your_mongodb_connection_string
     PORT=3000
     ```

### Running the Backend
1. Start the backend server:
   ```sh
   npm start
   ```
2. The backend will run on:  
   **http://localhost:3000**

### Running the Frontend
1. Start the frontend application:
   ```sh
   cd client
   npm run dev
   ```
2. The frontend will run on:  
   **http://localhost:5173/**

## Contribution
Feel free to fork the repo and submit pull requests to improve the project.

## License
This project is open-source and free to use.
