# Atividade 17 — Da esteira ao diagrama (BiblioTech)

- **Aluno(a):** Rafael Lopes Paz Oliveira
- **Turma:** 2º ano — Técnico em Informática Integrado
- **Disciplina:** Análise e Projeto de Sistemas — Profe. Berssa

## O que tem nesta pasta

| Arquivo | O que é |
|---|---|
| [esteira-da-analise.md](esteira-da-analise.md) | As esteiras e a autoavaliação |
| [diagrama-casos-de-uso.png](diagrama-casos-de-uso.png) | O diagrama (imagem) |
| [diagrama-casos-de-uso.drawio](diagrama-casos-de-uso.drawio) | O diagrama (arquivo editável) |

## Diagrama

![Diagrama de Casos de Uso do BiblioTech](diagrama-casos-de-uso.png)

## Decisão de Modelagem

A decisão mais difícil foi definir o tipo de relacionamento entre "Emprestar livro" e "Buscar livro no acervo". Optou-se pelo uso de `«extend»` em relação à consulta de pendências do leitor porque ela é uma validação condicional necessária apenas sob regras específicas do sistema antes do empréstimo, mantendo o caso de uso principal coeso e focado na operação principal de balcão.

## Conceito pretendido

**Conceito:** A

A justificativa está no fim do arquivo `esteira-da-analise.md`.