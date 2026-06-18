# 🛡️ API Security Risk Analysis – Task 3

## 📌 Overview
This project is part of a Cyber Security Internship program.  
The objective is to analyze a public API and identify potential security risks related to authentication, data exposure, and access control.

---

## 🌐 API Tested
https://jsonplaceholder.typicode.com/posts

- Method: GET  
- Type: Public REST API  
- Purpose: Testing and learning environment  

---

## 🧰 Tools Used
- Web Browser (Chrome / Edge)
- Developer Tools (Inspection of JSON response)
- Manual security analysis

---

## 🔍 Security Analysis

### 🔹 Authentication
- No authentication mechanism is implemented.
- The API is publicly accessible without API keys or tokens.

### 🔹 Data Exposure
- The API returns structured JSON data including:
  - userId
  - id
  - title
  - body
- All data is publicly visible without restriction.

### 🔹 Access Control & Rate Limiting
- No access control mechanisms observed.
- No rate limiting or request throttling detected.

---

## ⚠️ Identified Security Risks

- **Unauthorized Access Risk:** Anyone can access the API without verification.
- **Data Exposure Risk:** All returned data is openly accessible.
- **Denial of Service Risk:** Lack of rate limiting may allow abuse through excessive requests.

---

## 💡 Recommendations

- Implement authentication (API keys, JWT, OAuth2)
- Apply role-based access control (RBAC)
- Add rate limiting and request throttling
- Validate and monitor API requests
- Restrict sensitive data exposure

---

## 📌 Conclusion
The API is suitable for testing and educational purposes but lacks essential security controls required for production environments. Proper security mechanisms are necessary to ensure safe deployment in real-world applications.

---

## 📁 Project Structure
