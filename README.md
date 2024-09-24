## Backend Repository - README.md

```markdown
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
- **PostgreSQL/MySQL** (Optional) - For database storage.
- **CORS** - Configured for cross-origin requests between frontend and backend.

## 🔧 Installation and Setup

To run the API locally, follow these steps:

1. **Clone the repository:**

    ```bash
    git clone https://github.com/your-username/recipes-website-backend.git
    cd recipes-website-backend
    ```

2. **Install dependencies:**

    ```bash
    npm install
    ```

3. **Create a `.env` file** with your API keys and server settings:

    ```plaintext
    SPOONACULAR_API_KEY=your_api_key
    COOKIE_SECRET=your_cookie_secret
    PORT=3000
    ```

4. **Run the server:**

    ```bash
    npm start
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

## 🌐 Live API

Check out the live API: [API Demo Link](https://your-api-link.com)

## 📈 Future Improvements

- **JWT Authentication**: Migrate to JWT for better scalability.
- **Database Integration**: Integrate with a relational database like PostgreSQL for persistent data storage.

## 🤝 Contributing

Contributions are welcome! Please check the [issues page](#) for opportunities to contribute.

---
