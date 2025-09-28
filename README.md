# React Shop with JSON Server

A modern, responsive e-commerce front-end application built with React. This project features a complete shopping experience, including user authentication, product browsing, a shopping cart, and a favorites list, all powered by a mock REST API using `json-server`.

![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)![React Router](https://img.shields.io/badge/React_Router-CA4245?style=for-the-badge&logo=react-router&logoColor=white)![React Bootstrap](https://img.shields.io/badge/React--Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white)![JSON Server](https://img.shields.io/badge/JSON--Server-3178C6?style=for-the-badge&logo=json&logoColor=white)

## Table of Contents

- [Live Demo](#live-demo)
- [Key Features](#key-features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Project Structure](#project-structure)
- [Screenshots](#screenshots)
- [License](#license)

## Live Demo

*[Add a link to your live demo here if you have one deployed (e.g., on Netlify, Vercel).]*

## Key Features

- **User Authentication**: Secure user registration and login functionality.
- **Protected Routes**: Certain pages like Profile and Checkout are only accessible to logged-in users.
- **Product Catalog**: Browse, search, and filter products by category and price range.
- **Product Details**: View detailed information for each product.
- **Dynamic Shopping Cart**: Add products to the cart, adjust quantities (+/-), or remove items. The cart total updates automatically.
- **Favorites List**: Add products to a personal favorites list for future reference.
- **Responsive Design**: A fully responsive layout that works on desktops, tablets, and mobile devices, built with React Bootstrap.
- **Mock Backend**: Uses `json-server` to simulate a real-world REST API for users and products.

## Technologies Used

- **Frontend**:
  - [React](https://reactjs.org/)
  - [React Router](https://reactrouter.com/) for page navigation.
  - [React Context API](https://reactjs.org/docs/context.html) for state management (authentication, cart, favorites).
  - [React Bootstrap](https://react-bootstrap.github.io/) for UI components.
  - [Axios](https://axios-http.com/) for making API requests.
- **Backend (Mock)**:
  - [JSON Server](https://github.com/typicode/json-server) to create a fake REST API.

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Make sure you have the following installed on your machine:
- [Node.js](https://nodejs.org/en/) (v14 or later recommended)
- [npm](https://www.npmjs.com/) (Node Package Manager)

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/me-elshenawy/React-Shop-with-JSON-Server.git
    cd React-Shop-with-JSON-Server
    ```

2.  **Install frontend dependencies:**
    ```bash
    npm install
    ```

3.  **Set up and run the mock backend:**
    This project requires `json-server` to handle user and product data. The data is stored in the `db.json` file.
    
    Open a **new terminal** and run the following command from the project root:
    ```bash
    npx json-server --watch db.json --port 3005
    ```
    This will start the mock API server on `http://localhost:3005`. Keep this terminal running.

4.  **Start the React application:**
    In your original terminal, run:
    ```bash
    npm start
    ```    The application will open automatically in your browser at `http://localhost:3000`.

## Project Structure

```
/src
|-- /components     # Reusable UI components (Header, Footer, Products)
|-- /context        # React Context for state management (Auth, Cart)
|-- /css            # CSS files for custom styling
|-- /pages          # Top-level page components (Home, Login, Cart)
|-- App.js          # Main application component
|-- main.jsx        # Entry point of the React app
```

## Screenshots

*[Add screenshots of your application here to showcase the UI. You can drag and drop images directly into the GitHub editor.]*

**Example:**

| Home Page                                       | Cart Page                                      |
| ----------------------------------------------- | ---------------------------------------------- |
| ![Home Page Screenshot](https://cdn.corenexis.com/files/b/5395683168.png) | ![Cart Page Screenshot](https://cdn.corenexis.com/files/b/6823788168.png)|


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
