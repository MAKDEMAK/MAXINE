# MAXINE

> **FROZEN COHORT — 2026-09-16**

MAXINE es una cohorte cerrada de investigación y desarrollo dentro del programa FARMAKSIA. Sus cuatro automatizaciones fueron detenidas y el repositorio queda preservado como snapshot histórico: futuras combinaciones de frentes deben abrir una cohorte/repositorio nuevo.

## Resultado final

MAXINE cierra en **M2** como un solo ecosistema: **MAXINE Adaptive Observability System**.

La arquitectura final une dos componentes verificables:

1. **Adaptive Visual Sampling (M2)** — política de asignación de un presupuesto finito de sensado según prioridad espacial, cambio temporal, información espectral, estado de adaptación y utilidad de tarea.
2. **Retinal Measurement Stack (M2)** — capa de adquisición/medición que mantiene separados datos crudos, restauración, mediciones derivadas, incertidumbre y procedencia.

`Multi-State Focus` (M1) fue fusionado dentro de Adaptive Visual Sampling como operador óptico opcional de estado focal/light-field; no se conserva como proyecto independiente.

La especificación integradora está en `project/architecture.yaml` y la auditoría de cierre en `docs/closure.md`.

## Evidencia

La cohorte conserva **33 registros estructurados**:

- F1 — farmacología / visión / neuro-oftalmología: **9**
- F2 — visión animal comparada: **12**
- F3 — visión digital / óptica computacional / imagen: **12**

Cada registro completo vive en los ledgers de `evidence/`; `graph/nodes.jsonl` funciona como índice canónico y `graph/edges.jsonl` contiene únicamente relaciones explícitamente justificadas. Un nodo sin arista de diseño significa **no integrado**, no inválido.

## Madurez

- `M0` señal interesante
- `M1` convergencia sustentada
- `M2` especificación funcional
- `M3` prototipo mínimo
- `M4` prueba / medición
- `M5` pieza, obra o producto demostrable

MAXINE **no alcanzó M3**: no existe un artefacto ejecutable que haya pasado los criterios de validación definidos. El cierre no fabrica prototipos vacíos para elevar artificialmente la madurez.

## Estructura relevante

- `evidence/` — registros científicos/técnicos normalizados por frente
- `graph/` — nodos, relaciones y vocabulario
- `project/state.yaml` — estado final congelado
- `project/architecture.yaml` — arquitectura unificada
- `project/modules/` — especificaciones M2 retenidas
- `project/archive/` — módulos fusionados/archivados
- `docs/methodology.md` — reglas metodológicas
- `docs/decisions.md` — decisiones de diseño y cierre
- `docs/closure.md` — auditoría final

## Principio FARMAKSIA preservado

Los tres frentes investigaron independientemente para limitar bucles de sesgo. La síntesis conectó evidencia sólo cuando existía una relación defendible y distinguió evidencia, inferencia de diseño y especulación. MAXINE se congela sin reescribir esa historia.
