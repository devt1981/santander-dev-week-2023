# Santander Dev Week 2023


## Diagrama de Classes (Domínio da API)

```mermaid
classDiagram
  class usuario {
    -String nome
    -Account conta
    -Feature[] features
    -Card cartao
    -News[] news
  }

  class Account {
    -String numero
    -String agencia
    -Number balanco
    -Number limite
  }

  class Feature {
    -String icon
    -String description
  }

  class Card {
    -String numero
    -Number limite
  }

  class News {
    -String icon
    -String descricao
  }

  User "1" *-- "1" Conta
  User "1" *-- "N" Feature
  User "1" *-- "1" Cartao
  User "1" *-- "N" News
```


