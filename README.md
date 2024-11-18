# Permalist - Advanced Todo List Application

## 🎯 Overview
Permalist is a robust and persistent todo list application that allows users to create, read, update, and delete tasks. Built with Node.js and PostgreSQL, it offers reliable data persistence and a clean, user-friendly interface.



## ✨ Features
- Create new tasks with custom titles
- View all existing tasks in a clean interface
- Edit task titles easily
- Delete tasks when completed
- Persistent storage using PostgreSQL
- Responsive design for all devices

## 🛠️ Tech Stack
- **Backend**: Node.js, Express.js
- **Database**: PostgreSQL
- **View Engine**: EJS (Embedded JavaScript)
- **Frontend**: HTML, CSS, JavaScript
- **Other Tools**: 
  - `body-parser` for request parsing
  - `pg` for PostgreSQL integration
  - `express.static` for serving static files

## 📋 Prerequisites
Before you begin, ensure you have the following installed:
- [Node.js](https://nodejs.org/) (v14 or higher)
- [PostgreSQL](https://www.postgresql.org/) (v13 or higher)
- [npm](https://www.npmjs.com/) (usually comes with Node.js)

## 🚀 Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/Krishnasai8500/Permalist.git
   cd permalist
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up the database**
   ```sql
   -- Log into PostgreSQL and run:
   CREATE DATABASE permalist;
   
   -- Connect to the database
   \c permalist
   
   -- Create the items table
   CREATE TABLE items (
       id SERIAL PRIMARY KEY,
       title VARCHAR(255) NOT NULL
   );
   ```

4. **Configure database connection**
   - Create a `.env` file in the root directory
   ```env
   DB_USER=postgres
   DB_HOST=localhost
   DB_NAME=permalist
   DB_PASSWORD=your_password
   DB_PORT=5432
   ```

5. **Start the server**
   ```bash
   npm start
   ```

6. **Access the application**
   - Open your browser and navigate to `http://localhost:3000`

## 📁 Project Structure
```
permalist/
├── public/
│   ├── assets/
│   │   └── icons/
│   │       ├── check-solid.svg
│   │       └── pencil-solid.svg
│   └── styles/
│       └── main.css
├── views/
│   ├── partials/
│   │   ├── footer.ejs
│   │   ├── header.ejs
│   │   └── index.ejs
│   └── index.js
├── server.js
├── queries.sql
├── package.json
├── package-lock.json
└── README.md
```

## 💻 Usage
1. Add a new task by typing in the input field and clicking "Add"
2. Edit existing tasks by clicking the edit button and updating the text
3. Delete tasks by clicking the delete button
4. Tasks persist between sessions and server restarts

## 🔧 API Endpoints
- `GET /` - Renders the main todo list page
- `POST /add` - Adds a new todo item
- `POST /edit` - Updates an existing todo item
- `POST /delete` - Deletes a todo item

## 🤝 Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙌 Acknowledgments
- [Express.js](https://expressjs.com/) - The web framework used
- [PostgreSQL](https://www.postgresql.org/) - Database
- [EJS](https://ejs.co/) - Templating engine

## 📫 Contact
Krishna Sai - [@Krishna528131](https://x.com/Krishna528131)

Project Link: [https://github.com/yourusername/permalist](https://github.com/Krishnasai8500/Permalist)

---
Made with ❤️ by Krishna Sai
