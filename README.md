# Virtual Tour Project

A comprehensive virtual tour platform showcasing Rajasthan's rich cultural heritage, cuisine, and famous restaurants.

## 🏗️ Project Structure

```
virtual-tour-project/
├── backend/                    # Node.js/Express API
│   ├── config/               # Database configuration
│   ├── controllers/           # Request handlers
│   ├── middleware/           # Custom middleware
│   ├── models/               # Mongoose schemas
│   ├── routes/               # API routes
│   ├── scripts/              # Database seeding
│   ├── services/             # Business logic
│   ├── utils/                # Helper functions
│   ├── validators/            # Input validation
│   ├── constants/            # Application constants
│   └── server.js             # Entry point
├── frontend/                  # React application
│   ├── public/               # Static assets
│   └── src/
│       ├── api/              # API integration
│       ├── assets/           # Images, fonts
│       ├── components/        # React components
│       │   ├── common/      # Reusable components
│       │   └── statePage/  # Page-specific components
│       ├── constants/        # Frontend constants
│       ├── hooks/            # Custom React hooks
│       ├── pages/            # Page components
│       ├── styles/           # Theme and styling
│       └── utils/            # Helper functions
└── README.md
```

## 🚀 Features

### Backend
- **RESTful API** with Express.js
- **MongoDB** database with Mongoose ODM
- **Modular Architecture** with organized directories
- **Input Validation** using express-validator
- **Error Handling** middleware
- **Database Seeding** for initial data
- **CRUD Operations** for all resources

### Frontend
- **React 19** with modern hooks
- **Framer Motion** animations
- **Responsive Design** with mobile-first approach
- **Component Architecture** with reusable components
- **Custom Hooks** for common functionality
- **Theme System** with consistent styling
- **Google Maps Integration** for restaurant directions

## 🍛️ Dal Baati Churma Restaurants

Comprehensive database of famous restaurants across Rajasthan:

### Featured Cities
- **Jaipur**: Suvarna Mahal, Chokhi Dhani, Rawat Mishtan Bhandar
- **Jodhpur**: On The Rocks, Indique

### Restaurant Information
- Complete address and Google Maps integration
- Ratings, price ranges, and specialties
- Features: parking, AC, delivery, outdoor seating
- Must-try dishes and opening hours
- Phone numbers and average prices

## 🛠️ Getting Started

### Prerequisites
- Node.js 16+
- MongoDB
- npm or yarn

### Installation

1. **Clone the repository**
```bash
git clone <repository-url>
cd virtual-tour-project
```

2. **Install dependencies**
```bash
# Backend
cd backend
npm install

# Frontend
cd ../frontend
npm install
```

3. **Environment Setup**
```bash
# Backend
cd backend
cp .env.example .env
# Edit .env with your MongoDB URI

# Frontend
cd ../frontend
# No additional setup needed
```

4. **Seed Database**
```bash
cd backend
node scripts/seedDalBaatiRestaurants.js
```

5. **Start Development Servers**
```bash
# Backend (Terminal 1)
cd backend
npm run dev

# Frontend (Terminal 2)
cd frontend
npm start
```

## 📡 API Endpoints

### Dal Baati Restaurants
- `GET /api/dal-baati-restaurants` - Get all restaurants
- `GET /api/dal-baati-restaurants/:id` - Get restaurant by ID
- `GET /api/dal-baati-restaurants/city/:city` - Get restaurants by city
- `GET /api/dal-baati-restaurants/search` - Search restaurants
- `GET /api/dal-baati-restaurants/top-rated` - Get top-rated restaurants
- `GET /api/dal-baati-restaurants/cities` - Get all cities

### Other Endpoints
- `GET /api/cuisines` - Cuisines data
- `GET /api/festivals` - Festivals data
- `GET /api/blogs` - Blog posts
- `GET /api/state-spotlight` - State spotlight data

## 🎨 Frontend Routes

- `/` - Home page
- `/state/:name` - State information page
- `/rajasthan-cuisine` - Rajasthan cuisine details
- `/dal-baati-restaurants` - Famous Dal Baati restaurants

## 🏛️ Architecture Highlights

### Backend Organization
- **Separation of Concerns**: Controllers, models, routes, middleware
- **Central Exports**: Index files for clean imports
- **Validation**: Input validation with express-validator
- **Error Handling**: Consistent error responses
- **Utilities**: Common helper functions

### Frontend Organization
- **Component-Based**: Reusable UI components
- **Custom Hooks**: Encapsulated logic
- **Theme System**: Consistent styling approach
- **Constants**: Centralized configuration
- **Responsive**: Mobile-first design

## 📱 Responsive Design

- **Mobile**: < 768px
- **Tablet**: 768px - 1024px
- **Desktop**: > 1024px

## 🎯 Key Features

### Restaurant Discovery
- Advanced filtering by city, rating, price
- Search functionality with debouncing
- Sort options (featured, rating, price)
- Detailed restaurant information

### User Experience
- Smooth animations and transitions
- Loading states and error handling
- Google Maps integration
- Mobile-optimized interface

## 🛠️ Development

### Adding New Restaurants
```javascript
// Use the seed script or API POST
const newRestaurant = {
  name: "Restaurant Name",
  address: "Full Address",
  city: "City",
  specialty: "Specialty description",
  // ... other fields
};
```

### Custom Styling
```javascript
// Use the theme system
import { theme } from './styles';

const customStyle = {
  background: theme.gradients.primary,
  borderRadius: theme.borderRadius.md
};
```

## 📝 Scripts

### Backend
- `npm run dev` - Start development server
- `npm start` - Start production server
- `node scripts/seedDalBaatiRestaurants.js` - Seed database

### Frontend
- `npm start` - Start development server
- `npm run build` - Build for production
- `npm test` - Run tests

## 🤝 Contributing

1. Follow the established code patterns
2. Use the organized directory structure
3. Maintain consistent styling with theme system
4. Add proper validation for new endpoints
5. Test responsive design

## 📄 License

This project is licensed under the MIT License.
