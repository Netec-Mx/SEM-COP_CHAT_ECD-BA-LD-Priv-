# Práctica. Seguimiento de nuevas disposiciones y regulaciones del sector financiero

## Metadatos

| Duration | Complexity | Bloom level |
|---|---|---|
| 9 minutos | Media | Crear |

## Descripción General

En esta práctica construirá un registro inicial y verificable de vigilancia regulatoria para una organización financiera ficticia. Utilizará Microsoft Copilot para localizar posibles novedades regulatorias en España y la Unión Europea durante los últimos 90 días, pero validará manualmente las fuentes antes de registrarlas. El resultado será un libro de Excel con hallazgos trazables, candidatos descartados, la consulta utilizada y un resumen ejecutivo sujeto a revisión por las áreas de Cumplimiento y Legal.

## Objetivos de Aprendizaje

- [ ] Formular una consulta delimitada por jurisdicción, periodo, organismos emisores y temas regulatorios financieros.
- [ ] Usar Microsoft Copilot para identificar candidatos regulatorios y priorizar enlaces a fuentes oficiales primarias.
- [ ] Verificar manualmente al menos dos fuentes oficiales antes de considerar un hallazgo como validado.
- [ ] Crear un registro de seguimiento con fuente, fecha, disposición, estado, impacto preliminar y acción de revisión.
- [ ] Aplicar validación humana, distinguiendo información preliminar de asesoramiento legal, normativo o de cumplimiento.

## Prerrequisitos

El estudiante debe contar con:

- Conocimientos básicos de Microsoft Copilot, navegación web y formulación de prompts.
- Comprensión básica de los conceptos de fuente primaria, fecha de publicación, fecha de entrada en vigor y vigencia normativa.
- Capacidad para distinguir entre una disposición jurídica, una guía, una consulta pública, una nota de prensa y una comunicación institucional.
- Una cuenta personal activa de Microsoft. No utilice cuentas compartidas, genéricas ni información real de clientes.
- Acceso a Internet estable y a Microsoft Edge.
- Acceso a Excel para la Web mediante una cuenta Microsoft personal.
- Criterios de calidad de prompts o plantillas de verificación desarrolladas en módulos previos, si están disponibles.

> **Límite de responsabilidad:** esta práctica no permite interpretar jurídicamente normas, determinar obligaciones definitivas ni automatizar decisiones de cumplimiento. Copilot es una herramienta de apoyo a la investigación; sus resultados deben ser revisados por personal competente de Cumplimiento y Legal.

## Entorno de Laboratorio

### Hardware recomendado

| Componente | Especificación mínima |
|---|---|
| Equipo | Computadora portátil o de escritorio |
| Procesador | Intel Core i3 de 8.ª generación o equivalente; 2 núcleos a 2.0 GHz o superior |
| Memoria | 8 GB de RAM |
| Espacio disponible | 2 GB libres |
| Pantalla | 1366 × 768 píxeles; se recomienda 1920 × 1080 |
| Conexión | 10 Mbps de descarga y 2 Mbps de carga |

### Software y servicios

| Elemento | Versión o uso |
|---|---|
| Sistema operativo | Windows 11 Pro, 23H2 o 24H2 |
| Navegador | Microsoft Edge 128.0.2739.79 o versión disponible equivalente |
| IA generativa | Microsoft Copilot web |
| Hoja de cálculo | Excel para la Web |
| URL de acceso | `https://copilot.microsoft.com/` |

### Preparación del directorio de evidencias

Todos los archivos de evidencia deben almacenarse en el directorio obligatorio:

```powershell
New-Item -ItemType Directory -Force -Path C:\CopilotLabs\Batch1\
Set-Location C:\CopilotLabs\Batch1\
Get-ChildItem
```

Durante esta práctica se creará el archivo de evidencia:

```text
C:\CopilotLabs\Batch1\06_registro_seguimiento_regulatorio.xlsx
```

No elimine ni modifique los archivos obligatorios de prácticas anteriores:

```text
01_matriz_inclusion_financiera.md
02_comparacion_pagos_digitales.md
02_comparacion_pagos_digitales.png
03_mapa_perspectivas_servicios_financieros.md
04_respuesta_competencia.md
05_escenarios_financieros_el_salvador.md
```

## Instrucciones Paso a Paso

### Paso 1: Preparar el alcance y la ventana de revisión

**Objetivo:** Definir criterios claros para evitar búsquedas regulatorias ambiguas o resultados fuera del alcance establecido.

