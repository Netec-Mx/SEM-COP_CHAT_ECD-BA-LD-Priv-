# Práctica. Comparación visual de experiencias de pagos digitales

## Metadatos

| Duration | Complexity | Bloom level |
|---|---|---|
| 15 minutos | Media | Crear |

## Descripción General

En esta práctica transformarás dos oportunidades de inclusión financiera priorizadas en el Laboratorio 01-00-01 en criterios observables para comparar experiencias de pago digital. Utilizarás Microsoft Copilot para proponer un storyboard, una tabla comparativa y, si la función está disponible, un concepto visual que contraste una experiencia inclusiva con otra que presenta barreras de acceso. Finalmente, aplicarás una revisión humana para identificar sesgos, lenguaje excluyente, afirmaciones no verificadas y elementos que no correspondan al contexto de El Salvador.

## Objetivos de Aprendizaje

- [ ] Convertir dos oportunidades priorizadas de inclusión financiera en criterios comparables para experiencias de pago digital.
- [ ] Diseñar un prompt visual que incluya perfiles de usuario, canal, contexto, accesibilidad y momentos de fricción.
- [ ] Generar una propuesta visual o storyboard con Microsoft Copilot y documentar sus resultados.
- [ ] Revisar críticamente la representación generada para detectar sesgos, exclusión o afirmaciones no verificadas.
- [ ] Crear los archivos de evidencia `02_comparacion_pagos_digitales.md` y `02_comparacion_pagos_digitales.png`.

## Prerrequisitos

Antes de iniciar, confirma lo siguiente:

- Haber completado el Laboratorio 01-00-01.
- Disponer del archivo `C:\CopilotLabs\Batch1\01_matriz_inclusion_financiera.md`.
- Haber identificado dos oportunidades priorizadas de inclusión financiera. Ejemplos: facilitar pagos de servicios para personas con conectividad limitada, mejorar la accesibilidad de aplicaciones de pago para personas mayores, reducir errores en pagos digitales o aumentar la claridad de comisiones.
- Conocer criterios básicos de accesibilidad digital:
  - lenguaje claro y comprensible;
  - contraste suficiente;
  - tipografía legible;
  - instrucciones visibles;
  - no depender únicamente del color;
  - alternativas para personas con baja alfabetización digital, discapacidad visual, motricidad limitada o conectividad intermitente.
- Tener una cuenta Microsoft personal activa para iniciar sesión en Microsoft Copilot.
- No usar cuentas compartidas, información real de clientes, números de tarjetas, datos bancarios, documentos de identidad ni credenciales personales en los prompts.

## Entorno de Laboratorio

