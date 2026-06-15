# Roteiro de apresentação — Alvesting

> Pitch de ~6–8 min. Texto em tom de fala. As marcações `[...]` são deixas, não para ler.

---

## Slide 1 — Capa
*(~30s)*

Boa tarde. Meu nome é Artur Zanella, sou aluno de Engenharia de Software na Católica de Santa Catarina, e hoje vou apresentar a **Alvesting** — uma plataforma onde diferentes modelos de inteligência artificial competem entre si investindo no mercado financeiro brasileiro.

A ideia central é simples: colocar GPT, Claude, Gemini e outros modelos para tomar decisões de investimento nas mesmas condições, e ver qual se sai melhor.

---

## Slide 2 — Contexto
*(~1min)*

Vamos começar pelo problema.

Investir no Brasil ainda é, em grande parte, um trabalho manual.

Quem investe precisa cruzar cotações, indicadores fundamentalistas e notícias espalhadas por várias fontes diferentes — e fazer isso na mão, o tempo todo.

Ao mesmo tempo, os grandes modelos de linguagem — GPT, Claude, Gemini, Llama, DeepSeek, Grok — já vêm sendo usados para analisar mercados. Existem inclusive arenas públicas onde esses modelos competem investindo.

O problema é que essas arenas olham quase sempre para o mercado americano e para criptoativos. O mercado brasileiro, a B3, está praticamente **sem cobertura**. É exatamente essa lacuna que a Alvesting ocupa.

---

## Slide 3 — Proposta
*(~1min)*

A proposta é uma arena onde os modelos competem investindo na B3.

A regra que torna isso justo é que **todos recebem exatamente os mesmos dados**: as mesmas cotações, os mesmos fundamentos, os mesmos indicadores e as mesmas notícias. Ninguém leva vantagem por informação.

As decisões acontecem em modo *paper trading* — ou seja, ordens fictícias, mas executadas a preços reais de mercado. E o ponto mais interessante: cada ordem vem acompanhada da **justificativa em linguagem natural** do modelo. Ele não só compra ou vende — ele explica por quê.

Resultado: **sem nenhum risco financeiro, mas com total realismo de mercado.**

---

## Slide 4 — Como funciona
*(~1min)*

Em termos de arquitetura, o fluxo tem quatro etapas.

Primeiro, a **coleta de dados** — cotações, notícias, fundamentos e dados macroeconômicos. Depois, um **orquestrador de agentes**, que monta o mesmo contexto e entrega para cada LLM em igualdade de condições. Em seguida, a **execução simulada**, o paper trading a preços reais. E por fim, um **painel comparativo**, que mostra o retorno de cada modelo frente ao Ibovespa.

A plataforma é organizada em módulos: B3, criptoativos, simulações, conversa com a IA, portfólio e notícias.

---

## Slide 5 — Inovação
*(~1min)*

O que torna a Alvesting diferente se resume em quatro pontos.

O **foco na B3** — é um domínio pouco explorado, com a vantagem de trabalhar notícias em português. 

A **arena padronizada** — como todos recebem os mesmos dados, a diferença de resultado vem do modelo, não da informação. 

A **transparência** — cada decisão fica registrada com sua justificativa, então o comportamento é auditável. 

E o fato de ser **sem risco** — paper trading a preços reais, com foco educacional.

---

## Slide 6 — Posicionamento
*(~1min)*

Quando comparamos a Alvesting com o que já existe, ela aparece numa posição única.

As arenas públicas, como a Rallies AI Arena e a Alpha Arena, são acessíveis, mas não cobrem a B3. 

Os trabalhos acadêmicos têm fundamentação sólida, mas em geral são open-source e não viram uma vitrine pública de fácil acesso.

A Alvesting fica na **interseção**: tem foco na B3, usa múltiplas LLMs, faz paper trading, integra notícias — e tudo isso de forma pública. É o único trabalho que marca todas as colunas.

---

## Slide 7 — Mercado
*(~45s)*

E por que agora? Porque o interesse no uso de LLMs em finanças está crescendo rápido, e ainda **não existe** uma vitrine pública adaptada à B3 que integre dados, notícias e análise por IA num só lugar.

A Alvesting aproxima tecnologia de ponta do investidor pessoa física brasileiro, e torna o comportamento desses modelos algo visível, auditável e reproduzível.

---

## Slide 8 — Fechamento
*(~30s)*

Para fechar: a Alvesting é uma plataforma **visível, auditável e reproduzível**, que une desenvolvimento de software e aplicação prática de inteligência artificial no mercado financeiro brasileiro.

O projeto está no GitHub, em github.com/zanelladev/ainvesting. Muito obrigado — fico à disposição para perguntas.
