# EcoHub

EcoHub is a comprehensive e-commerce application dedicated to electric products and electric vehicles. Our platform offers a wide range of services including an electric cab service, electric product repair and service, direct communication with sales managers, and a rich articles section with the latest news and innovations in the electric industry.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Tech Stack](#tech-stack)
4. [Getting Started](#getting-started)
5. [Installation](#installation)
6. [Running the Project](#running-the-project)
7. [Folder Structure](#folder-structure)
8. [API Endpoints](#api-endpoints)
9. [Contributing](#contributing)
10. [License](#license)

## Project Overview

EcoHub aims to centralize all electric products and services in one place, making it easier for consumers to find, purchase, and get support for their electric needs. Whether you're looking for the latest electric vehicles, need a repair service for your electric products, or want to stay updated with the latest news and innovations, EcoHub has got you covered.

## Features

- **Electric Product Marketplace**: Buy a variety of electric products and vehicles.
- **Electric Cab Service**: Book electric cabs for your transportation needs.
- **Repair and Service**: Get your electric products repaired and serviced.
- **Sales Manager Communication**: Directly chat with sales managers for any doubts or queries.
- **Articles Section**: Read the latest news and articles about electric products and innovations.

## Tech Stack

- **Frontend**: React.js
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JWT (JSON Web Tokens)
- **Hosting**: Hosted using free service - [Render](https://render.com/) & [Vercel](https://vercel.com/)

## Getting Started

### Prerequisites

Before you begin, ensure you have met the following requirements:

- Node.js (v14.x or later)
- npm or yarn
- MongoDB

### Installation

1. **Clone the Repository**

    ```bash
    git clone https://github.com/your-username/ecohub.git
    cd ecohub
    ```

2. **Install Dependencies**

    ```bash
    # Install server dependencies
    cd server
    npm install
    
    # Install client dependencies
    cd ../client
    npm install
    ```

3. **Environment Variables**

    Create a `.env` file in the `server` directory and add the following:

    ```plaintext
    PORT=5000
    MONGO_URI=your_mongodb_uri
    JWT_SECRET=your_jwt_secret
    ```

## Running the Project

1. **Start the Backend Server**

    ```bash
    cd server
    npm start
    ```

    The backend server should now be running on `http://localhost:5000`.

2. **Start the Frontend Server**

    Open a new terminal window and run:

    ```bash
    cd client
    npm start
    ```

    The frontend server should now be running on `http://localhost:3000`.

## Folder Structure

```plaintext
ecohub/
├── client/             # React frontend code
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── App.js
│   │   ├── index.js
│   └── package.json
├── server/             # Node.js backend code
│   ├── config/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── utils/
│   ├── server.js
│   └── package.json
└── README.md
```

## API Endpoints

### User Endpoints

- `POST /api/users/register` - Register a new user
- `POST /api/users/login` - Authenticate a user and get a token
- `GET /api/users/profile` - Get user profile (requires token)

### Product Endpoints

- `GET /api/products` - Get all products
- `GET /api/products/:id` - Get a single product by ID
- `POST /api/products` - Add a new product (admin only)
- `PUT /api/products/:id` - Update a product (admin only)
- `DELETE /api/products/:id` - Delete a product (admin only)

### Order Endpoints

- `POST /api/orders` - Create a new order
- `GET /api/orders` - Get all orders (admin only)
- `GET /api/orders/:id` - Get a single order by ID
- `PUT /api/orders/:id` - Update an order status (admin only)

### Service Endpoints

- `POST /api/services/repair` - Request a repair service
- `POST /api/services/cab` - Book a cab service

### Article Endpoints

- `GET /api/articles` - Get all articles
- `GET /api/articles/:id` - Get a single article by ID
- `POST /api/articles` - Add a new article (admin only)
- `PUT /api/articles/:id` - Update an article (admin only)
- `DELETE /api/articles/:id` - Delete an article (admin only)

## Contributing

Contributions are always welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Thank you for using EcoHub! If you have any questions or feedback, feel free to open an issue or contact us directly.