| Componente | Configuración esperada |
|---|---|
| Sistema operativo | Windows 11 |
| Navegador | Microsoft Edge 128.0.2739.79 o versión disponible equivalente |
| Herramienta principal | Microsoft Copilot, experiencia web |
| URL de acceso | `https://copilot.microsoft.com/` |
| Editor de texto | Visual Studio Code, Bloc de notas u otro editor Markdown |
| Directorio obligatorio | `C:\CopilotLabs\Batch1\` |
| Idioma de interacción | Español |
| Contexto geográfico | El Salvador |

La evidencia de este laboratorio debe almacenarse exclusivamente en:

```powershell
C:\CopilotLabs\Batch1\
```

Abre PowerShell y verifica la carpeta de trabajo:

```powershell
New-Item -ItemType Directory -Force -Path "C:\CopilotLabs\Batch1" | Out-Null
Set-Location "C:\CopilotLabs\Batch1"
Get-ChildItem
```

Confirma que esté disponible el archivo de entrada:

```powershell
Test-Path "C:\CopilotLabs\Batch1\01_matriz_inclusion_financiera.md"
```

El resultado esperado es:

```text
True
```

Los archivos requeridos para esta práctica son:

```text
C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.md
C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.png
```

> **Uso responsable:** Copilot puede producir contenido plausible pero incorrecto, estereotipos visuales o detalles que no representan la realidad salvadoreña. El resultado visual es un concepto de diseño para discusión; no constituye evidencia de que un servicio, una regulación, una institución o una población se comporte de la forma mostrada.

## Instrucciones Paso a Paso

### Paso 1: Revisar las oportunidades priorizadas y la matriz previa

**Objetivo:** Recuperar del laboratorio anterior dos oportunidades de inclusión financiera y convertirlas en una base de comparación verificable.

**Instructions:**

1. Abre el archivo anterior en Visual Studio Code o en un editor de texto:

   ```powershell
   code "C:\CopilotLabs\Batch1\01_matriz_inclusion_financiera.md"
   ```

   Si el comando `code` no está disponible, abre el archivo desde el Explorador de archivos.

2. Lee la matriz e identifica las dos oportunidades que usarás en esta práctica. Selecciona oportunidades que se puedan representar como una experiencia de pago digital.

3. Registra para cada oportunidad:
   - necesidad o problema detectado;
   - población o perfil de usuario asociado;
   - canal de pago relevante;
   - posible barrera de acceso;
   - posible medida de inclusión o accesibilidad.

4. Define dos perfiles comparables. No uses nombres reales ni información de personas reales. Puedes utilizar perfiles ficticios, por ejemplo:
   - **Perfil A:** persona adulta que paga un servicio básico desde un teléfono móvil, tiene conectividad variable y prefiere instrucciones claras.
   - **Perfil B:** persona usuaria de una aplicación de pago con acceso estable, pero que enfrenta un flujo con demasiados pasos, términos técnicos o validaciones poco claras.

5. Asegúrate de que ambos perfiles enfrenten la misma tarea principal: por ejemplo, pagar un servicio básico, recargar saldo, enviar un pago pequeño o consultar el estado de una transacción.

6. Decide el contraste central de la comparación:
   - **Experiencia inclusiva:** pocos pasos, lenguaje claro, confirmación visible, opciones de accesibilidad, manejo de conectividad limitada y ayuda contextual.
   - **Experiencia con barreras:** pasos excesivos, iconos ambiguos, dependencia de conectividad constante, lenguaje técnico, errores sin orientación o confirmación poco clara.

**Expected output:**

Debes contar con dos oportunidades y dos perfiles ficticios comparables, vinculados a una misma tarea de pago digital en El Salvador.

**Verification:**

Verifica que puedas responder estas preguntas antes de continuar:

- ¿Las dos experiencias comparan la misma tarea principal?
- ¿Los perfiles están basados en necesidades y no en estereotipos?
- ¿La experiencia inclusiva contiene medidas concretas de accesibilidad?
- ¿La experiencia con barreras describe problemas de diseño y no “deficiencias” de la persona usuaria?
- ¿Evitaste datos personales, datos bancarios y nombres reales?

---

### Paso 2: Definir criterios de comparación de la experiencia de pago

**Objetivo:** Crear criterios claros que permitan contrastar ambas experiencias sin depender únicamente de impresiones visuales.

**Instructions:**

1. Crea un borrador del archivo de evidencia:

   ```powershell
   New-Item -ItemType File -Force -Path "C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.md"
   code "C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.md"
   ```

2. Copia la siguiente estructura inicial en el archivo. Sustituye los textos entre corchetes por tus decisiones:

   ```markdown
   ## Comparación visual de experiencias de pagos digitales

   **Contexto:** El Salvador  
   **Tarea comparable:** [Ejemplo: pago de servicio básico desde teléfono móvil]  
   **Oportunidad priorizada 1:** [describir]  
   **Oportunidad priorizada 2:** [describir]  

   ### Perfiles ficticios

   | Elemento | Perfil A | Perfil B |
   |---|---|---|
   | Tipo de usuario | [describir sin estereotipos] | [describir sin estereotipos] |
   | Necesidad principal | [describir] | [describir] |
   | Canal | [aplicación móvil, web móvil u otro] | [mismo canal o canal comparable] |
   | Condición de acceso | [conectividad, dispositivo, idioma, apoyo] | [conectividad, dispositivo, idioma, apoyo] |
   | Tarea | [misma tarea] | [misma tarea] |

   ### Criterios de comparación

   | Criterio | Experiencia inclusiva | Experiencia con barreras |
   |---|---|---|
   | Claridad del propósito | [describir] | [describir] |
   | Número y claridad de pasos | [describir] | [describir] |
   | Lenguaje y comprensión | [describir] | [describir] |
   | Accesibilidad visual | [describir] | [describir] |
   | Manejo de conectividad limitada | [describir] | [describir] |
   | Confirmación del pago | [describir] | [describir] |
   | Prevención y recuperación de errores | [describir] | [describir] |
   | Ayuda o soporte contextual | [describir] | [describir] |
   | Riesgo de exclusión | [describir] | [describir] |
   ```

3. Completa la tabla con criterios específicos. Evita descripciones vagas como “es buena” o “es mala”. Describe elementos observables, por ejemplo:
   - “Muestra el monto, destinatario y comisión antes de confirmar”.
   - “Permite revisar y corregir un dato sin reiniciar todo el flujo”.
   - “Presenta un mensaje de error que explica qué ocurrió y cuál es el siguiente paso”.
   - “Requiere conexión continua sin explicar qué sucede si la señal se interrumpe”.
   - “Usa texto pequeño y botones identificados solo por color”.

4. Incluye al menos un criterio de accesibilidad y uno de conectividad o continuidad operativa.

5. Trata la comparación como un escenario hipotético de diseño. No atribuyas características a bancos, billeteras, empresas o instituciones reales si no cuentas con una fuente oficial verificable.

**Expected output:**

El archivo Markdown contiene una descripción del contexto, dos perfiles ficticios y una tabla con al menos nueve criterios de comparación.

**Verification:**

Revisa que la tabla cumpla estas condiciones:

- Cada fila compara el mismo criterio en ambas experiencias.
- Los criterios se relacionan con las oportunidades seleccionadas.
- La diferencia entre ambos flujos puede observarse o representarse visualmente.
- No existen afirmaciones sobre productos reales sin fuente oficial.
- El texto no culpa a la persona usuaria por una barrera generada por el diseño.

---

### Paso 3: Construir un prompt visual detallado para Copilot

**Objetivo:** Redactar una solicitud que permita a Copilot generar una comparación visual centrada en la persona usuaria, accesible y situada en El Salvador.

**Instructions:**

1. Abre Microsoft Edge y accede a:

   ```text
   https://copilot.microsoft.com/
   ```

2. Inicia sesión con tu cuenta Microsoft personal.

3. Verifica que el idioma de interacción sea español. Si Copilot responde en otro idioma, solicita explícitamente una respuesta en español.

4. Prepara un prompt con los elementos obligatorios:
   - contexto geográfico;
   - tarea de pago comparable;
   - dos perfiles ficticios;
   - experiencia inclusiva;
   - experiencia con barreras;
   - criterios de accesibilidad;
   - momentos de fricción;
   - restricciones de representación responsable;
   - formato de salida solicitado.

5. Adapta el siguiente prompt modelo con la información de tu matriz:

   ```text
   Actúa como diseñador de experiencia de usuario especializado en inclusión financiera.
   Crea una propuesta de storyboard e infografía comparativa en español para El Salvador.

   Contexto:
   - Tarea: [describir la misma tarea de pago para ambos casos].
   - Perfil A: [describir perfil ficticio y necesidad].
   - Perfil B: [describir perfil ficticio y necesidad].
   - Oportunidad 1: [describir].
   - Oportunidad 2: [describir].

   Compara dos flujos hipotéticos:
   1. Experiencia inclusiva: aplicación móvil con lenguaje claro, contraste legible,
      confirmación de monto y destinatario, pasos reducidos, ayuda contextual,
      alternativa ante conectividad intermitente y recuperación de errores.
   2. Experiencia con barreras: flujo con muchos pasos, términos técnicos,
      mensajes de error poco claros, dependencia de conexión constante,
      confirmación ambigua y controles difíciles de identificar.

   Entrega:
   A. Un storyboard de 4 escenas por cada experiencia.
   B. Una tabla comparativa con los criterios: claridad, pasos, accesibilidad,
      conectividad, confirmación, errores, soporte y riesgo de exclusión.
   C. Una descripción para una infografía visual de dos columnas titulada
      “Pago digital inclusivo” y “Pago digital con barreras”.
   D. Si la función visual está disponible, genera una imagen conceptual
      horizontal de dos columnas que represente ambos flujos.

   Reglas de representación responsable:
   - No uses logotipos, nombres de bancos ni marcas reales.
   - No muestres datos personales, números de cuenta, tarjetas ni documentos reales.
   - No asocies barreras de acceso con incapacidad personal, pobreza, edad,
     género, discapacidad u origen territorial.
   - Representa diversidad de forma respetuosa y evita estereotipos.
   - No afirmes que el escenario representa un producto real o una regulación vigente.
   - Usa moneda, entorno y lenguaje compatibles con El Salvador solo cuando sea
     necesario para el contexto, sin inventar requisitos legales ni institucionales.
   ```

6. Envía el prompt.

7. Si Copilot solicita aclaraciones, responde manteniendo el mismo alcance: escenario hipotético, usuarios ficticios, contexto salvadoreño y ausencia de marcas o datos reales.

8. Si la generación de imágenes no está disponible, solicita únicamente el storyboard y la descripción de la infografía. El archivo PNG se obtendrá mediante una captura de pantalla del resultado textual o visual más representativo en el siguiente paso.

**Expected output:**

Copilot devuelve una propuesta estructurada que incluye storyboard, comparación de criterios y una descripción de infografía. Cuando esté habilitada la función visual, también genera un concepto de imagen.

**Verification:**

Comprueba que el resultado de Copilot:

- esté en español;
- compare exactamente dos experiencias;
- mantenga la misma tarea de pago;
- incluya al menos un punto de fricción relacionado con conectividad, claridad o accesibilidad;
- no presente marcas, clientes reales ni afirmaciones regulatorias;
- no use representaciones ofensivas, paternalistas o estereotipadas.

---

### Paso 4: Revisar críticamente la propuesta generada

**Objetivo:** Aplicar validación humana al contenido generado antes de convertirlo en evidencia del laboratorio.

**Instructions:**

1. Lee el resultado completo de Copilot antes de copiarlo o capturarlo.

2. Revisa la propuesta usando los siguientes criterios:

   | Área de revisión | Pregunta de validación |
   |---|---|
   | Contexto | ¿La escena podría ocurrir razonablemente en El Salvador sin presentar datos inventados como hechos? |
   | Inclusión | ¿La experiencia inclusiva elimina barreras de diseño concretas? |
   | Sesgo | ¿La imagen o el texto asocia una característica personal con incompetencia, riesgo o incapacidad? |
   | Lenguaje | ¿El contenido usa términos claros y respetuosos? |
   | Accesibilidad | ¿Se consideran contraste, texto legible, instrucciones, recuperación de errores o alternativas de interacción? |
   | Conectividad | ¿Se representa la conectividad intermitente como una condición del entorno y no como culpa de la persona? |
   | Precisión | ¿Se evitan afirmaciones sobre leyes, instituciones, comisiones, productos o requisitos reales no verificados? |
   | Comparabilidad | ¿Las dos columnas realizan la misma tarea y permiten observar diferencias? |

3. Identifica al menos dos observaciones de revisión humana. Pueden ser:
   - una mejora solicitada a Copilot;
   - un elemento que debe eliminarse;
   - una representación que se debe ajustar;
   - una afirmación que debe marcarse como hipotética;
   - un detalle visual que necesita más contraste o claridad.

4. Si detectas una representación problemática, envía una solicitud de corrección a Copilot. Ejemplo:

   ```text
   Revisa la propuesta anterior. Sustituye cualquier lenguaje que atribuya la
   dificultad a la persona usuaria por una explicación de la barrera de diseño.
   Mantén el contexto hipotético de El Salvador, elimina afirmaciones no verificadas
   sobre instituciones o regulaciones y mejora la claridad visual de las etiquetas,
   botones y mensajes de error.
   ```

5. Conserva la versión corregida o la versión que consideres más adecuada para la evidencia.

6. Añade al archivo Markdown una sección de revisión humana:

   ```markdown
   ### Revisión humana del resultado de Copilot

   | Elemento revisado | Hallazgo | Decisión aplicada |
   |---|---|---|
   | Sesgo o estereotipo | [hallazgo o “No se identificó”] | [corrección, eliminación o justificación] |
   | Lenguaje inclusivo | [hallazgo] | [decisión] |
   | Accesibilidad | [hallazgo] | [decisión] |
   | Contexto de El Salvador | [hallazgo] | [decisión] |
   | Afirmaciones no verificadas | [hallazgo] | [decisión] |

   **Nota de uso responsable:** La comparación representa escenarios hipotéticos de diseño.
   No describe necesariamente productos, tarifas, requisitos ni regulaciones de entidades reales.
   ```

**Expected output:**

El archivo Markdown documenta una revisión humana con hallazgos y decisiones explícitas.

**Verification:**

La revisión es satisfactoria si:

- contiene al menos dos decisiones humanas concretas;
- diferencia claramente entre contenido generado por IA y decisiones tomadas por el estudiante;
- aclara que el material es hipotético;
- elimina o corrige afirmaciones no verificadas;
- evita lenguaje que responsabilice a la persona usuaria por barreras de diseño.

---

### Paso 5: Crear y guardar la evidencia visual en formato PNG

**Objetivo:** Guardar una imagen de la comparación visual o del storyboard revisado como evidencia del laboratorio.

**Instructions:**

1. En Copilot, deja visible la propuesta visual, storyboard o tabla comparativa más representativa y revisada.

2. Si Copilot generó una imagen conceptual:
   - abre la imagen en el tamaño más legible disponible;
   - verifica que se observen ambas experiencias;
   - confirma que no muestre datos sensibles, marcas reales o texto ilegible.

3. Si Copilot no generó una imagen:
   - deja visible el storyboard o la tabla comparativa de dos columnas;
   - ajusta el zoom del navegador para que el contenido sea legible;
   - utiliza una captura de pantalla como evidencia visual del concepto generado.

4. Realiza una captura de pantalla con la Herramienta Recortes de Windows:
   - presiona `Windows + Shift + S`;
   - selecciona el área de la comparación;
   - abre la notificación de la captura;
   - usa **Guardar como**.

5. Guarda el archivo exactamente con este nombre:

   ```text
   C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.png
   ```

6. Si guardaste primero una imagen descargada de Copilot con otro nombre, renómbrala desde PowerShell:

   ```powershell
   Rename-Item -Path "C:\CopilotLabs\Batch1\[nombre_original].png" -NewName "02_comparacion_pagos_digitales.png"
   ```

7. Abre el PNG desde el Explorador de archivos y confirma que:
   - la imagen se visualiza correctamente;
   - ambas experiencias pueden distinguirse;
   - el texto principal se puede leer;
   - no hay información sensible visible.

**Expected output:**

Existe un archivo PNG válido con una comparación visual, storyboard o infografía conceptual en:

```text
C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.png
```

**Verification:**

Ejecuta:

```powershell
Get-Item "C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.png" |
Select-Object Name, Length, LastWriteTime
```

Verifica que:

- el nombre sea exactamente `02_comparacion_pagos_digitales.png`;
- el tamaño del archivo sea mayor que 0 bytes;
- la fecha de modificación corresponda a la sesión actual;
- el archivo abra como imagen PNG.

---

### Paso 6: Completar el análisis comparativo y las tensiones identificadas

**Objetivo:** Traducir el resultado visual en hallazgos utilizables para el análisis de perspectivas del siguiente laboratorio.

**Instructions:**

1. Regresa al archivo:

   ```powershell
   code "C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.md"
   ```

2. Agrega una sección de storyboard resumido. No es necesario copiar toda la respuesta de Copilot; conserva solo los elementos que sustentan tu análisis.

   ```markdown
   ### Storyboard resumido

   | Escena | Experiencia inclusiva | Experiencia con barreras |
   |---|---|---|
   | 1. Inicio de la tarea | [describir] | [describir] |
   | 2. Ingreso de información | [describir] | [describir] |
   | 3. Confirmación o fricción | [describir] | [describir] |
   | 4. Resultado y siguiente paso | [describir] | [describir] |
   ```

3. Agrega la referencia al archivo visual:

   ```markdown
   ### Evidencia visual

   Archivo asociado: `02_comparacion_pagos_digitales.png`

   La imagen representa un concepto hipotético generado o estructurado con apoyo de IA
   y revisado por el estudiante. No representa un producto financiero real.
   ```

4. Documenta al menos tres tensiones o puntos de vista que puedan ser retomados en el Laboratorio 03-00-01. Ejemplos de tensiones válidas:
   - simplicidad del flujo frente a controles de confirmación;
   - conveniencia digital frente a conectividad intermitente;
   - automatización frente a necesidad de soporte humano;
   - rapidez del pago frente a comprensión del monto, destinatario y comisión;
   - diseño uniforme frente a necesidades de accesibilidad diversas.

5. Utiliza el siguiente formato:

   ```markdown
   ### Tensiones y puntos de vista para el siguiente laboratorio

   | Tensión o punto de vista | Evidencia en la comparación | Posible pregunta para analizar |
   |---|---|---|
   | [ejemplo: rapidez frente a comprensión] | [escena o criterio] | [pregunta] |
   | [tensión 2] | [evidencia] | [pregunta] |
   | [tensión 3] | [evidencia] | [pregunta] |
   ```

6. Finaliza el documento con una conclusión breve de tres a cinco oraciones. Explica qué características hacen más inclusiva una experiencia de pago digital y qué riesgos aparecen cuando el diseño no considera accesibilidad, claridad o condiciones de conectividad.

**Expected output:**

El archivo Markdown contiene criterios, perfiles, storyboard, revisión humana, referencia al PNG y al menos tres tensiones para el laboratorio siguiente.

**Verification:**

Revisa que el documento incluya todas estas secciones:

- comparación visual de experiencias de pagos digitales;
- perfiles ficticios;
- criterios de comparación;
- revisión humana;
- storyboard resumido;
- evidencia visual;
- tensiones y puntos de vista;
- conclusión.

---

### Paso 7: Verificar los entregables finales

**Objetivo:** Confirmar que la evidencia está completa, tiene el nombre requerido y se encuentra en el directorio obligatorio.

**Instructions:**

1. Guarda el archivo Markdown.

2. Ejecuta el siguiente comando en PowerShell:

   ```powershell
   Get-ChildItem "C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.*" |
   Select-Object Name, Length, LastWriteTime
   ```

3. Confirma que se muestran los dos archivos requeridos:

   ```text
   02_comparacion_pagos_digitales.md
   02_comparacion_pagos_digitales.png
   ```

4. Comprueba el contenido mínimo del archivo Markdown:

   ```powershell
   Select-String -Path "C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.md" `
   -Pattern "Perfiles ficticios","Criterios de comparación","Revisión humana","Tensiones"
   ```

