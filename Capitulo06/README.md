# Práctica. Seguimiento de nuevas disposiciones y regulaciones del sector financiero

Esta práctica transforma una necesidad recurrente de búsqueda en un prompt reutilizable para localizar nuevas regulaciones, normativas, disposiciones o actualizaciones relevantes para el sector financiero en El Salvador. No se implementan automatizaciones ni agentes.

## Metadatos

| Campo | Detalle |
|---|---|
| Duración | 9 min |
| Complejidad | Media |
| Nivel de Bloom | Crear |
| Tipo de actividad | Diseño y reutilización de prompt de investigación |
| Aplicaciones | Microsoft Copilot Chat |
| Modalidad | Individual, guiada |
| Insumos previos | Ninguno |
| Resultado | Prompt reutilizable probado en dos consultas y boletín ejecutivo de actualización regulatoria descargable como Word (.docx) |

## Distribución de tiempo

| Fase | Actividad | Tiempo |
|---|---|---:|
| 1 | Preparar y ejecutar el prompt reutilizable | 5 min |
| 2 | Modificar parámetros y repetir la consulta | 3 min |
| 3 | Validar la reutilización | 1 min |
| **TOTAL** |  | **9 min** |

## Descripción general

Definirás una estructura de prompt en la que algunos criterios se mantienen constantes y otros se sustituyen en cada búsqueda. La consulta priorizará fuentes oficiales de El Salvador y pedirá, como mínimo, fecha de publicación, organismo emisor, propósito y enlace a la fuente original. Después repetirás la búsqueda cambiando únicamente el periodo y los temas de interés.

## Objetivos de aprendizaje

- Identificar qué elementos deben permanecer constantes en una búsqueda recurrente.
- Definir variables de periodo, fuentes y temas dentro de un prompt reutilizable.
- Solicitar resultados trazables hacia fuentes oficiales.
- Reutilizar la misma estructura cambiando solo los parámetros necesarios.

## Escenario de la práctica

Se necesita revisar periódicamente nuevas regulaciones, normativas, disposiciones o actualizaciones publicadas por organismos oficiales que puedan ser relevantes para el sector financiero en El Salvador.

## Prerrequisitos

- Conocimientos básicos de Copilot y prompting.
- Acceso a Internet y Microsoft Copilot Chat.
- No se requiere Microsoft 365 Copilot Premium.

## Preparación del entorno

1. Abre `https://copilot.cloud.microsoft/chat` o el acceso equivalente de tu organización.
2. Confirma que Copilot puede consultar información pública de la Web.
3. Inicia una conversación nueva.

Como fuentes prioritarias para el ejercicio pueden utilizarse organismos oficiales como la Superintendencia del Sistema Financiero (SSF), el Banco Central de Reserva de El Salvador (BCR) y la Defensoría del Consumidor, además de otras fuentes gubernamentales oficiales que resulten pertinentes para el tema consultado.

## Desarrollo de la práctica

### Fase 1 - Preparar y ejecutar el prompt reutilizable

**Tiempo:** 5 min  
**Aplicación:** Microsoft Copilot Chat  
**Objetivo:** crear una estructura que pueda repetirse sin reescribir toda la consulta.

### Paso 1. Utiliza la plantilla

> **PROMPT 1 - PLANTILLA REUTILIZABLE DE SEGUIMIENTO REGULATORIO**

```text
Realiza una búsqueda de información pública sobre nuevas regulaciones, normativas, disposiciones, comunicados regulatorios o actualizaciones relevantes para el sector financiero en El Salvador.

Parámetros de esta ejecución:
- PERIODO: [PERIODO]
- TEMAS DE INTERÉS: [TEMAS]
- FUENTES PRIORITARIAS: Superintendencia del Sistema Financiero de El Salvador (ssf.gob.sv), Banco Central de Reserva de El Salvador (bcr.gob.sv), Defensoría del Consumidor (defensoria.gob.sv) y otras fuentes gubernamentales oficiales claramente pertinentes.

Para cada resultado extrae:
1. fecha de publicación;
2. organismo emisor;
3. título del documento, disposición o actualización;
4. propósito o tema principal en una frase;
5. tipo de publicación, cuando pueda determinarse;
6. enlace directo a la fuente original;
7. por qué podría ser relevante para el sector financiero;
8. elemento que requiere revisión adicional, si existe.

Reglas:
- Prioriza siempre la fuente oficial original.
- Incluye solo publicaciones dentro del PERIODO indicado.
- No inventes fechas, títulos, vigencia, obligaciones ni efectos jurídicos.
- Si no puedes confirmar un dato, escribe “pendiente de verificar”.
- No realices asesoramiento legal ni determines obligaciones de cumplimiento.
- Si no encuentras resultados verificables, indícalo en lugar de completar la tabla con información dudosa.

Devuelve una tabla ordenada de la publicación más reciente a la más antigua.
```

### Paso 2. Ejecuta la primera búsqueda

Sustituye los parámetros por:

- **PERIODO:** `últimos 30 días hasta la fecha de ejecución`
- **TEMAS:** `pagos digitales, inclusión financiera y protección al consumidor`

Envía el prompt y revisa la tabla.

**Criterio de finalización:** la consulta devuelve resultados dentro del periodo indicado o declara de forma explícita que no encontró resultados verificables.

