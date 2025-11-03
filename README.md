# HR Application

A full-stack Human Resources management application built with Spring Boot and React.

## 🚀 Quick Start

### Prerequisites
- Docker and Docker Compose
- Git

### Running the Application

1. **Clone the repository**
   ```bash
   git clone https://github.com/Teoflr/hrapp.git
   cd hrapp
   git submodule update --init --recursive
   ```

2. **Set up environment variables**
   ```bash
   cp .env.example .env
   # Edit .env with your configuration
   ```

3. **Start all services**
   ```bash
   docker compose up -d --build
   ```

4. **Access the application**
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:8080
   - API Documentation: http://localhost:8080/swagger-ui.html
   - Database: localhost:5432

5. **Stop the application**
   ```bash
   docker compose down
   ```

## 📁 Project Structure

```
hrapp/
├── backend/          # Spring Boot REST API
├── frontend/         # React + Vite application
├── db_data/          # PostgreSQL data (gitignored)
├── docker-compose.yml
└── .env             # Environment variables (gitignored)
```

## 📚 Documentation

- [Backend Documentation](https://github.com/Teoflr/hrapplication-backend) - Spring Boot API details
- [Frontend Documentation](https://github.com/Teoflr/hrapplication-frontend) - React application details

## 🛠️ Technology Stack

### Backend
- Java 17
- Spring Boot 3.5.7
- PostgreSQL 15
- Flyway (Database migrations)
- Spring Security + JWT
- SpringDoc OpenAPI (Swagger)

### Frontend
- React 19
- TypeScript
- Vite
- Material-UI (MUI)
- React Router
- Zustand (State management)
- Axios

### DevOps
- Docker & Docker Compose
- Multi-stage builds for optimized images

## 🔧 Development

### Backend Development
See [backend/README.md](https://github.com/Teoflr/hrapplication-backend) for detailed backend development instructions.

### Frontend Development
See [frontend/README.md](https://github.com/Teoflr/hrapplication-frontend) for detailed frontend development instructions.

## 📝 Environment Variables

Key environment variables (see `.env.example` for full list):

```bash
# Database
DB_HOST=db
DB_PORT=5432
DB_NAME=hrapp
DB_USERNAME=postgres
DB_PASSWORD=postgres

# Backend
JWT_SECRET=your-secret-key
HUGGINGFACE_API_KEY=your-api-key
LLM_ENABLED=true

# Frontend
VITE_API_BASE_URL=http://localhost:8080/api
```

## 📄 License

This project is licensed under the MIT License.
