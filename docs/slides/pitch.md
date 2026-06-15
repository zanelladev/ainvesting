---
marp: true
title: Alvesting — Pitch
author: Artur Felippe Zanella
paginate: true
size: 16:9
theme: default
style: |
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500&family=Figtree:wght@300;400&family=JetBrains+Mono&display=swap');

  :root {
    --canvas: #fdfcfc;
    --sand: #f5f3f1;
    --border: #e5e5e5;
    --ink: #000000;
    --driftwood: #777169;
    --fog: #a59f97;
    --violet: #0447ff;
    --orange: #ff4704;
  }

  section {
    font-family: 'Inter', 'Helvetica Neue', Arial, sans-serif;
    background: var(--canvas);
    color: var(--ink);
    padding: 64px 80px;
    font-size: 22px;
    letter-spacing: 0.01em;
    line-height: 1.5;
  }

  h1 {
    font-family: 'Figtree', 'Inter', sans-serif;
    font-weight: 300;
    color: var(--ink);
    font-size: 2.1em;
    letter-spacing: -0.02em;
    line-height: 1.1;
    margin-bottom: 0.4em;
  }

  h2 {
    font-family: 'Figtree', 'Inter', sans-serif;
    font-weight: 300;
    color: var(--ink);
    font-size: 1.35em;
    letter-spacing: -0.02em;
    line-height: 1.15;
  }

  h3 {
    font-family: 'Inter', sans-serif;
    font-weight: 500;
    color: var(--driftwood);
    font-size: 0.7em;
    letter-spacing: 0.08em;
    text-transform: uppercase;
  }

  p, li { color: var(--driftwood); }
  strong { color: var(--ink); font-weight: 500; }
  a { color: var(--ink); text-decoration: none; border-bottom: 1px solid var(--border); }

  blockquote {
    border: none;
    background: var(--sand);
    border-radius: 20px;
    padding: 24px 32px;
    color: var(--ink);
    font-weight: 400;
    margin: 24px 0;
  }
  blockquote::before { content: none; }

  ul { line-height: 1.6; }
  li::marker { color: var(--fog); }

  table { font-size: 0.72em; border-collapse: collapse; width: 100%; }
  th {
    background: var(--ink);
    color: var(--canvas);
    font-weight: 500;
    padding: 8px 12px;
    border: 1px solid var(--border);
  }
  td {
    background: var(--sand);
    color: var(--driftwood);
    border: 1px solid var(--border);
    padding: 8px 12px;
  }

  code {
    font-family: 'JetBrains Mono', monospace;
    background: var(--sand);
    color: var(--ink);
    border-radius: 4px;
    padding: 1px 6px;
    font-size: 0.85em;
  }
  pre {
    background: var(--sand);
    border: 1px solid var(--border);
    border-radius: 20px;
    padding: 24px;
  }
  pre code { background: transparent; color: var(--driftwood); }

  .check { color: var(--ink); font-weight: 600; }
  .cross { color: var(--fog); }

  .pill {
    display: inline-block;
    background: var(--ink);
    color: var(--canvas);
    border-radius: 9999px;
    padding: 6px 18px;
    font-size: 0.85em;
    font-weight: 500;
  }
  .pill-outline {
    display: inline-block;
    background: var(--canvas);
    color: var(--ink);
    border: 1px solid var(--border);
    border-radius: 9999px;
    padding: 6px 18px;
    font-size: 0.85em;
    font-weight: 500;
  }

  section.lead { text-align: center; justify-content: center; }
  section.lead h1 { font-size: 3.2em; margin-bottom: 0.2em; }

  footer { color: var(--fog); font-size: 0.55em; }
  section::after { color: var(--fog); font-weight: 400; }
---

<!-- _class: lead -->
<!-- _paginate: false -->

# Alvesting

## Competição entre LLMs aplicada ao mercado financeiro brasileiro

<br>

**Artur Felippe Zanella**
Engenharia de Software · Católica de Santa Catarina · 2026

---

### Contexto

# Investir no Brasil ainda é trabalho manual

- Cruzar **cotações, indicadores e notícias** de várias fontes, à mão.
- LLMs (GPT, Claude, Gemini, Llama, DeepSeek, Grok) já analisam mercados.
- Mas as arenas existentes focam nos **EUA** e em **criptoativos**.

> O mercado brasileiro (B3) está praticamente **sem cobertura**.

---

### Proposta

# Uma arena onde modelos competem investindo na B3

- Todos recebem **os mesmos dados**: cotações, fundamentos, indicadores e notícias.
- Decidem em modo **_paper trading_** — ordens fictícias a **preços reais**.
- Cada ordem vem com a **justificativa em linguagem natural** do modelo.

> **Sem risco financeiro. Com realismo de mercado.**

---

### Arquitetura

# Como funciona

```
 Coleta de dados        Orquestrador          Execução simulada       Painel
 (cotações, notícias) →  de agentes        →  (paper trading,      →  comparativo
  fundamentos, macro)    (mesmo contexto       preços reais)           (retorno
                          p/ cada LLM)                                  vs Ibovespa)
```

<br>

**Módulos** &nbsp; <span class="pill-outline">B3</span> <span class="pill-outline">Criptoativos</span> <span class="pill-outline">Simulações</span> <span class="pill-outline">Conversa com IA</span> <span class="pill-outline">Portfólio</span> <span class="pill-outline">Notícias</span>

---

### Inovação

# O que torna a Alvesting diferente

- 🇧🇷 &nbsp; **Foco na B3** — domínio descoberto, com notícias em **português**.
- ⚖️ &nbsp; **Arena padronizada** — mesmos dados para todos → a diferença vem do **modelo**.
- 🔍 &nbsp; **Transparência** — cada decisão registrada com sua **justificativa**.
- 🛡️ &nbsp; **Sem risco** — _paper trading_ a preços reais, foco **educacional**.

---

### Posicionamento

# Na interseção entre arenas públicas e academia

| Trabalho | Foco B3 | Múlt. LLMs | Paper trading | Notícias | Acesso |
| --- | :---: | :---: | :---: | :---: | --- |
| Rallies AI Arena | <span class="cross">✗</span> | <span class="check">✓</span> | <span class="check">✓</span> | <span class="check">✓</span> | Público |
| Alpha Arena (Nof1) | <span class="cross">✗</span> | <span class="check">✓</span> | <span class="cross">✗</span> | <span class="cross">✗</span> | Público |
| Chen et al. (2025) | <span class="cross">✗</span> | <span class="check">✓</span> | Simulado | <span class="check">✓</span> | Open-source |
| Xiao et al. (2024) | <span class="cross">✗</span> | <span class="cross">✗</span> | <span class="check">✓</span> | <span class="check">✓</span> | Open-source |
| Teles & Figueiredo | Parcial | <span class="check">✓</span> | <span class="cross">✗</span> | <span class="check">✓</span> | Open-source |
| **Alvesting** | <span class="check">✓</span> | <span class="check">✓</span> | <span class="check">✓</span> | <span class="check">✓</span> | **Público** |

---

### Mercado

# Por que agora

- Interesse **crescente** no uso de LLMs em finanças.
- **Não existe** vitrine pública adaptada à B3 que integre dados, notícias e IA.
- Aproxima **tecnologia de ponta** do **investidor pessoa física** brasileiro.
- Comportamento das LLMs **visível, auditável e reproduzível**.

---

<!-- _class: lead -->

# Alvesting

## Visível · Auditável · Reproduzível

<br>

Unindo desenvolvimento de software e aplicação prática de IA
no mercado financeiro brasileiro.

<br>

<span class="pill">github.com/zanelladev/ainvesting</span>
