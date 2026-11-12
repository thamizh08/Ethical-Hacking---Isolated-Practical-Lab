
## Isolated Practice Lab and Rules of Engagement

**Prepared by:** Thamizhmaran S  
**Operating System:** Windows 11  
**Virtualization Platform:** Docker Desktop  
**Practice Application:** OWASP Juice Shop

### 1. Objective

The objective of this task is to establish a controlled and safe environment for practicing ethical hacking and web application security testing.

### 2. Tools and Technologies

- Windows 11
- Docker Desktop
- OWASP Juice Shop
- Nginx Reverse Proxy
- Docker Bridge Networks
- Google Chrome

### 3. Lab Architecture

The lab consists of two Docker containers:

1. **OWASP Juice Shop:** The vulnerable web application used as the authorized testing target.
2. **Nginx Reverse Proxy:** Provides browser access to Juice Shop through localhost.

The Juice Shop container is connected only to the Docker internal network named `juice-lab-isolated`.

The Nginx proxy is connected to both `juice-lab-isolated` and `juice-proxy-net`.

The application is accessed through:

`http://127.0.0.1:3000`

Refer to `lab-topology.png` for the network architecture.

### 4. Network Isolation

The Juice Shop container is not directly connected to the proxy's second network.

An external connectivity test using Node.js returned:

`OUTBOUND BLOCKED: EAI_AGAIN`

This indicates that DNS resolution for the external test hostname failed.

### 5. Security Rules

- Testing is restricted to the locally hosted OWASP Juice Shop application.
- No unauthorized public or third-party systems will be tested.
- Denial-of-service attacks and destructive testing are prohibited.
- Only synthetic test data will be used.
- Testing will stop immediately if the scope or network boundary is compromised.

### 6. Evidence

The `Evidence` directory contains screenshots documenting:

- Application accessibility.
- Running Docker containers.
- Juice Shop network configuration.
- Nginx proxy network configuration.
- External DNS connectivity test.

### 7. Conclusion

A local OWASP Juice Shop practice environment was established using Docker and Nginx. The target application is accessible through localhost while remaining attached only to its designated internal Docker network.

The environment provides a controlled foundation for authorized web security learning and testing.

**Prepared by:** Thamizhmaran S
