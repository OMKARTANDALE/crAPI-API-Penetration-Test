# crAPI API Penetration Testing Assessment

## Overview

This repository contains a comprehensive API security assessment conducted against the OWASP crAPI (Completely Ridiculous API) application.

The assessment was performed using manual API testing techniques and Burp Suite to identify vulnerabilities aligned with the OWASP API Security Top 10 (2023).

---

## Assessment Details

| Category            | Details                          |
| ------------------- | -------------------------------- |
| Target Application  | OWASP crAPI                      |
| Assessment Type     | API Penetration Testing          |
| Methodology         | OWASP API Security Top 10 (2023) |
| Testing Approach    | Manual + Burp Suite              |
| Environment         | Training Lab                     |
| Overall Risk Rating | High                             |

---

## Objectives

* Identify authentication and authorization flaws
* Assess API security controls
* Evaluate business logic weaknesses
* Test for injection vulnerabilities
* Assess JWT implementation security
* Validate access control mechanisms
* Analyze API response data exposure

---

## Tools Used

* Burp Suite
* Browser Developer Tools
* JWT.io
* cURL
* Python
* Chrome Browser

---

## Vulnerabilities Identified

| ID   | Vulnerability                                            | Severity | OWASP API Top 10 |
| ---- | -------------------------------------------------------- | -------- | ---------------- |
| API1 | Broken Object Level Authorization (BOLA / IDOR)          | High     | API1:2023        |
| API2 | Broken User Authentication                               | High     | API2:2023        |
| API3 | Excessive Data Exposure                                  | Medium   | API3:2023        |
| API4 | Unrestricted Resource Consumption / Rate Limiting Issues | Medium   | API4:2023        |
| API5 | Broken Function Level Authorization (BFLA)               | High     | API5:2023        |
| API6 | Mass Assignment                                          | High     | API6:2023        |
| API7 | SQL Injection / NoSQL Injection                          | Critical | API8:2023        |
| API8 | Server-Side Request Forgery (SSRF)                       | High     | API7:2023        |
| API9 | JWT Security Weaknesses                                  | High     | API2:2023        |

---

## Testing Methodology

### 1. Reconnaissance

* Application mapping
* Endpoint discovery
* API workflow analysis

### 2. API Enumeration

* Request and response analysis
* Endpoint identification
* Parameter discovery

### 3. Authentication Testing

* Login functionality review
* Password reset testing
* OTP validation testing
* JWT analysis

### 4. Authorization Testing

* Horizontal privilege escalation
* Vertical privilege escalation
* Role-based access control testing

### 5. Business Logic Testing

* Workflow abuse
* OTP bypass scenarios
* Rate limiting assessment

### 6. Injection Testing

* SQL Injection
* NoSQL Injection
* Input validation testing

### 7. SSRF Testing

* URL parameter manipulation
* Internal resource access testing

---

## Repository Structure

```text
crAPI-API-Penetration-Test
│
├── README.md
│
├── REPORT
│   └── crAPI_API_Penetration_Test_Report.pdf
│
├── EVIDENCE
│   ├── IDOR
│   ├── OTP_BYPASS
│   ├── EXCESSIVE_DATA_EXPOSURE
│   ├── RATE_LIMITING
│   ├── BFLA
│   ├── MASS_ASSIGNMENT
│   ├── INJECTION
│   ├── SSRF
│   └── JWT
```

---

## Skills Demonstrated

* API Security Testing
* Burp Suite
* OWASP API Top 10
* Authentication Testing
* Authorization Testing
* JWT Analysis
* SQL Injection Testing
* NoSQL Injection Testing
* SSRF Testing
* Vulnerability Assessment
* Security Reporting
* Manual Penetration Testing

---

## Report

The complete penetration testing report is available in the REPORT directory.

---

## Disclaimer

This project was conducted exclusively within the OWASP crAPI intentionally vulnerable training environment for educational and defensive security research purposes. No unauthorized systems were tested.
