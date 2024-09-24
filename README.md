## Backend Repository 

# Recipes Website API 🍴

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

**Recipes Website API** is the backend powering the Recipes Website. It handles user authentication, favorites management, and integrates with the Spoonacular API to fetch recipe data dynamically.

## 🚀 Features

- **User Authentication**: Secure login and registration with password hashing (bcrypt).
- **Favorites Management**: API endpoints for users to add, view, and remove favorite recipes.
- **Recipe API Integration**: Interacts with the Spoonacular API to retrieve various recipes.
- **Express.js HTTPS Server**: Runs on HTTPS with secure cookies for session management.
- **Session Handling**: Session management using `client-sessions` to handle user login states.

## 🛠️ Technologies Used

- **Node.js & Express.js** - Server-side framework.
- **bcrypt** - For secure password hashing.
- **client-sessions** - Session management for user authentication.
- **Spoonacular API** - External API for fetching recipes.
- **MySQL** - For database storage.
- **CORS** - Configured for cross-origin requests between frontend and backend.

## 🔧 Installation and Setup

To run the API locally, follow these steps:

1. **Clone the repository:**

    ```windows
    git clone https://github.com/your-username/recipes-website-backend.git
    cd recipes-website-backend
    ```

2. **Install dependencies:**

    ```windows
    npm install ...
    ```

3. **Create a `.env` file** with your API keys and server settings:

    ```plaintext
    SPOONACULAR_API_KEY=your_api_key
    COOKIE_SECRET=your_cookie_secret
    PORT=3000
    ```

4. **Run the server:**

    ```windwos
    node main
    ```

    The backend server will be running at `https://localhost:3000`.

## 📂 Project Structure
📦src ┣ 📂routes ┣ 📂controllers ┣ 📂middlewares ┣ 📂services ┗ 📂utils


- `routes/` - API routes like `/register`, `/login`, `/favorites`.
- `controllers/` - User authentication and recipe management logic.
- `services/` - External API communication and internal business logic.
- `middlewares/` - Session handling and authentication middleware.
- `utils/` - Helper functions and utilities.

## API Documentation

Here’s a quick summary of the key API endpoints:

### `POST /register`
- Registers a new user.

### `POST /login`
- Logs in an existing user and starts a session.

### `POST /favorites`
- Adds a recipe to the user's favorites.

### `GET /favorites`
- Retrieves the logged-in user's favorite recipes.

### `POST /my-recipes`
- Create a new user-recipe which will be saved in my-recipes table in my-SQL.

### `GET /my-recipes`
- Retrieves the user-made recipes 

### and many many more ! 

---
