# Secure Web Application - HTTPS and SHA-256 Implementation
# Author: Jessica Johnson
# Language: Java

## Summary
This project demonstrates several core software security practices implemented in a Java web application. The application was updated to use HTTPS encryption, generate SHA-256 checksums for data integrity, and scan dependencies for known vulnerabilities using the OWASP Dependency-Check Maven plugin.

These improvements help ensure secure communication, verify data integrity, and identify potential security risks within third-party libraries.

## System Architecture

```
Client Browser
      │
      ▼
HTTPS Secure Connection (SSL)
      │
      ▼
Java Web Application
      │
      ├── SHA-256 Hash Generation
      │
      └── OWASP Dependency Vulnerability Scan
```

## Technologies Used
- Java
- HTTPS / SSL
- SHA-256
- Maven
- OWASP Dependency-Check

## Security Improvements Implemented
- Enabled HTTPS communication using a self-signed SSL certificate
- Implemented SHA-256 hashing to generate secure checksums  
- Scanned project dependencies for vulnerabilities using OWASP Dependency-Check Maven plugin

## Running the Application
1. Ensure Maven dependencies are installed
2. Run the ServerApplication.java file
3. Access the application at:

https://localhost:8443/hash

Note: Because a self-signed certificate is used, the browser may display a security warning. Accept the warning to continue.

## Testing the Code
-  The /hash returns a correct SHA-256 Checksum
-  Static Scan to identify vulneribilietes using the OWASP
-  HTTPS encryption is working

## Thank You
This project helped me understand how encryption, hashing, and vulnerability scanning work together to improve application security. It also provided hands-on experience configuring HTTPS and using security tools such as OWASP Dependency-Check.