5. Abre ambos archivos manualmente:
   - el archivo `.md` debe mostrar texto estructurado y tablas;
   - el archivo `.png` debe abrirse como imagen;
   - los dos deben contener evidencia consistente de la misma comparación.

6. No modifiques ni elimines el archivo `01_matriz_inclusion_financiera.md`, ya que es una entrada de trazabilidad para el laboratorio.

**Expected output:**

Los archivos requeridos están disponibles, son legibles y documentan una comparación visual responsable entre dos experiencias de pagos digitales.

**Verification:**

La práctica queda completa si se cumple la siguiente lista:

- [ ] Existe `C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.md`.
- [ ] Existe `C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.png`.
- [ ] La comparación utiliza dos oportunidades del laboratorio anterior.
- [ ] Las experiencias realizan una tarea de pago comparable.
- [ ] La propuesta considera accesibilidad y conectividad.
- [ ] La evidencia visual fue revisada por una persona.
- [ ] El documento identifica al menos tres tensiones para el siguiente laboratorio.
- [ ] No se incluyeron datos personales, datos financieros reales ni afirmaciones regulatorias no verificadas.

## Validación y Pruebas

Realiza las siguientes validaciones finales:

| Prueba | Método | Resultado esperado |
|---|---|---|
| Existencia del archivo Markdown | `Test-Path "C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.md"` | `True` |
| Existencia del archivo PNG | `Test-Path "C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.png"` | `True` |
| Tamaño de la evidencia visual | `Get-Item` sobre el PNG | Tamaño mayor que 0 bytes |
| Contenido del análisis | Revisar títulos y tablas del Markdown | Incluye perfiles, criterios, revisión, storyboard y tensiones |
| Comparabilidad | Revisar ambas columnas | Las dos experiencias ejecutan la misma tarea de pago |
| Inclusión | Revisar criterios y visual | Incluye claridad, accesibilidad, ayuda, errores o conectividad |
| Uso responsable | Revisar texto e imagen | Sin datos reales, marcas no autorizadas ni afirmaciones no verificadas |
| Contexto | Revisar descripciones | El Salvador aparece como contexto, no como una afirmación estereotipada |

