# Práctica. Diferentes perspectivas ante la evolución de los servicios financieros digitales

Esta práctica utiliza información pública para analizar una tendencia de los servicios financieros digitales desde varias perspectivas y comprobar cómo cambian las prioridades, beneficios y preocupaciones según el actor observado.

## Metadatos

| Campo | Detalle |
|---|---|
| Duración | 15 min |
| Complejidad | Media |
| Nivel de Bloom | Analizar |
| Tipo de actividad | Investigación y análisis de perspectivas |
| Aplicaciones | Microsoft Copilot Chat |
| Modalidad | Individual, guiada |
| Insumos previos | Ninguno |
| Resultado | Matriz de perspectivas con coincidencias, tensiones y preguntas pendientes |

## Distribución de tiempo

| Fase | Actividad | Tiempo |
|---|---|---:|
| 1 | Identificar una tendencia sustentada en fuentes públicas | 4 min |
| 2 | Analizar la tendencia desde diferentes perspectivas | 7 min |
| 3 | Contrastar coincidencias y tensiones | 4 min |
| **TOTAL** |  | **15 min** |

## Descripción general

Primero identificarás una tendencia reciente relacionada con servicios financieros digitales. Después pedirás a Copilot que la observe desde las perspectivas de clientes, instituciones financieras, pequeños negocios y otro actor pertinente. El resultado se revisará para evitar asumir que todos los actores tienen las mismas necesidades o que una perspectiva representa por sí sola la situación completa.

## Objetivos de aprendizaje

- Identificar una tendencia utilizando información pública reciente.
- Analizar una misma situación desde perspectivas diferentes.
- Contrastar beneficios, necesidades, preocupaciones y prioridades.
- Identificar coincidencias, tensiones y aspectos que requieren investigación adicional.

## Escenario de la práctica

Se analizará la evolución de los servicios financieros digitales utilizando información pública. Deben considerarse, como mínimo, las perspectivas de clientes, instituciones financieras y pequeños negocios, además de otro actor relacionado que resulte pertinente para la tendencia seleccionada.

## Prerrequisitos

- Conocimientos básicos de Copilot y prompting.
- Acceso a Internet y Microsoft Copilot Chat.
- No se requiere Microsoft 365 Copilot Premium.

## Preparación del entorno

1. Abre `https://copilot.cloud.microsoft/chat` o el acceso equivalente de tu organización.
2. Confirma que Copilot puede consultar información pública de la Web.
3. Inicia una conversación nueva.

## Desarrollo de la práctica

### Fase 1 - Identificar una tendencia sustentada

**Tiempo:** 4 min  
**Aplicación:** Microsoft Copilot Chat  
**Objetivo:** elegir una tendencia que pueda analizarse con evidencia pública.

### Paso 1. Busca tendencias recientes

> **PROMPT 1 - IDENTIFICAR UNA TENDENCIA**

```text
Investiga información pública reciente sobre la evolución de los servicios financieros digitales en El Salvador y, cuando ayude a contextualizar, en Centroamérica.

Identifica 3 tendencias que puedan documentarse con fuentes públicas. Para cada una indica:
- nombre breve de la tendencia;
- qué cambio o evolución se observa;
- fuente u organización;
- fecha de publicación, cuando esté disponible;
- enlace directo;
- qué aspecto sigue siendo incierto o requiere más evidencia.

Prioriza fuentes oficiales, instituciones reconocidas y fuentes originales. No inventes cifras ni conviertas una expectativa en un hecho.
```

### Paso 2. Selecciona una tendencia

Elige la tendencia que tenga fuentes más claras y que permita observar efectos sobre distintos actores.

**Criterio de finalización:** hay una tendencia seleccionada respaldada por al menos 2 fuentes públicas o por una fuente original suficientemente clara.

### Fase 2 - Analizar diferentes perspectivas

**Tiempo:** 7 min  
**Aplicación:** Microsoft Copilot Chat  
**Objetivo:** observar la misma tendencia desde distintas necesidades e intereses.

