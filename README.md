# BankingAutomation-ParaBank

## Project Overview
This project is a simulation of a banking system where users can perform various banking operations seamlessly. The system aims to provide a user-friendly experience along with a robust backend architecture.

## Tech Stack
- **Frontend:** HTML, CSS, JavaScript
- **Backend:** Java, Spring Boot
- **Database:** MySQL
- **Testing:** JUnit, Selenium

## Installation Instructions
1. Clone the repository: `git clone https://github.com/rbchy/BankingAutomation-ParaBank.git`
2. Navigate to the project directory: `cd BankingAutomation-ParaBank`
3. Install dependencies:
   - For the frontend: Navigate to the frontend directory and run `npm install`
   - For the backend: Use Maven to install dependencies by running `mvn install`

## Test Scenarios
- **User Login:** Verify if the user can log in with valid credentials.
- **Account Creation:** Validate that new users can create accounts successfully.
- **Transactions:** Ensure that users can perform fund transfers and check balances correctly.

## Running Tests
Run the tests using the following command:
```bash
mvn test
```

## Reporting
Test reports can be found in the target/surefire-reports directory after running the tests.

## Configuration
Configuration settings can be modified in the `application.properties` file located in the backend directory.

## Contributing Guidelines
1. Fork the repository.
2. Create a new branch: `git checkout -b feature/YourFeature`
3. Make your changes and commit: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature/YourFeature`
5. Create a new pull request.

Feel free to reach out for any clarifications regarding contributions!