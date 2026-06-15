---
marp: true
title: Alvesting — Pitch
author: Artur Felippe Zanella
paginate: true
size: 16:9
theme: default
style: |
  section {
    font-family: 'Helvetica Neue', Arial, sans-serif;
    background: #0d1b2a;
    color: #e0e1dd;
    padding: 60px 70px;
  }
  h1 { color: #ffffff; font-size: 1.9em; }
  h2 { color: #4cc9f0; font-size: 1.3em; }
  strong { color: #4cc9f0; }
  a { color: #90e0ef; }
  table { font-size: 0.78em; border-collapse: collapse; }
  th { background: #1b263b; color: #ffffff; }
  td, th { border: 1px solid #415a77; padding: 6px 10px; }
  .check { color: #57cc99; font-weight: bold; }
  .cross { color: #e76f51; font-weight: bold; }
  section.lead { text-align: center; }
  section.lead h1 { font-size: 2.6em; }
  footer { color: #778da9; }
  ul { line-height: 1.5; }
---

<!-- _class: lead -->
<!-- _paginate: false -->

# Alvesting

## Competição entre LLMs aplicada ao mercado financeiro brasileiro

**Artur Felippe Zanella**
Engenharia de Software · Católica de Santa Catarina · 2026

---

## O contexto

- Investir no Brasil ainda exige **cruzar manualmente** cotações, indicadores e notícias de várias fontes.
- LLMs (GPT, Claude, Gemini, Llama, DeepSeek, Grok) já são usadas para analisar mercados.
- Mas as arenas existentes focam nos **EUA** e em **criptoativos**.

> O mercado brasileiro (B3) está praticamente **sem cobertura**.

---

## A proposta

Uma **plataforma web** onde várias LLMs **competem investindo na B3**.

- Todos os modelos recebem **os mesmos dados**: cotações, fundamentos, indicadores e notícias.
- Decidem em modo **_paper trading_** — ordens fictícias a **preços reais**.
- Cada ordem vem com a **justificativa em linguagem natural** do modelo.

**Sem risco financeiro. Com realismo de mercado.**

---

## Como funciona

```
 Coleta de dados        Orquestrador          Execução simulada       Painel
 (cotações, notícias) →  de agentes        →  (paper trading,      →  comparativo
  fundamentos, macro)    (mesmo contexto       preços reais)           (retorno,
                          p/ cada LLM)                                  vs Ibovespa)
```

**Módulos:** B3 · Criptoativos · Simulações · Conversa com IA · Portfólio · Notícias

---

## Inovação

- 🇧🇷 **Foco na B3** — domínio descoberto, com notícias em **português**.
- ⚖️ **Arena padronizada** — mesmos dados para todos → a diferença vem do **modelo**.
- 🔍 **Transparência** — cada decisão registrada com sua **justificativa**.
- 🛡️ **Sem risco** — _paper trading_ a preços reais, foco **educacional**.

---

## Posicionamento

| Trabalho | Foco B3 | Múlt. LLMs | Paper trading | Notícias | Acesso |
| --- | :---: | :---: | :---: | :---: | --- |
| Rallies AI Arena | <span class="cross">✗</span> | <span class="check">✓</span> | <span class="check">✓</span> | <span class="check">✓</span> | Público |
| Alpha Arena (Nof1) | <span class="cross">✗</span> | <span class="check">✓</span> | <span class="cross">✗</span> | <span class="cross">✗</span> | Público |
| Chen et al. (2025) | <span class="cross">✗</span> | <span class="check">✓</span> | Simulado | <span class="check">✓</span> | Open-source |
| Xiao et al. (2024) | <span class="cross">✗</span> | <span class="cross">✗</span> | <span class="check">✓</span> | <span class="check">✓</span> | Open-source |
| Teles & Figueiredo | Parcial | <span class="check">✓</span> | <span class="cross">✗</span> | <span class="check">✓</span> | Open-source |
| **Alvesting** | <span class="check">**✓**</span> | <span class="check">**✓**</span> | <span class="check">**✓**</span> | <span class="check">**✓**</span> | **Público** |

Na **interseção** entre arenas públicas e fundamentação acadêmica.

---

## Necessidade de mercado

- Interesse **crescente** no uso de LLMs em finanças.
- **Não existe** vitrine pública adaptada à B3 que integre dados, notícias e análise por IA.
- Aproxima **tecnologia de ponta** do **investidor pessoa física** brasileiro.
- Comportamento das LLMs **visível, auditável e reproduzível**.

---

<!-- _class: lead -->

# Alvesting

**Visível · Auditável · Reproduzível**

Unindo desenvolvimento de software e aplicação prática de IA
no mercado financeiro brasileiro.

🔗 github.com/&lt;seu-usuario&gt;/ainvesting

Obrigado!
