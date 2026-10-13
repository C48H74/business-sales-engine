---
name: motor-comercial-negocios-es
description: "Diseñar, diagnosticar u operar el motor comercial de cualquier negocio: oferta y precio, calificación de leads (MEDDPICC, gap selling), llamadas de descubrimiento (SPIN), objeciones y negocios parados (JOLT), negociación y descuentos, comités de compra y multithreading, prospección outbound y entregabilidad de email, narrativa de pitch, ventas lideradas por el fundador, PLG y leads calificados por producto, B2B enterprise, SaaS, churn y retención, métricas CAC/LTV/payback, garantías, escasez, referidos, casos de éxito y contenido. Disparadores: ventas, precio, oferta, negocio atascado, 'lo voy a pensar', negociación, cold email, cold call, llamada de descubrimiento, comité de compra, churn, pipeline, propuesta, business case."
metadata:
  version: "2.0.0"
  last_reviewed: "2026-10-13"
  review_cadence: "Cada 6 meses: revisar trends.md, los benchmarks de metrics.md y reading-list.md con fuentes nuevas."
  license: "CC BY 4.0"
---

# Motor Comercial de Negocios (v2)

Este archivo es un **orquestador**, no una enciclopedia. Decide qué módulo cargar según la situación. La teoría vive en `references/`, los artefactos rellenables en `templates/`, los guiones en `objections/`, los criterios go/no-go en `checklists/` y los contrastes prácticos en `examples/`. Carga solo lo que la situación necesita.

Responde en el idioma del usuario. Sé directo. Toda recomendación termina en un artefacto, un guion o un número, nunca en un eslogan.

## Paso 0 — Elige el modo

| Modo | Cuándo | Entregable |
|---|---|---|
| **Revisión rápida** | El usuario trae una sola cosa (un email, un precio, una propuesta, una objeción) | Veredicto + versión corregida + un motivo por cambio |
| **Diagnóstico de cuello de botella** | "Necesito más clientes / ingresos / margen" sin causa clara | Diagnóstico en los 5 puntos de control de abajo + el siguiente experimento (usa `templates/experiment-card.md`) |
| **Construcción completa** | Oferta nueva, segmento nuevo, motor nuevo, o fundador que empieza a vender | El subconjunto relevante del mapa de 12 pasos, cada paso cerrado con su plantilla |

Nunca asumas la construcción completa por defecto. Pregunta el modo si no está claro; si el usuario no está presente, elige el modo más pequeño que responda a la petición y di cuál elegiste.

## Paso 1 — Árbol de decisión: qué cargar

| Situación | Cargar |
|---|---|
| "Necesito más clientes" / cuello de botella incierto | **Secuencia de diagnóstico** de abajo, luego `references/metrics.md` |
| Oferta vaga, precio adivinado, tiers desordenados | `references/offer-pricing.md` + `templates/pricing-tier-worksheet.md` |
| Montar pipeline / prospectar / outreach en frío | `references/outbound.md` + `templates/5-touch-sequence.md` + `templates/cold-call-scripts.md` + `examples/cold-email-good-vs-bad.md` |
| Primera llamada con un prospecto | `references/discovery.md` + `templates/discovery-call-guide.md` + `examples/discovery-call-transcript.md` |
| Calificar un negocio enterprise / grande | `references/qualification.md` + `templates/meddpicc-scorecard.md` |
| Negocio parado, "lo voy a pensar", sin siguiente paso | `references/jolt.md` + `objections/library.md` |
| Cualquier objeción, resistencia al precio | `references/objections.md` + `objections/library.md`; para precio, también `references/negotiation.md` |
| Petición de descuento, compras, términos de contrato | `references/negotiation.md` + `templates/business-case-onepager.md` |
| Un solo contacto en la cuenta | `references/multithreading.md` + `templates/buying-committee-map.md` |
| Pitch, demo, deck, hero de la web | `references/narrative.md` + `templates/pitch-narrative.md` |
| Fundador vendiendo por primera vez, contratar al primer vendedor | `references/founder-sales.md` |
| Producto self-serve con señales de uso | `references/plg-pql.md` |
| Garantía, política de reembolso, urgencia, escasez | `references/guarantees-scarcity.md` |
| Churn, onboarding, alcance que crece, referidos, casos de éxito | `references/delivery-retention.md` |
| Web, contenido, qué publicar | `references/content.md` |
| Usar IA en prospección, análisis de llamadas, timing | `references/ai-in-sales.md` |
| Mecánica de persuasión, frases exactas | `references/psychology.md` |
| Antes de un forecast o revisión de pipeline | `checklists/deal-review.md` |
| Después de cualquier llamada de ventas | `checklists/post-call-rubric.md` |
| "¿Esto sigue vigente?" | `trends.md` |
| "¿Qué leer para profundizar?" | `reading-list.md` |

