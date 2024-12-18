# mdx-testing

# Velora

**Velora** is a website generator that allows users to customize templates or convert MDX/DOC files into websites and export them as code. This project is built using the MERN stack (MongoDB, Express, React, Node.js).

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [General File/Folder Structure](#general-filefolder-structure)
- [Contributing](#contributing)
- [License](#license)

## Features

- Generate websites from customizable templates.
- Convert MDX/DOC files into web formats.
- User authentication and management (coming soon).
- Simple RESTful API for data management.

## Technologies Used

- **Frontend:** React, React Router, Axios
- **Backend:** Node.js, Express
- **Database:** MongoDB (with Mongoose)
- **Development Tools:** Concurrently, Nodemon

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/Lekhya25/Velora.git
   cd velora
   ```

2. **Install server dependencies:**

   Navigate to the server directory and install dependencies:

   ```bash
   cd server
   npm install
   ```

3. **Install client dependencies:**

   Navigate to the client directory and install dependencies:

   ```bash
   cd client
   npm install
   ```

4. **Set Up MongoDB:**

   Make sure to set up MongoDB either locally or using MongoDB Atlas, and replace the connection string in `app.js` with your actual MongoDB URI.

5. **Start the application:**

   You can run both the client and server simultaneously with:

   ```bash
   cd server
   npm run dev
   ```

   This will start the server and client concurrently.

## Usage

Once the application is running, you can access it at `http://localhost:3000`. The main functionality includes generating websites and managing templates.

## API Endpoints

- **GET /** - Welcome to the homepage.
- **GET /about** - About us page.
- **POST /add-user** - Add a new user (requires JSON body with `name` and `email`).

### Example Request to Add a User

```bash
curl -X POST http://localhost:3000/add-user \
-H "Content-Type: application/json" \
-d '{"name": "John Doe", "email": "john@example.com"}'
```

## General File/Folder Structure

```
velora/
├── client/                     # React frontend
│   ├── public/                 # Public assets
│   ├── src/                    # Source files
│   │   ├── components/         # React components
│   │   ├── App.js              # Main app component
│   │   └── index.js            # Entry point
│   └── package.json             # Client dependencies and scripts
├── server/                     # Node.js backend
│   ├── models/                 # Mongoose models
│   ├── routes/                 # Express routes
│   ├── public/                 # Static files
│   ├── app.js                  # Main server file
│   ├── package.json            # Server dependencies and scripts
└── README.mdx                  # Project documentation
```

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.