### Fase 2 - Modificar parámetros y repetir la consulta

**Tiempo:** 3 min  
**Aplicación:** Microsoft Copilot Chat  
**Objetivo:** demostrar que la estructura puede reutilizarse cambiando solo variables.

### Paso 3. Ejecuta una segunda búsqueda

Abre una conversación nueva o reutiliza la plantilla original. Cambia únicamente:

- **PERIODO:** `últimos 90 días hasta la fecha de ejecución`
- **TEMAS:** `ciberseguridad, prevención de fraude y servicios financieros digitales`

No cambies las demás instrucciones.

### Paso 4. Compara las dos ejecuciones

Comprueba que la estructura de salida se mantiene y que solo cambian los resultados debido a los parámetros nuevos.

**Criterio de finalización:** existen dos ejecuciones de la misma plantilla con distintos valores de periodo y temas.

### Fase 3 - Validar la reutilización

**Tiempo:** 1 min  
**Aplicación:** Microsoft Copilot Chat  
**Objetivo:** identificar las partes fijas y variables del prompt.

### Paso 5. Identifica la estructura

Verifica que puedas distinguir:

- **Variables:** PERIODO y TEMAS.
- **Constantes:** jurisdicción El Salvador, prioridad de fuentes oficiales, campos de salida y reglas de verificación.

**Criterio de finalización:** puedes reutilizar el prompt en una consulta futura modificando solo los parámetros necesarios.

### Paso 6. Genera el boletín ejecutivo

Utiliza los hallazgos verificables obtenidos durante la práctica para crear el entregable final.

En la misma conversación, envía:

> **PROMPT 2 - GENERAR BOLETÍN EJECUTIVO**

```text
Utiliza los resultados verificados obtenidos durante esta práctica para crear un boletín ejecutivo de actualización regulatoria para el sector financiero en El Salvador.

Incluye únicamente publicaciones respaldadas por una fuente oficial original.

Para cada hallazgo incluye:
- título de la publicación, disposición o actualización;
- fecha de publicación;
- organismo emisor;
- propósito o tema principal;
- breve explicación de su posible relevancia para el sector financiero;
- enlace directo a la fuente oficial original;
- elemento pendiente de revisión adicional, cuando corresponda.

Organiza el documento con esta estructura:

1. Título del boletín.
2. Periodo de consulta.
3. Resumen ejecutivo.
4. Principales actualizaciones identificadas.
5. Tabla de hallazgos.
6. Aspectos pendientes de validación.
7. Fuentes oficiales consultadas.

Reglas:
- No inventes fechas, vigencia, obligaciones ni efectos jurídicos.
- No realices asesoramiento legal.
- Si un dato no puede confirmarse, indícalo como “pendiente de verificar”.
- No incluyas una publicación si no puede vincularse con una fuente oficial original.

Genera el resultado como un documento de Word descargable.
```

## Validación y pruebas finales

| # | Criterio | Estado |
|---|---|---|
| 1 | La plantilla contiene variables explícitas para periodo y temas. | ☐ |
| 2 | Prioriza fuentes oficiales salvadoreñas. | ☐ |
| 3 | Cada resultado solicita fecha, organismo, propósito y enlace original. | ☐ |
| 4 | La primera ejecución usa los últimos 30 días. | ☐ |
| 5 | La segunda ejecución usa los últimos 90 días y temas diferentes. | ☐ |
| 6 | La estructura del prompt se mantiene entre ambas ejecuciones. | ☐ |
| 7 | Los datos no confirmados se marcan como pendientes. | ☐ |
| 8 | La práctica no utiliza automatizaciones, agentes ni herramientas avanzadas. | ☐ |
| 9 | El boletín contiene únicamente hallazgos respaldados por fuentes oficiales o marcados como pendientes. | ☐ |
| 10 | Cada hallazgo conserva un enlace a la fuente original. | ☐ |
| 11 | El boletín fue generado y descargado correctamente como documento de Word (.docx). | ☐ |

## Solución de problemas

| Situación | Qué hacer |
|---|---|
| Copilot devuelve fuentes de prensa o blogs. | Pide que conserve solo fuentes oficiales originales y descarte resultados sin enlace primario. |
| Aparecen resultados fuera del periodo. | Repite el periodo en una línea separada y pide excluir cualquier publicación fuera de la ventana. |
| Copilot interpreta una publicación como obligación legal. | Pide que describa únicamente el propósito publicado y marque la aplicabilidad como pendiente de revisión especializada. |
| La segunda consulta cambia el formato. | Reutiliza exactamente la plantilla y modifica solo los valores de PERIODO y TEMAS. |

## Limpieza y conservación

- Conserva la plantilla del PROMPT 1 como resultado reutilizable de la práctica.
- Puedes conservar las dos conversaciones para demostrar la reutilización.
- Conserva el boletín ejecutivo de actualización regulatoria en formato Word (.docx) como entregable final.

## Entregable

**Boletín ejecutivo de actualización regulatoria**, con los principales hallazgos y referencias a las fuentes originales, descargable como documento de **Word (.docx)**.

## Resumen de la práctica

Construiste un prompt reutilizable con variables de periodo y temas, lo ejecutaste dos veces con parámetros distintos y comprobaste cómo mantener criterios constantes de fuentes, estructura y trazabilidad en búsquedas recurrentes.
