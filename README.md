# APITest

Automated API testing suite using **Java + RestAssured + JUnit 5**.  
This project demonstrates testing for REST endpoints of [JSONPlaceholder](https://jsonplaceholder.typicode.com).

---

## Table of Contents
- [Project Overview](#project-overview)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Running Tests](#running-tests)
- [Test Scenarios](#test-scenarios)
- [Contributing](#contributing)
- [Author](#author)
- [License](#license)

---

## Project Overview
This project contains automated tests for REST APIs, including GET, POST, PUT, PATCH, and DELETE requests. Tests are structured with **JUnit 5** and **RestAssured**, organized in order to ensure proper execution flow.

---

## Prerequisites
- **Java JDK 17+**  
- **Maven**  
- IDE (e.g., IntelliJ IDEA)  

---

## Getting Started
1. Clone the repository:  
   ```bash
   git clone https://github.com/BrutaruMihaiGeorgian/APITest.git
   ```
2. Navigate to the project directory:
   ```bash
   cd APITest
   ```
3. Install dependencies:
   ```bash
   mvn clean install
   ```

---

## Project Structure
```
APITest/
├── src/
│   └── test/
│       └── java/
│           └── ApiTests.java       ← Contains all API test cases
├── pom.xml                           ← Maven configuration
└── README.md
```

---

## Running Tests
Run all tests via Maven:
```bash
mvn test
```
Or run directly from IDE using JUnit 5 runner.

---

## Test Scenarios
1. **GET /posts** → Validate all posts returned (positive)  
2. **GET /posts/1** → Validate single post by ID (positive)  
3. **GET /posts/1/comments** → Validate comments for a post (positive)  
4. **GET /comments?postId=1** → Validate query parameter filtering (positive)  
5. **POST /posts** → Create a new post (positive)  
6. **PUT /posts/1** → Update existing post (positive)  
7. **PATCH /posts/1** → Partially update post (positive)  
8. **DELETE /posts/1** → Delete post (positive)  
9. **GET /postssss** → Invalid endpoint test (negative)  

---

## Contributing
Contributions are welcome! To contribute:
1. Fork the repository  
2. Create a branch: `git checkout -b feature/new-feature`  
3. Commit changes with clear messages  
4. Push the branch and create a Pull Request  

---

## Author
**Mihai Brutaru**

---

## License
*(Add license, e.g., MIT, if applicable)*
