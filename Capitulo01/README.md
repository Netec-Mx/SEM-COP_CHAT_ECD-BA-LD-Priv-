# Práctica. Exploración de oportunidades de inclusión financiera

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 12 minutos |
| Complejidad | Media |
| Nivel de Bloom | Aplicar |

## Descripción General

En este laboratorio utilizará Microsoft Copilot para explorar oportunidades de inclusión financiera digital en El Salvador. Formulará una consulta estructurada, evaluará críticamente la respuesta generada y documentará una matriz verificable de segmentos, barreras, soluciones, beneficios, riesgos y datos pendientes de validación. Finalmente, seleccionará dos oportunidades prioritarias que servirán como insumo obligatorio para laboratorios posteriores de comparación visual y análisis de servicios financieros digitales.

## Objetivos de Aprendizaje

- [ ] Formular un prompt con contexto, audiencia, restricciones y formato de salida para explorar oportunidades de inclusión financiera.
- [ ] Identificar barreras de acceso, segmentos potencialmente excluidos, beneficios esperados y riesgos asociados con servicios financieros digitales.
- [ ] Distinguir entre hechos verificables, hipótesis, recomendaciones y datos que requieren validación externa.
- [ ] Crear una matriz estructurada y reutilizable sobre oportunidades de inclusión financiera en El Salvador.
- [ ] Seleccionar y justificar dos oportunidades prioritarias para análisis posteriores.

## Prerrequisitos

**Conocimientos requeridos**

- Conocimientos básicos sobre inteligencia artificial generativa y formulación de prompts.
- Comprensión básica del concepto de inclusión financiera.
- Capacidad para distinguir una afirmación verificable de una hipótesis o recomendación.
- Conocimiento básico de edición de archivos Markdown.

**Acceso requerido**

- Cuenta personal de Microsoft iniciada en Microsoft Edge.
- Acceso a Microsoft Copilot mediante `https://copilot.microsoft.com/`.
- No utilice cuentas compartidas, credenciales genéricas ni datos reales de clientes.
- No ingrese información personal, financiera, confidencial o regulada en Copilot.

## Entorno de Laboratorio

