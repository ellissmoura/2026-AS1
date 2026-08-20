# Atividade 18 — Diagrama de Classes do BiblioTech

- **Nome:** SEU NOME COMPLETO
- **Turma:** 2º ano — Técnico em Informática Integrado

## Diagrama
![Diagrama de Classes do BiblioTech](diagrama-classes.png)

## Multiplicidade (Bibliotecario — Emprestimo)
- **`0..*` perto de Emprestimo:** Um bibliotecário pode registrar nenhum ou vários empréstimos no seu turno.
- **`1` perto de Bibliotecario:** Cada empréstimo é registrado por exatamente um bibliotecário.

## Rastreabilidade (Nível B)
- A operação `registrarEmprestimo()` em `Bibliotecario` atende ao caso de uso **Emprestar livro** (RF01).
- A operação `pesquisarLivro()` em `Leitor` atende ao caso de uso **Buscar livro no acervo** (RF02).

## Enxugamento e Nova Classe (Nível A)
- **Nova Classe:** Adicionada a classe `Reserva` associada a `Leitor` (1 para 0..*) e `Livro` (1 para 0..*).
- **Limpeza:** Removido o atributo `nomeLeitor` de `Emprestimo` para evitar redundância, mantendo apenas a associação de classes.

## Defesa Técnica (Nível A)
- **Objeção:** *Bibliotecario deveria ser apenas um atributo String em Emprestimo?*
- **Resposta:** **Não.** O Bibliotecário é uma entidade com ações e regras próprias (login, gestão do acervo). Usar apenas `String` viola a Orientação a Objetos e impede o controle de acesso e permissões.

## Autoavaliação
- **Conceito pretendido:** A
- **Justificativa:** Cumpri a ligação do Bibliotecario, adicionei a classe Reserva, enxuguei o modelo, mapeei a rastreabilidade com a Atividade 17 e respondi à objeção técnica.
