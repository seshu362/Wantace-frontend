# Recipe Management System - Frontend

This is the frontend for a **Recipe Management System** built with **React**. It provides a user-friendly interface for managing recipes, including features like user authentication, recipe creation, editing, and viewing. The frontend interacts with a backend API to fetch and manage data.

## Features

- **User Authentication**:
  - Login and signup functionality.
  - JWT token-based authentication.
- **Recipe Management**:
  - View a list of recipes.
  - View detailed information about a specific recipe.
  - Create new recipes.
  - Edit existing recipes.
- **Image Upload**:
  - Upload recipe images using a file or provide an image URL.
- **Responsive Design**:
  - Mobile-friendly and responsive UI.
- **Theme Toggle**:
  - Switch between light and dark themes.

---

## Technologies Used

- **React**: JavaScript library for building user interfaces.
- **React Router**: For handling routing and navigation.
- **Fetch**: For making HTTP requests to the backend API.
- **CSS**: For styling components.
- **FontAwesome**: For adding icons to the UI.
- **Multer**: For handling image uploads (backend integration).

---

## Folder Structure

The project is organized as follows:
```
  src/
  ├── components/
  │ ├── Auth/
  │ │ ├── Login.js
  │ │ ├── Signup.js
  │ │ └── index.css
  │ ├── RecipeDetails/
  │ │ ├── index.js
  │ │ └── index.css
  │ ├── RecipeEditForm/
  │ │ ├── index.js
  │ │ └── index.css
  │ ├── RecipeList/
  │ │ ├── index.js
  │ │ └── index.css
  │ └── RecipeSubmissionForm/
  │ ├── index.js
  │ └── index.css
  ├── App.js
  ├── App.css
  ├── index.js
  └── index.css
```


### Key Files and Folders

- **`components/Auth/`**: Contains components for user authentication (Login and Signup).
- **`components/RecipeDetails/`**: Displays detailed information about a specific recipe.
- **`components/RecipeEditForm/`**: Allows users to edit existing recipes.
- **`components/RecipeList/`**: Displays a list of all recipes.
- **`components/RecipeSubmissionForm/`**: Allows users to create new recipes.
- **`App.js`**: Main application component with routing and theme toggling.

---

## Setup Instructions

### Prerequisites

- Node.js (v14 or higher)
- npm (Node Package Manager)

### Installation

### 1. Clone the repository
   ```bash
   git clone https://github.com/seshu362/Wantace-Recipe-Assignment.git
   cd Wantace-Recipe-Assignment/frontend--project
   ```
### 2. Install Dependencies
```
  npm install
```
### 2. Start the development server:
```
  npm start
```
The application will start on http://localhost:3000.

# API Integration

The frontend interacts with the backend API for the following operations:

## Authentication

- **Login**: `POST /login`
- **Signup**: `POST /signup`

## Recipe Management

- **Get all recipes**: `GET /recipes`
- **Get a single recipe**: `GET /recipes/:id`
- **Create a recipe**: `POST /recipes`
- **Update a recipe**: `PUT /recipes/:id`

## Image Upload

- **Upload an image**: `POST /upload`

---

# Key Components

## 1. App Component

- Manages the theme (light/dark mode).
- Handles user authentication and routing.
- Displays a logout button for authenticated users.

## 2. RecipeList Component

- Fetches and displays a list of recipes.
- Provides a link to add a new recipe.

## 3. RecipeDetails Component

- Displays detailed information about a specific recipe.
- Allows users to navigate back to the recipe list or edit the recipe.

## 4. RecipeSubmissionForm Component

- Allows users to submit a new recipe.
- Supports image upload via file or URL.

## 5. RecipeEditForm Component

- Allows users to edit an existing recipe.
- Pre-fills the form with the current recipe data.

## 6. Login and Signup Components

- Handle user authentication.
- Display validation errors and success messages.
