# 2026-AS1
# Aula 16 - Modelagem do Sistema BiblioTech

Diagrama Bibliotech: [Acessar Diagrama no Google Drive](https://drive.google.com/file/d/1NMkiQzhSFbN8MgcLZzvAo725oHCOyGtO/view?usp=sharing)

# Aula 17 - Seu BiblioTech Conectado

Diagrama da aula 17: [Acessar Diagrama no Google Drive](https://drive.google.com/file/d/1_dq5NpcJPebZcBn49VEU9OfgQGJOkvja/view?usp=sharing)

Defesa das Escolhas de Modelagem

`<<include>>` em Autenticar no Sistema: Decidi colocar a autenticação como inclusão obrigatória antes de ações como *Reservar* ou *Emprestar Livro*. Como essas operações alteram o status do acervo e geram responsabilidade sobre o exemplar, o sistema precisa confirmar quem está executando a ação antes de prosseguir.

`<<extend>>` em Pagar Multa: O pagamento de multa estende o processo de *Devolver Livro* de forma opcional. Nem toda devolução gera cobrança; o fluxo de pagamento só é ativado se o sistema identificar um atraso no prazo de entrega.

Generalização dos Atores: Criei um ator genérico *Usuário* que se conecta diretamente a *Consultar Acervo*. Como tanto o *Aluno* quanto o *Bibliotecário* realizam buscas, fazer ambos herdarem as permissões de *Usuário* evita ter que puxar várias linhas repetidas e deixa o diagrama mais limpo.