# Maison Location Website

A web application that facilitates house rental searches and listings, allowing visitors to find houses based on their preferences and users to publish rental advertisements.

## 🏠 About

This platform enables users to:

- **Search for houses** based on specific preferences such as:
  - Location (emplacement)
  - Number of bedrooms (chambres)
  - Available amenities (Wi-Fi, heating, washing machine, air conditioning, etc.)
- **Publish rental listings** to rent out their properties
- **Browse and filter** available rental properties

The main purpose is to facilitate house hunting and make the rental process more efficient for both tenants and landlords.

## 🚀 Features

- User authentication (Sign up, Sign in, Logout)
- House listing management (Create, Read, Update, Delete)
- Search and filter functionality
- Responsive design
- JWT-based authentication
- Role-based access control

## 🛠 Tech Stack

### Backend

- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MongoDB** - Database
- **Mongoose** - ODM for MongoDB
- **bcrypt** - Password hashing
- **JWT** - Authentication tokens
- **CORS** - Cross-origin resource sharing

### Frontend

- **React.js** - Frontend framework
- **Tailwind CSS** - Styling framework
- **Context API** - State management

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- MongoDB
- npm or yarn

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/mouhebboubaker/ekri.tn.git
   cd maison-location-website
   ```

2. **Backend Setup**

   ```bash
   cd backend
   npm install
   ```

   Create a `.env` file in the backend directory:

   ```env
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   PORT=5000
   ```

3. **Frontend Setup**
   ```bash
   cd ../frontend
   npm install
   ```

### Running the Application

1. **Start the Backend Server**

   ```bash
   cd backend
   npm start
   ```

   The backend server will run on `http://localhost:5000`

2. **Start the Frontend Application**
   ```bash
   cd frontend
   npm start
   ```
   The frontend application will run on `http://localhost:3000`

## 📝 API Endpoints

### Authentication

- `POST /api/signup` - User registration
- `POST /api/signin` - User login
- `POST /api/logout` - User logout
- `POST /api/refresh` - Refresh JWT token

### Houses (Maisons)

- `GET /api/maisons` - Get all houses
- `GET /api/maisons/:id` - Get single house
- `POST /api/maisons` - Create new house listing
- `PUT /api/maisons/:id` - Update house listing
- `DELETE /api/maisons/:id` - Delete house listing

## 🔒 Authentication

The application uses JWT (JSON Web Tokens) for authentication. Users must register and login to:

- Create house listings
- Manage their listings
- Access protected routes

## 🏡 House Listing Features

Each house listing includes:

- Title (titre)
- Phone number (numero)
- Description
- Address (adresse)
- Faculty/Area (faculte)
- Photos
- Rental type (typeDeLocation)
- Number of bedrooms (chambres)
- Price (prix)
- Equipment/Amenities (Equipment)

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License.

## 📞 Contact

For any questions or suggestions, please open an issue or contact the development team.
