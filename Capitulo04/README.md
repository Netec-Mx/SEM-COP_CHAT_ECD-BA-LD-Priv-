# Práctica. ¿Qué responder cuando un cliente afirma que la competencia tiene una mejor opción?

## Metadatos

| Elemento | Valor |
|---|---|
| Duración | 17 minutos |
| Complejidad | Media |
| Nivel de Bloom | Crear |

## Descripción General

En este laboratorio elaborará una respuesta comercial responsable para el caso de un cliente que afirma que la competencia ofrece una mejor opción de pago digital. Usará Microsoft Copilot para generar un borrador, alternativas para perfiles distintos y una matriz de comparación basada en necesidades verificables. Finalmente, aplicará una revisión humana para eliminar promesas, comparaciones no comprobadas, recomendaciones personalizadas o afirmaciones que puedan tener implicaciones financieras, legales o regulatorias.

## Objetivos de Aprendizaje

- [ ] Crear una respuesta comercial empática que reconozca la inquietud de un cliente sin desacreditar a la competencia.
- [ ] Formular preguntas de clarificación sobre costos, disponibilidad, facilidad de uso, seguridad, soporte, accesibilidad, aceptación en comercios y condiciones de uso.
- [ ] Diseñar una matriz de comparación responsable basada en evidencia y criterios relevantes para el cliente.
- [ ] Adaptar una respuesta para un microcomerciante, un usuario rural y una persona con baja experiencia digital.
- [ ] Aplicar validación humana para retirar afirmaciones absolutas, no verificables o interpretables como asesoría financiera personalizada.

## Prerrequisitos

**Conocimientos requeridos**

- Haber completado el Laboratorio 03-00-01.
- Comprender los conceptos de comunicación empática, comparación responsable y gestión de objeciones.
- Reconocer que Microsoft Copilot puede generar contenido útil, pero no sustituye asesoría financiera, legal, regulatoria ni de cumplimiento.
- Distinguir entre hechos verificables, opiniones comerciales, supuestos y recomendaciones que requieren revisión humana.

**Archivos y acceso requeridos**

