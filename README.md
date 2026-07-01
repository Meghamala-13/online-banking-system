# Online Banking System (Enterprise Banking)

A comprehensive enterprise-grade banking application built with Java Spring Boot, featuring customer management, money transfers, loan management, and advanced security features.

## 🌟 Features

### Core Banking Features
- **Customer Login** - Secure authentication for customers
- **Admin Dashboard** - Administrative controls and management
- **Employee Portal** - Employee access and operations
- **KYC (Know Your Customer)** - Customer verification process
- **Money Transfer** - Fund transfer between accounts
- **UPI Simulation** - UPI payment simulation
- **Loan Management** - Loan application and management
- **Credit Card** - Credit card operations
- **EMI** - Equated Monthly Installment calculations
- **Statements** - Account statements and reports
- **Cheque Book** - Cheque management
- **Transaction History** - Complete transaction tracking
- **Notifications** - Real-time notifications

### Advanced Security
- **OTP Login** - One-Time Password authentication
- **QR Payments** - QR code-based payments
- **JWT** - JSON Web Token authentication
- **Spring Security** - Comprehensive security framework
- **Encryption** - Data encryption
- **Audit Logs** - Complete audit trail
- **Role-Based Access Control (RBAC)** - Fine-grained permissions

### DevOps & Deployment
- **Docker** - Containerization support
- **Cloud Deployment** - Cloud-ready architecture

## 🛠️ Tech Stack

- **Framework:** Spring Boot 3.x
- **Language:** Java 17+
- **Database:** PostgreSQL / MySQL
- **Security:** Spring Security, JWT
- **Build Tool:** Maven
- **Containerization:** Docker
- **ORM:** Hibernate/JPA

## 📋 Project Structure

```
online-banking-system/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/banking/
│   │   │       ├── auth/              # Authentication & JWT
│   │   │       ├── customer/          # Customer management
│   │   │       ├── admin/             # Admin operations
│   │   │       ├── employee/          # Employee management
│   │   │       ├── transaction/       # Money transfers & transactions
│   │   │       ├── loan/              # Loan management
│   │   │       ├── creditcard/        # Credit card operations
│   │   │       ├── kyc/               # KYC verification
│   │   │       ├── notification/      # Notifications
│   │   │       ├── fraud/             # Fraud detection
│   │   │       ├── audit/             # Audit logs
│   │   │       ├── upi/               # UPI simulation
│   │   │       ├── config/            # Configuration classes
│   │   │       └── util/              # Utility classes
│   │   └── resources/
│   │       ├── application.properties
│   │       └── db/
│   │           └── migration/         # Database migrations (Flyway)
│   └── test/
│       └── java/
│           └── com/banking/           # Unit & integration tests
├── docker/
│   └── Dockerfile
├── docker-compose.yml
├── pom.xml
└── README.md
```

## 🚀 Getting Started

### Prerequisites
- Java 17 or higher
- Maven 3.6+
- PostgreSQL 12+ or MySQL 5.7+
- Docker (optional)

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/Meghamala-13/online-banking-system.git
cd online-banking-system
```

2. **Configure Database**
```bash
# Create database
createdb banking_db

# Update application.properties with your database credentials
```

3. **Build the project**
```bash
mvn clean package
```

4. **Run the application**
```bash
mvn spring-boot:run
```

The application will start on `http://localhost:8080`

### Using Docker

```bash
# Build Docker image
docker build -t online-banking-system .

# Run with docker-compose
docker-compose up -d
```

## 📚 API Documentation

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/api/auth/login` | POST | Customer login |
| `/api/auth/register` | POST | Customer registration |
| `/api/customers/profile` | GET | Get customer profile |
| `/api/transactions/transfer` | POST | Money transfer |
| `/api/loans/apply` | POST | Apply for loan |
| `/api/cards/create` | POST | Create credit card |

## 🔐 Security

- JWT-based authentication
- Role-based access control (RBAC)
- Spring Security integration
- OTP verification
- Data encryption for sensitive information
- SQL injection prevention
- CSRF protection

## 🧪 Testing

```bash
# Run all tests
mvn test

# Run specific test class
mvn test -Dtest=UserControllerTest
```

## 📦 Database Schema

The database includes tables for:
- Users (customers, employees, admins)
- Accounts
- Transactions
- Loans
- Credit Cards
- KYC Documents
- Audit Logs
- Notifications

## 🐛 Troubleshooting

### Common Issues

1. **Database connection error**
   - Ensure PostgreSQL is running
   - Check credentials in `application.properties`

2. **Port already in use**
   - Change port in `application.properties`: `server.port=8081`

3. **Maven build failure**
   - Clear cache: `mvn clean`
   - Update dependencies: `mvn dependency:resolve`

## 📝 Contributing

1. Create a feature branch (`git checkout -b feature/AmazingFeature`)
2. Commit your changes (`git commit -m 'Add AmazingFeature'`)
3. Push to the branch (`git push origin feature/AmazingFeature`)
4. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see LICENSE file for details.

## 👨‍💼 Author

**Mallavarapu.Meghamala**

## 📞 Support

For support, email support@bankingsystem.com or create an issue in the repository.

---

**Last Updated:** July 2026
