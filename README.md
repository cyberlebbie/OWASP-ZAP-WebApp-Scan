# Web Application Vulnerability Assessment Using OWASP ZAP

## Overview
This repository documents a hands-on web application security assessment conducted using OWASP ZAP. The project focuses on identifying common web application vulnerabilities, analyzing their impact, and proposing appropriate remediation strategies in an ethical and authorized testing environment.

---

## Objectives
- Perform a full web application vulnerability scan using OWASP ZAP  
- Identify and analyze common web security vulnerabilities  
- Document findings with screenshots and reports  
- Propose remediation strategies aligned with security best practices  
- Reflect on lessons learned and challenges encountered  

---

## Tools & Technologies
- OWASP ZAP  
- Kali Linux / Windows  
- Firefox / Chrome (configured with ZAP proxy)  
- Intentionally vulnerable web application (DVWA / OWASP Juice Shop)  

---

## Ethical Considerations
All scans were performed on authorized and intentionally vulnerable applications for educational purposes only.  
No unauthorized systems were targeted during this assessment.

---

## Methodology
1. Configured browser proxy to route traffic through OWASP ZAP  
2. Crawled the target application using the Traditional Spider  
3. Conducted passive scanning during normal browsing  
4. Executed active scans to identify exploitable vulnerabilities  
5. Generated reports and documented findings with remediation notes  


---

## Key Vulnerabilities Identified

| Vulnerability | Risk Level | Description |
|---------------|------------|-------------|
| Cross-Site Scripting (XSS) | High | Unsanitized user input reflected in responses |
| Missing Security Headers | Medium | CSP and clickjacking protections not implemented |
| SQL Injection (Potential) | High | Input fields not properly validated |
| Cookie Without HttpOnly Flag | Low | Cookies accessible via client-side scripts |

---

## Remediation Summary
- Implement proper input validation and output encoding  
- Use prepared statements and parameterized queries  
- Apply essential HTTP security headers  
- Configure cookies with secure attributes  
- Follow secure coding best practices  

Detailed remediation steps are available in the `remediation` directory.

---

## Evidence
Screenshots of the OWASP ZAP dashboard, spidering process, active scans, and identified vulnerabilities are included in the `screenshots` directory.

---

## Key Lessons Learned
- Automated security tools require manual analysis to validate findings  
- Many critical vulnerabilities result from simple misconfigurations  
- Proper scan scope management reduces false positives  
- Secure development practices significantly lower security risks  


---

## Author
Mohamed Lebbie  
Cybersecurity Analyst | Ethical Hacking Enthusiast  

---

## Conclusion
This project enhanced practical skills in web application security testing, vulnerability assessment, and professional cybersecurity documentation, emphasizing the importance of proactive security assessments in modern web environments.
