# Advanced MERN B2B Teams Project Management SaaS

A modern, full-stack project management application built with the MERN stack (MongoDB, Express.js, React, Node.js) and TypeScript. This application is designed for B2B teams to manage projects, tasks, and team collaboration effectively.

## 🚀 Features

- **Authentication & Authorization**
  - Secure user authentication with Passport.js
  - Google OAuth 2.0 integration
  - Role-based access control
  - Session management with cookie-session

- **Project Management**
  - Create and manage projects
  - Task tracking and management
  - Team collaboration tools
  - Real-time updates

- **Modern UI/UX**
  - Built with React 18 and TypeScript
  - Responsive design using Tailwind CSS
  - Beautiful UI components with Radix UI
  - Dark/Light mode support
  - Emoji picker integration
  - Interactive tables with TanStack Table
  - Toast notifications
  - Form handling with React Hook Form and Zod validation

- **State Management & Data Fetching**
  - Global state management with Zustand
  - Data fetching with TanStack Query
  - Optimistic updates
  - Efficient caching

## 🛠️ Tech Stack

### Frontend
- React 18 with TypeScript
- Vite for build tooling
- Tailwind CSS for styling
- Radix UI for accessible components
- React Router for navigation
- Zustand for state management
- TanStack Query for data fetching
- React Hook Form with Zod for form handling
- Axios for HTTP requests

### Backend
- Node.js with Express
- TypeScript
- MongoDB with Mongoose
- Passport.js for authentication
- Cookie-session for session management
- Zod for schema validation
- CORS enabled
- Environment variables with dotenv

## 📦 Prerequisites

- Node.js (v18 or higher)
- MongoDB
- npm or yarn
- Git

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd Advanced-MERN-B2B-Teams-Project-Management-Saas
   ```

2. **Install dependencies**
   ```bash
   # Install backend dependencies
   cd backend
   npm install

   # Install frontend dependencies
   cd ../frontend
   npm install
   ```

3. **Environment Setup**
   
   Create a `.env` file in the backend directory with the following variables:
   ```
   PORT=5000
   MONGODB_URI=your_mongodb_uri
   GOOGLE_frontend_ID=your_google_frontend_id
   GOOGLE_frontend_SECRET=your_google_frontend_secret
   SESSION_SECRET=your_session_secret
   ```

4. **Start the development servers**

   In the backend directory:
   ```bash
   npm run dev
   ```

   In the frontend directory:
   ```bash
   npm run dev
   ```

   The backend will run on `http://localhost:8000` and the frontend on `http://localhost:5173`

## 📝 Available Scripts

### Backend
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run seed` - Seed the database with initial data

### Frontend
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

## 🔒 Security Features

- Secure password hashing with bcrypt
- Protected routes with authentication middleware
- CSRF protection
- Secure session management
- Environment variable protection
- Input validation with Zod

## 🧪 Testing

The application uses TypeScript for type safety and includes ESLint for code quality. To run the linter:

```bash
# In the frontend directory
npm run lint
```

📦 Advanced-MERN-B2B-Teams-Project-Management-Saas
├── 📂 backend
│   ├── 📂 src
│   │   ├── 📂 api                    # API versioning and documentation
│   │   │   ├── 📂 v1                # API version 1
│   │   │   └── 📄 swagger.json      # API documentation
│   │   ├── 📂 @types                # TypeScript type definitions
│   │   ├── 📂 config                # Configuration files
│   │   │   ├── 📄 database.ts       # Database configuration
│   │   │   ├── 📄 passport.ts       # Passport configuration
│   │   │   └── 📄 cors.ts           # CORS configuration
│   │   ├── 📂 controllers           # Route controllers
│   │   │   ├── 📂 auth              # Authentication controllers
│   │   │   ├── 📂 project           # Project controllers
│   │   │   └── 📂 user              # User controllers
│   │   ├── 📂 errors               # Custom error classes
│   │   │   ├── 📄 ApiError.ts
│   │   │   └── 📄 errorHandler.ts
│   │   ├── 📂 enums                # Enumeration types
│   │   ├── 📂 interfaces           # TypeScript interfaces
│   │   │   ├── 📄 user.interface.ts
│   │   │   └── 📄 project.interface.ts
│   │   ├── 📂 middlewares          # Express middlewares
│   │   │   ├── 📄 auth.middleware.ts
│   │   │   └── 📄 error.middleware.ts
│   │   ├── 📂 models               # Mongoose models
│   │   │   ├── 📄 User.ts
│   │   │   └── 📄 Project.ts
│   │   ├── 📂 routes               # API routes
│   │   │   ├── 📂 auth
│   │   │   ├── 📂 project
│   │   │   └── 📂 user
│   │   ├── 📂 seeders             # Database seeders
│   │   ├── 📂 services            # Business logic
│   │   │   ├── 📂 auth
│   │   │   ├── 📂 project
│   │   │   └── 📂 user
│   │   ├── 📂 tests               # Test files
│   │   │   ├── 📂 unit
│   │   │   └── 📂 integration
│   │   ├── 📂 utils               # Utility functions
│   │   │   ├── 📄 logger.ts
│   │   │   └── 📄 helpers.ts
│   │   ├── 📂 validation          # Zod validation schemas
│   │   └── 📄 index.ts            # Entry point
│   └── 📄 .env                    # Environment variables
│
├── 📂 frontend
│   ├── 📂 src
│   │   ├── 📂 api                 # API frontend and endpoints
│   │   │   ├── 📂 auth
│   │   │   ├── 📂 project
│   │   │   └── 📂 user
│   │   ├── 📂 assets             # Static assets
│   │   │   ├── 📂 images
│   │   │   └── 📂 icons
│   │   ├── 📂 components         # Reusable UI components
│   │   │   ├── 📂 common
│   │   │   ├── 📂 forms
│   │   │   └── 📂 layout
│   │   ├── 📂 constant           # Constants
│   │   │   ├── 📄 routes.ts
│   │   │   └── 📄 config.ts
│   │   ├── 📂 context            # React context
│   │   ├── 📂 features           # Feature-based modules
│   │   │   ├── 📂 auth
│   │   │   ├── 📂 project
│   │   │   └── 📂 dashboard
│   │   ├── 📂 hooks              # Custom React hooks
│   │   ├── 📂 layout             # Layout components
│   │   ├── 📂 lib                # Utility libraries
│   │   │   ├── 📄 axios.ts
│   │   │   └── 📄 utils.ts
│   │   ├── 📂 store              # Zustand store
│   │   │   ├── 📂 auth
│   │   │   └── 📂 project
│   │   ├── 📂 styles             # Global styles
│   │   │   ├── 📄 themes
│   │   │   └── 📄 global.css
│   │   ├── 📂 tests              # Test files
│   │   │   ├── 📂 unit
│   │   │   └── 📂 integration
│   │   ├── �� types              # TypeScript types
│   │   ├── 📄 App.tsx
│   │   └── 📄 main.tsx
│   └── 📄 .env                   # Environment variables
│
└── 📄 README.md



