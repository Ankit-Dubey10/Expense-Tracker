# Expense Tracker

A full-stack web application for tracking personal expenses and income. Built with the MERN stack (MongoDB, Express.js, React.js, Node.js).

## ✨ Features

- 📊 Track income and expenses
- 💰 Real-time balance calculation
- 📱 Responsive design
- 🗄️ Persistent data storage
- ⚡ Fast and intuitive interface

## 🛠️ Built With

- **Frontend**: React.js, CSS3
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Additional Tools**: Axios for API calls

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- MongoDB (local installation or MongoDB Atlas)
- npm or yarn

### Installation

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd expense-tracker
   ```

2. **Install server dependencies**
   ```bash
   cd server
   npm install
   ```

3. **Install client dependencies**
   ```bash
   cd ../client
   npm install
   ```

4. **Set up environment variables**
   
   Create a `config.env` file in the `server/config` directory:
   ```env
   NODE_ENV=development
   PORT=5000
   MONGO_URI=mongodb://localhost:27017/expense_tracker
   ```

5. **Start the application**

   **Start the server:**
   ```bash
   cd server
   npm start
   ```

   **Start the client (in a new terminal):**
   ```bash
   cd client
   npm start
   ```

   The application will be available at `http://localhost:3000`

## 📁 Project Structure

```
expense-tracker/
├── client/                 # React frontend
│   ├── public/
│   │   ├── components/     # React components
│   │   ├── context/        # Global state management
│   │   └── utils/          # Utility functions
│   └── package.json
├── server/                 # Node.js backend
│   ├── config/            # Configuration files
│   ├── controllers/       # Route controllers
│   ├── models/           # MongoDB models
│   ├── routes/           # API routes
│   └── package.json
└── README.md
```

## 🗄️ Database Schema

### Transaction Collection
- `_id`: Unique identifier
- `text`: Transaction description
- `amount`: Transaction amount (positive for income, negative for expense)
- `createdAt`: Timestamp

## 🔧 API Endpoints

- `GET /api/v1/transactions` - Get all transactions
- `POST /api/v1/transactions` - Add new transaction
- `DELETE /api/v1/transactions/:id` - Delete transaction

## 📸 Screenshots

![Expense Tracker](expense-tracker.PNG)

## 🚀 Deployment

### Production Build

1. **Build the React app:**
   ```bash
   cd client
   npm run build
   ```

2. **Copy build folder to server:**
   ```bash
   cp -r build ../server/
   ```

3. **Set environment to production:**
   ```env
   NODE_ENV=production
   ```

4. **Start the server:**
   ```bash
   cd server
   npm start
   ```

## 🤝 Contributing

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License.

## 👨‍💻 Author

**Your Name**
- GitHub: [@yourusername](https://github.com/yourusername)

---

⭐ If you found this project helpful, please give it a star!
