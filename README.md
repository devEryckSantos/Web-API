# Decola Tech Avanade 2025
Java RESTful API criada para o Decola Tech 2025

## Diagrama de Classes

```mermaid
classDiagram
    class User {
        +string name
        +Account account
        +Feature[] features
        +Card card
        +News[] news
    }

    class Account {
        +string number
        +string agency
        +string balance
        +string limit
    }

    class Feature {
        +string icon
        +string description
    }

    class Card {
        +string number
        +float limit
    }

    class News {
        +string icon
        +string description
    }

    User "1" *-- "1" Account
    User "1" *-- "n" Feature
    User "1" *-- "1" Card
    User "1" *-- "n" News
```
