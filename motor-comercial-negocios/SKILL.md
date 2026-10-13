---
name: motor-comercial-negocios
description: "Projetar, diagnosticar ou operar o motor comercial de qualquer negócio: oferta e preço, qualificação de leads (MEDDPICC, gap selling), calls de descoberta (SPIN), objeções e negócios parados (JOLT), negociação e descontos, comitês de compra e multithreading, prospecção outbound e entregabilidade de e-mail, narrativa de pitch, vendas lideradas pelo fundador, PLG e leads qualificados por produto, B2B enterprise, SaaS, churn e retenção, métricas CAC/LTV/payback, garantias, escassez, indicações, cases e conteúdo. Gatilhos: vendas, preço, oferta, negócio travado, 'vou pensar', negociação, cold email, cold call, call de descoberta, comitê de compra, churn, pipeline, proposta, business case."
metadata:
  version: "2.0.0"
  last_reviewed: "2026-10-13"
  review_cadence: "A cada 6 meses: rever trends.md, os benchmarks de metrics.md e reading-list.md com fontes novas."
  license: "CC BY 4.0"
---

# Motor Comercial de Negócios (v2)

Este arquivo é um **orquestrador**, não uma enciclopédia. Ele decide qual módulo carregar para a situação. A teoria fica em `references/`, os artefatos preenchíveis em `templates/`, os roteiros em `objections/`, os critérios go/no-go em `checklists/` e os contrastes práticos em `examples/`. Carregue só o que a situação pede.

Responda no idioma do usuário. Seja direto. Toda recomendação termina em um artefato, um roteiro ou um número, nunca em um slogan.

## Passo 0 — Escolha o modo

| Modo | Quando | Entregável |
|---|---|---|
| **Revisão rápida** | O usuário traz uma coisa só (um e-mail, um preço, uma proposta, uma objeção) | Veredito + versão corrigida + um motivo por mudança |
| **Diagnóstico de gargalo** | "Preciso de mais clientes / receita / margem" sem causa clara | Diagnóstico nos 5 pontos de checagem abaixo + o próximo experimento (use `templates/experiment-card.md`) |
| **Construção completa** | Oferta nova, segmento novo, motor novo, ou fundador começando a vender | O subconjunto relevante do mapa de 12 passos, cada passo fechado com seu template |

Nunca assuma a construção completa por padrão. Pergunte o modo se não estiver claro; se o usuário não estiver presente, escolha o menor modo que responde ao pedido e diga qual escolheu.

## Passo 1 — Árvore de decisão: o que carregar

| Situação | Carregar |
|---|---|
| "Preciso de mais clientes" / gargalo incerto | **Sequência de diagnóstico** abaixo, depois `references/metrics.md` |
| Oferta vaga, preço chutado, tiers bagunçados | `references/offer-pricing.md` + `templates/pricing-tier-worksheet.md` |
| Montar pipeline / prospectar / outreach frio | `references/outbound.md` + `templates/5-touch-sequence.md` + `templates/cold-call-scripts.md` + `examples/cold-email-good-vs-bad.md` |
| Primeira call com um prospect | `references/discovery.md` + `templates/discovery-call-guide.md` + `examples/discovery-call-transcript.md` |
| Qualificar um negócio enterprise / grande | `references/qualification.md` + `templates/meddpicc-scorecard.md` |
| Negócio parado, "vou pensar", sem próximo passo | `references/jolt.md` + `objections/library.md` |
| Qualquer objeção, resistência de preço | `references/objections.md` + `objections/library.md`; para preço, também `references/negotiation.md` |
| Pedido de desconto, compras, termos de contrato | `references/negotiation.md` + `templates/business-case-onepager.md` |
| Só um contato na conta | `references/multithreading.md` + `templates/buying-committee-map.md` |
| Pitch, demo, deck, hero do site | `references/narrative.md` + `templates/pitch-narrative.md` |
| Fundador vendendo pela primeira vez, contratar o primeiro vendedor | `references/founder-sales.md` |
| Produto self-serve com sinais de uso | `references/plg-pql.md` |
| Garantia, política de reembolso, urgência, escassez | `references/guarantees-scarcity.md` |
| Churn, onboarding, escopo que cresce, indicações, cases | `references/delivery-retention.md` |
| Site, conteúdo, o que publicar | `references/content.md` |
| Usar IA em prospecção, análise de calls, timing | `references/ai-in-sales.md` |
| Mecânica de persuasão, frases exatas | `references/psychology.md` |
| Antes de um forecast ou revisão de pipeline | `checklists/deal-review.md` |
| Depois de qualquer call de vendas | `checklists/post-call-rubric.md` |
| "Isto ainda está atual?" | `trends.md` |
| "O que ler para aprofundar?" | `reading-list.md` |

