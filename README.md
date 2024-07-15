 Bootcamp Desenvolvimento Java IA
Java RESTful api criado para Desenvolvimento Java IA

## Diagrama de Classe


```mermaid
classDiagram
    class User {
        +String name
        +Account accunt
        +Card card
        +Feature[] feature
        +News[] news
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

    User "1" *-- "1" Account
    User "1" *-- "1" Card
    User "1" *--  "N" Feature
    User "1" *-- "N" News
```
