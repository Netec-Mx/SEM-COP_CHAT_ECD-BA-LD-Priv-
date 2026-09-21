# Práctica. Comparación visual de experiencias de pagos digitales

Esta práctica muestra cómo pasar de una pregunta general como “¿cuál es mejor?” a una comparación estructurada de alternativas de pago digital disponibles en el mercado salvadoreño y regional, utilizando criterios explícitos y fuentes públicas.

## Metadatos

| Campo | Detalle |
|---|---|
| Duración | 15 min |
| Complejidad | Media |
| Nivel de Bloom | Analizar |
| Tipo de actividad | Investigación, comparación y representación visual |
| Aplicaciones | Microsoft Copilot Chat |
| Modalidad | Individual, guiada |
| Insumos previos | Ninguno |
| Resultado | Comparación sustentada y matriz visual de alternativas de pago digital |

## Distribución de tiempo

| Fase | Actividad | Tiempo |
|---|---|---:|
| 1 | Identificar alternativas con fuentes públicas | 4 min |
| 2 | Comparar mediante criterios explícitos | 7 min |
| 3 | Convertir la comparación en un recurso visual | 4 min |
| **TOTAL** |  | **15 min** |

## Descripción general

Copilot localizará alternativas de pago digital con información pública vigente, ayudará a definir criterios de comparación y organizará la evidencia para identificar ventajas, limitaciones y condiciones de uso. Finalmente, el resultado se transformará en una matriz visual que permita contrastar las alternativas sin reducir el análisis a una única “mejor opción”.

## Objetivos de aprendizaje

- Establecer criterios antes de comparar alternativas.
- Utilizar información pública y fuentes originales para sustentar una comparación.
- Diferenciar datos verificables de interpretaciones sobre facilidad o conveniencia.
- Comunicar una comparación mediante una representación visual simple.

## Escenario de la práctica

Se requiere comparar distintas alternativas de pago digital disponibles en el mercado salvadoreño y regional. La comparación debe considerar criterios como facilidad de uso, disponibilidad, requisitos, conveniencia y posibles escenarios de utilización.

## Prerrequisitos

- Conocimientos básicos de Microsoft Copilot y formulación de prompts.
- Acceso a Internet y Microsoft Copilot Chat.
- No se requiere Microsoft 365 Copilot Premium.

## Preparación del entorno

Antes de iniciar el tiempo de práctica:

1. Abre `https://copilot.cloud.microsoft/chat` o el acceso equivalente habilitado por tu organización.
2. Confirma que Copilot puede consultar información pública de la Web.
3. Inicia una conversación nueva.

## Desarrollo de la práctica

### Fase 1 - Identificar alternativas con fuentes públicas

**Tiempo:** 4 min  
**Aplicación:** Microsoft Copilot Chat  
**Objetivo:** seleccionar alternativas que puedan compararse con evidencia accesible.

### Paso 1. Localiza alternativas actuales

> **PROMPT 1 - IDENTIFICAR ALTERNATIVAS DE PAGO DIGITAL**

```text
Busca información pública vigente sobre alternativas de pago digital disponibles en El Salvador y, cuando aporte valor, en el mercado regional centroamericano.

Propón hasta 3 alternativas que puedan compararse entre sí y para las que exista información pública suficiente. Deben existir al menos 2 alternativas verificables para continuar.

Para cada alternativa indica:
- nombre del servicio o alternativa;
- institución o proveedor;
- país o alcance de disponibilidad que la fuente permita confirmar;
- tipo de pago o transferencia que permite realizar;
- requisitos públicos identificados;
- enlace a la fuente oficial o fuente original.

Reglas:
- Prioriza páginas oficiales de las instituciones o proveedores.
- No afirmes que una alternativa está disponible en El Salvador si la fuente no lo confirma.
- Si la disponibilidad o un requisito no puede verificarse, escribe “pendiente de confirmar”.
- No elijas todavía una alternativa ganadora.
```

### Paso 2. Verifica que sean comparables

Selecciona 2 o 3 alternativas con fuentes suficientes. Si una carece de información oficial o no puede compararse con las demás, pide a Copilot que la sustituya o continúa con las alternativas verificables.

**Criterio de finalización:** existen al menos 2 alternativas comparables y cada una cuenta con al menos una fuente pública identificable.

### Fase 2 - Comparar mediante criterios explícitos

**Tiempo:** 7 min  
**Aplicación:** Microsoft Copilot Chat  
**Objetivo:** organizar la comparación y hacer visibles ventajas, limitaciones y condiciones.

