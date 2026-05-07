# Smart Expense Tracker with OCR 💸 🤖

> AI-powered expense management platform with OCR receipt scanning, intelligent categorization, budget tracking, and financial insights using Java + Spring Boot

![Java](https://img.shields.io/badge/Java-17-orange) ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.1.5-green) ![Tesseract OCR](https://img.shields.io/badge/Tesseract-OCR-blue) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Latest-blue) ![React](https://img.shields.io/badge/React-18.2-blue)

## 🌟 Features

### OCR & AI Capabilities
- **Receipt Scanning** - Camera/upload receipt images with Tesseract OCR text extraction
- **Smart Categorization** - ML-based automatic expense category detection
- **Merchant Recognition** - AI-powered vendor identification
- **Duplicate Detection** - Prevent duplicate expense entries

### Core Features
- **Expense Tracking** - Record and manage all expenses
- **Budget Management** - Set category-wise budgets with alerts
- **Analytics Dashboard** - Visual charts and spending insights
- **Recurring Expenses** - Auto-track subscriptions
- **Multi-Currency Support** - Handle expenses in different currencies
- **Export Reports** - PDF/Excel reports generation

## 🛠️ Tech Stack

### Backend
- **Java 17** - Core language
- **Spring Boot 3.1.5** - Application framework
- **Spring Data JPA** - Database ORM
- **PostgreSQL** - Relational database
- **Spring Security + JWT** - Authentication

### OCR & AI
- **Tesseract OCR** - Text extraction from images
- **Apache Tika** - Document parsing
- **Stanford NLP** - Natural language processing
- **Weka/DJL** - ML categorization models

### Frontend
- **React 18.2** - UI framework
- **Chart.js** - Data visualization
- **Material-UI** - Component library
- **React Camera** - Receipt capture

### Cloud & Storage
- **AWS S3** - Receipt image storage
- **Redis** - Caching layer

## 🚀 Installation

### Prerequisites
- Java 17+
- Maven 3.8+
- PostgreSQL 14+
- Tesseract OCR installed
- Docker & Docker Compose

### Quick Start

```bash
git clone https://github.com/kratikachaudhary298/smart-expense-tracker.git
cd smart-expense-tracker
docker-compose up --build
```

Backend: `http://localhost:8080`  
Frontend: `http://localhost:3000`

### Local Development

#### Backend
```bash
cd backend
mvn clean install
mvn spring-boot:run
```

#### Frontend
```bash
cd frontend
npm install
npm start
```

## 📖 Usage

### Adding Expenses
1. **Manual Entry** - Enter amount, category, date
2. **Receipt Scan** - Take photo or upload receipt
3. **AI Processing** - System extracts amount, merchant, date
4. **Review & Save** - Confirm details and save

### Budget Management
1. Set monthly/yearly budgets per category
2. Track spending vs budget in real-time
3. Get alerts when nearing limits

### Analytics
- View spending trends over time
- Category-wise breakdown
- Compare monthly expenses
- Export financial reports

## 🏗️ Architecture

```
├── backend/
│   ├── src/main/java/com/expense/
│   │   ├── config/          # Security, OCR configs
│   │   ├── controller/      # REST APIs
│   │   ├── service/         # Business logic
│   │   ├── ocr/             # OCR processing
│   │   ├── ml/              # ML categorization
│   │   ├── model/           # JPA entities
│   │   └── repository/      # Data access
│   └── pom.xml
├── frontend/
│   ├── src/
│   │   ├── components/      # React components
│   │   ├── pages/           # Main pages
│   │   ├── services/        # API integration
│   │   └── utils/           # Helper functions
│   └── package.json
└── docker-compose.yml
```

## 📊 Key Endpoints

- `POST /api/expenses` - Create expense
- `POST /api/expenses/scan` - Upload receipt for OCR
- `GET /api/expenses` - Get all expenses
- `GET /api/analytics/summary` - Get spending summary
- `POST /api/budgets` - Set budget
- `GET /api/reports/export` - Export PDF/Excel

## 🔮 Future Enhancements
- Voice input for expenses
- Bank statement auto-import
- Predictive budgeting with AI
- Split expense sharing
- Mobile app (React Native)
- Cryptocurrency tracking

## 👤 Author

**Kratika Chaudhary**  
Full-Stack Java Developer | FinTech Enthusiast  
GitHub: [@kratikachaudhary298](https://github.com/kratikachaudhary298)

---

⭐ Star this repo if you find it helpful!
