# ️ Bitee – Food Discovery & AI Recipe Generator Web App

Bitee is a full-featured web app designed for food lovers. It allows users to either explore local restaurants using detailed filters or stay at home and generate recipes based on ingredients they already have. The app integrates OpenAI's API to generate smart, customized recipes.

##  Features

- Filter restaurants by city, cuisine, budget, occasion, and more
- View shop details with menus, descriptions, and categories
- Generate recipes from ingredients using OpenAI API
- Find similar meals at nearby restaurants
- Locate grocery stores with missing ingredients (conceptual)
- Clean, responsive user interface
- Built using HTML, CSS, JavaScript, Node.js, and SQLite

##  Project Structure

**Additional files/folders:**
- `bitee.db` – SQLite database file that stores all app data (created by `fix_database.py` or included manually)

```
├── index.html               # Homepage
├── login.html               # Login page
├── signup.html              # Signup page
├── filter.html              # Filter options for restaurants
├── shop.html                # Restaurant/shop detail page
├── recipes.html             # AI-generated recipes
├── help.html                # FAQ / support
├── script.js                # Frontend logic
├── server.js                # Node.js backend
├── fix_database.py          # Initializes SQLite database
└── README.md                # This file
```

## ️ Prerequisites

Before running this project, make sure you have the following installed:

- [Node.js](https://nodejs.org/) (v14 or later)
- [Python 3](https://www.python.org/) (for setting up the database)
- An OpenAI API key (for recipe generation)
- Git (for cloning the repo)

## Installation & Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/bitee.git
   cd bitee
   ```

2. **Install backend dependencies**:
   ```bash
   npm install
   ```

3. **Set up the database**:
   Run the following Python script to create the initial SQLite database:
   ```bash
   python fix_database.py
   ```

4. **Add your OpenAI API key**:
   In `server.js`, find the placeholder for the API key and insert your actual key:
   ```js
   const apiKey = 'your-openai-api-key-here';
   ```

5. **Add your Pexels Image API key**:
   In `recipes.html`, find the placeholder for the API key and insert your actual key:
   ```js
   const pexelsKey = 'your-pexels-api-key-here';
   ```

## Running the App

1. Start the Node.js server:
   ```bash
   node server.js
   ```

2. Open your browser and go to:
   ```
   http://localhost:3000
   ```

3. You can now navigate between pages using the homepage.

## AI Integration Notes

- The recipe generation uses the OpenAI API based on user inputs.
- Ensure you have a working API key before testing the recipe feature.
- The image-generation feature is still pending.

## Database

- The app currently uses a **SQLite** database.
- You can switch to a more scalable database like PostgreSQL by updating the backend logic.
- All initial tables and data are created by `fix_database.py`.

##  Future Improvements

- Connect authentication pages (`login.html`, `signup.html`) to the backend
- Add real-time restaurant reservation system
- Finalize recipe image generation
- Enhance grocery store integration
- Build a mobile-responsive version

##  Contact

Developed by **Adam Hawash**  
Email: adamhawashmain@gmail.com  
Phone number: +970 594444403  
Senior Capstone Project – 2025  
Feel free to reach out or fork the project!