### Paso 3. Construye la comparación

En la misma conversación, envía:

> **PROMPT 2 - COMPARAR CON CRITERIOS**

```text
Compara las alternativas seleccionadas usando únicamente la información pública encontrada.

Usa como mínimo estos criterios:
- facilidad de uso;
- disponibilidad;
- requisitos;
- conveniencia;
- posibles escenarios de utilización.

Añade hasta 2 criterios adicionales solo si ayudan a comprender diferencias importantes y pueden sustentarse con información pública.

Para cada criterio y alternativa:
- indica el dato o condición observada;
- identifica una ventaja o limitación solo cuando pueda justificarse;
- añade el enlace de la fuente correspondiente;
- si “facilidad de uso” no puede comprobarse objetivamente con la fuente, indícalo como “requiere prueba o validación de usuario” en lugar de afirmarlo como hecho.

Entrega:
1. una tabla comparativa;
2. una lista breve de ventajas y limitaciones de cada alternativa;
3. una sección “Información insuficiente o pendiente”.

No respondas cuál es “la mejor” en términos generales. Explica que la conveniencia depende de los criterios y del escenario de uso.
```

### Paso 4. Revisa las conclusiones

Comprueba que las ventajas y limitaciones se desprenden de la evidencia. Si Copilot usa expresiones como “más fácil”, “más seguro” o “más conveniente” sin respaldo suficiente, pide que las reformule como interpretación o aspecto por validar.

**Criterio de finalización:** la comparación usa los criterios solicitados y distingue claramente datos, interpretaciones y vacíos de información.

### Fase 3 - Crear la representación visual

**Tiempo:** 4 min  
**Aplicación:** Microsoft Copilot Chat  
**Objetivo:** convertir la comparación en un recurso visual fácil de interpretar.

### Paso 5. Solicita una matriz visual

> **PROMPT 3 - REPRESENTACIÓN VISUAL**

```text
Convierte la comparación anterior en una matriz visual compacta para mostrar en una sola pantalla.

Requisitos:
- columnas: las alternativas seleccionadas;
- filas: facilidad de uso, disponibilidad, requisitos, conveniencia y escenarios de utilización, más los criterios adicionales utilizados;
- en cada celda usa una frase muy breve basada en la evidencia;
- utiliza símbolos simples solo como apoyo visual y agrega una leyenda;
- no conviertas los símbolos en una puntuación total ni declares un ganador general;
- marca “pendiente” donde falte evidencia;
- al final incluye 3 conclusiones: una situación en la que cada alternativa podría resultar adecuada según los criterios observados.
```

Si tu interfaz ofrece generación de imágenes, puedes pedir opcionalmente una infografía basada en la matriz. La matriz textual es suficiente para completar la práctica.

**Criterio de finalización:** existe una matriz visual que permite contrastar las alternativas seleccionadas sin presentar un ranking general.

## Validación y pruebas finales

| # | Criterio | Estado |
|---|---|---|
| 1 | Se comparan al menos 2 alternativas y no más de 3. | ☐ |
| 2 | Cada alternativa tiene al menos una fuente pública identificable. | ☐ |
| 3 | Se utilizan los 5 criterios obligatorios. | ☐ |
| 4 | La comparación identifica ventajas y limitaciones sustentadas. | ☐ |
| 5 | Los vacíos de información están marcados como pendientes. | ☐ |
| 6 | Existe una matriz visual en una sola pantalla. | ☐ |
| 7 | No se declara una “mejor opción” universal. | ☐ |

## Solución de problemas

| Situación | Qué hacer |
|---|---|
| Copilot propone opciones sin fuentes oficiales. | Pide sustituirlas por alternativas con documentación pública verificable. |
| Las alternativas no son comparables. | Limita la búsqueda al mismo tipo de experiencia o transacción. |
| Copilot asigna puntuaciones sin explicar criterios. | Elimina la puntuación y pide descripciones breves basadas en evidencia. |
| No está disponible la generación de imágenes. | Utiliza la matriz visual en Markdown; cumple el objetivo de comparación visual. |

## Limpieza y conservación

- Conserva la conversación si deseas reutilizar la comparación durante la sesión.
- No es necesario descargar archivos ni capturas de pantalla.

## Resumen de la práctica

Identificaste alternativas de pago digital con fuentes públicas, estableciste criterios de comparación, contrastaste ventajas y limitaciones y convertiste el análisis en una matriz visual que evita una conclusión general sin contexto.