**Instructions:**

1. Abra Microsoft Edge.
2. Verifique que la fecha del equipo sea correcta.
3. Determine la fecha actual de ejecución y calcule la fecha inicial correspondiente a los últimos 90 días.
4. Registre ambas fechas en una nota temporal. Use el formato `DD/MM/AAAA`.
5. Utilice los siguientes criterios obligatorios de seguimiento:

   | Criterio | Alcance obligatorio |
   |---|---|
   | Jurisdicción principal | España y Unión Europea |
   | Periodo | Últimos 90 días hasta la fecha de ejecución |
   | Organismos prioritarios | Banco de España, CNMV, Banco Central Europeo, Autoridad Bancaria Europea y EUR-Lex |
   | Temas | Prevención de blanqueo de capitales, pagos, protección del consumidor, ciberresiliencia y gobierno de IA |
   | Tipo de fuente preferida | Fuente oficial primaria |
   | Resultado esperado | Candidatos regulatorios con enlaces, fechas y nivel de certeza |

6. Establezca estas reglas de exclusión:
   - No trate una noticia de prensa como una disposición jurídica si no enlaza al documento oficial.
   - No registre como validada una fuente que esté fuera del periodo de 90 días.
   - No convierta una consulta pública, una guía o una recomendación en una obligación definitiva sin revisar su naturaleza jurídica.
   - No incluya conclusiones jurídicas ni recomendaciones de cumplimiento definitivo.

**Expected output:**

Una ventana temporal definida y criterios concretos para la investigación regulatoria.

**Verification:**

Confirme que puede responder estas cuatro preguntas antes de continuar:

1. ¿Cuál es la fecha inicial exacta del periodo de 90 días?
2. ¿Cuál es la fecha de corte de la búsqueda?
3. ¿Qué organismos son prioritarios?
4. ¿Qué tipos de resultados deben descartarse o marcarse como pendientes de revisión?

---

### Paso 2: Formular una consulta verificable en Microsoft Copilot

**Objetivo:** Solicitar a Copilot resultados estructurados, limitados por periodo y sustentados en enlaces oficiales.

**Instructions:**

1. Abra `https://copilot.microsoft.com/`.
2. Inicie sesión con su cuenta Microsoft personal si se solicita.
3. Copie el siguiente prompt.
4. Sustituya los valores entre corchetes por las fechas calculadas en el paso anterior.
5. Envíe la consulta en Copilot.

```text
Actúa como asistente de investigación regulatoria, no como asesor legal ni de cumplimiento.

Identifica disposiciones, reglamentos, directrices, consultas regulatorias, comunicaciones supervisoras o novedades normativas potencialmente relevantes para una organización financiera ficticia.

Alcance obligatorio:
- Jurisdicción: España y Unión Europea.
- Periodo de publicación: desde [FECHA_INICIAL_90_DIAS] hasta [FECHA_DE_CORTE].
- Organismos prioritarios: Banco de España, CNMV, Banco Central Europeo, Autoridad Bancaria Europea (EBA) y EUR-Lex.
- Temas: prevención de blanqueo de capitales, pagos, protección del consumidor, ciberresiliencia y gobierno de IA.

Devuelve una tabla con un máximo de 8 resultados y estas columnas:
1. Organismo emisor.
2. Fecha de publicación.
3. Título exacto de la disposición o documento.
4. Tipo de documento.
5. Tema regulatorio.
6. Fecha de entrada en vigor, si está expresamente indicada.
7. Enlace oficial primario completo.
8. Nivel de certeza: alto, medio o bajo.
9. Razón de relevancia preliminar.
10. Elemento que requiere validación humana.

Reglas obligatorias:
- Prioriza enlaces oficiales de bde.es, cnmv.es, ecb.europa.eu, eba.europa.eu y eur-lex.europa.eu.
- No inventes fechas, títulos, enlaces ni fechas de entrada en vigor.
- Si un dato no está confirmado en una fuente oficial, escribe “pendiente de verificación”.
- Distingue claramente entre una norma vinculante, una guía, una consulta, una noticia y una comunicación institucional.
- Excluye o marca explícitamente resultados fuera del periodo indicado.
- No emitas asesoramiento legal, interpretación jurídica ni conclusiones de cumplimiento.
```

6. Revise la respuesta sin copiarla todavía a Excel.
7. Identifique resultados que aparenten ser candidatos útiles y resultados que tengan enlaces incompletos, dominios no oficiales o fechas ausentes.

**Expected output:**

