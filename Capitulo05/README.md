# Práctica. Escenarios visuales sobre la evolución de los servicios financieros en El Salvador

Esta práctica utiliza tendencias públicas para explorar futuros posibles de los servicios financieros en El Salvador. Los escenarios se construyen mediante preguntas de tipo “¿qué pasaría si...?” y se presentan como posibilidades condicionadas, no como predicciones.

## Metadatos

| Campo | Detalle |
|---|---|
| Duración | 17 min |
| Complejidad | Media |
| Nivel de Bloom | Analizar |
| Tipo de actividad | Investigación, diseño de escenarios y visualización |
| Aplicaciones | Microsoft Copilot Chat |
| Modalidad | Individual, guiada |
| Insumos previos | Ninguno |
| Resultado | Tres escenarios contrastantes y una matriz visual de variables, condiciones, señales e implicaciones |

## Distribución de tiempo

| Fase | Actividad | Tiempo |
|---|---|---:|
| 1 | Identificar tendencias y variables | 5 min |
| 2 | Construir escenarios “¿qué pasaría si...?” | 7 min |
| 3 | Crear la comparación visual | 5 min |
| **TOTAL** |  | **17 min** |

## Descripción general

Copilot ayudará a identificar tendencias públicas relacionadas con digitalización, inclusión financiera, pagos digitales y hábitos de los usuarios. A partir de ellas seleccionarás variables y modificarás sus condiciones para construir escenarios contrastantes. El resultado final será una representación visual que muestre características, señales e implicaciones sin afirmar que un escenario ocurrirá.

## Objetivos de aprendizaje

- Identificar tendencias y variables relevantes utilizando información pública.
- Formular preguntas de tipo “¿qué pasaría si...?” para explorar posibilidades.
- Construir escenarios contrastantes sin tratarlos como predicciones.
- Identificar condiciones y señales que permitirían observar la evolución de cada escenario.
- Comparar los escenarios mediante una representación visual.

## Escenario de la práctica

Se explorará cómo podrían evolucionar los servicios financieros en El Salvador ante cambios en variables relacionadas con digitalización, inclusión financiera, pagos digitales y hábitos de los usuarios.

## Prerrequisitos

- Conocimientos básicos de Copilot y prompting.
- Acceso a Internet y Microsoft Copilot Chat.
- No se requiere Microsoft 365 Copilot Premium.

## Preparación del entorno

1. Abre `https://copilot.cloud.microsoft/chat` o el acceso equivalente de tu organización.
2. Confirma que Copilot puede consultar información pública de la Web.
3. Inicia una conversación nueva.

## Desarrollo de la práctica

### Fase 1 - Identificar tendencias y variables

**Tiempo:** 5 min  
**Aplicación:** Microsoft Copilot Chat  
**Objetivo:** construir una base de señales actuales antes de explorar escenarios.

### Paso 1. Busca tendencias públicas

> **PROMPT 1 - IDENTIFICAR TENDENCIAS Y VARIABLES**

```text
Investiga información pública reciente sobre El Salvador relacionada con estas cuatro áreas:
- digitalización de servicios financieros;
- inclusión financiera;
- pagos digitales;
- hábitos o comportamiento de los usuarios de servicios financieros.

Para cada área identifica al menos una tendencia o señal pública que pueda documentarse.

Devuelve una tabla con:
Área | Tendencia o señal | Dato o evidencia | Fuente | Fecha | Enlace | Variable que podría cambiar en el futuro.

Reglas:
- Prioriza fuentes oficiales, institucionales y originales.
- No inventes cifras ni extrapoles una tendencia como predicción.
- Si la evidencia es insuficiente, indícalo expresamente.
- La variable final debe poder formularse como algo que podría aumentar, disminuir o cambiar.
```

### Paso 2. Elige dos variables

Selecciona dos variables que permitan construir escenarios distintos. Ejemplos de forma, no de contenido obligatorio: nivel de adopción, disponibilidad de conectividad, confianza, aceptación de pagos digitales o familiaridad de los usuarios.

**Criterio de finalización:** hay 2 variables seleccionadas y cada una se relaciona con al menos una fuente pública.

### Fase 2 - Construir escenarios “¿qué pasaría si...?”

**Tiempo:** 7 min  
**Aplicación:** Microsoft Copilot Chat  
**Objetivo:** explorar cómo cambiarían las implicaciones al modificar las variables seleccionadas.

### Paso 3. Construye tres escenarios contrastantes

