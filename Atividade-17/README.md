# Esteira da Análise — BiblioTech

**Estudante:** Ellis Moura

## Funcionalidade 1: Emprestar livro

- **1. Fala do cliente:** "O aluno chega aqui no balcão com o livro e a gente precisa registrar no sistema que ele levou, pra ter o controle de quem está com o quê."
- **2. História de usuário:** Como leitor, quero retirar um livro emprestado no balcão, para ter acesso ao material de estudo durante o período letivo.
- **3. Requisito:** RF01 — O sistema deve permitir o registro do empréstimo de um livro para um leitor.
- **4. Caso de uso (RF01):** Ator Bibliotecário → "Emprestar livro" (verbo + objeto)

## Funcionalidade 2: Buscar livro no acervo

- **1. Fala do cliente:** "Os alunos vivem perguntando se o livro X ou Y está disponível na biblioteca, então seria ótimo se eles pudessem pesquisar isso direto do celular."
- **2. História de usuário:** Como leitor, quero buscar livros no acervo por título ou autor, para verificar se estão disponíveis sem ter que ir até a biblioteca.
- **3. Requisito:** RF02 — O sistema deve permitir a busca de livros no acervo.
- **4. Caso de uso (RF02):** Ator Leitor → "Buscar livro no acervo" (verbo + objeto)

## Rastreabilidade

| Elipse no diagrama | Veio do requisito | Que veio da fala |
|---|---|---|
| Emprestar livro | RF01 | "O aluno chega aqui no balcão... a gente precisa registrar no sistema que ele levou" |
| Buscar livro no acervo | RF02 | "Os alunos vivem perguntando se o livro X ou Y está disponível... pudessem pesquisar isso direto" |

## Relacionamento entre casos de uso (nível A)

- **Tipo:** «include»
- **Entre:** "Emprestar livro" e "Autenticar no Sistema"
- **Por que é esse e não o outro:** Trata-se de um «include» porque o passo de autenticar o usuário/bibliotecário é obrigatoriamente executado para validar as permissões antes de efetivar o registro do empréstimo no sistema.

## Autoavaliação

**Conceito pretendido:** A

- **Conversei sobre esta atividade com:** Ninguém
- **Esteira da análise:** Cumprida na íntegra no arquivo `esteira-da-analise.md`, contendo 2 esteiras completas com as 4 estações na ordem exata e falas do cliente entre aspas.
- **Diagrama e notação:** Construído no Draw.io com fronteira "BiblioTech", atores externos, linhas de associação sem ponta de seta e inclusão do relacionamento «include».
- **Rastreabilidade:** Mapeada na tabela de rastreabilidade, mantendo a consistência exata dos nomes e dos códigos RF01 e RF02.
- **Organização da entrega:** Pasta `Atividade-17` organizada com os 4 arquivos com nomes exatos e inclusão da justificativa das decisões no README.md.