## Passo 2 — Sequência de diagnóstico (antes de concluir qualquer coisa)

"Preciso de mais marketing" é uma hipótese, não um diagnóstico. Verifique nesta ordem e pare no primeiro elo quebrado:

1. **Alcance** — As pessoas certas, em número suficiente, estão vendo a oferta? (impressões, tamanho da lista, reuniões marcadas)
2. **Qualidade dos leads** — Dos que respondem, quantos se encaixam no perfil ideal? (qualificados / total)
3. **Conversão** — Dos leads qualificados, quantos compram e em que etapa caem? (etapa por etapa, veja os critérios de etapa em `references/qualification.md`)
4. **Capacidade** — O negócio consegue entregar mais sem que a qualidade desabe? (utilização, backlog)
5. **Retenção e expansão** — Os clientes ficam e compram mais? (churn, NRR, indicações)

Consertar o alcance quando a conversão está quebrada compra mais derrotas. Consertar a conversão quando a capacidade está cheia compra clientes irritados. Números de cada ponto: `references/metrics.md`.

## Passo 3 — Princípios centrais (revisados na v2)

1. **Um negócio é arbitragem com margem de segurança.** A receita por cliente precisa superar o custo de adquiri-lo e atendê-lo, com folga para erro. Meça: CAC, payback, margem de contribuição, retenção por coorte.
2. **Ordem de trabalho: Oferta → Preço → Vendas → Demanda**, mas diagnostique primeiro (Passo 2). Mais demanda sobre uma oferta fraca expõe a fraqueza mais rápido.
3. **Confiança é o ativo.** O comprador carrega risco de dinheiro, tempo e reputação. Todo artefato deve reduzir esse risco com evidência, não com adjetivos.
4. **O posicionamento segue demanda, custo e capacidade**, não um slogan. Premium, médio e volume funcionam quando a economia unitária fecha. A "zona da morte" é qualquer posição em que preço, custo de atender e expectativa do comprador não combinam.
5. **Venda resultados que o comprador definiu**, não funcionalidades que você construiu. Descubra o que ele valoriza antes de assumir que velocidade, preço ou comodidade é a alavanca.
6. **Oferta e demanda definem o teto do preço; o custo define o piso; as alternativas definem a referência.** Quando a demanda excede a capacidade, suba o preço ou corte vagas; quando não excede, conserte a oferta antes de cortar preço.
7. **"Não decidir" é o principal concorrente.** A indecisão perde mais negócios qualificados do que os rivais; trate-a como uma objeção com playbook próprio (`references/jolt.md`).
8. **O mercado expõe a vagueza.** Oferta vaga aparece como leads desqualificados; preço ilógico aparece na negociação; cliente errado aparece na entrega; conteúdo vazio aparece como silêncio.

## Passo 4 — O mapa de 12 passos (o que uma construção completa cobre)

| # | Passo | Módulo | Fecha com |
|---|---|---|---|
| 0 | Levantamento de contexto | abaixo | Levantamento preenchido |
| 1 | Cliente ideal, dor, pesquisa | `references/discovery.md` (seção Mom Test) | Notas de pesquisa com clientes |
| 2 | Oferta | `references/offer-pricing.md` | Declaração da oferta |
| 3 | Economia e preço | `references/offer-pricing.md`, `references/metrics.md` | `templates/pricing-tier-worksheet.md` |
| 4 | Qualificação e descoberta | `references/qualification.md`, `references/discovery.md` | `templates/meddpicc-scorecard.md`, `templates/discovery-call-guide.md` |
| 5 | Narrativa e prova | `references/narrative.md`, `references/delivery-retention.md` | `templates/pitch-narrative.md` |
| 6 | Redução de risco, escassez | `references/guarantees-scarcity.md` | Garantia com conta de exposição |
| 7 | Pipeline e outbound | `references/outbound.md` | `templates/5-touch-sequence.md` |
| 8 | Objeções, indecisão, negociação | `references/objections.md`, `references/jolt.md`, `references/negotiation.md` | `templates/business-case-onepager.md` |
| 9 | Comitê de compra | `references/multithreading.md` | `templates/buying-committee-map.md` |
| 10 | Contrato e transição | `references/delivery-retention.md` (seção de contrato) | Checklist de contrato, documento de transição |
| 11 | Entrega, retenção, indicações, cases | `references/delivery-retention.md` | Plano 30/60/90, momento da indicação, consentimento do case |
| 12 | Conteúdo e alavancagem de IA | `references/content.md`, `references/ai-in-sales.md` | Plano de conteúdo, fluxo de IA |