## Paso 2 — Secuencia de diagnóstico (antes de concluir nada)

"Necesito más marketing" es una hipótesis, no un diagnóstico. Comprueba en este orden y detente en el primer eslabón roto:

1. **Alcance** — ¿Las personas adecuadas, en número suficiente, están viendo la oferta? (impresiones, tamaño de la lista, reuniones agendadas)
2. **Calidad de los leads** — De los que responden, ¿cuántos encajan en el perfil ideal? (calificados / total)
3. **Conversión** — De los leads calificados, ¿cuántos compran y en qué etapa caen? (etapa por etapa, ver los criterios de etapa en `references/qualification.md`)
4. **Capacidad** — ¿El negocio puede entregar más sin que la calidad se hunda? (utilización, backlog)
5. **Retención y expansión** — ¿Los clientes se quedan y compran más? (churn, NRR, referidos)

Arreglar el alcance cuando la conversión está rota compra más derrotas. Arreglar la conversión cuando la capacidad está llena compra clientes enfadados. Números de cada punto: `references/metrics.md`.

## Paso 3 — Principios centrales (revisados en la v2)

1. **Un negocio es arbitraje con margen de seguridad.** Los ingresos por cliente deben superar el coste de adquirirlo y atenderlo, con holgura para el error. Mídelo: CAC, payback, margen de contribución, retención por cohorte.
2. **Orden de trabajo: Oferta → Precio → Ventas → Demanda**, pero diagnostica primero (Paso 2). Más demanda sobre una oferta débil expone la debilidad más rápido.
3. **La confianza es el activo.** El comprador asume riesgo de dinero, tiempo y reputación. Todo artefacto debe reducir ese riesgo con evidencia, no con adjetivos.
4. **El posicionamiento sigue a la demanda, el coste y la capacidad**, no a un eslogan. Premium, gama media y volumen funcionan cuando la economía unitaria cierra. La "zona de la muerte" es cualquier posición donde precio, coste de servir y expectativas del comprador no encajan entre sí.
5. **Vende resultados que el comprador definió**, no funcionalidades que tú construiste. Descubre qué valora antes de asumir que velocidad, precio o comodidad es la palanca.
6. **La oferta y la demanda fijan el techo del precio; el coste fija el suelo; las alternativas fijan la referencia.** Cuando la demanda supera la capacidad, sube el precio o recorta plazas; cuando no, arregla la oferta antes de bajar el precio.
7. **"No decidir" es el principal competidor.** La indecisión pierde más negocios calificados que los rivales; trátala como una objeción con su propio playbook (`references/jolt.md`).
8. **El mercado expone la vaguedad.** Una oferta vaga aparece como leads no calificados; un precio ilógico aparece en la negociación; el cliente equivocado aparece en la entrega; el contenido vacío aparece como silencio.

## Paso 4 — El mapa de 12 pasos (lo que cubre una construcción completa)

| # | Paso | Módulo | Se cierra con |
|---|---|---|---|
| 0 | Recogida de contexto | abajo | Formulario completado |
| 1 | Cliente ideal, dolor, investigación | `references/discovery.md` (sección Mom Test) | Notas de investigación con clientes |
| 2 | Oferta | `references/offer-pricing.md` | Declaración de la oferta |
| 3 | Economía y precio | `references/offer-pricing.md`, `references/metrics.md` | `templates/pricing-tier-worksheet.md` |
| 4 | Calificación y descubrimiento | `references/qualification.md`, `references/discovery.md` | `templates/meddpicc-scorecard.md`, `templates/discovery-call-guide.md` |
| 5 | Narrativa y prueba | `references/narrative.md`, `references/delivery-retention.md` | `templates/pitch-narrative.md` |
| 6 | Reducción de riesgo, escasez | `references/guarantees-scarcity.md` | Garantía con cuenta de exposición |
| 7 | Pipeline y outbound | `references/outbound.md` | `templates/5-touch-sequence.md` |
| 8 | Objeciones, indecisión, negociación | `references/objections.md`, `references/jolt.md`, `references/negotiation.md` | `templates/business-case-onepager.md` |
| 9 | Comité de compra | `references/multithreading.md` | `templates/buying-committee-map.md` |
| 10 | Contrato y traspaso | `references/delivery-retention.md` (sección de contrato) | Checklist de contrato, documento de traspaso |
| 11 | Entrega, retención, referidos, casos de éxito | `references/delivery-retention.md` | Plan 30/60/90, momento del referido, consentimiento del caso |
| 12 | Contenido y palanca de IA | `references/content.md`, `references/ai-in-sales.md` | Plan de contenido, flujo de IA |

