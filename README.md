# Penetration Test & Security Assessment - ENPM685 Pictures, Inc.

This repository contains documentation and findings from a security assessment and penetration test conducted for **ENPM685 Pictures, Inc.** The assessment was performed to evaluate the security posture of the company and provide recommendations for improvement, with a particular focus on the risks posed by their cost-effective IT setup.

## Background

**ENPM685 Pictures, Inc.** is a small movie production studio specializing in low-budget “mockbusters,” which are spoofs of high-budget movies. The company has operated with a very lean IT structure and hiring model, consisting only of its CEO, **Bob Dobbs**, and numerous contractors. However, due to recent data leaks and a planned expansion involving new hires, the company is looking to upgrade its IT infrastructure and secure its operations.

The CEO has engaged our security firm to conduct a penetration test on their environment, which currently consists of a single server that functions as:
- The primary file server
- Web hosting for the company’s website
- General resource storage and access point for the company

This penetration test will help highlight vulnerabilities and offer solutions for improving the company's IT security.

## Objective

The goal of this penetration test and security assessment is to:
- Identify and exploit security weaknesses within ENPM685 Pictures, Inc.’s IT environment.
- Demonstrate the current risks and potential impacts to the company’s operations.
- Provide actionable recommendations to improve the security posture of ENPM685 Pictures, Inc.

## Methodology

The assessment follows a structured penetration testing methodology:
1. **Reconnaissance**: Gather information on the company's IT environment, including open ports, services, and possible attack vectors.
2. **Scanning**: Use tools like `Nmap` and vulnerability scanners to map out the server’s weaknesses.
3. **Exploitation**: Attempt to exploit identified vulnerabilities, demonstrating the risk to sensitive data and systems.
4. **Post-exploitation**: Assess the extent of access and data exposure upon gaining initial access, simulating the actions of an attacker.
5. **Reporting**: Document findings with detailed explanations of the vulnerabilities and provide recommendations.

## Key Findings

The following are highlights of some key vulnerabilities found in the assessment:
- **Weak Password Policies**: Password cracking using shadow and passwd files revealed easily guessable passwords.
- **Unrestricted File Uploads**: Exploitable file upload functionality, allowing potential remote code execution.
- **SQL Injection Vulnerabilities**: Exposed sensitive data in backend databases.
- **Insecure File Permissions**: Critical files were accessible without proper permissions.
- **Improper Network Configuration**: Weak firewall rules allowing unnecessary open ports.

## Recommendations

1. **Implement Strong Password Policies**: Enforce complexity requirements and set expiration policies for all user accounts.
2. **Secure File Upload Mechanisms**: Restrict file types, scan uploaded files for malware, and enforce strict access permissions.
3. **Harden Network Security**: Limit open ports to only those necessary for business operations and ensure firewall rules restrict unnecessary traffic.
4. **Database Security Enhancements**: Sanitize inputs to prevent SQL injection attacks, and employ least privilege principles for database access.
5. **Implement Multi-Factor Authentication (MFA)**: Add an extra layer of security for accessing sensitive resources.

## Conclusion

The assessment shows that ENPM685 Pictures, Inc.’s current IT setup has significant vulnerabilities that could be exploited by attackers. By following the recommendations above, the company can greatly reduce the risk of data breaches and strengthen its overall security posture.

For full details, refer to the detailed documentation in this repository.
