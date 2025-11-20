CS50x Finance - Stock Trading Platform
A complete web-based stock trading simulation built for Harvard's CS50x final project. This platform allows users to manage virtual stock portfolios with real-time market data.

🎯 Project Overview
CS50x Finance is a Flask web application that simulates stock trading. Users can register accounts, check real-time stock quotes, buy/sell shares, track their investment portfolio, and manage their cash balance with full transaction history.

✨ Key Features
🔐 User Authentication - Secure registration and login system

📈 Real-time Stock Data - Live quotes via IEX Cloud API

💼 Portfolio Management - Track holdings and portfolio value

🔄 Trading System - Buy and sell stocks with validation

💰 Cash Management - Add funds to your account balance

📊 Transaction History - Complete audit trail of all trades

💵 Starting Balance - $1,000 initial virtual cash

🛠 Tech Stack
Backend: Python, Flask

Database: SQLite with SQLAlchemy ORM

Frontend: HTML, CSS, JavaScript, Bootstrap

API: IEX Cloud for stock data

Security: Werkzeug password hashing

🚀 Quick Start
Prerequisites
Python 3.6+

IEX Cloud API key (free tier available)

Installation & Setup
Clone the repository

bash
'''
git clone https://github.com/Darik10/Financial-App.git
cd Financial-App
Install dependencies
'''

bash
'''
pip install -r requirements.txt
Configure environment
'''

bash
'''
export API_KEY=your_iex_api_key_here
export FLASK_APP=app.py
Launch application
'''

bash
'''
flask run
Access platform
Navigate to http://localhost:5000 in your browser
'''

📁 Project Structure
text
Financial-App/
├── app.py                 # Main Flask application
├── helpers.py             # Utility functions & decorators
├── finance.db            # SQLite database
├── requirements.txt      # Python dependencies
├── static/
│   ├── styles.css       # Custom CSS styling
│   └── logo.png         # Application logo
└── templates/
    ├── layout.html      # Base template
    ├── index.html       # Portfolio dashboard
    ├── quote.html       # Stock lookup
    ├── buy.html         # Purchase stocks
    ├── sell.html        # Sell stocks
    ├── add_cash.html    # Add funds to account
    ├── history.html     # Transaction history
    ├── login.html       # User login
    └── register.html    # User registration
💻 How to Use the Platform
**1. Account Setup**
Register with a unique username
Receive $1,000 starting virtual cash balance
Login to access trading features

**2. Cash Management**
**Starting Balance:** Every new account begins with $1,000
**Add Cash:** Use the "Add Cash" feature to increase your balance
**Track Spending:** Monitor cash balance during trading activities

**3. Stock Operations**
**Quote:** Look up current stock prices using symbols (AAPL, TSLA, etc.)
**Buy:** Purchase stocks by specifying symbol and quantity
**Sell:** Sell shares from your current portfolio

**5. Portfolio Management**
- View real-time portfolio value
- Monitor individual stock holdings
- Track cash balance and overall performance
- Access complete transaction history

🔧 My Implementation & Contributions
Core Features Developed
🔐 Authentication System
Implemented secure user registration with password hashing

Created session-based login/logout functionality

Added error handling for duplicate usernames

💾 Database Architecture
Designed SQL schema for users, transactions, and holdings

Implemented efficient portfolio calculation queries

Ensured data integrity with proper constraints

💰 Cash Management System
Default Starting Balance: Set $1,000 initial cash for all new users

Add Cash Feature: Implemented add_cash.html template and routing

Balance Updates: Real-time cash balance calculations

Transaction Tracking: Log all cash additions in history

📊 Stock Trading Engine
Integrated IEX Cloud API for real-time stock data

Built complete buy/sell transaction system

Implemented portfolio valuation calculations

🎨 User Interface
Developed responsive web interface with Bootstrap

Created intuitive navigation and data presentation

Added real-time form validation and error messages

Technical Highlights
Security Implementation
Password hashing with Werkzeug

SQL injection prevention via parameterized queries

Session management with automatic timeout

Input validation and sanitization

API Integration
Real-time stock price fetching

Symbol validation and error handling

Efficient caching to minimize API calls

Code Quality & Best Practices
Modular Design: Separated concerns with helper functions

Error Handling: Comprehensive validation and user feedback

Database Optimization: Efficient queries and indexing

Code Documentation: Clear comments and organized structure

🛡 Security Features
Password hashing with salt generation

Session management with automatic expiration

SQL injection prevention

Input validation and sanitization

CSRF protection measures

📈 API Integration
The application seamlessly integrates with IEX Cloud API to:

Fetch real-time stock prices

Validate stock symbols

Provide accurate market data for trading decisions

🎓 Skills Demonstrated
Full-Stack Development: Flask, Python, SQL, HTML/CSS, JavaScript

Database Design: SQLite, query optimization, ORM usage

API Integration: RESTful services, JSON handling, error management

Security Implementation: Authentication, data validation, protection

Financial Logic: Portfolio math, cash flow management, transaction tracking

Software Engineering: Modular code, testing, documentation

🔮 Future Enhancements
Potential improvements for production deployment:

Email verification for registration

Password reset functionality

Advanced charting and analytics

Watchlist feature

Mobile-responsive enhancements

Docker containerization

Note: This project was developed as part of Harvard's CS50x curriculum, demonstrating comprehensive full-stack web development capabilities with a focus on practical, real-world application building.