- El archivo `C:\CopilotLabs\Batch1\03_mapa_perspectivas_servicios_financieros.md` debe estar disponible.
- Una cuenta personal de Microsoft activa; no utilice cuentas compartidas, genéricas ni datos reales de clientes.
- Acceso a Internet y a Microsoft Copilot en `https://copilot.microsoft.com/`.
- Permisos para crear y guardar archivos en `C:\CopilotLabs\Batch1\`.

## Entorno de Laboratorio

| Categoría | Requisito |
|---|---|
| Sistema operativo | Windows 11 Pro, 23H2 o 24H2 |
| Navegador | Microsoft Edge 128.0.2739.79 o versión equivalente disponible |
| Herramienta de IA | Microsoft Copilot, experiencia web |
| Editor de texto | Visual Studio Code 1.93.1 o equivalente |
| Directorio de trabajo obligatorio | `C:\CopilotLabs\Batch1\` |
| Archivo de entrada | `03_mapa_perspectivas_servicios_financieros.md` |
| Archivo de evidencia de este laboratorio | `04_respuesta_competencia.md` |
| Contexto geográfico | El Salvador |
| Datos permitidos | Escenarios ficticios y datos públicos verificables |
| Datos prohibidos | Información real de clientes, credenciales, números de cuenta, documentos de identidad o datos financieros sensibles |

Abra Windows Terminal o Símbolo del sistema y ejecute los siguientes comandos para validar la carpeta de trabajo y el archivo de entrada:

```powershell
New-Item -ItemType Directory -Force -Path C:\CopilotLabs\Batch1 | Out-Null
Set-Location C:\CopilotLabs\Batch1
Get-ChildItem
Test-Path .\03_mapa_perspectivas_servicios_financieros.md
```

El último comando debe devolver:

```text
True
```

> **Uso responsable:** no solicite a Copilot que determine cuál producto financiero debe contratar una persona real. El objetivo es crear un guion de conversación y una matriz de evaluación. Toda afirmación sobre tarifas, cobertura, funcionalidades, seguridad, regulación o condiciones debe verificarse en fuentes oficiales vigentes antes de comunicarse como hecho.

## Instrucciones Paso a Paso

### Paso 1: Revisar el mapa de perspectivas del laboratorio anterior

**Objetivo:** Identificar las perspectivas, tensiones y riesgos que deben orientar la respuesta comercial responsable.

**Instrucciones:**

1. Abra Visual Studio Code.
2. Seleccione **File > Open Folder** y abra la carpeta:

   ```text
   C:\CopilotLabs\Batch1\
   ```

3. Abra el archivo:

   ```text
   03_mapa_perspectivas_servicios_financieros.md
   ```

4. Lea el documento e identifique, como mínimo, tres elementos que deban considerarse al responder a un cliente que compara opciones de pago digital. Busque perspectivas o tensiones relacionadas con:
   - Costos y comisiones.
   - Conectividad, disponibilidad y cobertura territorial.
   - Facilidad de uso y alfabetización digital.
   - Seguridad, fraude, privacidad o recuperación de acceso.
   - Atención al cliente y resolución de incidentes.
   - Aceptación en comercios.
   - Inclusión financiera y accesibilidad.
   - Condiciones, límites o restricciones de uso.

5. En una nota temporal, registre tres hallazgos con el siguiente formato:

   ```text
   - Perspectiva o tensión:
   - Posible necesidad del cliente:
   - Riesgo de hacer una afirmación no verificada:
   ```

6. No copie información personal ni use nombres de empresas si su mapa previo incluyó ejemplos no confirmados. Trabaje con criterios generales o con fuentes oficiales verificables.

**Resultado esperado:**

Debe contar con al menos tres hallazgos que orienten el lenguaje de su respuesta. Por ejemplo:

```text
- Perspectiva o tensión: El costo visible puede diferir del costo total por transacción, retiro o inactividad.
- Posible necesidad del cliente: Conocer los costos aplicables a su volumen y tipo de cobro.
- Riesgo de hacer una afirmación no verificada: Afirmar que una opción es "más barata" sin revisar tarifas y condiciones vigentes.
```

**Verificación:**

Confirme que sus hallazgos incluyen al menos una necesidad del cliente y un riesgo de comunicación. Si solo contienen opiniones como “la seguridad es importante”, reformúlelos para indicar qué se necesita verificar y por qué.

---

### Paso 2: Preparar una consulta responsable para Microsoft Copilot

**Objetivo:** Solicitar a Copilot un borrador estructurado que priorice empatía, preguntas de clarificación y verificación, sin producir publicidad engañosa ni recomendaciones personalizadas.

**Instrucciones:**

1. Abra Microsoft Edge y navegue a:

   ```text
   https://copilot.microsoft.com/
   ```

2. Inicie sesión con su cuenta personal de Microsoft si es necesario.
3. Verifique que el idioma de interacción sea español.
4. Copie los tres hallazgos identificados en el Paso 1.
5. Pegue el siguiente prompt en Copilot. Sustituya el contenido entre corchetes por sus hallazgos reales:

   ```text
   Actúa como asistente de redacción para una conversación comercial responsable en El Salvador. No eres asesor financiero, legal, regulatorio ni de cumplimiento.

   Escenario ficticio:
   Un cliente dice: “La competencia tiene una opción de pago digital mejor que la de ustedes”.

   Hallazgos del mapa de perspectivas previo:
   1. [Hallazgo 1]
   2. [Hallazgo 2]
   3. [Hallazgo 3]

   Redacta un borrador en español con estas secciones:
   1. Una respuesta inicial empática de 70 a 110 palabras.
   2. Ocho preguntas de clarificación, una para cada criterio: costos, disponibilidad, facilidad de uso, seguridad, soporte, accesibilidad, aceptación en comercios y condiciones de uso.
   3. Una matriz de comparación con las columnas: criterio, qué necesita aclarar el cliente, evidencia o fuente que debe revisarse, estado de verificación y acción siguiente.
   4. Una frase de cierre que invite a revisar información oficial vigente.

   Reglas obligatorias:
   - No desacredites a competidores ni afirmes que una opción es mejor, más barata, más segura o más accesible sin evidencia verificable.
   - No inventes tarifas, coberturas, regulación, tasas, funcionalidades ni condiciones.
   - No recomiendes un producto financiero a una persona concreta.
   - Usa lenguaje condicional cuando falte evidencia: “conviene verificar”, “podemos revisar”, “según la información oficial vigente”.
   - Distingue claramente entre preguntas, hechos por verificar y próximos pasos.
   ```

6. Revise la respuesta generada antes de copiarla. No la considere automáticamente correcta por haber sido producida por Copilot.
7. Si Copilot presenta afirmaciones específicas sobre proveedores, tarifas, regulación o cobertura sin citar una fuente oficial vigente, elimínelas o solicite una nueva versión con esta instrucción:

   ```text
   Reescribe el contenido eliminando cualquier dato específico no respaldado por una fuente oficial vigente. Mantén solamente criterios de evaluación, preguntas de clarificación y acciones de verificación.
   ```

**Resultado esperado:**

Debe obtener un borrador que contenga:

- Un reconocimiento respetuoso de la preocupación del cliente.
- Ocho preguntas, una por criterio requerido.
- Una matriz de comparación enfocada en evidencia.
- Lenguaje que evite concluir cuál alternativa es objetivamente superior.

**Verificación:**

Revise que el borrador no contenga expresiones como las siguientes, salvo que estén respaldadas por una fuente oficial revisada y fechada:

```text
“Siempre es más barato”
“Es la opción más segura”
“La competencia cobra más”
“Funciona en todo El Salvador”
“Le conviene cambiarse”
“Garantizamos que nunca tendrá problemas”
```

---

### Paso 3: Generar alternativas para perfiles de clientes

**Objetivo:** Crear variaciones del guion que respondan a necesidades distintas sin convertir la respuesta en una recomendación financiera personalizada.

**Instrucciones:**

1. En la misma conversación de Copilot, envíe el siguiente prompt:

   ```text
   A partir del borrador anterior, crea tres versiones breves de respuesta comercial responsable. Cada versión debe tener entre 55 y 85 palabras, incluir una frase empática, dos preguntas de clarificación y una acción de verificación.

   Perfiles ficticios:
   A. Microcomerciante que recibe pagos frecuentes y necesita controlar costos y aceptación en comercios.
   B. Usuario rural cuya conectividad puede ser intermitente y que necesita conocer canales de soporte y disponibilidad.
   C. Persona con baja experiencia digital que prioriza facilidad de uso, seguridad y ayuda para resolver dudas.

   Reglas:
   - No asumas ingresos, ubicación exacta, nivel educativo ni datos personales.
   - No recomiendes una entidad, aplicación o producto específico.
   - No afirmes características de ningún proveedor sin fuente oficial vigente.
   - No uses promesas de seguridad, disponibilidad, ahorro o aceptación.
   - Termina cada versión con una invitación a revisar condiciones y canales oficiales.
   ```

2. Revise si las respuestas cambian las preguntas según el perfil:
   - Para el microcomerciante, deben destacar costos totales, frecuencia de uso, tiempos de disponibilidad de fondos o aceptación, sin afirmar resultados.
   - Para el usuario rural, deben priorizar conectividad, canales alternos, disponibilidad y soporte.
   - Para la persona con baja experiencia digital, deben priorizar comprensión, recuperación de acceso, prevención de fraude y ayuda disponible.

3. Si una versión incluye sesgos o supuestos, por ejemplo “las personas rurales no saben usar tecnología” o “usted necesita una opción sencilla”, corrija la instrucción con el siguiente prompt:

   ```text
   Reescribe las tres versiones evitando estereotipos y supuestos sobre capacidad, ingresos, educación, ubicación o comportamiento. Formula las necesidades como preguntas abiertas y opciones de verificación.
   ```

4. Conserve únicamente las alternativas que cumplan las reglas de comunicación responsable.

**Resultado esperado:**

Debe tener tres respuestas diferenciadas por contexto de uso, pero consistentes en estos principios:

- Escuchar antes de concluir.
- Comparar criterios relevantes.
- Revisar evidencia oficial.
- Evitar declaraciones absolutas.
- No prescribir una decisión financiera.

**Verificación:**

Compruebe que cada versión contenga:

1. Una expresión empática.
2. Dos preguntas relevantes para el perfil.
3. Una acción concreta de verificación.
4. Ninguna promesa o comparación no demostrada.

---

### Paso 4: Construir la matriz de comparación responsable

**Objetivo:** Convertir el borrador generado en una matriz utilizable durante una conversación comercial y en revisiones posteriores.

**Instrucciones:**

1. Cree un archivo nuevo en Visual Studio Code.
2. Guárdelo con el nombre obligatorio:

   ```text
   C:\CopilotLabs\Batch1\04_respuesta_competencia.md
   ```

3. Copie la siguiente estructura al archivo:

   ```markdown
   # Respuesta responsable ante comparación con la competencia

   **Contexto:** Escenario ficticio en El Salvador. Un cliente afirma que un competidor ofrece una opción de pago digital mejor.

   **Propósito:** Guiar una conversación empática y basada en criterios verificables. Este documento no constituye asesoría financiera, legal, regulatoria ni de cumplimiento.

   ## Principios de comunicación responsable

   - Reconocer la inquietud sin desacreditar a la competencia.
   - Preguntar antes de concluir qué opción es adecuada.
   - Diferenciar información confirmada, información pendiente de verificar y opinión.
   - Consultar fuentes oficiales vigentes antes de comunicar características, tarifas, cobertura o condiciones como hechos.
   - Evitar recomendaciones financieras personalizadas y promesas de resultados.

   ## Respuesta inicial

   [Pegue y edite aquí su respuesta inicial validada.]

   ## Preguntas de clarificación

   | Criterio | Pregunta de clarificación |
   |---|---|
   | Costos | |
   | Disponibilidad | |
   | Facilidad de uso | |
   | Seguridad | |
   | Soporte | |
   | Accesibilidad | |
   | Aceptación en comercios | |
   | Condiciones de uso | |

   ## Matriz de comparación responsable

   | Criterio | Qué necesita aclarar el cliente | Evidencia o fuente por revisar | Estado de verificación | Acción siguiente |
   |---|---|---|---|---|
   | Costos | | Tarifario, contrato o página oficial vigente | Pendiente | |
   | Disponibilidad | | Condiciones oficiales, cobertura publicada y canales habilitados | Pendiente | |
   | Facilidad de uso | | Guías oficiales, demostración o prueba permitida | Pendiente | |
   | Seguridad | | Medidas oficiales de protección, proceso de recuperación y canales antifraude | Pendiente | |
   | Soporte | | Horarios, canales, tiempos publicados y procedimiento de reclamos | Pendiente | |
   | Accesibilidad | | Opciones de idioma, asistencia, requisitos técnicos y canales alternos | Pendiente | |
   | Aceptación en comercios | | Información oficial, red aplicable y verificación con comercios relevantes | Pendiente | |
   | Condiciones de uso | | Términos, límites, requisitos, restricciones y fecha de vigencia | Pendiente | |

   ## Alternativas según perfil

   ### Perfil A: Microcomerciante

   [Pegue y edite la versión validada.]

   ### Perfil B: Usuario rural

   [Pegue y edite la versión validada.]

   ### Perfil C: Persona con baja experiencia digital

   [Pegue y edite la versión validada.]

   ## Revisión humana y límites

   - [ ] No se afirma que una opción es mejor sin criterios y evidencia.
   - [ ] No se citan tarifas, cobertura, regulación o funcionalidades sin verificar una fuente oficial vigente.
   - [ ] No se desacredita a un competidor.
   - [ ] No se solicitan ni incluyen datos personales o financieros reales.
   - [ ] No se formula una recomendación financiera personalizada.
   - [ ] Se indica qué información debe verificarse y cuál es la fuente esperada.
   - [ ] La respuesta utiliza lenguaje claro, respetuoso y no absoluto.

   ## Fuentes por confirmar antes de uso externo

   | Fuente esperada | Propósito de la revisión | Fecha de consulta | Resultado |
   |---|---|---|---|
   | Sitio web oficial del proveedor correspondiente | Tarifas, funcionalidades, condiciones y vigencia | Pendiente | Pendiente |
   | Términos y condiciones oficiales | Límites, restricciones, requisitos y responsabilidades | Pendiente | Pendiente |
   | Canales oficiales de atención | Horarios, soporte, reclamos y recuperación de acceso | Pendiente | Pendiente |
   | Autoridad competente, cuando corresponda | Información regulatoria o de protección al usuario | Pendiente | Pendiente |
   ```

4. Complete la respuesta inicial con el contenido generado por Copilot que haya revisado y corregido.
5. Complete las ocho preguntas de clarificación con preguntas abiertas. Use un tono conversacional, respetuoso y neutral.
6. Complete cada fila de la matriz. En las columnas de evidencia y estado, indique claramente qué debe verificarse; no rellene datos que no haya confirmado.
7. Pegue las tres respuestas por perfil, editadas según su revisión.

**Resultado esperado:**

El archivo `04_respuesta_competencia.md` debe contener una respuesta inicial, ocho preguntas, una matriz de ocho criterios, tres alternativas por perfil y una lista de controles de revisión humana.

**Verificación:**

Use la vista previa de Markdown de Visual Studio Code con **Ctrl+Shift+V**. Compruebe que:

- Las tablas se visualizan correctamente.
- Hay exactamente ocho filas de criterios en cada tabla principal.
- Los perfiles A, B y C están presentes.
- Las secciones de revisión humana y fuentes por confirmar no están vacías.

---

### Paso 5: Aplicar la revisión humana de afirmaciones y riesgos

**Objetivo:** Validar el documento antes de considerarlo apto como evidencia y antes de cualquier uso comercial externo.

**Instrucciones:**

1. Lea el archivo completo desde la perspectiva de un cliente que podría interpretar una afirmación como promesa, garantía o recomendación.
2. Busque manualmente palabras o expresiones de riesgo, tales como:

   ```text
   mejor
   peor
   más barato
   más seguro
   garantizado
   siempre
   nunca
   conviene
   recomendado
   disponible en todo
   sin costo
   inmediato
   ```

3. En Visual Studio Code, use **Ctrl+F** para buscar las expresiones anteriores una por una.
4. Por cada coincidencia, aplique una de estas decisiones:
   - Eliminarla si no aporta información verificable.
   - Convertirla en una pregunta de clarificación.
   - Convertirla en una acción de verificación.
   - Mantenerla únicamente si está contextualizada, documentada y cuenta con una fuente oficial vigente registrada.

5. Revise especialmente las palabras “seguridad” y “disponibilidad”. Deben referirse a prácticas, información oficial o preguntas del cliente; no deben prometer ausencia de fraude, fallas o interrupciones.
6. Compruebe que la matriz trate a la competencia con neutralidad. El objetivo es comparar criterios, no ganar una discusión ni afirmar superioridad.
7. Añada al final de la sección **Revisión humana y límites** una nota breve de revisión, usando este formato:

   ```markdown
   **Nota de revisión:** Documento revisado por una persona. Las afirmaciones específicas sobre proveedores, tarifas, cobertura, condiciones y regulación permanecen pendientes de confirmación mediante fuentes oficiales vigentes antes de cualquier comunicación externa.
   ```

8. Guarde el archivo con **Ctrl+S**.

**Resultado esperado:**

El documento debe usar lenguaje prudente y verificable. Debe quedar claro que la matriz organiza una conversación y un proceso de revisión, no una recomendación definitiva.

**Verificación:**

La respuesta inicial debe poder leerse sin detectar ninguno de los siguientes problemas:

| Problema | Resultado esperado |
|---|---|
| Desacreditación de competencia | No aparece |
| Promesa de ahorro, seguridad o disponibilidad | No aparece |
| Recomendación personalizada | No aparece |
| Datos no verificados presentados como hechos | No aparece |
| Preguntas abiertas sobre necesidades | Aparecen |
| Referencia a fuentes oficiales vigentes | Aparece |
| Acción siguiente de verificación | Aparece |

---

### Paso 6: Guardar la evidencia y realizar la comprobación final

**Objetivo:** Confirmar que el archivo obligatorio existe, tiene contenido y se encuentra en el directorio requerido.

**Instrucciones:**

1. Cierre cualquier archivo temporal que no forme parte de la evidencia final.
2. Abra Windows Terminal o PowerShell.
3. Ejecute los siguientes comandos:

   ```powershell
   Set-Location C:\CopilotLabs\Batch1
   Test-Path .\04_respuesta_competencia.md
   Get-Item .\04_respuesta_competencia.md | Select-Object Name, Length, LastWriteTime
   Get-Content .\04_respuesta_competencia.md -TotalCount 25
   ```

4. Confirme que `Test-Path` devuelve `True`.
5. Confirme que el tamaño del archivo es mayor que 0 bytes.
6. Revise las primeras líneas para comprobar que el archivo comienza con el título de la respuesta responsable.
7. Mantenga el archivo en la ruta obligatoria. No lo guarde en Descargas, Escritorio, OneDrive personal u otra carpeta.

**Resultado esperado:**

Debe existir el archivo:

```text
C:\CopilotLabs\Batch1\04_respuesta_competencia.md
```

**Verificación:**

La salida debe incluir un resultado similar al siguiente:

```text
True

