# Penetration Test Guide based on the OWASP + Extra
This guide is for the penetration testers seeking for the appropriate test cases required during a penetration test project. I rearranged the [OWASP Testing Guide v4](https://www.owasp.org/index.php/OWASP_Testing_Guide_v4_Table_of_Contents) from my point of view including `9 Test Classes` and each class has several `Test Cases` to conduct against the target. Each `Test Case` covers several OWASP tests which also is useful for the report document. I've also added `15 extra Tests Cases` marked by the `EXTRA-TEST`. I hope it will be useful in both penetration test projects and bug-bounty.

### TODO: 
1. Add resources for each test.

## Information Gathering
*   *    **Fingerprint Technologies**
    *    Fingerprint Web Server (OTG-INFO-002)
    *    Enumerate Applications on Webserver (OTG-INFO-004)
    *    Fingerprint Web Application Framework (OTG-INFO-008)
    *    Fingerprint Web Application (OTG-INFO-009)
*   *    **Information Leakage**
    *    [Conduct Search Engine Discovery and Reconnaissance for Information Leakage (OTG-INFO-001)](https://github.com/Voorivex/pentest-guide/tree/master/Information-Leakage)
    *    [Review Webserver Metafiles for Information Leakage (OTG-INFO-003)](https://github.com/Voorivex/pentest-guide/tree/master/Information-Leakage)
    *    [Review Webpage Comments and Metadata for Information Leakage (OTG-INFO-005)](https://github.com/Voorivex/pentest-guide/tree/master/Information-Leakage)
    *    [Analysis of Error Codes (OTG-ERR-001)](https://github.com/Voorivex/pentest-guide/tree/master/Information-Leakage)
    *    [Analysis of Stack Traces (OTG-ERR-002)](https://github.com/Voorivex/pentest-guide/tree/master/Information-Leakag)
    *    [Conduct a Fuzzing for Hidden and Sensitive Files or Directories (EXTRA-TEST-014)](https://github.com/Voorivex/pentest-guide/tree/master/Information-Leakage)
*   *    **Directory Indexing**
    *    Search for Directory Indexing (EXTRA-TEST-001)
*   *    **Storing Sensitive Information on Client Side**
    *    Test Local Storage (OTG-CLIENT-012)

## Configuration and Deployment Management
*   *    **Enumerate Infrastructure and Application Admin Interfaces**
    *    Enumerate Infrastructure and Application Admin Interfaces (OTG-CONFIG-005)
    *    Test Network/Infrastructure Configuration (OTG-CONFIG-001)
*   *    **Hidden Resources Discovery**
    *    Review Old, Backup and Unreferenced Files for Sensitive Information (OTG-CONFIG-004)
*   *    **HTTP Security Headers**
    *    Testing for Lack of HTTP Security Headers (EXTRA-TEST-002)

## Identity Management and Authentication
*   *    **Secure Authentication Class**
    *    [Test User Registration Process (OTG-IDENT-002)](https://github.com/Voorivex/pentest-guide/tree/master/Insecure-Authentication-Class)
    *    [Testing for Weak Lock Out Mechanism (OTG-AUTHN-003)](https://github.com/Voorivex/pentest-guide/tree/master/Insecure-Authentication-Class)
    *    [Testing for Bypassing Authentication Schema (OTG-AUTHN-004)](https://github.com/Voorivex/pentest-guide/tree/master/Insecure-Authentication-Class)
    *    [Test Remember Password Functionality (OTG-AUTHN-005)](https://github.com/Voorivex/pentest-guide/tree/master/Insecure-Authentication-Class)
    *    [Testing for Browser Cache Weakness (OTG-AUTHN-006)](https://github.com/Voorivex/pentest-guide/tree/master/Insecure-Authentication-Class)
    *    [Testing for Weak Security Question/Answer (OTG-AUTHN-008)](https://github.com/Voorivex/pentest-guide/tree/master/Insecure-Authentication-Class)
    *    [Testing for Weak Password Change or Reset Functionalities (OTG-AUTHN-009)](https://github.com/Voorivex/pentest-guide/tree/master/Insecure-Authentication-Class)
    *    [Testing for Weaker Authentication in Alternative Channel (OTG-AUTHN-010)](https://github.com/Voorivex/pentest-guide/tree/master/Insecure-Authentication-Class)
    *    [Testing for Weak or Unenforced Username Policy (OTG-IDENT-005)](https://github.com/Voorivex/pentest-guide/tree/master/Insecure-Authentication-Class)
    *    [Testing for Default Credentials (OTG-AUTHN-002)](https://github.com/Voorivex/pentest-guide/tree/master/Insecure-Authentication-Class)
    *    [Testing for Two Factor Authentication Bypass (EXTRA-TEST-012)](https://github.com/Voorivex/pentest-guide/tree/master/Insecure-Authentication-Class)
*   *    **Username Enumeration**
    *    Testing for Account Enumeration and Guessable User Account (OTG-IDENT-004)
*   *    **Testing for Recovering Sensitive Information**
    *    Testing for Recovering Sensitive Information from Database (EXTRA-TEST-003)
*   *    **Testing against Brute Force attack**
    *    [Testing against Brute Force attack (EXTRA-TEST-004)](https://github.com/Voorivex/pentest-guide/tree/master/Brute-Force)
*   *    **Password policy**
    *    Testing for Weak password policy (OTG-AUTHN-007)
*   *    **Testing for SSL over User Authentication**
    *    Testing for Credentials Transported over an Encrypted Channel (OTG-AUTHN-001)

## Authorization and Boundary Test
*   *    **User Access Control**
    *    Test Role Definitions (OTG-IDENT-001)
    *    Test Account Provisioning Process (OTG-IDENT-003)
    *    Testing for Bypassing Authorization Schema (OTG-AUTHZ-002)
    *    [Testing for Privilege Escalation (OTG-AUTHZ-003)](https://github.com/Voorivex/pentest-guide/tree/master/Privilege-Escalation)
    *    [Testing for HTTP Verb Tampering (OTG-INPVAL-003)](https://github.com/Voorivex/pentest-guide/tree/master/HTTP_Verb_Tampering)
    *    [Testing for JSON Web Token Flaw (EXTRA-TEST-006)](https://github.com/Voorivex/pentest-guide/tree/master/JSON-Web-Token-Flaw)
    *    [Test Cross Origin Resource Sharing (OTG-CLIENT-007)](https://github.com/Voorivex/pentest-guide/tree/master/Cross-Origin-Resource-Sharing)
*   *    **File Inclusions**
    *    [Testing Directory Traversal/File Include (OTG-AUTHZ-001)](https://github.com/Voorivex/pentest-guide/tree/master/Directory-Traversal-File-Include)
*   *    **Execution after Redirect**
    *    Execution after Redirect (EXTRA-TEST-005)
*   *    **Cross Site Request Forgery**
    *    [Testing for Cross Site Request Forgery (CSRF) (OTG-SESS-005)](https://github.com/Voorivex/pentest-guide/tree/master/Cross-Site-Request-Forgery)
*   *    **Secured File Upload**
    *    [Test Upload of Unexpected File Types (OTG-BUSLOGIC-008)](https://github.com/Voorivex/pentest-guide/tree/master/Secured-File-Upload)
    *    [Test Upload of Malicious Files (OTG-BUSLOGIC-009)](https://github.com/Voorivex/pentest-guide/tree/master/Secured-File-Upload)
*   *    **Insecure Direct Object References**
    *    [Testing for Insecure Direct Object References (OTG-AUTHZ-004)](https://github.com/Voorivex/pentest-guide/tree/master/Insecure-Direct-Object-References)
*   *    **Secured Captcha implementation**
    *    Test for Secured Captcha Workflow (EXTRA-TEST-007)
    
## Cookie and Session Management
*   *    **Testing for Cookies attributes**
    *    [Testing for Cookies attributes (OTG-SESS-002)](https://github.com/Voorivex/pentest-guide/tree/master/Cookies-Attributes)
*   *    **Secure Session Management**
    *    Testing for Bypassing Session Management Schema (OTG-SESS-001)
    *    Testing for Session Fixation (OTG-SESS-003)
    *    Testing for Exposed Session Variables (OTG-SESS-004)
    *    Testing for Logout functionality (OTG-SESS-006)
    *    Test Session Timeout (OTG-SESS-007)
    *    Testing for Session puzzling (OTG-SESS-008)

## Accessibility
*   *    **Denial of Service**
    *    Test for Denial of Service (EXTRA-TEST-008)
    
## Input/Output Validation
*   *    **Cross Site Scripting**
    *    [Testing for Reflected Cross Site Scripting (OTG-INPVAL-001)](https://github.com/Voorivex/pentest-guide/tree/master/Cross-Site-Scripting)
    *    [Testing for Stored Cross Site Scripting (OTG-INPVAL-002)](https://github.com/Voorivex/pentest-guide/tree/master/Cross-Site-Scripting)
    *    [Testing for DOM based Cross Site Scripting (OTG-CLIENT-001)](https://github.com/Voorivex/pentest-guide/tree/master/Cross-Site-Scripting)
    *    [Testing for JavaScript Execution (OTG-CLIENT-002)](https://github.com/Voorivex/pentest-guide/tree/master/Cross-Site-Scripting)
    *    [Testing for HTML Injection (OTG-CLIENT-003)](https://github.com/Voorivex/pentest-guide/tree/master/Cross-Site-Scripting)
    *    [Testing for CSS Injection (OTG-CLIENT-005)](https://github.com/Voorivex/pentest-guide/tree/master/Cross-Site-Scripting)
    *    [Testing for Client Side Resource Manipulation (OTG-CLIENT-006)](https://github.com/Voorivex/pentest-guide/tree/master/Cross-Site-Scripting)
    *    [Testing for Clickjacking (OTG-CLIENT-009)](https://github.com/Voorivex/pentest-guide/tree/master/Cross-Site-Scripting)
*   *    **SQL Injection**
    *    [Testing for SQL Injection (OTG-INPVAL-005)](https://github.com/Voorivex/pentest-guide/tree/master/SQL-Injection)
    *    Testing for Incubated Vulnerabilities (OTG-INPVAL-015)
*   *    **NoSQL Injection**
    *    Testing for XPath Injection (OTG-INPVAL-010)
    *    Testing for XML Injection (OTG-INPVAL-008)
    *    Testing for MongoDB Injection (EXTRA-TEST-011)
*   *    **Server Side Code Injection**
    *    Testing for LDAP Injection (OTG-INPVAL-006)
    *    Testing for ORM Injection (OTG-INPVAL-007)
    *    Testing for SSI Injection (OTG-INPVAL-009)
    *    IMAP/SMTP Injection (OTG-INPVAL-011)
    *    [Testing for Code Injection (OTG-INPVAL-012)](https://github.com/Voorivex/pentest-guide/tree/master/Command-Injection)
    *    [Testing for Server Side Template Injection (EXTRA-TEST-013)](https://github.com/Voorivex/pentest-guide/tree/master/Server-Side-Template-Injection)
*   *    **Remote Command Execution**
    *    [Testing for Command Injection (OTG-INPVAL-013)](https://github.com/Voorivex/pentest-guide/tree/master/Command-Injection)
*   *    **Buffer Overflow**
    *    Testing for Buffer Overflow (OTG-INPVAL-014)
*   *    **XML External Entity (XXE)**
    *    [Testing for XML External Entity (XXE) (EXTRA-TEST-009)](https://github.com/Voorivex/pentest-guide/tree/master/XML-External-Entity)
*   *    **Server Side Request Forgery (SSRF)**
    *    [Testing for Server Side Request Forgery (SSRF) (EXTRA-TEST-010)](https://github.com/Voorivex/pentest-guide/tree/master/Server-Side-Request-Forgery)
*   *    **Open Redirect**
    *    [Testing for Client Side URL Redirect (OTG-CLIENT-004)](https://github.com/Voorivex/pentest-guide/tree/master/Open-Redirect)
*   *    **HTTP Splitting/Smuggling**
    *    [Testing for HTTP Splitting/Smuggling (OTG-INPVAL-016)](https://github.com/Voorivex/pentest-guide/tree/master/HTTP-Smuggling)
*   *    **Race Condition**
    *    [Testing for Race Condition (EXTRA-TEST-15)](https://github.com/Voorivex/pentest-guide/tree/master/Race-Condition)
    
## Testing for weak Cryptography
*   *    **Testing for Weak SSL/TLS Ciphers, Insufficient Transport Layer Protection**
    *    Testing for Weak SSL/TLS Ciphers, Insufficient Transport Layer Protection (OTG-CRYPST-001)
*   *    **Testing for Sensitive Information Sent via Unencrypted Channels**
    *    Testing for Sensitive Information Sent via Unencrypted Channels (OTG-CRYPST-003)
    *    Testing for Padding Oracle (OTG-CRYPST-002)

## Workflow/Dataflow Tests
*   *    **Business Logic Testing**
    *    [Test Business Logic Data Validation (OTG-BUSLOGIC-001)](https://github.com/Voorivex/pentest-guide/tree/master/Business-Logic)
    *    [Test Ability to Forge Requests (OTG-BUSLOGIC-002)](https://github.com/Voorivex/pentest-guide/tree/master/Business-Logic)
    *    [Test Integrity Checks (OTG-BUSLOGIC-003)](https://github.com/Voorivex/pentest-guide/tree/master/Business-Logic)
    *    [Test for Process Timing (OTG-BUSLOGIC-004)](https://github.com/Voorivex/pentest-guide/tree/master/Business-Logic)
    *    [Test Number of Times a Function Can be Used Limits (OTG-BUSLOGIC-005)](https://github.com/Voorivex/pentest-guide/tree/master/Business-Logic)
    *    [Test for the Circumvention of Work Flows (OTG-BUSLOGIC-006)](https://github.com/Voorivex/pentest-guide/tree/master/Business-Logic)
    *    [Test Defenses Against Application Mis-use (OTG-BUSLOGIC-007)](https://github.com/Voorivex/pentest-guide/tree/master/Business-Logic)