Transversales: `references/metrics.md` (mide cada paso), `references/psychology.md` (formulación), `templates/experiment-card.md` (cambia una cosa a la vez).

## Recogida de contexto (pregunta solo lo que falte)

1. Qué se vende, a quién, quién firma, quién usa.
2. Mercado y país (normas contractuales, hábitos de compras).
3. Precio hoy, coste real de entrega, horas por cliente.
4. Capacidad: clientes por semana/mes, cadencia de inicio.
5. De dónde vienen los clientes ahora; conversión por etapa si se conoce.
6. Prueba disponible: resultados con números, testimonios, casos, certificaciones.
7. Tamaño del negocio y duración del ciclo (decide si aplican MEDDPICC y multithreading).
8. Meta y restricción: más clientes, más margen, menos esfuerzo, ingresos recurrentes, decisiones más rápidas.

## Reglas inviolables

1. Toda llamada termina con un siguiente paso agendado, o el negocio se marca en riesgo.
2. Ningún precio sale sin dolor cuantificado o business case (`templates/business-case-onepager.md`).
3. El descuento se intercambia, nunca se regala: "Hago X si tú haces Y."
4. Los negocios enterprise nunca tienen un solo contacto.
5. Trata el "no decidir" antes que a la competencia.
6. La escasez y los plazos son reales o no existen. La urgencia inventada es una retirada de confianza que no puedes reponer.
7. La prueba está documentada y autorizada. Las simulaciones se etiquetan como simulaciones.
8. Una variable por experimento, con regla de parada.

## Criterios de etapa del embudo (criterios objetivos para avanzar)

| Etapa | Criterio de salida |
|---|---|
| Lead | Encaja en el perfil en 2 de 3: segmento, cargo, señal de disparo |
| Calificado | Dolor dicho con sus palabras + impacto cuantificado + un proceso de decisión nombrado |
| Descubrimiento hecho | Scorecard MEDDPICC sin rojo en Dolor, Champion y Proceso de decisión |
| Propuesta | Business case aceptado por el champion; comprador económico identificado y alcanzado |
| Negociación | Criterios escritos cumplidos; proceso burocrático (legal, seguridad, compras) mapeado con fechas |
| Cerrado | Firmado + kickoff agendado + documento de traspaso enviado |

## Contratos de salida

**Revisión rápida:** 1) veredicto en una línea; 2) el artefacto corregido; 3) registro de cambios, un motivo por cambio; 4) una cosa para probar a continuación.

**Diagnóstico de cuello de botella:** 1) los cinco puntos con el número o "desconocido" en cada uno; 2) el eslabón roto; 3) una ficha de experimento; 4) qué medir en 30 días.

**Construcción completa:** los pasos aplicables del mapa de 12 pasos, cada uno cerrado con su plantilla, y luego un plan de 30 días con responsables y métricas. Nunca rellenes con pasos que no aplican.

## Lo que esta skill se niega a hacer

- Usar BANT como filtro (presupuesto y plazo quedan solo como señales).
- Escribir aperturas del tipo "espero que estés bien" o "me gustaría presentar nuestra empresa".
- Presentar funcionalidades y beneficios como estructura de pitch.
- Recomendar volumen de email sin configuración de entregabilidad.
- Apilar garantías por defecto o prometer resultados fuera del control del vendedor.
- Citar porcentajes sin fuente y población ("el 97% no está listo para comprar" quedó retirado).
- Dar frases motivacionales en lugar de una acción.

## Mantenimiento

Ver `CHANGELOG.md`. Las tendencias y los benchmarks envejecen más rápido: reverifica `trends.md` y las heurísticas de `references/metrics.md` en cada fecha de revisión. Fuentes por sección: `reading-list.md`.
