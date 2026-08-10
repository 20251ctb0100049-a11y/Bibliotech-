# Esteira da Análise — BiblioTech

**Estudante:** Rafael Lopes Paz Oliveira Palhano

## Funcionalidade 1: Cadastrar leitor

- **1.2 Fala do cliente:** "Precisamos registrar os novos alunos e professores rapidamente no sistema, senão não temos como controlar quem pegou cada livro."
- **2.3 História de usuário:** Como leitor, quero me cadastrar no sistema da biblioteca para poder realizar empréstimos de livros do acervo.
- **3.4 Requisito:** RF01 — O sistema deve permitir o cadastro de leitores no acervo da biblioteca.
- **4.5 Caso de uso (RF01):** Ator Bibliotecário → "Cadastrar leitor"

## Funcionalidade 2: Emprestar livro

- **1.6 Fala do cliente:** "O aluno escolhe o livro na estante e traz até a mesa para fazermos o registro de retirada com a data de devolução."
- **2.7 História de usuário:** Como leitor, quero pegar um livro emprestado para poder realizar minha leitura em casa dentro do prazo estabelecido.
- **3.8 Requisito:** RF02 — O sistema deve permitir o registro de empréstimo de livros para leitores cadastrados.
- **4.9 Caso de uso (RF02):** Ator Bibliotecário → "Emprestar livro"

---

## Rastreabilidade

| Elipse no diagrama | Veio do requisito | Que veio da fala | Caminho Completo |
|---|---|---|---|
| Cadastrar leitor (RF01) | RF01 | "Precisamos registrar os novos alunos..." | A necessidade de controle gerou o RF01, refinado para a estória do leitor, operado pelo Bibliotecário no caso de uso "Cadastrar leitor". |
| Emprestar livro (RF02) | RF02 | "O aluno escolhe o livro na estante..." | A necessidade da retirada gerou o RF02, originando a história do leitor e o caso de uso operado no balcão pelo Bibliotecário. |

---

## Relacionamento entre casos de uso (nível A)

- **Tipo:** «include»
- **Entre:** "Emprestar livro" e "Validar pendências do leitor"
- **Por que é esse e não o outro:** Foi utilizado o «include» pois a validação de pendências (débitos ou atrasos) é uma etapa obrigatória e executada em 100% das vezes em que o processo de "Emprestar livro" é iniciado.

---

## Autoavaliação

**Conceito pretendido:** A


- **Esteira da análise:** As 2 esteiras estão completas, com falas entre aspas, histórias no padrão, requisitos numerados (RF01, RF02) e atores baseados em quem opera o sistema.
- **Diagrama e notação:** Criado no draw.io com a fronteira retangular "BiblioTech", ator fora da fronteira, linhas de associação sem ponta de seta e relacionamento `«include»` aplicado e justificado corretamente.
- **Rastreabilidade:** Mapeamento explícito desde a fala do cliente, RFs vinculados nas elipses e tabela descritiva do caminho completo.
- **Organização da entrega:** Pasta `Atividade-17` criada com nomes exatos, arquivo editável `.drawio` e `.png` incluídos, e README.md configurado como índice e exibindo o diagrama.

---

## Bilhete de saída

1. **Aprendizado:** Aprendi que a história de usuário foca na necessidade de quem se beneficia, enquanto o caso de uso define quem realmente opera o sistema e como ele interage com a regra do software.
2. **Ponto nebuloso:** A diferenciação prática entre quando usar «include» ou «extend» em fluxos alternativos muito complexos.
3. **Aplicação prática:** Em sistemas de e-commerce, mapeando desde o desejo do cliente de comprar até o caso de uso de processamento de pagamento feito pelo gateway.