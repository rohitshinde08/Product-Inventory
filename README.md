# Product Inventory Management System

A full-stack web application designed to manage product inventories efficiently. Built with a robust **FastAPI** backend and a dynamic **React** frontend, this system allows users to perform complete CRUD (Create, Read, Update, Delete) operations on product data.

## 🚀 Features

- **Product Management**: Add, view, update, and delete products.
- **Real-time Updates**: Seamless integration between frontend and backend.
- **Persistent Storage**: Data is stored securely in a PostgreSQL database.
- **Responsive UI**: A clean and modern user interface for managing stock.

## 🛠️ Tech Stack

### Frontend
- **React.js**: For building a responsive user interface.
- **Axios**: For making API requests to the backend.
- **CSS3**: Custom styling for a premium look.

### Backend
- **FastAPI**: High-performance Python framework for building APIs.
- **SQLAlchemy**: SQL toolkit and Object-Relational Mapper (ORM).
- **PostgreSQL**: Robust relational database for data persistence.
- **Uvicorn**: ASGI server for running the FastAPI application.

## 📋 Prerequisites

Before you begin, ensure you have the following installed:
- [Python 3.8+](https://www.python.org/)
- [Node.js & npm](https://nodejs.org/)
- [PostgreSQL](https://www.postgresql.org/)

## ⚙️ Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/rohitshinde08/Product-Inventory.git
cd Product-Inventory
```

### 2. Backend Setup
Create a virtual environment and install the required Python packages:

```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate

# Install dependencies
pip install fastapi uvicorn sqlalchemy psycopg2 axios
```

**Database Configuration:**
Ensure you have a PostgreSQL database named `practice`. Update the connection string in `database.py` if necessary:
```python
db_url = "postgresql://postgres:admin@localhost:5432/practice"
```

**Run the Backend:**
```bash
uvicorn main:app --reload
```
The API will be available at `http://localhost:8000`.

### 3. Frontend Setup
Navigate to the frontend directory and install dependencies:

```bash
cd frontend
npm install
```

**Run the Frontend:**
```bash
npm start
```
The application will be available at `http://localhost:3000`.

## 🌐 API Endpoints

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| **GET** | `/products` | Retrieve all products |
| **GET** | `/products/{id}` | Retrieve a specific product by ID |
| **POST** | `/products` | Add a new product |
| **PUT** | `/products/{id}` | Update an existing product |
| **DELETE** | `/products/{id}` | Delete a product |

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

---
Developed by [Rohit Shinde](https://github.com/rohitshinde08)
