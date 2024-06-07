```mermaid
graph TD
    A[Start] --> B[Sign Up]
    B --> C[Greetings]
    C --> D[Choose Plan]
    D --> E[Payment Method]
    E -->|Decline| J[Customer Service]
    E -->|Approve| F[User Agreement]
    F -->|Decline| J
    F -->|Approve| G[Profile Setup]
    G -->|Decline| H[Feedback]
    H --> K[Pending]
    G -->|Approve| I[Account Created]
    I --> L[Share Profile]
    L -->|Decline| J
    L -->|Approve| K
```