### Paso 3. Solicita el análisis multiperspectiva

> **PROMPT 2 - ANALIZAR PERSPECTIVAS**

```text
Analiza la tendencia seleccionada desde estas perspectivas:
1. clientes o usuarios;
2. instituciones financieras;
3. pequeños negocios;
4. un actor adicional que resulte relevante según las fuentes consultadas.

Para el cuarto actor, explica primero por qué es pertinente para esta tendencia.

Para cada perspectiva identifica:
- beneficios potenciales;
- necesidades;
- preocupaciones;
- prioridades;
- qué evidencia pública respalda el análisis;
- qué parte es una inferencia o hipótesis por validar.

Reglas:
- No supongas que todos los integrantes de un grupo piensan igual.
- No presentes beneficios potenciales como resultados garantizados.
- Separa hechos respaldados, interpretaciones e información pendiente.
- Incluye enlaces a las fuentes utilizadas.

Entrega una matriz con una fila por perspectiva.
```

### Paso 4. Revisa las perspectivas

Confirma que cada perspectiva tiene prioridades diferentes y que Copilot no atribuye opiniones concretas a un actor sin evidencia.

**Criterio de finalización:** la matriz contiene 4 perspectivas y diferencia hechos de inferencias.

### Fase 3 - Contrastar coincidencias y tensiones

**Tiempo:** 4 min  
**Aplicación:** Microsoft Copilot Chat  
**Objetivo:** mostrar cómo una misma tendencia puede interpretarse de maneras diferentes.

### Paso 5. Pide una síntesis comparativa

> **PROMPT 3 - CONTRASTAR INTERPRETACIONES**

```text
A partir de la matriz anterior, identifica:
- 2 coincidencias entre actores;
- 2 tensiones o prioridades que puedan entrar en conflicto;
- 2 preguntas que sería necesario investigar antes de tomar una decisión;
- 1 conclusión que cambiaría si solo se observara la tendencia desde una de las perspectivas.

Para cada punto indica si proviene directamente de una fuente o si es una interpretación derivada del análisis.

No elijas una perspectiva como la correcta. El objetivo es hacer visibles diferencias y puntos de encuentro.
```

**Criterio de finalización:** existen coincidencias, tensiones y preguntas pendientes sin presentar una perspectiva como única explicación válida.

## Validación y pruebas finales

| # | Criterio | Estado |
|---|---|---|
| 1 | La tendencia analizada está respaldada por información pública. | ☐ |
| 2 | Se analizan exactamente 4 perspectivas. | ☐ |
| 3 | Incluye clientes, instituciones financieras y pequeños negocios. | ☐ |
| 4 | El cuarto actor tiene una justificación de pertinencia. | ☐ |
| 5 | Se diferencian hechos, interpretaciones e hipótesis. | ☐ |
| 6 | Se identifican al menos 2 coincidencias y 2 tensiones. | ☐ |
| 7 | Hay al menos 2 preguntas pendientes de investigación. | ☐ |

## Solución de problemas

| Situación | Qué hacer |
|---|---|
| Copilot presenta opiniones de un actor como hechos. | Pide la fuente concreta o cambia la redacción a “posible preocupación” o “hipótesis por validar”. |
| Las cuatro perspectivas son casi iguales. | Pide que destaque objetivos, restricciones y riesgos específicos de cada actor. |
| La tendencia es demasiado amplia. | Acótala a un cambio concreto: canal, hábito, tecnología, tipo de servicio o patrón de uso. |

## Limpieza y conservación

- Conserva la conversación como evidencia de la progresión del análisis si resulta útil.
- No es necesario crear archivos adicionales.

## Resumen de la práctica

Seleccionaste una tendencia sustentada, la analizaste desde cuatro perspectivas y contrastaste coincidencias, tensiones y preguntas pendientes para evitar conclusiones construidas desde un único punto de vista.
