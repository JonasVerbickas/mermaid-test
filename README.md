# mermaid-test

Flowchart:
```mermaid
flowchart TD
    A[Start] --> B{Is it raining?}
    B -->|Yes| C[Take umbrella]
    B -->|No| D[Enjoy the sun]
    C --> E[Go outside]
    D --> E
    E --> F[End]
```

Sequence:
```mermaid
sequenceDiagram
    participant User
    participant Frontend
    participant API
    participant Database
    
    User->>Frontend: Submit form
    Frontend->>API: POST /data
    API->>Database: Insert record
    Database-->>API: Confirm success
    API-->>Frontend: Return 201 Created
    Frontend-->>User: Show success message
```

User purchase journey:
```mermaid
journey
    title User Purchase Journey
    section Visit Website
      See product: 5: User
      Browse options: 3: User
      Read reviews: 4: User
    section Purchase
      Add to cart: 5: User
      Enter information: 3: User
      Pay: 5: User
    section After Purchase
      Receive confirmation: 5: User, System
      Track shipping: 4: User, System
      Receive product: 5: User
```

Git graph:
```
gitGraph
    commit
    commit
    branch develop
    checkout develop
    commit
    commit
    checkout main
    merge develop
    commit
    branch feature
    checkout feature
    commit
    commit
    checkout develop
    merge feature
    checkout main
    merge develop
    commit
```
