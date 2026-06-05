# OctoFit Tracker - Multi-Tier Application

A modern multi-tier application for tracking fitness activities using GitHub Copilot agent mode.

## Architecture

```
octofit-tracker/
├── frontend/          # React 19 + Vite application
│   └── Port: 5173
├── backend/           # Node.js + Express + TypeScript API
│   └── Port: 8000
└── MongoDB Database
    └── Port: 27017
```

## Prerequisites

- Node.js 18+ and npm/yarn
- MongoDB 5.0+
- TypeScript 5.0+

## Setup Instructions

### Frontend Setup

```bash
cd octofit-tracker/frontend
npm install
npm run dev
```

The frontend will be available at `http://localhost:5173`

### Backend Setup

```bash
cd octofit-tracker/backend
npm install

# Create .env file
cp .env.example .env

# Start development server
npm run dev
```

The backend API will be available at `http://localhost:8000`

### MongoDB Setup

Ensure MongoDB is running on `localhost:27017` or update the `MONGODB_URI` in the backend `.env` file.

## Technologies

### Frontend
- **React 19**: Latest version of React with new features
- **Vite**: Next generation frontend tooling
- **TypeScript**: Type-safe JavaScript

### Backend
- **Express.js**: Fast web framework
- **Node.js**: Runtime environment
- **TypeScript**: Type-safe backend development
- **Mongoose**: MongoDB object modeling

## Development

### Frontend Development
```bash
cd frontend
npm run dev      # Start development server
npm run build    # Build for production
npm run preview  # Preview production build
```

### Backend Development
```bash
cd backend
npm run dev         # Start with auto-reload
npm run build       # Compile TypeScript
npm start           # Run compiled code
npm run type-check  # Check types without emitting
```

## Project Structure

### Frontend
```
frontend/
├── src/
│   ├── App.tsx
│   ├── App.css
│   ├── main.tsx
│   └── index.css
├── index.html
├── package.json
├── tsconfig.json
└── vite.config.ts
```

### Backend
```
backend/
├── src/
│   └── index.ts
├── dist/
├── package.json
├── tsconfig.json
└── .env.example
```

## API Endpoints

- `GET /` - Welcome message
- `GET /api/health` - Health check

## Port Configuration

- **Frontend**: 5173 (Vite dev server)
- **Backend**: 8000 (Express server)
- **MongoDB**: 27017 (Default MongoDB port)

## Next Steps

1. Install dependencies for both frontend and backend
2. Configure MongoDB connection
3. Start MongoDB service
4. Run development servers
5. Begin building features with GitHub Copilot agent mode
