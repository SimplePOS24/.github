# SimplePOS24 🛒

> **Note**: This is a student project developed for educational purposes.

A modern, full-stack Point of Sale (POS) system built with Next.js and Spring Boot. SimplePOS24 provides an intuitive interface for managing products and processing transactions.

![SimplePOS24 Main Interface](public/image-0.png)
![SimplePOS24 Main Interface](public/image-2.png)

## ✨ Features

### 🛍️ Product Management
- **Category-based Organization**: Products organized by categories (Fruits, Vegetables, Bakery)
- **Barcode Support**: Each product includes barcode scanning functionality
- **Real-time Pricing**: Dynamic pricing with discount support
- **Inventory Tracking**: Monitor product availability and stock levels

![Product Selection - Bakery Items](public/image-1.png)

### 💰 Transaction Processing
- **Multi-item Transactions**: Add multiple products to a single transaction
- **Quantity Management**: Easy quantity adjustment with intuitive controls
- **Discount Application**: Apply discounts with visual feedback
- **Transaction History**: Complete transaction tracking with unique IDs
- **Receipt Generation**: Automatic receipt creation for each transaction

### 🎨 Modern User Interface
- **Dark/Light Theme**: Toggle between themes for different environments
- **Responsive Design**: Optimized for both desktop and mobile devices
- **Intuitive Navigation**: Easy-to-use interface for quick operations
- **Real-time Updates**: Live transaction updates and calculations

### ⚙️ Administration
- **Settings Panel**: Comprehensive configuration options
- **Product Management**: Add, edit, and remove products
- **Deposit Configuration**: Manage bottle deposits and returns
- **Password Protection**: Secure access to administrative functions

## 🏗️ Architecture

### Frontend (Next.js)
- **Framework**: Next.js 14 with TypeScript
- **Styling**: Tailwind CSS with Radix UI components
- **State Management**: React Context API
- **Theme Support**: Next-themes for dark/light mode
- **API Integration**: RESTful API communication with backend

### Backend (Spring Boot)
- **Framework**: Spring Boot 3.x with Java
- **Database**: MongoDB for flexible document storage
- **REST API**: Comprehensive API endpoints for all operations
- **Security**: Environment-based configuration
- **Testing**: Complete test coverage with JUnit

## 🚀 Getting Started

### Prerequisites
- **Node.js** 18+ (for Frontend)
- **Java** 11+ (for Backend)
- **MongoDB** (local or cloud instance)
- **Maven** 3.6+ (for Backend)

### Quick Start

1. **Clone the repositories**
   ```bash
   # Clone Backend
   git clone https://github.com/SimplePOS24/Backend.git
   
   # Clone Frontend (in separate directory)
   git clone https://github.com/SimplePOS24/Frontend.git
   ```

2. **Setup Backend**
   ```bash
   cd Backend
   
   # Set environment variables
   export MONGODB_URI="mongodb://localhost:27017"
   export MONGODB_DATABASE="kassensystem"
   
   # Install and run
   mvn clean install
   mvn spring-boot:run
   ```

3. **Setup Frontend**
   ```bash
   cd Frontend
   
   # Install dependencies
   npm install
   
   # Create environment file
   echo "NEXT_PUBLIC_API_URL=http://localhost:8081" > .env
   
   # Start development server
   npm run dev
   ```

4. **Access the application**
   - Frontend: `http://localhost:3000`
   - Backend API: `http://localhost:8081`

## 📁 Repositories

The SimplePOS24 system is split into separate repositories for better maintainability:

- **[Backend](https://github.com/SimplePOS24/Backend)** - Spring Boot REST API
- **[Frontend](https://github.com/SimplePOS24/Frontend)** - Next.js React application