Ejecuta una comprobación consolidada:

```powershell
$archivos = @(
  "C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.md",
  "C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.png"
)

$archivos | ForEach-Object {
  [PSCustomObject]@{
    Archivo = $_
    Existe = Test-Path $_
    TamanoBytes = if (Test-Path $_) { (Get-Item $_).Length } else { 0 }
  }
}
```

La validación es aprobada cuando ambos archivos existen y tienen contenido. La calidad del resultado se confirma mediante la revisión humana documentada, no solo por la existencia técnica de los archivos.

## Solución de Problemas

### Problema 1: Copilot no muestra la opción de generar imágenes

**Síntomas:** Copilot entrega únicamente texto, no aparece un botón de creación visual o la respuesta indica que no puede generar una imagen.

**Causa:** La disponibilidad de funciones visuales puede variar según la versión de Copilot, región, cuenta, configuración temporal del servicio o límites de la sesión.

**Solución:**

1. No cambies de cuenta ni intentes usar credenciales compartidas.
2. Solicita a Copilot un storyboard textual de dos columnas y una descripción de infografía.
3. Ajusta el navegador para mostrar claramente el storyboard o la tabla comparativa.
4. Realiza una captura de pantalla con `Windows + Shift + S`.
5. Guarda la captura como:

   ```text
   C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.png
   ```

