
# DIVA Mobile Application Penetration Testing Report

## Overview
This repository contains the penetration testing report for the **Damn Insecure and Vulnerable App (DIVA)** mobile application, conducted from November 18th to November 24th, 2024. The testing aimed to uncover vulnerabilities within the app and provide recommendations to strengthen its security posture.

## Report Contents
The testing adhered to the **OWASP Mobile Application Security Testing Guide (MASTG)** and focused on identifying vulnerabilities in:
- Insecure data storage
- Authentication mechanisms
- Input validation
- Hardcoding of sensitive information

### Testing Methodology
The following steps were performed:
1. Reconnaissance and information gathering
2. Static and dynamic analysis
3. Backend/API testing
4. Device-level security assessment
5. Reverse engineering and tampering analysis

## Identified Vulnerabilities
### Critical Vulnerabilities
1. **SQL Injection**
   - Vulnerability: Inadequate input validation in SQL queries.
   - Impact: Unauthorized database access, data manipulation, and credential theft.

### High-Severity Vulnerabilities
1. **Hardcoded Sensitive Information**
   - Vulnerability: Hardcoded credentials, API keys, or encryption keys in the application code.
   - Impact: Data exposure and unauthorized access.

2. **Sensitive Data Stored in Shared Preferences**
   - Vulnerability: Insecure storage of sensitive user data.
   - Impact: Data breaches and privacy violations.

3. **Sensitive Data Stored in Local Storage**
   - Vulnerability: Exposed sensitive information due to improper storage mechanisms.
   - Impact: Increased risk of unauthorized data access.

### Medium-Severity Vulnerabilities
1. **Insecure Logging**
   - Vulnerability: Logging of sensitive data (e.g., credit card numbers).
   - Impact: Information leakage and privilege escalation.

2. **Sensitive Data Stored in Temporary Files**
   - Vulnerability: Storing sensitive credentials in temporary files.
   - Impact: Unauthorized access to sensitive data.

3. **URL Injection**
   - Vulnerability: Insufficient validation of URL parameters.
   - Impact: Unauthorized access to application resources and sensitive data.

## Tools Used
- **Genymotion Simulator**: Emulating mobile environments.
- **ADB Shell**: Device interaction and command execution.
- **JADX CLI**: Decompiling APK files for static code analysis.

## Recommendations
The report provides comprehensive recommendations for mitigating each vulnerability, including:
- Avoiding hardcoded sensitive data.
- Implementing secure data storage practices.
- Using parameterized queries to prevent SQL injection.
- Encrypting sensitive data and enhancing input validation.

## How to Use This Repository
1. Review the [Full Report](./diva_pentestingreport.pdf) for detailed findings, proof of concept, and mitigation strategies.
2. Use the recommendations to secure similar mobile applications.
3. Conduct regular security assessments to address potential vulnerabilities.

## Author
**Amjad Ameen P P**  
Cybersecurity Analyst  
[LinkedIn](#) | [GitHub](#)
