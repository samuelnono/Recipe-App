# Forkast - Smart Meal Planner 🍱

Forkast is a data-driven meal planning application designed to support user decision-making through structured data intake, processing, and analysis.

Rather than focusing only on recommendations, this project emphasizes how user input data can be collected, stored, inspected, and interpreted to inform personalized outcomes.

---

## Project Focus

This project was built to explore:
- How user-provided data (ingredients, preferences, budgets) flows through a system
- How APIs and databases support analytics-ready pipelines
- How structured data can be inspected and validated in real time

---

## My Contribution

My work on Forkast focused on the **data and analytics layer** of the system:

- Testing and validating API endpoints using `curl`
- Ingesting structured JSON user inputs
- Inspecting and verifying stored data in MongoDB using MongoDB Compass
- Understanding and validating database schemas and collections
- Interpreting how user data supports downstream decision logic

This project strengthened my ability to reason about data pipelines, data quality, and how analytics systems operate in practice.

---

## Tech Stack

- Frontend: React  
- Backend: Flask (Python)  
- Database: MongoDB  
- Containerization: Docker & Docker Compose  

---

## Running the Application

```bash
docker-compose up --build


---

## 🚀 How to Run the App

### 📁 Step 1: Open Terminal and Navigate to Project

```bash
cd path/to/forkast
# Example:
cd "C:\Users\\Desktop\forkast"


🐳 Step 2: Start All Services

docker-compose up --build

Use --build only if dependencies or code changed.
For normal runs, just use:

docker-compose up


🧪 Step 3: Test Flask API
curl -X POST http://localhost:5000/upload-groceries ^
  -H "Content-Type: application/json" ^
  -d "{\"ingredients\": [\"rice\", \"tofu\"], \"dietary_preferences\": [\"vegan\"], \"budget\": 25}"

🧭 Step 4: View Data in MongoDB Compass
Connection: mongodb://localhost:27017

Database: forkast

Collection: user_inputs
Click the 🔄 refresh icon to see new documents.

🛑 Step 5: Stop Everything
To stop the app:

Ctrl + C
To remove all containers:



docker-compose down
