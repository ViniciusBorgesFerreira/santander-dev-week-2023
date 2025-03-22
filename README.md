# Santander Dev Week 2023

## Diagrama de Classes:

```mermaid
classDiagram
    class User {
        +string name
    }
    
    class Account {
        +string accountNumber
        +string accountAgency
        +float accountBalance
        +float accountLimit
    }

    class Features {
        +string icon
        +string description
    }

    class Card {
        +string cardNumber
        +float cardLimit
    }

    class News {
        +string newsIcon
        +string newsDescription
    }

    User "1" *-- "1"Account
    User "1" *-- "N" Features
    User "1" *-- "1" Card
    User "1" *-- "N" News
```