6. En el Markdown, indica que la evidencia visual corresponde a una captura del storyboard o la tabla conceptual generada con apoyo de Copilot.

### Problema 2: La imagen o respuesta incluye estereotipos, texto ilegible o afirmaciones no verificadas

**Síntomas:** La propuesta muestra usuarios de forma paternalista, atribuye dificultades a una característica personal, utiliza texto muy pequeño, presenta elementos irreales como hechos o menciona entidades financieras reales sin respaldo.

**Causa:** Los modelos generativos producen contenido basado en patrones estadísticos y no validan automáticamente inclusión, accesibilidad, precisión local ni vigencia de información financiera.

**Solución:**

1. No utilices la primera salida como evidencia final.
2. Identifica el problema concreto y solicita una corrección dirigida. Por ejemplo:

   ```text
   Corrige la propuesta para eliminar estereotipos, no atribuir barreras a la persona
   usuaria, mejorar el contraste y la legibilidad, usar lenguaje claro y eliminar
   referencias a instituciones, requisitos o regulaciones reales no verificadas.
   Mantén el escenario como una comparación hipotética para El Salvador.
   ```

3. Revisa nuevamente el resultado con la tabla de validación humana.
4. Documenta el hallazgo y la decisión tomada en `02_comparacion_pagos_digitales.md`.
5. Captura o guarda solamente la versión revisada que cumpla los criterios de uso responsable.

