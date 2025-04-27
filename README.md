# CS-305-Software-Security
Jessica Johnson
## Summary
Adding HTTPS encryption, SHA-256 checksums, and static dependency checks were all implemented in Artemis Financial's web application. All of these met the request of making the application safter and more upto date with current software security standards.

## Changes to the Code
- HTTPS enabled using a self-signed SSL
- Checksum using SHA-256 Hash Algorithm
- Scanned dependencies for Vulnerabilities with the OWASP Dependency-Check Maven plugin

## How to Run the Code and Configurations

-  Before running the Java project, make sure you have the proper maven dependnecies installed. Once all are installed, Run the ServerApplication.java. You can then access the API at https://localhost:8443/hash.
*** The browser may give you a security warning. Just accept it and move forward. Its due to the certificate being self-signed ***

-  Use port 8443 for the HTTPS
-  keystore.jks is included (application.properties)

## Testing the Code
-  The /hash returns a correct SHA-256 Checksum
-  Static Scan to identify vulneribilietes using the OWASP
-  HTTPS encryption is working