Una tabla preliminar de Copilot con candidatos regulatorios, enlaces oficiales potenciales y advertencias de incertidumbre.

**Verification:**

La respuesta debe contener, como mínimo:

- Una fecha de publicación por candidato o la marca “pendiente de verificación”.
- Un organismo emisor identificable.
- Un enlace específico, no solo el nombre de un sitio web.
- Una distinción entre el tipo de documento y una norma vinculante.
- Algún nivel de certeza o indicación de incertidumbre.

Si Copilot no incluye enlaces oficiales o mezcla documentos fuera del periodo, no considere la respuesta suficiente; refine el prompt antes de continuar.

---

### Paso 3: Clasificar candidatos preliminares y seleccionar fuentes para revisión

**Objetivo:** Separar resultados potencialmente verificables de aquellos que deben descartarse o mantenerse como pendientes.

**Instructions:**

1. Revise cada fila sugerida por Copilot.
2. Clasifique mentalmente cada resultado con uno de estos estados preliminares:

   | Estado preliminar | Uso |
   |---|---|
   | Pendiente de verificación | Existe un posible enlace oficial, pero aún no se ha abierto y revisado. |
   | Candidato descartable | No posee fuente primaria, está fuera del periodo o no se relaciona con el alcance. |
   | Prioridad de validación | Tiene fuente oficial primaria aparente, fecha dentro del periodo y relación clara con un tema definido. |

3. Seleccione al menos dos candidatos con enlaces a fuentes oficiales primarias.
4. Priorice candidatos relacionados con dos temas diferentes cuando sea posible, por ejemplo:
   - Pagos y protección del consumidor.
   - Ciberresiliencia y gobierno de IA.
   - Prevención de blanqueo de capitales y supervisión.
5. No seleccione únicamente noticias de terceros, publicaciones de blogs, resúmenes comerciales o resultados sin fecha.
6. Si Copilot devuelve menos de dos enlaces oficiales aptos, solicite una corrección con este prompt:

```text
Refina la respuesta anterior. Muestra solo resultados publicados dentro del periodo indicado que tengan un enlace oficial primario verificable. Excluye medios de comunicación, blogs, resúmenes de terceros y enlaces sin fecha. Si no encuentras dos resultados verificables, indícalo de forma explícita en lugar de completar información no confirmada.
```

**Expected output:**

Dos o más candidatos prioritarios con enlaces oficiales listos para validación manual.

**Verification:**

Antes de abrir las fuentes, confirme que cada candidato seleccionado cumple preliminarmente con estos criterios:

- El dominio parece oficial.
- La fecha indicada podría estar dentro de la ventana de 90 días.
- El organismo emisor está dentro de los organismos prioritarios.
- El tema se relaciona con uno de los cinco temas definidos.
- El resultado no ha sido tratado erróneamente como obligación definitiva.

---

### Paso 4: Validar manualmente al menos dos fuentes oficiales

**Objetivo:** Confirmar que los hallazgos proceden de fuentes oficiales, se encuentran dentro del periodo y no han sido interpretados indebidamente por la IA.

**Instructions:**

1. Abra el primer enlace seleccionado en una nueva pestaña de Edge.
2. Compruebe manualmente los siguientes elementos en la página oficial:
   - Dominio del organismo emisor.
   - Título exacto del documento.
   - Fecha de publicación, actualización o adopción.
   - Tipo de documento.
   - Jurisdicción aplicable.
   - Fecha de entrada en vigor, si aparece de forma explícita.
   - Enlace al texto jurídico, documento, expediente o publicación oficial correspondiente.
3. Determine si la fecha relevante está dentro del periodo de 90 días.
4. Registre una de estas decisiones para el candidato:
   - **Validado:** la fuente es oficial, la fecha está dentro del periodo y el contenido corresponde al alcance.
   - **Pendiente de revisión:** la fuente es oficial, pero falta confirmar un dato crítico, como la entrada en vigor, el alcance o la naturaleza jurídica.
   - **Descartado:** no es una fuente primaria, está fuera del periodo o no corresponde a los temas definidos.
5. Repita el proceso con un segundo enlace oficial.
6. Anote la fecha y hora en la que realizó cada comprobación.
7. Si el enlace lleva a una nota de prensa, siga los vínculos hacia la disposición, consulta, reglamento, guía o publicación oficial original. Si no existe un documento primario identificable, no lo registre como validado.
8. No infiera la entrada en vigor a partir de una fecha de publicación. Registre “pendiente de verificación” cuando la fuente no la indique claramente.