| Componente | Especificación de referencia |
|---|---|
| Sistema operativo | Windows 11 Pro 23H2 o Windows 11 24H2 |
| Navegador | Microsoft Edge 128.0.2739.79 |
| Herramienta de IA | Microsoft Copilot, experiencia web 2024.10 |
| Editor | Visual Studio Code 1.93.1 o editor de texto equivalente |
| Memoria | 8 GB de RAM |
| Conectividad | Mínimo 10 Mbps de descarga y 2 Mbps de carga |
| Resolución recomendada | 1920 x 1080 píxeles |
| Directorio obligatorio | `C:\CopilotLabs\Batch1\` |

Abra **Windows PowerShell** y ejecute el siguiente comando para crear y acceder al directorio de trabajo obligatorio:

```powershell
New-Item -ItemType Directory -Path "C:\CopilotLabs\Batch1" -Force
Set-Location "C:\CopilotLabs\Batch1"
```

Verifique el directorio actual:

```powershell
Get-Location
```

La salida debe mostrar:

```text
Path
----
C:\CopilotLabs\Batch1
```

> **Importante:** Todos los archivos de evidencia de esta secuencia deben almacenarse en `C:\CopilotLabs\Batch1\`. En este laboratorio se creará el archivo obligatorio `01_matriz_inclusion_financiera.md`. El registro de prompts se incluirá dentro de ese mismo archivo para no crear archivos de evidencia adicionales.

## Instrucciones Paso a Paso

### Paso 1: Preparar el directorio y el archivo de evidencia

**Objetivo:** Crear el archivo Markdown obligatorio donde se documentarán el prompt, la respuesta analizada, la matriz y las oportunidades priorizadas.

**Instrucciones:**

1. Abra **Windows PowerShell**.
2. Confirme que está trabajando en el directorio obligatorio:

   ```powershell
   Set-Location "C:\CopilotLabs\Batch1"
   ```

3. Cree el archivo de evidencia vacío:

   ```powershell
   New-Item -ItemType File -Path "01_matriz_inclusion_financiera.md" -Force
   ```

4. Abra el archivo en Visual Studio Code:

   ```powershell
   code "C:\CopilotLabs\Batch1\01_matriz_inclusion_financiera.md"
   ```

5. Agregue la siguiente estructura inicial al archivo y guárdela con `Ctrl+S`:

   ```markdown
   ### Matriz de inclusión financiera digital en El Salvador

   **Fecha de elaboración:** [AAAA-MM-DD]  
   **Herramienta utilizada:** Microsoft Copilot, experiencia web  
   **Contexto geográfico:** El Salvador  
   **Propósito:** Identificar oportunidades iniciales de inclusión financiera digital que requieren validación humana y consulta de fuentes oficiales.

   ### Registro de prompts

   | N.° | Propósito | Prompt utilizado | Fecha |
   |---|---|---|---|
   | 1 | Exploración inicial | Pendiente | [AAAA-MM-DD] |
   | 2 | Generación de matriz | Pendiente | [AAAA-MM-DD] |

   ### Matriz de oportunidades

   Pendiente de completar.

   ### Oportunidades prioritarias

   Pendiente de completar.

   ### Validación humana y límites

   Pendiente de completar.
   ```

6. Reemplace `[AAAA-MM-DD]` por la fecha actual.
7. Mantenga este archivo abierto durante el resto del laboratorio.

**Resultado esperado:**

Existe el archivo:

```text
C:\CopilotLabs\Batch1\01_matriz_inclusion_financiera.md
```

El archivo contiene las secciones para el registro de prompts, la matriz, las oportunidades prioritarias y la validación humana.

**Verificación:**

En PowerShell, ejecute:

```powershell
Get-Item "C:\CopilotLabs\Batch1\01_matriz_inclusion_financiera.md" | Select-Object Name, Length, LastWriteTime
```

Confirme que el nombre del archivo es exactamente:

```text
01_matriz_inclusion_financiera.md
```

---

### Paso 2: Formular una consulta estructurada en Microsoft Copilot

**Objetivo:** Obtener una exploración inicial de oportunidades de inclusión financiera digital sin asumir que la respuesta constituye evidencia definitiva.

**Instrucciones:**

1. Abra Microsoft Edge.
2. Navegue a:

   ```text
   https://copilot.microsoft.com/
   ```

3. Inicie sesión con su **cuenta personal de Microsoft**, si se solicita.
4. Verifique que la conversación se realizará en español.
5. Copie y pegue el siguiente prompt en Copilot:

   ```text
   Actúa como analista inicial de inclusión financiera digital. Analiza oportunidades potenciales en El Salvador para una institución financiera que desea mejorar el acceso responsable a servicios financieros digitales.

   Considera específicamente estos segmentos:
   1. Población rural.
   2. Microemprendedores y trabajadores por cuenta propia.
   3. Personas con baja alfabetización digital.
   4. Adultos mayores.
   5. Personas sin historial crediticio formal.

   Para cada segmento, identifica:
   - Una o dos barreras de acceso financiero o digital.
   - Una posible solución o servicio financiero digital.
   - El beneficio esperado para el segmento.
   - Riesgos de implementación, protección al consumidor, fraude, exclusión o privacidad.
   - Datos, normas, estadísticas o fuentes que deben validarse antes de tomar una decisión comercial.

   Restricciones:
   - Contexto geográfico: El Salvador.
   - No inventes estadísticas, leyes, instituciones ni porcentajes.
   - Si no puedes confirmar un dato, indícalo como hipótesis o dato pendiente de validación.
   - Distingue claramente entre hecho verificable, hipótesis y recomendación.
   - No proporciones asesoría legal ni financiera individual.

   Formato de salida:
   Presenta primero un resumen de máximo 150 palabras y después una tabla Markdown con las columnas:
   Segmento | Barrera | Posible solución digital | Beneficio esperado | Riesgo | Tipo de afirmación | Dato o fuente que debe validarse.
   ```

6. Espere la respuesta de Copilot.
7. Revise si Copilot:
   - Menciona explícitamente a El Salvador.
   - Incluye los cinco segmentos solicitados.
   - Diferencia datos, hipótesis y recomendaciones.
   - Evita presentar afirmaciones no verificadas como hechos.
8. Copie el prompt utilizado en la sección **Registro de prompts** del archivo Markdown, en la fila 1. Puede resumir el texto del prompt si es demasiado extenso, siempre que conserve sus componentes esenciales: contexto, segmentos, restricciones y formato de salida.
9. Registre la fecha de ejecución.

**Resultado esperado:**

Copilot genera una primera exploración de oportunidades y riesgos relacionados con inclusión financiera digital en El Salvador. La respuesta debe tratarse como un insumo de análisis, no como una fuente oficial ni una decisión comercial final.

**Verificación:**

En el archivo `01_matriz_inclusion_financiera.md`, confirme que la primera fila del registro incluye:

- El propósito: `Exploración inicial`.
- La fecha actual.
- Una descripción o copia del prompt utilizado.
- La referencia a El Salvador y a los segmentos analizados.

---

### Paso 3: Solicitar una matriz estructurada y verificable

**Objetivo:** Convertir la exploración inicial en una matriz que separe oportunidades, riesgos y elementos pendientes de validación.

**Instrucciones:**

1. En la misma conversación de Copilot, envíe el siguiente prompt de seguimiento:

   ```text
   Con base en tu respuesta anterior, crea una matriz consolidada para El Salvador.

   Reglas de calidad:
   - Incluye los cinco segmentos analizados.
   - No presentes como hechos las inferencias o recomendaciones.
   - En la columna "Tipo de afirmación", utiliza solamente: Hecho verificable potencial, Hipótesis o Recomendación.
   - En la columna "Dato o fuente que debe validarse", indica una fuente institucional o categoría de evidencia apropiada, por ejemplo: Banco Central de Reserva de El Salvador, Superintendencia del Sistema Financiero, normativa aplicable, encuesta nacional, datos de conectividad, estudios de usuarios o documentación del proveedor.
   - Si propones un producto financiero, señala al menos un riesgo de fraude, privacidad, exclusión, accesibilidad o protección al consumidor.
   - No inventes números, requisitos regulatorios ni nombres de programas.

   Entrega únicamente una tabla Markdown con estas columnas:
   Segmento | Barrera | Posible solución digital | Beneficio esperado | Riesgo | Tipo de afirmación | Dato o fuente que debe validarse.
   ```

2. Revise la tabla devuelta por Copilot.
3. No copie automáticamente toda la salida sin revisar. Antes de transferirla a su archivo, evalúe cada fila:
   - ¿La barrera es plausible para el segmento?
   - ¿La solución responde a la barrera identificada?
   - ¿El beneficio es razonable y no está garantizado?
   - ¿El riesgo es específico?
   - ¿La fuente de validación es oficial, institucional o metodológicamente apropiada?
4. Copie la tabla revisada en la sección **Matriz de oportunidades** del archivo Markdown.
5. Si Copilot no incluye una fuente adecuada, complete la última columna con una categoría válida de verificación, como:
   - `Estadísticas oficiales de acceso a internet y cobertura territorial.`
   - `Normativa y comunicados de la Superintendencia del Sistema Financiero.`
   - `Documentación pública del Banco Central de Reserva de El Salvador.`
   - `Pruebas de usabilidad con el segmento objetivo.`
   - `Políticas internas de prevención de fraude y protección de datos.`
6. Actualice la fila 2 de **Registro de prompts** con el propósito `Generación de matriz`, la fecha y el prompt usado.
7. Guarde el archivo.

**Resultado esperado:**

La sección **Matriz de oportunidades** contiene una tabla Markdown con al menos cinco filas, una por cada segmento requerido.

**Verificación:**

La matriz debe incluir las siguientes columnas, en este orden:

```text
Segmento | Barrera | Posible solución digital | Beneficio esperado | Riesgo | Tipo de afirmación | Dato o fuente que debe validarse
```

Además, debe incluir al menos una fila para cada uno de estos segmentos:

- Población rural.
- Microemprendedores y trabajadores por cuenta propia.
- Personas con baja alfabetización digital.
- Adultos mayores.
- Personas sin historial crediticio formal.

---

### Paso 4: Evaluar críticamente la respuesta generada

**Objetivo:** Aplicar validación humana para diferenciar hechos, hipótesis y recomendaciones antes de priorizar oportunidades.

**Instrucciones:**

1. Debajo de la matriz, agregue una subsección con el siguiente formato:

   ```markdown
   #### Revisión crítica de la respuesta de Copilot

   | Elemento revisado | Clasificación | Evaluación humana | Acción requerida |
   |---|---|---|---|
   | [Afirmación o propuesta 1] | Hecho verificable potencial / Hipótesis / Recomendación | [Por qué requiere confirmación o por qué es útil] | [Fuente o actividad de validación] |
   | [Afirmación o propuesta 2] | Hecho verificable potencial / Hipótesis / Recomendación | [Por qué requiere confirmación o por qué es útil] | [Fuente o actividad de validación] |
   | [Afirmación o propuesta 3] | Hecho verificable potencial / Hipótesis / Recomendación | [Por qué requiere confirmación o por qué es útil] | [Fuente o actividad de validación] |
   ```

2. Seleccione al menos tres afirmaciones de la matriz o de la respuesta de Copilot.
3. Clasifique cada afirmación usando uno de estos criterios:

   | Clasificación | Uso correcto |
   |---|---|
   | Hecho verificable potencial | Afirmación que puede contrastarse con una fuente oficial, informe institucional, normativa vigente o estudio documentado. |
   | Hipótesis | Posibilidad plausible que necesita investigación, pruebas con usuarios o evidencia contextual antes de aceptarse. |
   | Recomendación | Propuesta de acción o diseño que requiere evaluación de viabilidad, riesgos, costos y cumplimiento. |

4. Para cada elemento, indique una acción concreta de validación. Por ejemplo:
   - Revisar publicaciones del Banco Central de Reserva de El Salvador.
   - Consultar normativa o comunicados de la Superintendencia del Sistema Financiero.
   - Revisar estadísticas oficiales de conectividad y cobertura.
   - Realizar entrevistas o pruebas de usabilidad con usuarios representativos.
   - Solicitar revisión de cumplimiento, seguridad, fraude y protección al consumidor.
5. Agregue el siguiente texto adaptándolo a sus hallazgos:

   ```markdown
   La respuesta de Copilot se utilizó como una herramienta de ideación y estructuración inicial. No se consideró evidencia suficiente para confirmar condiciones regulatorias, cifras de mercado, necesidades de usuarios ni viabilidad comercial. Toda afirmación con impacto legal, financiero, operativo o de protección al consumidor requiere validación con fuentes oficiales y revisión humana competente.
   ```

6. Guarde el archivo.

**Resultado esperado:**

El archivo contiene una revisión crítica que demuestra que el estudiante no acepta automáticamente el contenido generado por IA.

**Verificación:**

Confirme que existen al menos tres filas en la tabla de revisión crítica y que cada una contiene:

- Una clasificación.
- Una evaluación humana.
- Una acción de validación concreta.
- Una referencia a una fuente, actividad de investigación o revisión responsable.

---

### Paso 5: Seleccionar dos oportunidades prioritarias

**Objetivo:** Priorizar dos oportunidades de inclusión financiera digital con una justificación basada en barrera, beneficio, riesgo y necesidad de validación.

**Instrucciones:**

1. Revise todas las filas de la matriz.
2. Seleccione dos oportunidades que considere prioritarias para análisis posterior.
3. Use los siguientes criterios de priorización:
   - Relevancia de la barrera para el segmento.
   - Potencial de ampliar acceso o uso responsable de servicios financieros.
   - Claridad del beneficio esperado.
   - Riesgos identificables y mitigables.
   - Posibilidad de validar supuestos con fuentes oficiales o investigación de usuarios.
4. Reemplace el contenido de la sección **Oportunidades prioritarias** por una tabla como la siguiente:

   ```markdown
   | Prioridad | Segmento | Oportunidad seleccionada | Justificación | Riesgos principales | Validación requerida antes de avanzar |
   |---|---|---|---|---|---|
   | 1 | [Segmento] | [Solución u oportunidad] | [Relación entre barrera, beneficio y relevancia] | [Riesgos específicos] | [Fuente oficial, revisión interna o investigación requerida] |
   | 2 | [Segmento] | [Solución u oportunidad] | [Relación entre barrera, beneficio y relevancia] | [Riesgos específicos] | [Fuente oficial, revisión interna o investigación requerida] |
   ```

5. Después de la tabla, agregue una breve justificación de entre 80 y 120 palabras que responda:
   - ¿Por qué estas dos oportunidades son más relevantes que las demás?
   - ¿Qué suposición importante todavía debe comprobarse?
   - ¿Qué riesgo no debe minimizarse?
   - ¿Qué evidencia adicional sería necesaria antes de tomar una decisión comercial?
6. Evite afirmar que una oportunidad será exitosa, rentable, legalmente permitida o adecuada para todos los usuarios sin evidencia.
7. Guarde el archivo.

**Resultado esperado:**

El documento presenta dos oportunidades priorizadas con justificación, riesgos y requisitos de validación claramente documentados.

**Verificación:**

Compruebe que la tabla de oportunidades prioritarias contiene exactamente dos filas de prioridad:

```text
1
2
```

Cada fila debe incluir un segmento, una oportunidad, una justificación, al menos un riesgo y una actividad o fuente de validación.

---

### Paso 6: Revisar y finalizar la evidencia del laboratorio

**Objetivo:** Comprobar que el archivo es completo, reutilizable y apto para servir como entrada del siguiente laboratorio.

**Instrucciones:**

1. Revise el archivo completo en Visual Studio Code.
2. Confirme que la estructura del documento contiene:
   - Título de la matriz.
   - Fecha, herramienta y contexto geográfico.
   - Registro de dos prompts.
   - Matriz con los cinco segmentos.
   - Revisión crítica de al menos tres afirmaciones.
   - Dos oportunidades prioritarias.
   - Declaración de límites y validación humana.
3. Revise que no haya:
   - Datos personales o reales de clientes.
   - Contraseñas, correos privados o números de cuenta.
   - Estadísticas sin fuente o marcadas como hechos sin validación.
   - Recomendaciones presentadas como obligaciones legales.
4. Guarde el archivo con `Ctrl+S`.
5. En PowerShell, valide que el archivo existe y contiene contenido:

   ```powershell
   Get-Content "C:\CopilotLabs\Batch1\01_matriz_inclusion_financiera.md" | Measure-Object -Line -Word -Character
   ```

6. Opcionalmente, abra el archivo desde el Explorador de archivos o use la vista previa Markdown de Visual Studio Code para comprobar la legibilidad de las tablas.

**Resultado esperado:**

El archivo final está guardado en el directorio obligatorio y contiene una matriz estructurada que podrá reutilizarse en el Laboratorio 2.

**Verificación:**

Ejecute:

```powershell
Test-Path "C:\CopilotLabs\Batch1\01_matriz_inclusion_financiera.md"
```

La salida debe ser:

```text
True
```

## Validación y Pruebas

Realice las siguientes comprobaciones antes de dar por finalizado el laboratorio.

| Prueba | Procedimiento | Resultado esperado |
|---|---|---|
| Existencia del archivo | Ejecute `Test-Path "C:\CopilotLabs\Batch1\01_matriz_inclusion_financiera.md"` | El resultado es `True`. |
| Ubicación correcta | Ejecute `Get-Item "C:\CopilotLabs\Batch1\01_matriz_inclusion_financiera.md"` | El archivo está ubicado en `C:\CopilotLabs\Batch1\`. |
| Registro de prompts | Revise la sección **Registro de prompts**. | Existen dos registros: exploración inicial y generación de matriz. |
| Cobertura de segmentos | Revise la matriz. | Aparecen población rural, microemprendedores, personas con baja alfabetización digital, adultos mayores y personas sin historial crediticio formal. |
| Estructura de la matriz | Revise los encabezados de la tabla. | Incluye segmento, barrera, solución, beneficio, riesgo, tipo de afirmación y fuente pendiente de validación. |
| Validación humana | Revise la sección de revisión crítica. | Existen al menos tres elementos clasificados como hecho verificable potencial, hipótesis o recomendación. |
| Priorización | Revise la sección **Oportunidades prioritarias**. | Hay exactamente dos oportunidades justificadas. |
| Uso responsable | Revise el contenido completo. | No hay datos reales de clientes, asesoría individual, afirmaciones legales concluyentes ni cifras inventadas. |

Use esta lista de comprobación final:

- [ ] El archivo se llama exactamente `01_matriz_inclusion_financiera.md`.
- [ ] El archivo está guardado en `C:\CopilotLabs\Batch1\`.
- [ ] El contexto de análisis corresponde a El Salvador.
- [ ] Se utilizaron los cinco segmentos requeridos.
- [ ] La matriz diferencia hechos verificables potenciales, hipótesis y recomendaciones.
- [ ] Las fuentes o datos pendientes de validación están identificados.
- [ ] Las dos oportunidades prioritarias incluyen riesgos y acciones de revisión.
- [ ] Se documentó que la salida de Copilot no sustituye la validación humana, normativa ni legal.

## Solución de Problemas

### Problema 1: Copilot presenta estadísticas, leyes o requisitos regulatorios sin una fuente verificable

**Síntomas:** La respuesta incluye porcentajes, fechas regulatorias, obligaciones legales o nombres de programas, pero no muestra una fuente oficial clara. También puede expresar información incierta como si fuera un hecho confirmado.

**Causa probable:** Los modelos generativos pueden producir información plausible pero incompleta, desactualizada o no verificable. Una respuesta de IA no sustituye documentos oficiales ni asesoría profesional.

**Solución:**

1. No copie la afirmación como hecho confirmado.
2. Clasifíquela como `Hecho verificable potencial` o `Hipótesis`, según corresponda.
3. En la columna de validación, indique una fuente apropiada, como normativa vigente, publicaciones del Banco Central de Reserva de El Salvador o comunicados de la Superintendencia del Sistema Financiero.
4. Reformule la fila para eliminar cifras o condiciones no confirmadas.
5. Registre en la revisión crítica que el elemento requiere contraste externo antes de una decisión comercial, técnica o regulatoria.

### Problema 2: La matriz de Copilot omite segmentos, riesgos o el formato solicitado

**Síntomas:** La tabla no incluye los cinco segmentos requeridos, mezcla varias barreras en una sola celda, no identifica riesgos o no diferencia hipótesis de recomendaciones.

**Causa probable:** El modelo pudo priorizar un resumen narrativo, interpretar parcialmente las instrucciones o perder restricciones en una respuesta extensa.

**Solución:**

1. Envíe una solicitud de corrección en la misma conversación:

   ```text
   Corrige la matriz anterior. Debe incluir exactamente una fila para cada uno de estos segmentos: población rural, microemprendedores y trabajadores por cuenta propia, personas con baja alfabetización digital, adultos mayores y personas sin historial crediticio formal. Mantén las siete columnas solicitadas, agrega un riesgo específico por fila y usa únicamente las categorías Hecho verificable potencial, Hipótesis o Recomendación.
   ```

2. Revise nuevamente la respuesta antes de copiarla.
3. Si persiste una omisión, complete manualmente la matriz usando una formulación prudente y marque los elementos como hipótesis o pendientes de validación.
4. No elimine la revisión crítica: la corrección de formato no reemplaza la validación humana.

## Limpieza

1. Guarde el archivo final:

   ```text
   C:\CopilotLabs\Batch1\01_matriz_inclusion_financiera.md
   ```

2. Cierre la conversación de Copilot o elimine mensajes que contengan información transitoria, siempre que no se requieran como evidencia institucional.
3. Cierre las pestañas del navegador que no necesite.
4. Cierre Visual Studio Code después de confirmar que el archivo fue guardado.
5. **No elimine** el archivo `01_matriz_inclusion_financiera.md`, ya que será un insumo obligatorio para el siguiente laboratorio.
6. No cree archivos de evidencia fuera de `C:\CopilotLabs\Batch1\`.

## Resumen

En este laboratorio creó una matriz de oportunidades de inclusión financiera digital para El Salvador utilizando Microsoft Copilot como herramienta de exploración inicial. Documentó prompts, identificó segmentos potencialmente excluidos, registró barreras, soluciones, beneficios y riesgos, y separó afirmaciones verificables potenciales de hipótesis y recomendaciones. También seleccionó dos oportunidades prioritarias con criterios de validación humana, protección al consumidor y uso responsable de IA.

El archivo generado para conservar y reutilizar en la siguiente actividad es:

```text
C:\CopilotLabs\Batch1\01_matriz_inclusion_financiera.md
```

Como siguiente paso, utilice las dos oportunidades priorizadas para construir una comparación visual de pagos o servicios financieros digitales, manteniendo la distinción entre evidencia verificable, supuestos y recomendaciones.
