# Diagrama entidade-relacionamento
```mermaid
erDiagram
    jogadores ||--o{ itens : possui
    jogadores ||--o{ apostas : realiza
    jogadores {
        INTEGER id PK
        TEXT nome
        INTEGER saldo
        INTEGER xp
        INTEGER nivel
    }
    itens {
        INTEGER id PK
        INTEGER jogador_id FK
        TEXT nome
        TEXT raridade
        INTEGER preco
    }
    apostas {
        INTEGER id PK
        INTEGER jogador_id FK
        INTEGER valor
        TEXT resultado
        INTEGER premio
        TEXT data
    }
```
Cada jogador pode possuir zero ou vários itens e realizar zero ou várias apostas. Cada item e aposta pertence a exatamente um jogador. A exclusão do jogador remove os registros relacionados por ON DELETE CASCADE. O catálogo da loja é definido no Python; a tabela itens registra as compras individuais.
