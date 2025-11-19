# Resume AI

A full-stack AI-powered resume builder and analyzer application that helps users create professional resumes with intelligent suggestions and formatting.

## 🚀 Features

- **AI-Powered Resume Generation**: Generate professional resumes using AI assistance
- **Smart Resume Analysis**: Get intelligent feedback on your resume content
- **Modern UI/UX**: Clean, responsive interface built with React and Tailwind CSS
- **Real-time Preview**: See changes to your resume in real-time
- **Multiple Templates**: Choose from various professional resume templates
- **Export Options**: Download your resume in multiple formats

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** (v16 or higher)
- **Java JDK** (v17 or higher)
- **Maven** (v3.8 or higher)
- **Git**

## 🛠️ Tech Stack

### Frontend

- **React** with TypeScript
- **Vite** - Fast build tool
- **Tailwind CSS** - Utility-first CSS framework
- **shadcn/ui** - Re-usable component library
- **React Router** - Client-side routing

### Backend

- **Spring Boot** - Java framework
- **Maven** - Dependency management
- **RESTful API** architecture

## 📦 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Akhil-Ferry/Resume_AI.git
cd Resume_AI
```

### 2. Backend Setup

```bash
cd backend

# Build the project
./mvnw clean install

# Run the application
./mvnw spring-boot:run
```

The backend will start on `http://localhost:8080`

### 3. Frontend Setup

```bash
cd frontend

# Install dependencies
npm install

# Start development server
npm run dev
```

The frontend will start on `http://localhost:5173`

## 🔧 Configuration

### Backend Configuration

Configure your application properties in `backend/src/main/resources/application.properties`:

```properties
# Server port
server.port=8080

# Add your AI API keys and other configurations here
```

### Frontend Configuration

Update environment variables in `frontend/.env` (create if it doesn't exist):

```env
VITE_API_BASE_URL=http://localhost:8080/api
```

## 📝 Usage

1. **Start the Backend**: Navigate to the `backend` directory and run the Spring Boot application
2. **Start the Frontend**: Navigate to the `frontend` directory and run the Vite dev server
3. **Access the Application**: Open your browser and go to `http://localhost:5173`
4. **Create Your Resume**: Follow the on-screen instructions to build your AI-powered resume

## 🐳 Docker Support

### Build and Run with Docker

```bash
# Backend
cd backend
docker build -t resume-ai-backend .
docker run -p 8080:8080 resume-ai-backend

# Frontend (configure Dockerfile as needed)
cd frontend
docker build -t resume-ai-frontend .
docker run -p 5173:5173 resume-ai-frontend
```

## 📂 Project Structure

```
Resume_AI/
├── backend/                 # Spring Boot backend
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/       # Java source files
│   │   │   └── resources/  # Application properties
│   │   └── test/           # Unit tests
│   ├── Dockerfile
│   └── pom.xml             # Maven dependencies
│
└── frontend/               # React frontend
    ├── src/
    │   ├── components/     # Reusable UI components
    │   ├── routes/         # Page components
    │   ├── services/       # API service layer
    │   ├── lib/            # Utility functions
    │   ├── assets/         # Static assets
    │   ├── App.tsx         # Main app component
    │   ├── main.tsx        # Entry point
    │   └── UserContext.tsx # Global state management
    ├── public/             # Public assets
    ├── package.json
    └── vite.config.ts      # Vite configuration
```

## 🧪 Running Tests

### Backend Tests

```bash
cd backend
./mvnw test
```

### Frontend Tests

```bash
cd frontend
npm run test
```

## 🔨 Build for Production

### Backend

```bash
cd backend
./mvnw clean package
java -jar target/*.jar
```

### Frontend

```bash
cd frontend
npm run build
```

The production build will be in the `dist` folder.

## 🚀 Deployment

### Frontend (Vercel)

The frontend is configured for Vercel deployment with [`vercel.json`](frontend/vercel.json).

```bash
cd frontend
vercel deploy
```

### Backend

Deploy the Spring Boot application to your preferred hosting service (AWS, Heroku, Railway, etc.)

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👥 Authors

- **Akhil Ferry** - [GitHub Profile](https://github.com/Akhil-Ferry)

## 🙏 Acknowledgments

- Thanks to all contributors who have helped shape this project
- shadcn/ui for the beautiful component library
- The Spring Boot and React communities for excellent documentation

## 📧 Contact

For questions or support, please open an issue or contact:

- GitHub: [@Akhil-Ferry](https://github.com/Akhil-Ferry)

---

Made with ❤️ by Akhil Ferry
