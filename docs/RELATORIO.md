# Relatório técnico - entrega interna (rascunho)

Aluno: Guilherme Tonielo
Turma: 3C
Repositório público próprio: https://github.com/Icemangy/TrabalhoFinal-Back-End

## Objetivo e tecnologias
Banco RPG demonstra cadastro, consulta, atualização e exclusão de jogadores, além de compras, inventário, apostas com moedas fictícias e ranking. A interface React envia JSON por fetch à API Flask; SQLite persiste os dados. O projeto deriva da base creditada no README.

## Conferência das etapas
1. SQL e estrutura backend/bd presentes. DER acrescentado em docs/DER.md. Rota GET / acrescentada. Identificação e endereço do repositório preenchidos. Faltam capturas da API, terminal e banco no relatório final.
2. CRUD completo de jogadores existente e verificado. Coleção Postman preparada. Arquivos .db excluídos desta cópia e ignorados pelo Git. Faltam execução da coleção no Postman e prints reais de POST, GET, PUT e DELETE.
3. Interface integrada com fetch e persistência SQLite implementadas. A versão de origem compilou anteriormente; esta cópia ainda precisa da conferência visual final e de capturas de gravação/listagem na interface.
4. Para não participantes: README documenta endpoints, verbos e JSON. Banner não é exigido para esta modalidade. Relatório final em PDF e repositório público identificado está preparado; faltam evidências visuais e confirmação da publicação.
5. Para não participantes: apresentação de cinco minutos para turma e professora, projeção da tela, sistema funcionando e explicação do Python no VS Code. Roteiro em docs/PITCH.md. O vídeo já gravado só substitui essa apresentação se a professora aceitar.

## Validação executada
11 verificações da API passaram em banco temporário independente: status, criação, listagem, edição, compra e atualização de saldo/XP, inventário, saldo insuficiente, aposta, exclusão, registro inexistente e nome obrigatório. Respostas reais em RESULTADOS_TESTES.json. Essas verificações não são prints do Postman.

## Limitações e melhorias
Renda passiva, senha, uso e revenda de itens não constam como exigências nos PDFs. Não foram acrescentados. O sistema permanece uma demonstração local sem autenticação. A auditoria anterior de dependências sinalizou vulnerabilidade alta, ainda não investigada nesta cópia. Não há justificativa para declarar a entrega integralmente concluída antes das evidências e publicação.

## Observações da avaliação
A etapa 2 informa valor de 2 pontos; as demais informam 1 cada, totalizando 6, embora haja referência a parcial de 5. Confirmar a pontuação com a professora. Os prazos dos documentos são anteriores a 29/10/2026; eventual prazo de reposição não foi informado. O exemplo de gestão escolar é modelo didático: a etapa 2 permite banco temático e pede CRUD de ao menos uma entidade principal.
