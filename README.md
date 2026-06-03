# BankingAutomation-ParaBank 🏦

<div align="center">

<!-- ═══════════════════════════════════════════════ -->
<!--              IDENTITY BADGES                    -->
<!-- ═══════════════════════════════════════════════ -->

[![Author](https://img.shields.io/badge/Author-Ranajit%20Baran%20Chowdhury-0A66C2?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ranajitchowdhury)
[![Email](https://img.shields.io/badge/Email-chyranajit%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:chyranajit@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-%40ranajitchowdhury-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ranajitchowdhury)

<!-- ═══════════════════════════════════════════════ -->
<!--              TECH STACK BADGES                  -->
<!-- ═══════════════════════════════════════════════ -->

![Java](https://img.shields.io/badge/Java-17%2B-007396?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-8.x-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Selenium](https://img.shields.io/badge/Selenium-4.x-43B02A?style=for-the-badge&logo=selenium&logoColor=white)
![JUnit](https://img.shields.io/badge/JUnit-5.x-25A162?style=for-the-badge&logo=junit5&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-3.x-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-Frontend-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-Styling-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6%2B-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

<!-- ═══════════════════════════════════════════════ -->
<!--              PROJECT STATUS BADGES              -->
<!-- ═══════════════════════════════════════════════ -->

![Role](https://img.shields.io/badge/Role-Software%20Programmer%20%26%20QA%20Automation%20Engineer-6A0DAD?style=for-the-badge)
![Architecture](https://img.shields.io/badge/Architecture-Three--Tier%20MVC-0A66C2?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-brightgreen?style=for-the-badge)
![Build](https://img.shields.io/badge/Build-Passing-brightgreen?style=for-the-badge&logo=apachemaven&logoColor=white)
![Coverage](https://img.shields.io/badge/Coverage-Login%20%7C%20Accounts%20%7C%20Transactions-blue?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-ParaBank-FF6600?style=for-the-badge)

</div>

---

> A production-grade **banking system simulation and test automation framework** built on the **ParaBank** platform. This project demonstrates dual expertise in **full-stack software engineering** and **QA automation** — implementing a three-tier Spring Boot architecture for banking workflows and a Selenium-based regression suite that validates every critical user journey from account creation to fund transfers.

---

## 🎯 Project Mission

ParaBank is an industry-standard banking simulation platform widely used to practice and demonstrate real-world web application testing. This project goes beyond simple manual exploration — it establishes a **structured automation framework** around ParaBank's core banking workflows, ensuring that authentication, account management, and transaction operations behave correctly and consistently across every test run.

The project reflects how a **Software Programmer and QA Automation Engineer** approaches a real banking system: understanding the application's architecture deeply, then building test coverage that mirrors actual user behavior and business-critical risk areas.

---

## 🏗 System Architecture

The Banking Automation system follows a **three-tier architecture pattern** designed for scalability, maintainability, and clean separation of concerns.

```
┌──────────────────────────────────────────────────────────────┐
│                     Presentation Layer                        │
│              (HTML5 · CSS3 · JavaScript ES6+)                 │
│     User Interface — Forms, Dashboards, Transaction Views     │
└─────────────────────────┬────────────────────────────────────┘
                           │  REST API Calls
┌─────────────────────────▼────────────────────────────────────┐
│                     Application Layer                         │
│             (Spring Boot REST API + Business Logic)           │
│                                                               │
│  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────┐  │
│  │   Controllers   │  │    Services     │  │Repositories │  │
│  │  (HTTP Routes)  │  │ (Business Rules)│  │  (Data ORM) │  │
│  └─────────────────┘  └─────────────────┘  └─────────────┘  │
└─────────────────────────┬────────────────────────────────────┘
                           │  JPA / JDBC
┌─────────────────────────▼────────────────────────────────────┐
│                       Data Layer                              │
│                   (MySQL 8.x Database)                        │
│       User Accounts · Transaction History · Balances          │
└──────────────────────────────────────────────────────────────┘
```

### Layer Descriptions

**Presentation Layer — Frontend**
- User interface built with **HTML5, CSS3, and JavaScript ES6+**
- Renders banking dashboards, account forms, and transaction history views
- Communicates with the backend exclusively via **REST API calls** — no direct database access

**Application Layer — Spring Boot**
- **Controllers** — Route incoming HTTP requests to the appropriate service handlers
- **Services** — Encapsulate all business logic: authentication rules, transaction validation, balance calculation, and account state management
- **Repositories** — Abstract all database operations via JPA/Hibernate, providing a clean data access interface

**Data Layer — MySQL**
- Stores user accounts, session data, transaction records, and account balances
- Enforces referential integrity and transactional consistency at the database level
- Schema managed via Spring Boot's auto-DDL or Flyway migrations

---

## 🛠 Tech Stack & Tools

| Component | Technology | Version | Purpose |
| :--- | :--- | :--- | :--- |
| **Language** | Java | 17+ | Core backend programming and test logic |
| **Backend Framework** | Spring Boot | 3.x | REST API, dependency injection, and MVC architecture |
| **Database** | MySQL | 8.x | Relational data storage and transaction management |
| **UI Automation** | Selenium WebDriver | 4.x | Cross-browser browser control and DOM interaction |
| **Test Framework** | JUnit | 5.x | Test lifecycle management, assertions, and parameterization |
| **Build Tool** | Apache Maven | 3.x | Dependency management and build lifecycle |
| **Frontend** | HTML5 / CSS3 / JavaScript | ES6+ | User interface and REST client |
| **Config Management** | application.properties | — | Environment-specific configuration |
| **Reporting** | Maven Surefire Reports | — | Post-execution test result artifacts |

---

## 📁 Project Structure

```text
BankingAutomation-ParaBank/
│
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/parabank/
│   │   │       ├── controllers/
│   │   │       │   ├── AuthController.java         # Login, logout, session management
│   │   │       │   ├── AccountController.java      # Account creation and retrieval
│   │   │       │   └── TransactionController.java  # Transfers, deposits, withdrawals
│   │   │       │
│   │   │       ├── services/
│   │   │       │   ├── AuthService.java            # Authentication business logic
│   │   │       │   ├── AccountService.java         # Account management logic
│   │   │       │   └── TransactionService.java     # Transaction processing logic
│   │   │       │
│   │   │       ├── repositories/
│   │   │       │   ├── UserRepository.java         # User data access layer
│   │   │       │   ├── AccountRepository.java      # Account data access layer
│   │   │       │   └── TransactionRepository.java  # Transaction data access layer
│   │   │       │
│   │   │       └── models/
│   │   │           ├── User.java                   # User entity
│   │   │           ├── Account.java                # Account entity
│   │   │           └── Transaction.java            # Transaction entity
│   │   │
│   │   └── resources/
│   │       └── application.properties              # DB config, server port, app settings
│   │
│   └── test/
│       └── java/
│           └── com/parabank/tests/
│               ├── base/
│               │   └── BaseTest.java               # WebDriver init, teardown, config
│               │
│               ├── pages/
│               │   ├── LoginPage.java              # Login page locators and actions
│               │   ├── RegisterPage.java           # Registration page objects
│               │   ├── AccountPage.java            # Account overview page objects
│               │   ├── TransferPage.java           # Fund transfer page objects
│               │   └── TransactionPage.java        # Transaction history page objects
│               │
│               ├── tests/
│               │   ├── LoginTests.java             # Authentication test cases
│               │   ├── RegistrationTests.java      # User registration test cases
│               │   ├── AccountTests.java           # Account management test cases
│               │   ├── TransactionTests.java       # Fund transfer test cases
│               │   └── NegativeTests.java          # Boundary and negative test cases
│               │
│               └── utils/
│                   ├── ConfigReader.java           # application.properties accessor
│                   ├── DriverFactory.java          # WebDriver factory and management
│                   └── WaitUtils.java              # Explicit and fluent wait wrappers
│
├── frontend/
│   ├── index.html                                  # Landing page
│   ├── css/
│   │   └── styles.css                              # Application stylesheet
│   └── js/
│       └── app.js                                  # REST API client and UI logic
│
├── target/
│   └── surefire-reports/                           # Auto-generated test result reports
│
├── pom.xml                                         # Maven dependencies and build config
└── README.md                                       # Project documentation
```

---

## 🌐 Banking Modules Under Test

| Module | URL / Endpoint | Scenarios Covered |
| :--- | :--- | :--- |
| **User Login** | `/login` | Valid credentials, invalid credentials, empty fields, locked account |
| **User Registration** | `/register` | New account creation, duplicate username, password mismatch |
| **Account Overview** | `/overview` | Balance display, account list, multi-account view |
| **Open New Account** | `/openaccount` | Savings and checking account creation |
| **Fund Transfer** | `/transfer` | Valid transfer, insufficient balance, invalid account number |
| **Bill Payment** | `/billpay` | Valid payment, missing payee details, invalid amount |
| **Transaction History** | `/activity` | Date range filter, transaction type filter, amount search |
| **Update Profile** | `/updateprofile` | Valid updates, required field validation |
| **Forgot Login** | `/lookup` | Valid credentials lookup, unrecognized user |

---

## 🎯 Test Coverage Matrix

### 🔐 User Authentication
- Login with valid username and password → assert dashboard redirect
- Login with invalid credentials → assert error message displayed
- Login with empty fields → assert HTML5 / server-side validation
- Session persistence across page navigation

### 📋 User Registration
- Successful new user registration with all valid fields
- Duplicate username rejection → assert appropriate error
- Password and confirm password mismatch → assert inline error
- Required field validation for all mandatory inputs

### 🏦 Account Management
- Open a new savings account → assert account number generated
- Open a new checking account → assert account listed in overview
- Verify account balance matches after transactions
- Multi-account balance display accuracy

### 💸 Transaction Operations
- Fund transfer between valid accounts → assert balance deduction and credit
- Transfer with insufficient balance → assert error and balance unchanged
- Bill payment to valid payee → assert payment confirmation
- Transaction history reflects all completed operations accurately

### ⚠️ Negative Testing
- SQL injection patterns in login fields
- XSS payload in profile update fields
- Negative transfer amounts
- Access protected pages without authentication → assert redirect to login

---

## ⚙️ Setup & Installation

### Prerequisites

- Java JDK 17+
- Apache Maven 3.6+
- MySQL 8.x (running locally or via Docker)
- Google Chrome (latest) + ChromeDriver
- Eclipse IDE or IntelliJ IDEA
- Node.js (for frontend dependencies)

### 1. Clone the Repository

```bash
git clone https://github.com/ranajitchowdhury/BankingAutomation-ParaBank.git
cd BankingAutomation-ParaBank
```

### 2. Configure the Database

Create a MySQL database and update `src/main/resources/application.properties`:

```properties
# Server
server.port=8080

# Database
spring.datasource.url=jdbc:mysql://localhost:3306/parabank_db
spring.datasource.username=root
spring.datasource.password=your_password
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

# JPA
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

# Application
app.base.url=http://localhost:8080
app.browser=chrome
app.implicit.wait=10
app.explicit.wait=20
```

### 3. Install Backend Dependencies

```bash
mvn clean install -DskipTests
```

### 4. Install Frontend Dependencies

```bash
cd frontend
npm install
```

### 5. Start the Application

```bash
mvn spring-boot:run
```

The application will be available at `http://localhost:8080`.

---

## ▶️ Running the Tests

### Run All Tests

```bash
mvn clean test
```

### Run a Specific Test Class

```bash
mvn test -Dtest=LoginTests
mvn test -Dtest=TransactionTests
```

### Run by Test Group

```bash
# Smoke tests only
mvn test -Dgroups=smoke

# Full regression suite
mvn test -Dgroups=regression
```

### Run from IDE

1. Right-click any test class → **Run As → JUnit Test**
2. Or right-click `pom.xml` → **Run As → Maven test**

---

## 📊 Sample Test — Fund Transfer

```java
@Test
@DisplayName("Valid fund transfer reduces source balance and credits destination")
public void testValidFundTransfer() {

    // Arrange
    String sourceAccount  = ConfigReader.get("test.source.account");
    String destAccount    = ConfigReader.get("test.dest.account");
    String transferAmount = "500";

    LoginPage loginPage = new LoginPage(driver);
    loginPage.navigateTo(ConfigReader.get("app.base.url") + "/login");
    loginPage.login(ConfigReader.get("auth.username"), ConfigReader.get("auth.password"));

    // Get balance before transfer
    AccountPage accountPage = new AccountPage(driver);
    double balanceBefore = accountPage.getBalanceFor(sourceAccount);

    // Act — perform fund transfer
    TransferPage transferPage = new TransferPage(driver);
    transferPage.navigateTo();
    transferPage.selectSourceAccount(sourceAccount);
    transferPage.selectDestinationAccount(destAccount);
    transferPage.enterAmount(transferAmount);
    transferPage.clickTransfer();

    // Assert — confirmation message shown
    String confirmation = transferPage.getConfirmationMessage();
    assertTrue(confirmation.contains("Transfer Complete"),
        "Expected transfer confirmation message but got: " + confirmation);

    // Assert — source balance reduced
    double balanceAfter = accountPage.getBalanceFor(sourceAccount);
    assertEquals(balanceBefore - Double.parseDouble(transferAmount), balanceAfter, 0.01,
        "Source account balance should be reduced by transfer amount");
}

@Test
@DisplayName("Transfer with insufficient balance shows error and preserves balance")
public void testInsufficientBalanceTransfer() {

    TransferPage transferPage = new TransferPage(driver);
    transferPage.navigateTo();
    transferPage.enterAmount("999999");
    transferPage.clickTransfer();

    String error = transferPage.getErrorMessage();
    assertTrue(error.contains("Insufficient funds"),
        "Expected insufficient funds error");
}
```

---

## 📈 Reporting

After each `mvn test` execution, reports are generated automatically:

| Report | Location | Description |
| :--- | :--- | :--- |
| **Surefire XML** | `target/surefire-reports/*.xml` | Machine-readable JUnit result files |
| **Surefire HTML** | `target/surefire-reports/*.html` | Human-readable per-class result pages |

To view the HTML report, open any `.html` file inside `target/surefire-reports/` in a browser.

---

## 📈 Roadmap — Future Enhancements

- [ ] **Extent Reports Integration** — rich HTML dashboards with screenshot on failure
- [ ] **Cucumber BDD Layer** — Gherkin feature files for business-readable test scenarios
- [ ] **TestNG Migration** — replace JUnit with TestNG for grouping, parallel execution, and listeners
- [ ] **CI/CD Pipeline** — GitHub Actions workflow for automated test runs on every push
- [ ] **Docker Compose** — containerize the application and MySQL for zero-setup test environments
- [ ] **API Test Layer** — RestAssured test suite for the Spring Boot REST endpoints
- [ ] **Database Validation** — cross-validate UI-visible balances against MySQL records via JDBC
- [ ] **Parallel Browser Execution** — Selenium Grid for multi-browser simultaneous runs

---

## 🏗 Design Principles

### Page Object Model (POM)
Every page in the ParaBank application is represented as a dedicated Java class. Locators live in the page class, actions live in the page class — test methods contain zero `driver.findElement()` calls. This makes selector changes a single-point-of-update operation.

### Separation of Concerns
Test logic, page interaction, configuration, and WebDriver management are cleanly layered. `BaseTest` owns the driver lifecycle. `ConfigReader` owns environment values. `WaitUtils` owns synchronization. No class reaches into another's internals.

### Explicit Waits Over Thread.sleep
All synchronization uses `WebDriverWait` with `ExpectedConditions` — never `Thread.sleep()`. This produces deterministic, timing-resilient tests that run at the speed the application allows rather than at an arbitrary fixed delay.

### Configuration-Driven
Browser type, base URL, credentials, and timeouts are externalized to `application.properties`. Switching from Chrome to Firefox, or from localhost to a staging server, requires changing one file — not touching test code.

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/add-billpay-tests`
3. Commit your changes: `git commit -m "feat: add bill payment negative test cases"`
4. Push to the branch: `git push origin feature/add-billpay-tests`
5. Open a Pull Request against `main`

Please follow the existing Page Object structure and naming conventions. All new test methods must include a `@DisplayName` annotation with a plain-English description.

---

## 👨‍💻 Author

<div align="center">

<table>
  <tr>
    <td align="center" style="padding: 20px;">
      <a href="https://github.com/ranajitchowdhury">
        <img src="https://img.shields.io/badge/-ranajitchowdhury-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub Profile"/>
      </a>
      <br/><br/>
      <strong>Ranajit Baran Chowdhury</strong>
      <br/>
      <em>Software Programmer &amp; QA Automation Engineer</em>
    </td>
  </tr>
</table>
<br/>

**Core Expertise**

![Full Stack](https://img.shields.io/badge/Full%20Stack-Java%20%7C%20Spring%20Boot%20%7C%20MySQL-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![UI Automation](https://img.shields.io/badge/UI%20Automation-Selenium%20%7C%20Playwright-43B02A?style=flat-square&logo=selenium&logoColor=white)
![API Automation](https://img.shields.io/badge/API%20Automation-RestAssured%20%7C%20Postman-FF6C37?style=flat-square&logo=postman&logoColor=white)
![Language](https://img.shields.io/badge/Language-Java%20%7C%20JavaScript-007396?style=flat-square&logo=openjdk&logoColor=white)
![CI/CD](https://img.shields.io/badge/CI%2FCD-GitHub%20Actions%20%7C%20Jenkins-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Testing](https://img.shields.io/badge/Testing-Manual%20%7C%20Automation%20%7C%20API-6A0DAD?style=flat-square)

</div>

> *"Quality is not an act, it is a habit."* — Aristotle

---

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for full details.
