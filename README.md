# Publicando minha API REST na Nuvem Usando Spring Boot 3, Java 17 e Railway


# Diagrama de Classes em Mermaid
``` mermaid
classDiagram
    class User {
        name: string
        account: Account
        features: Feature[]
        card: Card
        news: News
    }

    class Account {
        number: string
        agency: string
        balance: float
        limit: float
    }

    class Feature {
        icon: string
        description: string
    }

    class Card {
        number: string
        limit: float
    }

    class News {
        icon: string
        description: string
    }

    User "1" -- "1" Account
    User "1" -- "*" Feature
    User "1" -- "1" Card
    User "1" -- "1" News

```
