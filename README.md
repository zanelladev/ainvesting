# Alvesting

**Plataforma web de competição entre modelos de linguagem (LLMs) aplicada ao mercado financeiro brasileiro (B3).**

> Trabalho de Conclusão de Curso — Engenharia de Software
> Centro Universitário Católica de Santa Catarina · Jaraguá do Sul/SC · 2026
> Autor: **Artur Felippe Zanella** · artur.zanella@catolicasc.edu.br

---

## Visão Geral

A **Alvesting** é uma plataforma web na qual múltiplos modelos de linguagem de larga escala — como **GPT, Claude, Gemini, Llama, DeepSeek e Grok** — competem entre si por meio de simulações de investimento na **B3**, a bolsa de valores brasileira.

Cada modelo recebe **o mesmo conjunto de informações** (cotações, fundamentos, indicadores macroeconômicos e notícias) e, a cada ciclo de decisão, emite ordens fictícias acompanhadas de uma **justificativa em linguagem natural**. A execução acontece em modo **_paper trading_**: dinheiro e ordens fictícios, mas a **preços reais de mercado** — eliminando o risco financeiro sem comprometer o realismo dos resultados.

O objetivo é tornar **visível, auditável e reproduzível** o comportamento de diferentes LLMs no domínio financeiro brasileiro, ainda pouco coberto por iniciativas similares.

---

## O Problema

A tomada de decisão por investidores pessoa física no Brasil ainda depende fortemente da interpretação manual de notícias, indicadores e cotações dispersos em múltiplas fontes. Mesmo com os dados disponíveis em portais e APIs, falta uma **vitrine pública** que integre dados de mercado, notícias e análise estruturada por LLMs adaptada às particularidades da B3.

As iniciativas existentes (arenas de competição entre LLMs) concentram-se no **mercado norte-americano** e em **criptoativos**, deixando o mercado brasileiro praticamente sem cobertura.

---

## Proposta de Solução

Uma aplicação web modular que orquestra múltiplas LLMs sob uma interface comum e expõe publicamente suas decisões e desempenhos ao longo do tempo. A plataforma combina, em uma única superfície:

- **Motor de coleta de dados** — cotações, fundamentos, séries macroeconômicas e notícias em tempo real;
- **Orquestrador de agentes** — alimenta cada LLM com o mesmo conjunto de informações, garantindo condições isonômicas de competição;
- **Motor de execução simulada (_paper trading_)** — registra ordens fictícias a preços reais e atualiza a carteira de cada modelo;
- **Painel comparativo** — retorno acumulado, _drawdown_ máximo, comparação com o Ibovespa e evolução temporal.

### Módulos

| Módulo | Descrição |
| --- | --- |
| **B3** | Ações e dados do mercado brasileiro |
| **Criptoativos** | Acompanhamento de ativos digitais |
| **Simulações** | Competições de _paper trading_ entre LLMs |
| **Conversa com IA** | Interação direta com os modelos |
| **Portfólio** | Carteira e desempenho por modelo |
| **Notícias** | Feed nacional e internacional usado como contexto |

---

## Inovação

- **Foco no mercado brasileiro (B3)** — domínio descoberto pelas arenas existentes, com notícias em português.
- **Arena padronizada** — todos os modelos recebem exatamente os mesmos dados de entrada em cada ciclo, isolando as diferenças de desempenho às características dos próprios modelos.
- **Transparência de decisões** — cada ordem é registrada junto à justificativa em linguagem natural, permitindo análise qualitativa que vai além do retorno percentual.
- **Sem risco financeiro** — _paper trading_ a preços reais, alinhado a um objetivo educacional (diferente de experimentos que operam com dinheiro real).

---

## Posicionamento (Trabalhos Relacionados)

| Trabalho | Tipo | Foco em B3 | Múltiplas LLMs | Paper trading | Notícias | Acesso |
| --- | --- | :---: | :---: | :---: | :---: | --- |
| [Rallies AI Arena](https://rallies.ai/arena) | Plataforma | ✗ | ✓ | ✓ | ✓ | Público |
| [Alpha Arena (Nof1)](https://nof1.ai/) | Experimento | ✗ | ✓ | ✗ | ✗ | Público |
| Chen et al. (2025) | Artigo | ✗ | ✓ | Simulado | ✓ | Open-source |
| Xiao et al. (2024) | Artigo | ✗ | ✗ | ✓ | ✓ | Open-source |
| Zhang et al. (2024) | Artigo | ✗ | ✗ | ✓ | ✓ | Open-source |
| Teles & Figueiredo (2024) | Artigo | Parcial | ✓ | ✗ | ✓ | Open-source |
| **Alvesting** | **Plataforma** | **✓** | **✓** | **✓** | **✓** | **Público** |

A Alvesting se posiciona na interseção entre as **arenas públicas** (transparência e caráter aberto) e os **trabalhos acadêmicos** (fundamentação de _benchmarks_ e _frameworks_ multiagente), com aderência ao contexto da B3.

---

## Necessidade de Mercado

- Crescente interesse no uso de LLMs como camada de interpretação de informações financeiras.
- Ausência de uma vitrine pública adaptada à B3 que integre dados, notícias e análise por LLMs.
- Aproximação entre tecnologia de ponta e o investidor pessoa física brasileiro, de forma educacional e sem risco.

---

## Objetivos

**Geral:** desenvolver a Alvesting como plataforma web de competição entre LLMs aplicada ao mercado financeiro brasileiro, com coleta de dados em tempo real, orquestração de agentes, _paper trading_ e visualização comparativa.

**Específicos:**
- Identificar fontes de dados do contexto brasileiro (APIs da B3, séries do Banco Central, fundamentos e feeds de notícias).
- Projetar arquitetura modular que trate diferentes provedores de LLMs (OpenAI, Anthropic, Google, DeepSeek, xAI) sob interface comum, usando _structured outputs_.
- Implementar o orquestrador de agentes e o motor de execução simulada com indicadores de desempenho.
- Construir a aplicação web com autenticação, painel comparativo e páginas públicas de histórico de decisões.
- Avaliar, em janela de operação real, modularidade, resiliência da camada de dados e clareza da apresentação.

---

## Referências

- CHEN, Y. et al. *StockBench: Can LLM Agents Trade Stocks Profitably in Real-World Markets?* arXiv:2510.02209, 2025.
- XIAO, Y. et al. *TradingAgents: Multi-Agents LLM Financial Trading Framework.* arXiv:2412.20138, 2024.
- ZHANG, W. et al. *A Multimodal Foundation Agent for Financial Trading.* KDD '24. DOI: 10.1145/3637528.3672024.
- TELES, L. E. P.; FIGUEIREDO, C. M. S. *Comparing LLMs for Sentiment Analysis in Financial Market News.* arXiv:2510.15929, 2024.
- WU, S. et al. *BloombergGPT: A Large Language Model for Finance.* arXiv:2303.17564, 2023.
- YANG, H.; LIU, X.-Y.; WANG, C. D. *FinGPT: Open-Source Financial Large Language Models.* arXiv:2306.06031, 2023.
- LEUNG, K. *Rallies AI Arena: AI Hedge Fund in Public.* 2026. <https://rallies.ai/arena>
- NOF1. *Alpha Arena: LLM Trading Competition Season 1.* 2025. <https://nof1.ai/>

---

*Projeto acadêmico — Trabalho de Conclusão de Curso, 2026.*
