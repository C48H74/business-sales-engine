# IA en el proceso de ventas

Carga cuando el usuario quiera aplicar IA a prospección, llamadas, forecast, timing o contenido. Principio: la IA eleva el suelo del trabajo mediocre y la vara de lo que cuenta como personal; no sustituye el criterio ni las relaciones.

## Dónde ayuda, con salvaguardas

| Uso | Cómo | Salvaguarda |
|---|---|---|
| **Investigación de cuentas** | Resumir información pública, noticias recientes, contrataciones y cambios de producto en un briefing de un párrafo con fuentes | Verifica un dato antes de usarlo en un mensaje; los detalles alucinados terminan conversaciones |
| **Personalización a escala** | Redactar primeras líneas a partir de señales reales; tú editas | Como todo el mundo lo hace, las líneas genéricas "personalizadas por IA" parecen plantilla. La vara es una observación específica, verdadera y reciente |
| **Transcripción y análisis de llamadas** | Puntuar contra `checklists/post-call-rubric.md`: proporción de habla, número y tipos de preguntas, siguiente paso registrado, objeciones planteadas, huecos de MEDDPICC | Revisa la puntuación en una muestra; los modelos sobrevaloran las llamadas amables |
| **Minería de objeciones** | Agrupar objeciones de transcripciones y emails; actualizar `objections/library.md` | Conserva las palabras del comprador |
| **Borradores de propuesta y business case** | Rellenar `templates/business-case-onepager.md` con las notas de descubrimiento | Los números vienen del cliente, nunca se generan |
| **Higiene del pipeline** | Señalar negocios sin siguiente paso, etapas estancadas, threads únicos | Primero con reglas; es más barato y más fiable |
| **Forecast y timing ("quién comprará, cuándo")** | Scores de intención/propensión a partir de señales | Ver la nota de calibración de abajo |
| **Presencia de marca en asistentes** | Pregunta a varios asistentes de IA cómo describen tu empresa, categoría y alternativas; corrige con páginas factuales | Reverifica cada trimestre; las respuestas cambian |
| **Role-play** | Ensayar descubrimiento y objeciones con un modelo que hace de persona compradora | Tómalo como práctica, no como investigación |

## Nota de calibración sobre los scores predictivos

Los modelos que predicen decisiones humanas (quién comprará, cuándo cierra un negocio, qué lead convertirá) son mucho más débiles de lo que afirman los proveedores, como sostienen Narayanan y Kapoor en *AI Snake Oil*: los resultados dependen de información que el modelo nunca ve. Antes de fiarte de un score de propensión:
1. Compáralo con una línea base simple (recencia de la señal + encaje) en tus propios negocios cerrados.
2. Comprueba la calibración: de los leads con score 80%, ¿convirtió aproximadamente el 80%?
3. Usa los scores para **priorizar** trabajo, nunca para **saltarte** el descubrimiento ni para rechazar un lead automáticamente.

## Qué no automatizar

- Conversaciones de descubrimiento (el comprador lo nota).
- Negociación.
- La petición de referidos.
- Cualquier mensaje que sugiera una relación humana que no existe.

## Datos y transparencia

- Graba llamadas solo con consentimiento conforme a la ley local; dilo al comenzar.
- Mantén los datos de clientes fuera de herramientas que entrenan con las entradas, salvo que haya cobertura contractual.
- No dejes que un modelo invente referencias, logos o resultados. Toda afirmación se remonta a las reglas de prueba de `references/delivery-retention.md`.

## Una configuración viable para un equipo pequeño

1. Briefing de investigación por cuenta (borrador de IA, comprobación humana de 2 minutos).
2. Borradores de secuencia a partir de `templates/5-touch-sequence.md` con primeras líneas basadas en señales (edición humana).
3. Transcripciones de llamadas puntuadas semanalmente contra la rúbrica; una nota de coaching por vendedor.
4. Minería mensual de objeciones hacia la biblioteca.
5. Comprobación trimestral de la marca en los asistentes.