Transversais: `references/metrics.md` (meça cada passo), `references/psychology.md` (formulação), `templates/experiment-card.md` (mude uma coisa de cada vez).

## Levantamento de contexto (pergunte só o que falta)

1. O que se vende, para quem, quem assina, quem usa.
2. Mercado e país (normas contratuais, hábitos de compras).
3. Preço hoje, custo real de entrega, horas por cliente.
4. Capacidade: clientes por semana/mês, cadência de início.
5. De onde vêm os clientes hoje; conversão por etapa, se conhecida.
6. Prova disponível: resultados com números, depoimentos, cases, certificações.
7. Tamanho do negócio e duração do ciclo (decide se MEDDPICC e multithreading se aplicam).
8. Meta e restrição: mais clientes, mais margem, menos esforço, receita recorrente, decisões mais rápidas.

## Regras invioláveis

1. Toda call termina com próximo passo agendado, ou o negócio é marcado como em risco.
2. Nenhum preço sai sem dor quantificada ou business case (`templates/business-case-onepager.md`).
3. Desconto se troca, nunca se dá: "Faço X se você fizer Y."
4. Negócios enterprise nunca têm um único contato.
5. Trate o "não decidir" antes de tratar a concorrência.
6. Escassez e prazos são reais ou não existem. Urgência inventada é um saque de confiança que você não consegue repor.
7. Prova é documentada e autorizada. Simulações são rotuladas como simulações.
8. Uma variável por experimento, com regra de parada.

## Critérios de etapa do funil (critérios objetivos para avançar)

| Etapa | Critério de saída |
|---|---|
| Lead | Encaixa no perfil em 2 de 3: segmento, cargo, sinal de gatilho |
| Qualificado | Dor dita nas palavras dele + impacto quantificado + um processo de decisão nomeado |
| Descoberta concluída | Scorecard MEDDPICC sem vermelho em Dor, Champion e Processo de Decisão |
| Proposta | Business case aceito pelo champion; comprador econômico identificado e alcançado |
| Negociação | Critérios escritos atendidos; processo burocrático (jurídico, segurança, compras) mapeado com datas |
| Fechado | Assinado + kickoff agendado + documento de transição enviado |

## Contratos de saída

**Revisão rápida:** 1) veredito em uma linha; 2) o artefato corrigido; 3) registro de mudanças, um motivo por mudança; 4) uma coisa para testar em seguida.

**Diagnóstico de gargalo:** 1) os cinco pontos com o número ou "desconhecido" em cada um; 2) o elo quebrado; 3) um cartão de experimento; 4) o que medir em 30 dias.

**Construção completa:** os passos aplicáveis do mapa de 12 passos, cada um fechado com seu template, e depois um plano de 30 dias com responsáveis e métricas. Nunca encha com passos que não se aplicam.

## O que esta skill se recusa a fazer

- Usar BANT como portão (orçamento e prazo ficam só como sinais).
- Escrever aberturas do tipo "espero que esteja bem" ou "gostaria de apresentar nossa empresa".
- Apresentar funcionalidades e benefícios como estrutura de pitch.
- Recomendar volume de e-mail sem configuração de entregabilidade.
- Empilhar garantias por padrão ou prometer resultados fora do controle do vendedor.
- Citar percentuais sem fonte e população ("97% não estão prontos para comprar" foi aposentado).
- Dar frases motivacionais no lugar de uma ação.

## Manutenção

Veja `CHANGELOG.md`. Tendências e benchmarks envelhecem mais rápido: reverifique `trends.md` e as heurísticas de `references/metrics.md` a cada data de revisão. Fontes por seção: `reading-list.md`.
