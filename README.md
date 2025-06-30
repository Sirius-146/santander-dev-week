# Santander Dev Week

Java RESTful API criada para a Santander Dev Week.

## Diagrama de Classes

```mermaid
classDiagram
    class User {
        +String name
    }

    class Account {
        +String accountNumber
        +String accountAgency
        +Double accountBalance
        +Double accountLimit
    }

    class Feature {
        +String icon
        +String description
    }

    class Card {
        +String number
        +Double limit
    }

    class News {
        +String icon
        +String description
    }

    User --> Account : has a
    User --> Card : has a
    User --> Feature : has many
    User --> News : has many
```