**Expected output:**

Al menos dos fuentes oficiales abiertas y revisadas por una persona, con una decisión documentada para cada candidato.

**Verification:**

Para cada fuente que se marcará como **Validado**, debe poder demostrar:

| Comprobación | Resultado esperado |
|---|---|
| Fuente | URL oficial accesible |
| Organismo | Coincide con el emisor indicado |
| Fecha | Está dentro de la ventana de 90 días |
| Documento | Título y tipo identificables |
| Tema | Relación clara con el alcance |
| Vigencia | Fecha confirmada o “pendiente de verificación” |
| Trazabilidad | Fecha de comprobación registrada |

> **Control humano obligatorio:** una fuente oficial puede seguir requiriendo análisis jurídico. “Validado” en este laboratorio significa que el dato fue contrastado contra una fuente primaria, no que se haya determinado una obligación legal definitiva.

---

### Paso 5: Crear el registro de seguimiento en Excel para la Web

**Objetivo:** Transformar los hallazgos verificados en un registro trazable y reutilizable.

**Instructions:**

1. Abra Excel para la Web desde Edge.
2. Cree un libro en blanco.
3. Renombre la primera hoja como `Registro_validado`.
4. Cree las siguientes columnas en la fila 1:

| Columna | Encabezado |
|---|---|
| A | ID |
| B | Organismo emisor |
| C | Jurisdicción |
| D | Fecha de publicación |
| E | Disposición o documento |
| F | Tipo de documento |
| G | Tema regulatorio |
| H | URL oficial primaria |
| I | Fecha de entrada en vigor |
| J | Estado |
| K | Nivel de certeza |
| L | Impacto preliminar |
| M | Acción de revisión |
| N | Fecha de verificación humana |
| O | Responsable de revisión |
| P | Observaciones y límites |

5. Registre únicamente los hallazgos revisados manualmente en el paso anterior.
6. Use identificadores simples, por ejemplo: `REG-001` y `REG-002`.
7. Para la columna **Estado**, use uno de estos valores:
   - `Validado`
   - `Pendiente de revisión`
   - `Descartado`
8. Para la columna **Impacto preliminar**, describa un posible efecto operativo sin afirmar obligaciones definitivas. Ejemplos:
   - `Posible revisión de controles de pagos; requiere análisis de Cumplimiento.`
   - `Posible impacto en políticas de ciberresiliencia; confirmar alcance y fechas.`
   - `Posible cambio informativo para canales de atención al consumidor; validar aplicabilidad.`
9. Para la columna **Acción de revisión**, indique una acción concreta. Ejemplos:
   - `Enviar a Cumplimiento para evaluación de aplicabilidad.`
   - `Solicitar revisión jurídica de vigencia y obligaciones.`
   - `Contrastar con el texto oficial publicado en EUR-Lex.`
10. Cree una segunda hoja llamada `Candidatos_descartados`.
11. En esa hoja, registre al menos los candidatos no usados que hayan sido descartados o dejados pendientes, incluyendo una columna llamada `Motivo de descarte o pendiente`.
12. Cree una tercera hoja llamada `Consulta_utilizada`.
13. Pegue en esa hoja el prompt final utilizado, la fecha de ejecución y la ventana temporal aplicada.
14. Guarde el libro en Excel para la Web.
15. Descargue una copia del libro y guárdela con el nombre obligatorio:

```text
06_registro_seguimiento_regulatorio.xlsx
```

16. Si el navegador descarga el archivo en `Descargas`, muévalo al directorio de evidencias:

```powershell
Move-Item "$env:USERPROFILE\Downloads\06_registro_seguimiento_regulatorio.xlsx" `
  -Destination "C:\CopilotLabs\Batch1\06_registro_seguimiento_regulatorio.xlsx" -Force
