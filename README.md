# Santander Dev Week 2023
Java RESTFul API criada para o Santander Dev Week.

## Diagrama de Classes 

```mermaid
classDiagram
    class User {
        +String name
    }

    class Account {
        +String number
        +String agency
        +float balance
        +float limit
    }

    class Feature {
        +String icon
        +String description
    }

    class Card {
        +String number
        +float limit
    }

    class News {
        +String icon
        +String description
    }

    User "1" *-- "1" Account : has
    User "1" *-- "N" Feature : has_many
    User "1" *-- "1" Card : has
    User "1" *-- "N" News : has_many
```
