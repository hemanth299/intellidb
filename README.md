IntelliDB 🗣️ - A Natural Language Database Interface
IntelliDB is a modern web application that bridges the gap between complex database queries and natural human language. It allows users to securely connect to their MySQL databases and ask questions in plain English, receiving instant SQL results and data tables. This tool is designed to empower team members of all technical levels to interact with data intuitively, without needing to write a single line of SQL.

✨ Features
Secure User Authentication: Full login and registration system with persistent user sessions, powered by Spring Security.

Encrypted Connection Management: Users can save, edit, and delete multiple database connections. Credentials are fully encrypted at rest using AES.

Natural Language to SQL: At its core, IntelliDB uses a Large Language Model (LLM) to translate questions like "show me the top 5 highest paid employees" into executable SQL queries.

Schema-Aware Intelligence: The AI is provided with the full table schema (CREATE TABLE statements) to generate accurate, context-aware queries.

Interactive Dashboard: A sleek, dark-themed dashboard to manage connections and view database schemas.

Dynamic Query Interface: Features a schema viewer, a query history panel, and an interactive results table.

Data Exploration Tools:

Table Previews: Click any table to see its structure and a preview of the first 10 rows.

Sortable Results: Click on any column header in the results table to sort the data.

Export to CSV: Download any query result set as a CSV file with a single click.

Built-in Security: Includes a confirmation step for potentially destructive queries (like UPDATE or DELETE) to prevent accidental data modification.

📸 Screenshots
Here's a look at the IntelliDB interface:

Connections Dashboard

Query Interface

🛠️ Tech Stack
Backend: Java 17, Spring Boot, Spring Security, Spring Data JPA

Database: H2 (for local user/app data), MySQL (for user-connected databases)

Frontend: Thymeleaf with Layout Dialect, HTML5, CSS3, JavaScript (Fetch API)

AI: Google Gemini API

Build Tool: Apache Maven

🚀 Getting Started
Follow these instructions to get a local copy of IntelliDB up and running.

Prerequisites
Java Development Kit (JDK) 17 or later

Apache Maven

Git

Installation & Setup
Clone the repository:

Bash

git clone https://github.com/your-username/intellidb.git
cd intellidb
Configure the application:
Open the src/main/resources/application.properties file. You need to provide your own secret keys for the application to function.

Properties

# Your API key from Google AI Studio
gemini.api.key=YOUR_GOOGLE_GEMINI_API_KEY

# A random 16-character string for encrypting passwords
encryption.secret.key=ThisIsA16CharKey
Run the application:
Use Maven to build and run the Spring Boot application.

Bash

mvn spring-boot:run
The application will be running at http://localhost:8080.

usage
Navigate to http://localhost:8080.

You will be redirected to the login page. Click "Sign Up" to create a new account.

After logging in, you'll see the main connections dashboard.

Click "Add Connection" to save the credentials for your MySQL database.

From the dashboard, click "Connect" on a saved connection to enter the query interface.

Ask questions in the text box and get instant results!

📞 Contact
Hemanth Yerra

Email: hemanthyerra.dev@gmail.com

LinkedIn: linkedin.com/in/hemanth299

GitHub: github.com/hemanth299

📄 License
This project is licensed under the MIT License. See the LICENSE file for details.