Name                          Length LastWriteTime
----                          ------ -------------
04_respuesta_competencia.md     ...  ...

## Respuesta responsable ante comparación con la competencia
```

## Validación y Pruebas

Realice la siguiente validación final sobre `C:\CopilotLabs\Batch1\04_respuesta_competencia.md`.

| Prueba | Método | Criterio de aprobación |
|---|---|---|
| Archivo obligatorio | Ejecutar `Test-Path .\04_respuesta_competencia.md` | Devuelve `True`. |
| Ubicación correcta | Revisar la ruta en Visual Studio Code o PowerShell | El archivo está en `C:\CopilotLabs\Batch1\`. |
| Escenario identificado | Revisar la sección de contexto | Indica que se trata de un escenario ficticio de pago digital en El Salvador. |
| Respuesta empática | Leer la sección “Respuesta inicial” | Reconoce la inquietud sin rechazarla ni desacreditar a la competencia. |
| Criterios completos | Revisar “Preguntas de clarificación” | Incluye costos, disponibilidad, facilidad de uso, seguridad, soporte, accesibilidad, aceptación en comercios y condiciones de uso. |
| Matriz completa | Contar filas de “Matriz de comparación responsable” | Contiene ocho criterios y las cinco columnas requeridas. |
| Adaptación por perfiles | Revisar “Alternativas según perfil” | Incluye una alternativa para microcomerciante, usuario rural y persona con baja experiencia digital. |
| Neutralidad competitiva | Buscar términos absolutos y leer el documento | No afirma superioridad o inferioridad sin evidencia verificable. |
| Uso responsable | Revisar “Revisión humana y límites” | Incluye lista de controles y nota de revisión humana. |
| Trazabilidad | Revisar “Fuentes por confirmar antes de uso externo” | Incluye fuentes oficiales esperadas, propósito, fecha y resultado pendientes o documentados. |

Puede ejecutar esta comprobación adicional para localizar frases que requieren revisión:

```powershell
Select-String -Path .\04_respuesta_competencia.md -Pattern "siempre|nunca|garant|más barato|más seguro|mejor opción|le conviene|sin costo|inmediato" -CaseSensitive:$false
```

Si el comando devuelve coincidencias, revíselas en contexto. Una coincidencia no implica automáticamente un error si forma parte de una advertencia, una pregunta o una regla de prohibición; sin embargo, no debe aparecer como una afirmación comercial no sustentada.

## Solución de Problemas

### Problema 1: Copilot inventa tarifas, funcionalidades o afirmaciones sobre un competidor

**Síntomas:** La respuesta incluye montos, porcentajes, cobertura territorial, características de seguridad o supuestas condiciones de una entidad sin una fuente oficial verificable.

**Causa:** Copilot genera texto probabilístico y puede completar información plausible sin conocer la vigencia, aplicabilidad o fuente exacta de una afirmación.

**Solución:**

1. No copie el dato al archivo final como hecho.
2. Elimine el dato o reemplácelo por una pregunta de clarificación.
3. Registre la fuente que debería revisarse, por ejemplo: tarifario oficial, términos y condiciones, sitio oficial o canal de atención.
4. Solicite una reescritura a Copilot usando esta instrucción:

   ```text
   Elimina todos los datos específicos no respaldados por una fuente oficial vigente. Convierte las afirmaciones sobre tarifas, cobertura, seguridad y condiciones en elementos por verificar dentro de una matriz.
   ```

5. Mantenga el estado como `Pendiente` hasta que una persona revise una fuente oficial vigente.

### Problema 2: El archivo de evidencia no aparece en la carpeta obligatoria

**Síntomas:** PowerShell devuelve `False` al ejecutar `Test-Path .\04_respuesta_competencia.md`, o el archivo aparece en Escritorio, Descargas u otra carpeta.

**Causa:** El archivo se guardó desde Visual Studio Code en una carpeta distinta o se abrió una ventana de editor con otro directorio de trabajo.

**Solución:**

1. En Visual Studio Code, use **File > Save As**.
2. Navegue explícitamente a:

   ```text
   C:\CopilotLabs\Batch1\
   ```

3. Guarde el archivo con el nombre exacto:

   ```text
   04_respuesta_competencia.md
   ```

4. En PowerShell, ejecute:

   ```powershell
   Set-Location C:\CopilotLabs\Batch1
   Get-ChildItem -Filter 04_respuesta_competencia.md
   ```

5. Si existen copias en otra ubicación, conserve como evidencia únicamente la versión final guardada en el directorio obligatorio.

## Limpieza

1. Guarde y cierre `04_respuesta_competencia.md`.
2. Cierre las pestañas de Copilot que contengan borradores o consultas del escenario ficticio, especialmente si incluyen texto que no fue validado.
3. No elimine el archivo de evidencia ni el archivo de entrada:

   ```text
   C:\CopilotLabs\Batch1\03_mapa_perspectivas_servicios_financieros.md
   C:\CopilotLabs\Batch1\04_respuesta_competencia.md
   ```

4. No elimine ni modifique los demás archivos obligatorios del batch.
5. Cierre sesión de Microsoft Copilot si trabaja en un equipo compartido, sin guardar credenciales en el navegador.

## Resumen

En este laboratorio creó el archivo `04_respuesta_competencia.md` con una respuesta comercial empática, preguntas de clarificación, una matriz de comparación responsable y alternativas para tres perfiles ficticios. El documento evita desacreditar a competidores, no presenta afirmaciones no verificadas como hechos y mantiene acciones explícitas de verificación mediante fuentes oficiales vigentes.

El contenido generado servirá como base narrativa para los escenarios visuales del siguiente laboratorio. Antes de utilizar cualquier parte del guion en una interacción externa, una persona responsable debe confirmar tarifas, condiciones, cobertura, medidas de seguridad, regulación aplicable y demás información cambiante en fuentes oficiales correspondientes.
