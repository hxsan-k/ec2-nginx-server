## 🧱 Architecture Diagram

```mermaid
graph TD
    A[User's Browser] -->|DNS Lookup| B[Route 53 Hosted Zone]
    B -->|A Record -> EC2 IP| C[EC2 Instance - Ubuntu]
    C -->|HTTP/HTTPS (80/443)| D[NGINX Web Server]
    D -->|Serves| E[Website Content]

    style A fill:#D0E7FF,stroke:#333,stroke-width:1px
    style B fill:#EAD1DC,stroke:#333,stroke-width:1px
    style C fill:#FFE599,stroke:#333,stroke-width:1px
    style D fill:#B6D7A8,stroke:#333,stroke-width:1px
    style E fill:#FFFFFF,stroke:#333,stroke-width:1px
```
