# certiflow-server

## 🔧 Setup Instructions

Before starting the application, follow these setup steps:

### 1. Configure CORS in `server.js`

Ensure the client application's port is allowed in the `corsOptions`:

```
const corsOptions = {
  origin: 'http://localhost:3000', // Replace with your frontend URL
  credentials: true,
};

app.use(cors(corsOptions));
```

### 2. Create a .env file in the project root
The file should contain the following environment variables:

```
PORT=5000 # Or any preferred port
AUTH_TOKEN_SECRET=your_jwt_secret_key
AUTH_TOKEN_TIME_LIMIT=1h # e.g., 1h, 24h
DEFAULT_PASSWORD=your_default_password
```

### 3. Install dependencies and start the server

```
npm install
npm start
```
