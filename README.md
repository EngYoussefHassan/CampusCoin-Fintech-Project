# CampusCoin – FinTech Project

🏆 Winner – FinYology FinTech Competition (University Level)  
🚀 Final Stage Project – FinTech Got Talent (National FinTech Competition)

---

## Overview

CampusCoin is a digital wallet platform designed to enable secure, cashless transactions within a university environment. The system models a multi-role, transaction-heavy application that requires strict validation of financial operations, authentication flows, and data integrity.

The platform involves three main actors:

- **Students (Users)** – manage balances, send money, and perform purchases  
- **Vendors** – accept payments and manage products  
- **Admins** – monitor system activity and analytics  

CampusCoin represents a real-world fintech system where end-to-end workflows, API reliability, and business logic accuracy are critical.

---

## Testing Scope

Testing CampusCoin focuses on ensuring:

- Accuracy of financial transactions  
- Security of authentication and authorization  
- Data consistency across multiple operations  
- Reliability of OTP-based purchase flows  
- System behavior under edge cases and invalid inputs  

---

## Key Test Areas

### 1. Authentication & Authorization

Testing ensures that only valid users and vendors can access the system.

**Test Scenarios:**
- User registration with valid/invalid data  
- Email verification flow (valid/expired tokens)  
- Login with correct and incorrect credentials  
- JWT validation and session handling  
- Role-based access (User / Vendor / Admin)  

---

### 2. Wallet & Balance Management

The wallet is a critical component requiring strict validation.

**Test Scenarios:**
- Balance updates after deposits  
- Balance deduction after purchases  
- Preventing negative balances  
- Concurrent transaction handling  
- Data consistency after multiple operations  

---

### 3. Peer-to-Peer Transfers

This feature involves updating two accounts in a single operation.

**Test Scenarios:**
- Successful transfer between users  
- Transfer with insufficient balance  
- Invalid recipient handling  
- Atomicity (both balances update correctly or fail together)  
- Transaction record validation  

---

### 4. Vendor & Product Management

Vendors interact with product listings and purchases.

**Test Scenarios:**
- Vendor registration and login  
- Product creation, update, and deletion  
- Product visibility in public listings  
- Invalid product data handling  

---

### 5. OTP-Based Purchase Flow

This is one of the most critical and complex features.

**Test Scenarios:**
- OTP generation and delivery  
- Purchase flow with valid OTP  
- Purchase failure with incorrect OTP  
- OTP expiration handling  
- Automatic refund after expiration  
- Preventing OTP reuse  

---

### 6. Spending Limits & Validation

The system enforces financial constraints.

**Test Scenarios:**
- Purchase within limit  
- Purchase exceeding category limit  
- Monthly limit reset behavior  
- Edge cases around limit boundaries  

---

### 7. Admin Dashboard

Admins monitor system-wide data and analytics.

**Test Scenarios:**
- Access control for admin-only endpoints  
- Accuracy of aggregated statistics  
- Filtering and search functionality  
- Data consistency in reports  

---

### 8. API Testing

The system exposes a RESTful API, making API testing essential.

**Test Focus:**
- Request/response validation  
- Status code verification  
- Authentication headers handling  
- Input validation (valid/invalid payloads)  
- Error handling and edge cases  

**Tools:**
- Postman  
- REST Assured (Java)  
- Automated API testing frameworks  

---

## Test Types Applied

- **Manual Testing**
  - Functional testing of all user flows  
  - Exploratory testing for edge cases  

- **Automation Testing**
  - UI automation (Selenium)  
  - API automation  

- **Integration Testing**
  - Validation of interactions between components  

- **System Testing**
  - End-to-end scenarios across all roles  

- **Regression Testing**
  - Ensuring new changes do not break existing functionality  

---

## Critical Test Scenarios (High Priority)

- Financial transaction integrity  
- OTP purchase validation and expiration  
- Authentication security (JWT handling)  
- Data consistency across multi-step operations  
- Error handling under invalid inputs  

---

## Risk Areas

- Incorrect balance calculations  
- Failed or partial transactions  
- OTP misuse or bypass  
- Unauthorized access to protected endpoints  
- Data inconsistency between system components  

---

## Conclusion

CampusCoin represents a real-world fintech system where accuracy, security, and reliability are critical.

Testing this system requires strong focus on:

- Business logic validation  
- Edge case handling  
- API correctness  
- Transaction safety  
