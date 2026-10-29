# Apresentação interna - 5 minutos

0:00–1:00 — Problema e solução. Explique que o Banco RPG é uma simulação acadêmica para praticar gerenciamento de dados e progressão de jogadores. Apresente os créditos da base e suas adequações.

1:00–3:00 — Demonstração. Cadastre um jogador; mostre 1.000 moedas. Compre Espada Comum: saldo 800 e 20 XP. Abra inventário. Edite o nome no painel. Recarregue a tela para demonstrar persistência. Mostre uma aposta de 100 e explique os dois resultados possíveis, sem prometer vitória. Mostre ranking.

3:00–4:00 — Código no VS Code. Abra backend/app.py e explique request.get_json, validação, INSERT com parâmetros, commit e jsonify. Mostre as rotas GET/POST/PUT/DELETE de jogadores. Abra bd/script.sql e o DER: jogador possui vários itens e apostas. Explique que fetch liga React à API.

4:00–5:00 — Conclusão. Mostre README e os testes. Explique limitações: moedas fictícias, sem senha e sem renda passiva. Encerre destacando o fluxo interface → API → SQLite → resposta JSON → atualização da tela.

## Perguntas para praticar
Onde ficam os dados? No arquivo SQLite criado automaticamente na pasta bd.
Como evita SQL Injection? Valores são passados separadamente com placeholders ?, sem concatenar a entrada na consulta.
O que faz commit? Confirma a transação; rollback desfaz em caso de falha.
Qual entidade tem CRUD completo? Jogadores.
O que acontece sem a API? As requisições falham e a interface mostra erro; a mensagem técnica de rede pode ser melhorada.
Por que CORS? Permite à interface local acessar a API em outra porta; não substitui autenticação.