> **PROMPT 2 - EXPLORAR ESCENARIOS**

```text
Utiliza las dos variables seleccionadas para construir 3 escenarios contrastantes sobre la evolución de los servicios financieros en El Salvador.

Formula cada escenario como respuesta a una pregunta de tipo “¿qué pasaría si...?” y cambia de manera explícita las condiciones de las variables entre escenarios.

Para cada escenario incluye:
- condición de la variable 1;
- condición de la variable 2;
- características del escenario;
- qué factores podrían favorecerlo;
- posibles implicaciones para usuarios, instituciones financieras y pequeños negocios;
- señales observables que convendría monitorear;
- supuestos o información pendiente de validar.

Reglas:
- Trátalos como escenarios exploratorios, no como predicciones.
- Usa lenguaje condicional: “podría”, “sería posible”, “si se cumple”.
- No asignes probabilidades.
- No inventes eventos regulatorios, cifras futuras ni comportamientos garantizados.
- Distingue lo que proviene de las tendencias actuales de lo que es una hipótesis del escenario.

Presenta los 3 escenarios en una tabla comparable.
```

### Paso 4. Revisa la diferencia entre escenarios

Comprueba que los escenarios cambian realmente al modificar las variables. Si son demasiado parecidos, pide a Copilot que haga más explícitas las condiciones que los diferencian.

**Criterio de finalización:** hay 3 escenarios con condiciones distintas, señales observables y supuestos identificados.

### Fase 3 - Crear la comparación visual

**Tiempo:** 5 min  
**Aplicación:** Microsoft Copilot Chat  
**Objetivo:** representar los escenarios de forma que puedan compararse rápidamente.

### Paso 5. Genera una matriz visual

> **PROMPT 3 - MATRIZ VISUAL DE ESCENARIOS**

```text
Convierte los 3 escenarios anteriores en una representación visual compacta para una sola pantalla.

Usa una matriz con:
- una columna por escenario;
- filas para: variable 1, variable 2, condición principal, señales a observar, posible implicación para usuarios, posible implicación para instituciones, posible implicación para pequeños negocios y principal incertidumbre.

Requisitos:
- utiliza frases breves;
- resalta claramente qué cambia entre escenarios;
- incluye una leyenda: “Escenarios exploratorios; no constituyen predicciones”.
- no uses probabilidades ni una clasificación de escenario mejor/peor;
- marca cualquier elemento no sustentado como “hipótesis”.

Después de la matriz, escribe 2 nuevas preguntas de investigación que surgieron al comparar los escenarios.
```

Si la interfaz permite crear imágenes, puedes solicitar opcionalmente una infografía basada en la matriz. La matriz textual es suficiente para completar la práctica.

**Criterio de finalización:** existe una representación visual que permite contrastar variables, señales e implicaciones de los 3 escenarios.

## Validación y pruebas finales

| # | Criterio | Estado |
|---|---|---|
| 1 | Se identifican señales o tendencias en las 4 áreas indicadas. | ☐ |
| 2 | Se seleccionan exactamente 2 variables. | ☐ |
| 3 | Se construyen exactamente 3 escenarios contrastantes. | ☐ |
| 4 | Cada escenario identifica factores, señales e incertidumbres. | ☐ |
| 5 | Los escenarios usan lenguaje condicional y no asignan probabilidades. | ☐ |
| 6 | Existe una matriz visual comparativa. | ☐ |
| 7 | La matriz incluye la advertencia de que no constituye una predicción. | ☐ |
| 8 | Se generan 2 nuevas preguntas de investigación. | ☐ |

## Solución de problemas

| Situación | Qué hacer |
|---|---|
| Copilot presenta un escenario como pronóstico. | Pide reformularlo en lenguaje condicional y eliminar probabilidades. |
| Los escenarios son casi iguales. | Cambia de forma explícita las condiciones de una o ambas variables. |
| Aparecen cifras futuras sin fuente. | Elimínalas o márcalas como hipótesis; no las uses como evidencia. |
| No está disponible la generación de imágenes. | Utiliza la matriz visual en Markdown. |

## Limpieza y conservación

- Conserva la conversación si deseas revisar los escenarios durante la sesión.
- No es necesario descargar imágenes ni crear archivos.

## Resumen de la práctica

Partiste de tendencias públicas, seleccionaste variables, exploraste tres combinaciones mediante preguntas “¿qué pasaría si...?” y organizaste los resultados en una matriz visual que compara posibilidades sin convertirlas en predicciones.
