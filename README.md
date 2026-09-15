# MAXINE

MAXINE es una cohorte de investigación y desarrollo dentro del programa FARMAKSIA.

## Alcance de esta cohorte

MAXINE trabaja con cuatro capas coordinadas:

1. **Frente 1 — Farmacología, visión, color y neurociencia**
2. **Frente 2 — Visión animal y percepción comparada**
3. **Frente 3 — Visión digital, oftalmología tecnológica, hardware, software y matemáticas**
4. **Capa 4 — Síntesis, arquitectura y desarrollo**

Los tres primeros frentes investigan de forma independiente para reducir sesgo y deriva temática. La cuarta capa no dirige sus búsquedas: recibe evidencia, detecta convergencias defendibles y transforma esas convergencias en módulos construibles.

## Principio de trabajo

MAXINE no busca acumular informes. El flujo esperado es:

`evidencia -> relación -> especificación -> prototipo -> prueba -> pieza/producto`

Cada módulo avanza por niveles de madurez:

- `M0` señal interesante
- `M1` convergencia sustentada
- `M2` especificación funcional
- `M3` prototipo mínimo
- `M4` prueba / medición
- `M5` pieza, obra o producto demostrable

Máximo recomendado: **3 módulos activos simultáneamente**.

## Estructura

- `evidence/` — paquetes de evidencia estructurados por frente
- `graph/` — nodos, relaciones y vocabulario del grafo de conocimiento
- `project/` — estado vivo de MAXINE y módulos activos
- `prototypes/` — prototipos reales M3+
- `artifacts/` — SVG, shaders, datos, imágenes y otros artefactos
- `src/` — código reutilizable
- `tests/` — pruebas
- `docs/` — metodología y registro de decisiones

## Relación con FARMAKSIA

FARMAKSIA es el programa general. MAXINE es una cohorte temporal con un conjunto concreto de frentes. Cuando esta cohorte cierre, sus resultados quedan congelados y una cohorte futura puede abrirse en otro repositorio con otros frentes sin reescribir la historia de MAXINE.
