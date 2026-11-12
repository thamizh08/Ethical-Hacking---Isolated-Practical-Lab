# RULES OF ENGAGEMENT (ROE)
## Ethical Hacking – Local Practice Lab

**Name:** Thamizhmaran S  
**Institution:** Chennai Institute of Technology  
**Operating System:** Windows 11  
**Target Application:** OWASP Juice Shop  
**Lab URL:** http://127.0.0.1:3000

### 1. Purpose

This document establishes the rules and boundaries for ethical hacking activities performed in my personally controlled local practice environment.

### 2. Authorized Scope

The following systems are authorized for testing:

- My personal Windows 11 laptop.
- Docker containers created and managed by me.
- OWASP Juice Shop running locally.
- The Docker network named `juice-lab-isolated`.

### 3. Permitted Activities

- Local reconnaissance and service identification.
- Manual web application security testing.
- Testing common OWASP Top 10 vulnerabilities.
- Inspecting HTTP requests and responses.
- Documenting vulnerabilities and possible remediation methods.

### 4. Prohibited Activities

- Testing public websites or external IP addresses.
- Testing college networks or other students' devices.
- Testing EdVyro infrastructure without explicit authorization.
- Denial-of-service attacks.
- Phishing, malware deployment, and credential theft.
- Accessing real users' confidential information.

### 5. Safety Measures

- The Juice Shop container is connected only to the internal Docker network.
- Browser access is provided through an Nginx reverse proxy.
- The application is published on the host loopback address `127.0.0.1`.
- Synthetic test data will be used.
- Testing will stop if the lab boundary is compromised.

### 6. Stop Conditions

Testing will immediately stop if:

- Any system outside the authorized scope is encountered.
- Real personal or confidential information is discovered.
- The host or Docker environment becomes unstable.
- Unauthorized external access is detected.

### 7. Authorization Declaration

I confirm that I own or control the computer and Docker environment used for this exercise. I agree to perform security testing only against the authorized local OWASP Juice Shop target.

**Name:** Thamizhmaran S

**Signature:** __________________________

**Date:** __________________________