```

**Expected output:**

El archivo `C:\CopilotLabs\Batch1\06_registro_seguimiento_regulatorio.xlsx` con las hojas `Registro_validado`, `Candidatos_descartados` y `Consulta_utilizada`.

**Verification:**

Abra el archivo descargado y confirme que:

- Existen al menos dos filas de hallazgos revisados manualmente.
- Cada fila posee fuente, fecha, disposición, estado, impacto preliminar y acción de revisión.
- Las URL apuntan a fuentes oficiales primarias.
- Las fechas de publicación corresponden al periodo definido o el registro está marcado como descartado.
- No hay afirmaciones de obligación legal definitiva sin revisión de Cumplimiento y Legal.

---

### Paso 6: Generar y registrar un resumen ejecutivo con advertencias

**Objetivo:** Comunicar los resultados de manera breve, sin ocultar incertidumbres ni reemplazar la revisión especializada.

**Instructions:**

1. Copie desde Excel los datos principales de los registros validados:
   - Organismo emisor.
   - Título del documento.
   - Fecha de publicación.
   - Tema.
   - Estado.
   - Impacto preliminar.
   - Acción de revisión.
2. Regrese a Microsoft Copilot.
3. Use el siguiente prompt y reemplace el bloque entre corchetes por los datos validados:

```text
Redacta un resumen ejecutivo en español de máximo cinco líneas a partir de los siguientes hallazgos regulatorios previamente verificados contra fuentes oficiales:

[PEGAR_HALLAZGOS_VALIDADOS]