## Limpieza

1. Guarda y cierra el archivo `02_comparacion_pagos_digitales.md`.
2. Confirma que el PNG final está guardado con el nombre obligatorio.
3. Cierra las pestañas de Copilot que contengan prompts o resultados de la práctica.
4. Cierra sesión en Copilot si utilizaste un equipo compartido o de uso institucional.
5. No elimines los siguientes archivos, ya que forman parte de la evidencia y trazabilidad del batch:

   ```text
   C:\CopilotLabs\Batch1\01_matriz_inclusion_financiera.md
   C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.md
   C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.png
   ```

6. No se requieren acciones sobre puertos, contenedores, servicios locales ni bases de datos.

## Resumen (+ optional resources)

En esta práctica convertiste oportunidades de inclusión financiera en una comparación visual entre dos experiencias hipotéticas de pago digital. Diseñaste un prompt estructurado para Copilot, revisaste críticamente el contenido generado y guardaste evidencia en Markdown y PNG. El resultado debe permitir discutir, en el siguiente laboratorio, tensiones entre rapidez, seguridad, comprensión, conectividad, accesibilidad y soporte humano.

Entregables finales:

```text
C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.md
C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.png
```

Recursos opcionales para profundizar:

- Microsoft Copilot: `https://copilot.microsoft.com/`
- Pautas de accesibilidad para contenido web (WCAG): `https://www.w3.org/WAI/standards-guidelines/wcag/`
- Principios de diseño centrado en las personas: priorizar comprensión, control, prevención de errores y recuperación ante fallos.
