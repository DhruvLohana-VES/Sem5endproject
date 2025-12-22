# CareCue - Medication Adherence Platform (Frontend)

A comprehensive healthcare platform frontend for managing medication adherence with separate modules for Patients, Caretakers, and Blood Donors.

## 🏗️ Project Structure

```
CC Frontend/         # React + Vite
```

**Note:** Backend is in a separate repository for security reasons.

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ installed
- Backend API running (separate repo)
- Git

### Frontend Setup

1. Navigate to frontend:
```bash
cd "CC Frontend"
```

2. Install dependencies:
```bash
npm install
```

3. Create `.env` file:
```env
VITE_API_BASE_URL=http://localhost:5001/api
VITE_USE_MOCK_API=false
```

4. Start frontend:
```bash
npm run dev
```

Frontend runs on: http://localhost:3000

## 📱 Features

### Patient Module
- Track daily medication doses
- View medication schedule
- Mark doses as taken/missed
- View adherence statistics

### Caretaker Module
- Manage multiple patients
- Add/edit medications for patients
- View patient adherence reports
- Send link invitations to patients

### Donor Module
- Blood donor profile management
- View active donation requests
- Accept donation requests
- Track donation history

## 🛠️ Tech Stack

### Backend
- Node.js & Express
- Supabase (PostgreSQL)
- JWT Authentication
- Express Validator

### Frontend
- React 18
- Vite
- TailwindCSS
- React Router
- Axios

## 📚 API Documentation

Base URL: `http://localhost:5001/api`

### Authentication
- `POST /auth/register` - Register new user
- `POST /auth/login` - Login user
- `GET /auth/me` - Get current user (protected)

### Medications
- `GET /medications` - Get user's medications
- `POST /medications` - Create medication (caretaker)
- `PATCH /medications/:id` - Update medication
- `DELETE /medications/:id` - Delete medication

### Doses
- `GET /doses/today` - Get today's doses
- `GET /doses/history` - Get dose history
- `PATCH /doses/:id/take` - Mark as taken
- `PATCH /doses/:id/miss` - Mark as missed

[See full API documentation in backend README]

## 🔒 Security

- JWT-based authentication
- Password hashing with bcrypt
- Environment variables for sensitive data
- Row Level Security in Supabase
- CORS protection

## 📝 License

MIT License

## 👥 Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## 🐛 Issues

Report issues at: [GitHub Issues]

## 📧 Contact

For questions or support, please open an issue.
