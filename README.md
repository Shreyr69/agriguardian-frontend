# Agri-Guardian Frontend Application

React + Vite frontend for the Agri-Guardian intelligent pest management and agricultural advisory platform.

## 🏗️ Architecture

- **Framework**: React 18
- **Build Tool**: Vite
- **Styling**: Tailwind CSS & Shadcn UI
- **Routing**: React Router DOM
- **State Management**: React Context / Hooks
- **Icons**: Lucide React
- **HTTP Client**: Context-based API Integration

## 📁 Project Structure

```
frontend/
├── src/
│   ├── components/       # Reusable UI components (Shadcn + Custom)
│   ├── config/           # Application configuration
│   ├── hooks/            # Custom React hooks
│   ├── lib/              # Utility functions and API clients
│   ├── pages/            # Main route page components
│   ├── types/            # TypeScript definitions
│   ├── App.tsx           # Root application component
│   └── main.tsx          # Application entry point
├── public/               # Static assets
├── index.html            # Main HTML template
├── package.json          # Dependencies
├── tailwind.config.ts    # Tailwind CSS configuration
├── tsconfig.json         # TypeScript configuration
└── vite.config.ts        # Vite build configuration
```

## 🚀 Quick Start

### 1. Install Dependencies

```bash
npm install
```

### 2. Set Up Environment Variables

Create a `.env` file in the root of the `frontend` directory:

```env
VITE_API_URL=http://localhost:5000/api
```

*(Note: Change the `VITE_API_URL` to your production backend URL when deploying)*

### 3. Start Development Server

```bash
npm run dev
```

The application will launch typically at `http://localhost:8080` (or `http://localhost:5173`).

### 4. Build for Production

```bash
npm run build
```

This will create an optimized production build in the `dist` directory.

## 📱 Key Features

1. **Authentication**: Complete user registration and login flow with JWT token management.
2. **Dashboard**: Personalized agricultural overview including active crops and recent alerts.
3. **Pest Identification**: AI-powered image recognition and symptom checking for crop diseases.
4. **Advisory System**: Context-aware AI chat assistant providing IPM (Integrated Pest Management) recommendations.
5. **Community Forum**: Interactive space for farmers to share knowledge, post questions, and interact.
6. **Spray Logs**: Detailed tracking of pesticide applications and maintenance.

## 🎨 UI/UX Design

The application utilizes **Shadcn UI** built on top of Tailwind CSS for a highly accessible, customizable, and modern interface. It features:
- Responsive design for mobile, tablet, and desktop viewing.
- Modern glassmorphism effects and clean typography.
- Interactive alerts and real-time notifications.
- Accessible forms and data tables.

## 🤝 Integration with Backend

This frontend is designed to work seamlessly with the `taskflow-backend` (Node + Express + MongoDB) service. 

Ensure the backend server is running and accessible at the URL defined in your `VITE_API_URL` environment variable for full functionality, including user authentication and AI advisory features.

## 📄 License

MIT
