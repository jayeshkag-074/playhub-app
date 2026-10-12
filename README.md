# playhub-app
This is a application for booking turf.

# 🎾 PlayHub — Sports Venue Booking Platform

PlayHub is a sports venue booking application designed to help users discover sports facilities, explore available venues, and manage their bookings in one place.

The platform aims to simplify sports venue discovery and booking through a user-friendly interface and a RESTful backend.

## ✨ Features

- 🏟️ Browse and explore sports venues
- 🔍 Search for venues by sport or location
- 📅 Book sports venues and manage reservations
- 👤 User registration and login
- 🔐 Authentication and authorization
- 🛠️ Manage venue details and bookings
- 📱 Responsive user interface
- 🔗 REST API integration between frontend and backend

> Note: Update this feature list to match the features currently implemented in your application.

## 🧰 Tech Stack

### Frontend
- Angular
- HTML5
- CSS3
- TypeScript

### Backend
- Java
- Spring Boot
- Spring Web
- Spring Data JPA
- Spring Security (if configured)

### Database
- MySQL

### Development Tools
- Git and GitHub
- IntelliJ IDEA
- Visual Studio Code
- Postman

## 🏗️ Project Structure

```text
playhub-app/
├── backend/
│   └── playhub-backend/
│       ├── src/
│       ├── pom.xml
│       └── ...
│
├── frontend/
│   └── playhub-frontend/
│       ├── src/
│       ├── angular.json
│       └── ...
│
└── README.md
```

## ⚙️ Prerequisites

Install the following before running the project:

- Java JDK 21
- Node.js (compatible with your Angular version)
- Angular CLI
- MySQL Server
- Maven (or use the Maven Wrapper if included)
- Git

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/jayeshkag-074/playhub-app.git
cd playhub-app
```

### 2. Configure the Database

Create a MySQL database:

```sql
CREATE DATABASE playhub;
```

Configure your backend's `application.properties` file:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/playhub
spring.datasource.username=${DB_USERNAME}
spring.datasource.password=${DB_PASSWORD}

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

Set `DB_USERNAME` and `DB_PASSWORD` in your environment, or configure your local credentials securely. Adjust the database name and JPA settings to match your application.

### 3. Run the Spring Boot Backend

Open a terminal:

```bash
cd backend/playhub-backend
```

Run using Maven:

```bash
mvn spring-boot:run
```

The backend will typically start at:

```text
http://localhost:8080
```

### 4. Run the Angular Frontend

Open another terminal:

```bash
cd frontend/playhub-frontend
npm install
ng serve
```

Open the application in your browser:

```text
http://localhost:4200
```

Ensure that the frontend API URL matches your backend URL and that CORS is configured appropriately.

## 🔌 API Endpoints

Example endpoint structure (actual endpoints depend on your implementation):

| Method | Endpoint | Purpose |
|---|---|---|
| GET | `/api/venues` | Retrieve venues |
| GET | `/api/venues/{id}` | Retrieve a venue by ID |
| POST | `/api/venues` | Create a venue |
| PUT | `/api/venues/{id}` | Update a venue |
| DELETE | `/api/venues/{id}` | Delete a venue |
| POST | `/api/bookings` | Create a booking |
| GET | `/api/bookings` | Retrieve bookings |

## 🔐 Security

If Spring Security is enabled, configure authentication and authorization according to your requirements.

- Protect endpoints that require authentication.
- Apply role-based access control where appropriate.
- Never commit passwords, API keys, JWT secrets, or other sensitive credentials.
- Validate incoming requests on the backend.

## 🧪 Testing

Backend:
- Run automated tests with `mvn test`.
- Test REST endpoints using Postman.

Frontend:
- Run Angular tests using `ng test` if the project's test setup is configured.

## 🛣️ Future Enhancements

- Online payment integration
- Real-time venue availability
- Booking cancellation and rescheduling
- Email and booking notifications
- Reviews and ratings
- Interactive maps and location-based discovery
- Admin dashboard and analytics

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository.
2. Create a feature branch:

   ```bash
   git switch -c feature/your-feature
   ```

3. Commit your changes:

   ```bash
   git add .
   git commit -m "Add your feature"
   ```

4. Push your branch:

   ```bash
   git push -u origin feature/your-feature
   ```

5. Open a Pull Request.

## 📄 License

Choose and add a license before distributing this project publicly.

---

**Built with ❤️ using Java, Spring Boot, Angular, and MySQL.**