Requisitos:
- Menciona solo hechos incluidos en los datos proporcionados.
- Distingue entre hallazgos validados y elementos pendientes.
- Incluye una advertencia explícita de que Cumplimiento y Legal deben revisar aplicabilidad, vigencia y obligaciones.
- No emitas asesoramiento legal ni afirmes obligaciones definitivas.
- Mantén un tono profesional y apto para seguimiento interno.
```

4. Revise que la respuesta tenga un máximo de cinco líneas.
5. Elimine cualquier afirmación que no esté respaldada por las filas verificadas en Excel.
6. Cree una cuarta hoja en el libro de Excel llamada `Resumen_ejecutivo`.
7. Pegue el resumen final, la fecha de elaboración y esta leyenda obligatoria:

```text
Uso interno preliminar. No constituye asesoramiento legal, interpretación normativa ni decisión de cumplimiento. Requiere revisión de las áreas de Cumplimiento y Legal.
```

8. Guarde nuevamente el libro y descargue la versión final al mismo archivo de evidencia.

**Expected output:**

Un resumen ejecutivo de máximo cinco líneas, registrado en la hoja `Resumen_ejecutivo`, con advertencia de revisión humana.

**Verification:**

Compruebe que el resumen:

- No supera cinco líneas.
- No presenta una sugerencia de Copilot como hecho no verificado.
- Indica que existen elementos pendientes o sujetos a revisión.
- Incluye la participación requerida de Cumplimiento y Legal.
- Está almacenado en el archivo de Excel dentro de `C:\CopilotLabs\Batch1\`.

---

### Paso 7: Realizar la revisión final de trazabilidad

**Objetivo:** Confirmar que el artefacto puede ser revisado posteriormente por otra persona sin depender de la memoria del estudiante o de la respuesta de Copilot.

**Instructions:**

1. Abra la hoja `Registro_validado`.
2. Revise cada fila utilizando esta lista de control:

   | Elemento | Criterio de aceptación |
   |---|---|
   | Fuente | URL oficial primaria completa y accesible |
   | Fecha | Fecha de publicación registrada |
   | Disposición | Título exacto o suficientemente identificable |
   | Estado | Validado, Pendiente de revisión o Descartado |
   | Impacto | Descrito como preliminar, no definitivo |
   | Acción | Acción concreta para Cumplimiento, Legal o el equipo responsable |
   | Verificación humana | Fecha de comprobación registrada |
   | Límites | Incertidumbres y datos no confirmados documentados |

3. Confirme que la hoja `Consulta_utilizada` contiene el prompt y el periodo aplicado.
4. Confirme que la hoja `Candidatos_descartados` explica por qué no se incluyeron ciertos resultados.
5. Confirme que la hoja `Resumen_ejecutivo` incluye la advertencia obligatoria.
6. Guarde el archivo por última vez.
7. Verifique la existencia del archivo mediante PowerShell:

```powershell
Get-Item C:\CopilotLabs\Batch1\06_registro_seguimiento_regulatorio.xlsx |
Select-Object FullName, Length, LastWriteTime
```

**Expected output:**

Un libro de Excel completo, trazable y listo para revisión interna preliminar.

**Verification:**

La práctica se considera completada si se cumplen todos los criterios siguientes:

- Se utilizó una consulta con jurisdicción, periodo, organismos y temas explícitos.
- Se revisaron manualmente al menos dos fuentes oficiales.
- Se descartaron o marcaron los resultados que no tenían fuente primaria o estaban fuera del periodo.
- El registro contiene los campos mínimos solicitados.
- El resumen tiene un máximo de cinco líneas y advierte sobre revisión por Cumplimiento y Legal.
- El archivo final se encuentra en `C:\CopilotLabs\Batch1\06_registro_seguimiento_regulatorio.xlsx`.

## Validación y Pruebas

Realice las siguientes pruebas finales sobre el archivo descargado:

| Prueba | Procedimiento | Resultado esperado |
|---|---|---|
| Existencia del archivo | Ejecute `Get-Item` sobre el archivo de evidencia. | El archivo existe en el directorio obligatorio. |
| Integridad de hojas | Abra el libro y revise las hojas creadas. | Existen `Registro_validado`, `Candidatos_descartados`, `Consulta_utilizada` y `Resumen_ejecutivo`. |
| Trazabilidad mínima | Revise las columnas del registro. | Cada fila contiene fuente, fecha, disposición, estado, impacto preliminar y acción de revisión. |
| Validación de fuentes | Abra dos URL registradas. | Las URL pertenecen a organismos oficiales y coinciden con los datos registrados. |
| Control temporal | Compare fechas con la ventana de 90 días. | Las filas validadas están dentro del periodo o están justificadamente marcadas como pendientes o descartadas. |
| Control de responsabilidad | Lea el resumen y las observaciones. | No hay asesoramiento legal ni conclusiones definitivas de cumplimiento. |
| Revisión humana | Revise la columna de verificación. | Cada hallazgo validado tiene fecha de comprobación humana y acción posterior definida. |

Criterio de calidad recomendado para el registro:

- **Alto:** fuente primaria oficial, fecha y tipo de documento confirmados, relación clara con el tema, acción de revisión definida.
- **Medio:** fuente oficial confirmada, pero entrada en vigor, aplicabilidad o alcance requiere revisión adicional.
- **Bajo:** fuente incompleta, resultado indirecto o dato no confirmado; no debe tratarse como hallazgo validado.

## Solución de Problemas

**Problema 1: Copilot muestra resultados sin enlaces oficiales, fuera del periodo o con fechas contradictorias.**

- **Síntomas:** la respuesta contiene artículos de prensa, blogs, enlaces genéricos, documentos sin fecha o resultados publicados antes de la ventana de 90 días.
- **Causa probable:** la consulta es demasiado amplia, Copilot priorizó contenido secundario o interpretó una fecha de actualización como fecha de publicación.
- **Solución:** reenvíe la consulta de refinamiento del Paso 3, exija dominios oficiales y solicite que marque “pendiente de verificación” cuando falte evidencia. Abra siempre la fuente primaria y registre como descartado cualquier resultado que no pueda verificarse manualmente.

**Problema 2: El libro de Excel se descarga en una ubicación distinta o no contiene los cambios recientes.**

- **Síntomas:** el archivo no aparece en `C:\CopilotLabs\Batch1\`, se encuentra en `Descargas` o la versión descargada no incluye la hoja de resumen.
- **Causa probable:** Excel para la Web guardó cambios en OneDrive, el navegador descargó una copia anterior o la descarga no terminó antes de cerrar la pestaña.
- **Solución:** espere a que Excel confirme el guardado, descargue nuevamente el libro, cierre cualquier copia local abierta y mueva la versión más reciente al directorio obligatorio con el comando indicado en el Paso 5. Verifique la fecha de modificación con `Get-Item`.

## Limpieza

1. Confirme que el archivo final permanece en:

   ```text
   C:\CopilotLabs\Batch1\06_registro_seguimiento_regulatorio.xlsx
   ```

2. No elimine el archivo de evidencia ni los artefactos obligatorios de prácticas anteriores.
3. Cierre las pestañas de Copilot, Excel y las fuentes regulatorias después de verificar que el archivo se guardó.
4. Cierre sesión de la cuenta Microsoft si el equipo es compartido o de uso público.
5. No conserve en el libro datos personales, credenciales, información de clientes ni contenido interno sensible.
6. Elimine únicamente descargas duplicadas fuera de `C:\CopilotLabs\Batch1\` cuando haya confirmado que la copia final es correcta.

## Resumen

En esta práctica utilizó Microsoft Copilot como apoyo para localizar posibles novedades regulatorias en España y la Unión Europea, delimitando organismos, temas y una ventana de 90 días. Contrastó manualmente al menos dos fuentes oficiales, registró hallazgos trazables en Excel y documentó candidatos descartados. El resultado es un artefacto preliminar de vigilancia regulatoria que requiere revisión posterior por las áreas de Cumplimiento y Legal antes de utilizarse para decisiones normativas u operativas.
