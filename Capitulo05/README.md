# Práctica. Escenarios visuales sobre la evolución de los servicios financieros en El Salvador

## Metadatos

| Elemento | Valor |
|---|---|
| Duración | 17 minutos |
| Complejidad | Difícil |
| Nivel de Bloom | Crear |

## Descripción General

En esta práctica integrará los artefactos desarrollados en los laboratorios anteriores para crear escenarios visuales plausibles sobre la evolución de los servicios financieros digitales en El Salvador. Los escenarios no son pronósticos ni recomendaciones regulatorias: son herramientas de exploración para contrastar oportunidades, barreras, riesgos, actores y señales de validación. Utilizará Microsoft Copilot para apoyar la redacción de descripciones visuales y, si está disponible, la generación de imágenes conceptuales respetuosas del contexto local.

## Objetivos de Aprendizaje

- [ ] Crear dos o tres escenarios visuales plausibles con horizonte temporal, usuarios, canales digitales, beneficios, barreras, riesgos y señales de validación.
- [ ] Integrar hallazgos de inclusión financiera, pagos digitales, perspectivas de actores y competencia en una comparación estructurada.
- [ ] Formular prompts visuales responsables que distingan posibilidades de hechos confirmados y eviten estereotipos sobre El Salvador.
- [ ] Seleccionar un escenario inclusivo y factible mediante criterios explícitos, documentando incertidumbres y preguntas de investigación pendientes.
- [ ] Guardar una evidencia verificable del análisis en `C:\CopilotLabs\Batch1\05_escenarios_financieros_el_salvador.md`.

## Prerrequisitos

El estudiante debe haber completado los laboratorios `01-00-01`, `02-00-01`, `03-00-01` y `04-00-01`. Debe comprender que una respuesta generada por IA puede contener información incompleta, desactualizada o no verificable, especialmente cuando trata regulaciones, servicios financieros, adopción tecnológica o proyecciones.

Debe disponer de los siguientes archivos en el directorio obligatorio:

- `C:\CopilotLabs\Batch1\01_matriz_inclusion_financiera.md`
- `C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.md`
- `C:\CopilotLabs\Batch1\02_comparacion_pagos_digitales.png`
- `C:\CopilotLabs\Batch1\03_mapa_perspectivas_servicios_financieros.md`
- `C:\CopilotLabs\Batch1\04_respuesta_competencia.md`

También necesita acceso a Internet y una cuenta Microsoft personal activa para iniciar sesión en Microsoft Copilot. No utilice cuentas compartidas, datos reales de clientes, números de cuenta, documentos de identidad, historiales financieros ni información confidencial.

## Entorno de Laboratorio

| Categoría | Especificación |
|---|---|
| Sistema operativo | Windows 11 Pro 23H2 o Windows 11 24H2 |
| Navegador | Microsoft Edge 128.0.2739.79 o versión compatible |
| Herramienta principal | Microsoft Copilot experiencia web |
| URL de referencia | `https://copilot.microsoft.com/` |
| Editor de archivos | Visual Studio Code 1.93.1 o editor Markdown equivalente |
| Cuenta requerida | Cuenta Microsoft personal |
| Directorio obligatorio | `C:\CopilotLabs\Batch1\` |
| Idioma de interacción | Español |
| Contexto geográfico | El Salvador |
| Servicios locales, puertos, bases de datos y contenedores | No aplican |

Abra PowerShell y ejecute los siguientes comandos para comprobar el directorio y los archivos de entrada:

```powershell
$LabPath = "C:\CopilotLabs\Batch1"
New-Item -ItemType Directory -Path $LabPath -Force | Out-Null

Get-ChildItem -Path $LabPath -File |
    Select-Object Name, Length, LastWriteTime |
    Format-Table -AutoSize
```

Compruebe específicamente la evidencia requerida:

```powershell
$RequiredFiles = @(
    "01_matriz_inclusion_financiera.md",
    "02_comparacion_pagos_digitales.md",
    "02_comparacion_pagos_digitales.png",
    "03_mapa_perspectivas_servicios_financieros.md",
    "04_respuesta_competencia.md"
)

foreach ($File in $RequiredFiles) {
    $FullPath = Join-Path $LabPath $File
    if (Test-Path $FullPath) {
        Write-Host "ENCONTRADO: $File" -ForegroundColor Green
    } else {
        Write-Host "FALTA: $File" -ForegroundColor Red
    }
}
```

## Instrucciones Paso a Paso

### Paso 1: Verificar los insumos y definir límites responsables

**Objetivo:** Confirmar que los artefactos previos están disponibles y establecer que los escenarios son hipótesis exploratorias, no predicciones garantizadas ni asesoría financiera o legal.

**Instrucciones:**

1. Abra Microsoft Edge y navegue a `https://copilot.microsoft.com/`.
2. Inicie sesión con su cuenta Microsoft personal.
3. Abra Visual Studio Code o su editor Markdown y revise los archivos previos almacenados en `C:\CopilotLabs\Batch1\`.
4. Identifique, como mínimo, los siguientes elementos de los laboratorios anteriores:
   - Dos necesidades o barreras de inclusión financiera.
   - Dos hallazgos de la comparación de pagos digitales.
   - Tres perspectivas de actores, por ejemplo: usuarios, comercios, instituciones financieras, reguladores, cooperativas, empresas tecnológicas o redes de agentes.
   - Un argumento o diferenciador relevante de la respuesta a la competencia.
5. Cree el archivo de evidencia final:
   
   ```powershell
   New-Item -ItemType File `
     -Path "C:\CopilotLabs\Batch1\05_escenarios_financieros_el_salvador.md" `
     -Force
   ```

6. Agregue al inicio del archivo la siguiente estructura. Reemplace los textos entre corchetes con sus propios hallazgos.

   ```markdown
   # Escenarios financieros digitales en El Salvador

   **Fecha de elaboración:** [AAAA-MM-DD]  
   **Propósito:** Explorar escenarios plausibles sobre la evolución de servicios financieros digitales en El Salvador.  
   **Advertencia responsable:** Este documento no presenta pronósticos garantizados, asesoría legal, regulación confirmada ni recomendaciones financieras personalizadas. Las afirmaciones sobre adopción, regulación, mercado o impacto requieren verificación humana con fuentes oficiales y evidencia actualizada.

   ## Insumos integrados de laboratorios anteriores

   | Artefacto | Hallazgo reutilizado | Implicación para escenarios |
   |---|---|---|
   | Matriz de inclusión financiera | [Hallazgo] | [Implicación] |
   | Comparación de pagos digitales | [Hallazgo] | [Implicación] |
   | Mapa de perspectivas | [Hallazgo] | [Implicación] |
   | Respuesta a la competencia | [Hallazgo] | [Implicación] |

   ## Límites del ejercicio

   - Los escenarios describen posibilidades plausibles, no hechos futuros.
   - No se asumirán cambios regulatorios sin una fuente oficial vigente.
   - No se utilizarán datos personales, perfiles reales de clientes ni cifras no verificadas.
   - Las imágenes conceptuales serán representaciones narrativas, no evidencia de adopción real.
   ```

7. Guarde el archivo con codificación UTF-8.

**Expected output:**

Un archivo `05_escenarios_financieros_el_salvador.md` creado en el directorio obligatorio, con una declaración de propósito, límites responsables y una tabla que conecte los cuatro artefactos previos con el nuevo análisis.

**Verification:**

Ejecute el siguiente comando y confirme que el archivo existe y no está vacío:

```powershell
$OutputFile = "C:\CopilotLabs\Batch1\05_escenarios_financieros_el_salvador.md"
Get-Item $OutputFile | Select-Object Name, Length, LastWriteTime

Get-Content $OutputFile -TotalCount 35
```

La verificación es correcta si observa el nombre del archivo, un tamaño mayor que cero y el texto de advertencia responsable.

### Paso 2: Formular una consulta de síntesis para Copilot

**Objetivo:** Obtener un borrador de posibles escenarios sin convertir respuestas generadas por IA en hechos confirmados.

**Instrucciones:**

1. Reúna en una nota breve los hallazgos seleccionados en el paso anterior. No copie información personal ni datos confidenciales.
2. En Copilot, use el siguiente prompt. Sustituya los campos entre corchetes por los hallazgos de sus propios archivos.

   ```text
   Actúa como facilitador de diseño de escenarios, no como predictor ni asesor legal o financiero. Estoy explorando posibles evoluciones de los servicios financieros digitales en El Salvador.

   Usa únicamente estos insumos de trabajo:
   - Barreras de inclusión identificadas: [barrera 1], [barrera 2].
   - Hallazgos sobre pagos digitales: [hallazgo 1], [hallazgo 2].
   - Perspectivas de actores: [actor y perspectiva 1], [actor y perspectiva 2], [actor y perspectiva 3].
   - Diferenciador o riesgo competitivo: [hallazgo de competencia].

   Propón 3 escenarios exploratorios plausibles para los próximos 12 a 36 meses. Para cada escenario, incluye:
   1. Un nombre neutral, sin prometer resultados.
   2. Horizonte temporal explícito.
   3. Usuarios principales.
   4. Servicio o canal digital.
   5. Beneficios potenciales.
   6. Barreras y riesgos emergentes.
   7. Actores involucrados.
   8. Señales observables que permitirían investigar si el escenario está ocurriendo.
   9. Supuestos que deben validarse.

   Separa claramente: hechos confirmados, supuestos, posibilidades y preguntas pendientes. No inventes regulación, estadísticas, alianzas, empresas, fechas de implementación ni niveles de adopción. Si no puedes verificar un dato, etiquétalo como “requiere validación”.
   ```

3. Lea la respuesta de Copilot de forma crítica.
4. Seleccione dos o tres escenarios que sean distintos entre sí. Procure que representen diferentes condiciones, por ejemplo:
   - Un escenario de expansión inclusiva y gradual.
   - Un escenario de crecimiento desigual o fragmentado.
   - Un escenario condicionado por confianza, conectividad, protección al consumidor o interoperabilidad.
5. No copie afirmaciones factuales de Copilot sin validación. Conserve solo ideas estructurales y etiquete claramente las hipótesis.
6. Agregue al archivo Markdown una sección de registro de la interacción:

   ```markdown
   ## Registro de consulta asistida por IA

   **Herramienta utilizada:** Microsoft Copilot, experiencia web  
   **Uso realizado:** Generación de hipótesis y estructura inicial de escenarios.  
   **Regla de validación:** Las salidas de IA se trataron como ideas de trabajo; no se aceptaron como fuentes regulatorias, estadísticas oficiales ni evidencia de mercado.

   **Resumen de resultados útiles:**
   - [Idea estructural o escenario preliminar 1]
   - [Idea estructural o escenario preliminar 2]
   - [Idea estructural o escenario preliminar 3]

   **Contenido que requiere validación antes de usarse como hecho:**
   - [Dato, supuesto o afirmación no verificada]
   - [Dato, supuesto o afirmación no verificada]
   ```

**Expected output:**

Una lista preliminar de dos o tres escenarios diferenciados, acompañada de una separación explícita entre ideas de exploración y afirmaciones que requieren evidencia adicional.

**Verification:**

Revise que cada escenario preliminar pueda responder estas preguntas:

1. ¿Tiene un horizonte temporal?
2. ¿Identifica usuarios y actores?
3. ¿Describe un canal o servicio digital concreto?
4. ¿Incluye al menos una barrera y un riesgo?
5. ¿Evita afirmar como hecho una predicción o cambio regulatorio no confirmado?
6. ¿Contiene señales observables y supuestos validables?

Si alguna respuesta es “no”, ajuste el escenario antes de continuar.

### Paso 3: Diseñar los escenarios con una matriz comparable

**Objetivo:** Convertir las ideas preliminares en escenarios completos, comparables y verificables.

**Instrucciones:**

1. En el archivo `05_escenarios_financieros_el_salvador.md`, agregue la sección `## Escenarios exploratorios`.
2. Documente dos o tres escenarios. Use la siguiente plantilla para cada uno.
3. Mantenga un lenguaje condicional: “podría”, “es posible que”, “si se cumplen determinadas condiciones”, “requiere validación”.
4. Incluya actores con perspectivas potencialmente diferentes. Por ejemplo, una experiencia conveniente para un comercio puede implicar costos operativos, requisitos de conectividad o necesidades de capacitación.
5. Evite representar a toda la población salvadoreña como homogénea. Considere diferencias de conectividad, edad, alfabetización digital, ubicación, discapacidad, ingresos, confianza y acceso a dispositivos.
6. Use como referencia el siguiente ejemplo de formato. Personalícelo con sus propios resultados; no es obligatorio usar estos nombres de escenarios.

   ```markdown
   ### Escenario 1: Pagos cotidianos asistidos por redes de confianza

   **Tipo de escenario:** Deseable condicionado  
   **Horizonte temporal:** 12 a 24 meses  
   **Nivel de certeza:** Hipótesis exploratoria; requiere validación de adopción, costos, protección al consumidor y viabilidad operativa.

   | Dimensión | Descripción |
   |---|---|
   | Usuarios principales | Personas con uso intermitente de servicios financieros digitales, pequeños comercios, emprendedores y redes familiares. |
   | Servicio o canal digital | Pagos de bajo monto mediante aplicaciones móviles, códigos QR, transferencias y apoyo presencial de agentes o comercios capacitados. |
   | Oportunidad de inclusión | Podría reducir desplazamientos y facilitar pagos cotidianos si la experiencia es comprensible, de bajo costo y con apoyo accesible. |
   | Beneficios potenciales | Mayor conveniencia, registro de transacciones, opciones de pago para comercios y posible reducción del uso exclusivo de efectivo. |
   | Barreras | Conectividad irregular, costo de datos, acceso desigual a teléfonos, baja confianza, lenguaje técnico y dificultades de recuperación de cuenta. |
   | Riesgos emergentes | Fraude, suplantación, comisiones poco claras, exclusión de personas sin teléfono inteligente y dependencia de intermediarios no capacitados. |
   | Actores involucrados | Usuarios, comercios, bancos, cooperativas, proveedores tecnológicos, redes de agentes, entidades de protección al consumidor y autoridades competentes. |
   | Supuestos por validar | Disponibilidad de soporte, claridad tarifaria, controles antifraude, capacitación de comercios, mecanismos de reclamo y accesibilidad. |
   | Señales de validación | Publicación de condiciones claras, aumento verificable de comercios que aceptan pagos digitales, materiales de educación financiera, reportes oficiales y evidencia de resolución de reclamos. |
   | Indicadores de alerta | Quejas recurrentes, rechazos de transacción, cobros inesperados, incidentes de fraude, exclusión por requisitos de dispositivo o identidad. |

   **Pregunta de investigación pendiente:** ¿Qué mecanismos de asistencia y reclamo resultan más accesibles para usuarios con conectividad limitada o baja alfabetización digital?
   ```

7. Cree al menos un escenario que describa una oportunidad inclusiva y al menos un escenario que exponga un riesgo o una evolución desigual.
8. Incluya un tercer escenario solo si puede completarlo con la misma calidad. Es preferible presentar dos escenarios bien sustentados que tres superficiales.

**Expected output:**

Dos o tres escenarios completos, cada uno con horizonte temporal, usuarios, servicio o canal, beneficios, barreras, riesgos, actores, supuestos y señales verificables.

**Verification:**

Utilice esta lista de control sobre cada escenario:

| Criterio | Sí/No |
|---|---|
| Expresa un horizonte temporal concreto. |  |
| Identifica usuarios principales sin generalizaciones absolutas. |  |
| Describe un servicio, canal o experiencia digital específica. |  |
| Diferencia beneficios potenciales de beneficios comprobados. |  |
| Incluye barreras de acceso e inclusión. |  |
| Incluye riesgos operativos, de fraude, confianza o protección al consumidor. |  |
| Reconoce actores con intereses o responsabilidades diferentes. |  |
| Define señales observables para validación. |  |
| Declara supuestos o preguntas pendientes. |  |

Complete la tabla en el archivo Markdown o realice la revisión manual antes de avanzar.

### Paso 4: Crear prompts visuales responsables

**Objetivo:** Diseñar representaciones visuales conceptuales que comuniquen posibilidades sin presentar el futuro como un hecho ni reforzar estereotipos.

**Instrucciones:**

1. Seleccione los dos escenarios más claros de la matriz.
2. Para cada escenario, redacte un prompt visual en español.
3. Incluya elementos de contexto local de manera respetuosa, sin asumir que todas las personas, comercios o zonas del país tienen las mismas condiciones.
4. Solicite una representación conceptual, storyboard o ilustración especulativa. Evite frases como “fotografía real de la adopción actual” o “prueba de que este servicio ya existe”.
5. Incluya elementos de seguridad y transparencia cuando sean relevantes: aviso de verificación, soporte al usuario, confirmación de transacción, señalización clara de costos o canales de reclamo.
6. Evite incluir marcas, logotipos, rostros identificables de personas reales, documentos de identidad, números de cuenta o pantallas con datos personales.
7. Use en Copilot un prompt similar al siguiente para el primer escenario:

   ```text
   Crea una ilustración conceptual tipo storyboard de tres viñetas sobre un escenario posible, no confirmado, de servicios financieros digitales en El Salvador durante los próximos 12 a 24 meses.

   Escenario: pagos cotidianos asistidos por redes de confianza.
   Personas representadas: diversidad de adultos, pequeños comerciantes y una persona de apoyo capacitada, sin usar rasgos estereotipados ni personas reales identificables.
   Contexto: un pequeño comercio urbano o semiurbano, conectividad variable y uso opcional de teléfono móvil.
   Viñeta 1: una persona consulta de forma clara el costo y el método de pago.
   Viñeta 2: el comercio confirma un pago digital de bajo monto con una interfaz simple.
   Viñeta 3: aparece una opción visible de soporte, verificación y reporte de problemas.

   Estilo: ilustración editorial limpia, colores sobrios, accesible, texto mínimo en español.
   Debe incluir una etiqueta discreta: “Escenario conceptual sujeto a validación”.
   No mostrar logotipos de empresas, dinero en efectivo con detalles realistas, datos personales, promesas de resultados ni afirmaciones de adopción masiva.
   ```

8. Para un escenario de riesgo o fragmentación, utilice un prompt que represente obstáculos sin dramatizar ni culpabilizar a usuarios:

   ```text
   Crea una infografía conceptual en dos columnas sobre un escenario exploratorio de adopción desigual de servicios financieros digitales en El Salvador durante los próximos 24 a 36 meses.

   Columna izquierda: oportunidades potenciales, como pagos más convenientes para algunos comercios y usuarios con conectividad estable.
   Columna derecha: barreras potenciales, como conectividad irregular, confusión sobre comisiones, dificultades de soporte y riesgo de exclusión de personas sin dispositivos compatibles.

   Mostrar actores diversos de manera respetuosa y no estereotipada. Usar íconos de conectividad, soporte, seguridad, accesibilidad y transparencia.
   Incluir el texto: “Visualización conceptual; no representa una predicción ni datos observados”.
   No usar logotipos, cifras inventadas, nombres de instituciones, rostros identificables ni mensajes de miedo.
   ```

9. Si Copilot ofrece generación de imágenes en su cuenta, genere una o dos imágenes conceptuales y revíselas antes de usarlas.
10. Si la función de imagen no está disponible, conserve los prompts y redacte una descripción visual detallada. Esto cumple el objetivo del laboratorio.
11. Agregue al archivo Markdown una sección por cada visual:

   ```markdown
   ## Visuales conceptuales y prompts

   ### Visual 1: [Nombre del escenario]

   **Propósito visual:** [Qué ayuda a comprender la imagen.]  
   **Estado:** [Generada con IA / Prompt documentado; generación no disponible.]  
   **Uso responsable:** Ilustración conceptual; no evidencia de adopción, regulación, alianza comercial ni comportamiento real de usuarios.

   **Prompt utilizado:**
   > [Pegue el prompt final.]

   **Revisión humana aplicada:**
   - [Ejemplo: Se eliminó una cifra no verificable.]
   - [Ejemplo: Se añadió una etiqueta de escenario conceptual.]
   - [Ejemplo: Se revisó que no incluyera marcas ni datos personales.]
   ```

12. Si genera una imagen adicional, guárdela solamente en `C:\CopilotLabs\Batch1\`. Use un nombre descriptivo, por ejemplo:

   ```text
   C:\CopilotLabs\Batch1\05_escenario_1_conceptual.png
   ```

**Expected output:**

Dos prompts visuales responsables documentados y, cuando la función esté disponible, una o dos imágenes conceptuales revisadas por el estudiante.

**Verification:**

Confirme que cada prompt visual:

- Indica que se trata de un escenario conceptual o exploratorio.
- Incluye contexto de El Salvador sin convertirlo en un estereotipo.
- No afirma adopción, regulación o resultados como hechos.
- No incluye datos personales, marcas, logotipos o rostros reales identificables.
- Representa al menos un beneficio y una condición de seguridad, apoyo, accesibilidad o transparencia.
- Puede vincularse claramente con uno de los escenarios documentados.

### Paso 5: Evaluar inclusión, riesgo y factibilidad

**Objetivo:** Seleccionar el escenario más inclusivo y factible mediante criterios transparentes, sin confundir preferencia personal con evidencia confirmada.

**Instrucciones:**

1. Agregue una sección titulada `## Evaluación comparativa de escenarios` en el archivo Markdown.
2. Evalúe cada escenario usando una escala de 1 a 5, donde:
   - `1` significa condición débil, incierta o con riesgo alto no mitigado.
   - `3` significa condición posible pero dependiente de validación o mejoras.
   - `5` significa condición relativamente sólida, inclusiva y factible bajo los supuestos identificados.
3. No interprete una puntuación alta como garantía. La puntuación solo ayuda a comparar hipótesis bajo criterios definidos.
4. Use la siguiente matriz:

   ```markdown
   | Criterio | Escenario 1 | Escenario 2 | Escenario 3, si aplica | Evidencia o supuesto principal |
   |---|---:|---:|---:|---|
   | Accesibilidad para personas con conectividad, dispositivos o habilidades diversas | [1-5] | [1-5] | [1-5] | [Fuente o supuesto] |
   | Claridad de costos, consentimiento y experiencia de usuario | [1-5] | [1-5] | [1-5] | [Fuente o supuesto] |
   | Protección ante fraude, errores y reclamos | [1-5] | [1-5] | [1-5] | [Fuente o supuesto] |
   | Factibilidad operativa para comercios y proveedores | [1-5] | [1-5] | [1-5] | [Fuente o supuesto] |
   | Valor para usuarios y pequeños comercios | [1-5] | [1-5] | [1-5] | [Fuente o supuesto] |
   | Riesgo de exclusión o brecha de acceso | [1-5] | [1-5] | [1-5] | [Fuente o supuesto] |
   | Dependencia de cambios regulatorios o tecnológicos no confirmados | [1-5] | [1-5] | [1-5] | [Fuente o supuesto] |
   | Total orientativo | [Suma] | [Suma] | [Suma] | No equivale a una predicción. |
   ```

5. Consulte a Copilot para revisar la coherencia de la matriz, no para sustituir su juicio ni verificar regulación. Puede utilizar este prompt:

   ```text
   Revisa la coherencia de esta matriz de evaluación de escenarios financieros digitales en El Salvador. No inventes datos, regulación, estadísticas ni hechos de mercado. Identifica:
   1. Posibles contradicciones entre beneficios y riesgos.
   2. Criterios de inclusión que podrían faltar.
   3. Supuestos que deben convertirse en preguntas de investigación.
   4. Frases que parezcan presentar una hipótesis como hecho.

   Matriz:
   [Pegue aquí su matriz y un resumen breve de los escenarios.]
   ```

6. Revise las sugerencias y acepte únicamente las que sean coherentes con sus artefactos previos.
7. Documente su decisión usando este formato:

   ```markdown
   ## Escenario seleccionado

   **Escenario seleccionado:** [Nombre]  
   **Decisión:** Se selecciona como escenario prioritario para investigación y diseño, no como pronóstico ni compromiso de implementación.

   **Justificación:**
   - Inclusión: [Explique cómo considera conectividad, habilidades, costo, accesibilidad o apoyo.]
   - Factibilidad: [Explique qué condiciones operativas parecen razonables y cuáles requieren evidencia.]
   - Perspectivas de actores: [Explique cómo incorpora usuarios, comercios, instituciones y autoridades.]
   - Riesgo y protección: [Explique riesgos y mitigaciones necesarias.]
   - Competencia y propuesta de valor: [Explique cómo se relaciona con el análisis previo sin afirmar ventajas no verificadas.]

   **Condiciones mínimas antes de avanzar:**
   - [Condición 1]
   - [Condición 2]
   - [Condición 3]
   ```

**Expected output:**

Una matriz comparativa con criterios de inclusión, protección, factibilidad y riesgo, seguida de una selección justificada de un escenario prioritario.

**Verification:**

La selección cumple los requisitos si:

- Se identifica un escenario con nombre.
- La decisión se presenta como priorización para investigación, no como pronóstico.
- La justificación menciona inclusión, factibilidad, actores y riesgos.
- Se declaran al menos tres condiciones mínimas que deben cumplirse antes de tomar una decisión real.
- Las puntuaciones están acompañadas por evidencia disponible o por un supuesto identificado.

### Paso 6: Documentar preguntas de investigación y cerrar la evidencia

**Objetivo:** Transformar los escenarios en un registro de seguimiento verificable que guíe futuras consultas, validaciones y decisiones responsables.

**Instrucciones:**

1. Agregue al final del archivo la sección `## Preguntas de investigación pendientes`.
2. Documente entre cinco y ocho preguntas. Cada pregunta debe ser específica, investigable y asociada a una fuente o método de validación.
3. Priorice preguntas relacionadas con regulación vigente, protección al consumidor, interoperabilidad, costos, conectividad, accesibilidad, fraude, adopción y soporte.
4. Use el siguiente formato:

   ```markdown
   | Pregunta pendiente | Por qué importa | Fuente o método de validación sugerido | Prioridad | Estado |
   |---|---|---|---|---|
   | ¿Qué disposiciones oficiales vigentes aplican al servicio o canal analizado? | Evita asumir requisitos regulatorios. | Sitio oficial de la autoridad competente; publicación normativa vigente. | Alta | Pendiente |
   | ¿Qué costos reales enfrentan usuarios y pequeños comercios? | Determina viabilidad e inclusión. | Tarifarios oficiales, condiciones publicadas y entrevistas controladas. | Alta | Pendiente |
   | ¿Qué mecanismos de reclamo y recuperación existen ante fraude o error? | Afecta confianza y protección al consumidor. | Términos oficiales, canales de soporte y fuentes regulatorias. | Alta | Pendiente |
   | ¿Qué grupos podrían quedar excluidos por conectividad o tipo de dispositivo? | Permite diseñar mitigaciones de inclusión. | Investigación de usuarios, encuestas y datos públicos confiables. | Media | Pendiente |
   | ¿Qué señales indicarían adopción sostenible y no solo uso ocasional? | Distingue interés inicial de valor continuo. | Métricas verificables, estudios y evidencia operativa. | Media | Pendiente |
   ```

5. Agregue una conclusión breve y responsable:

   ```markdown
   ## Conclusión

   Los escenarios elaborados permiten comparar posibilidades sobre la evolución de los servicios financieros digitales en El Salvador sin tratarlas como predicciones. El escenario seleccionado se considera una prioridad de investigación porque combina una oportunidad de inclusión con condiciones de factibilidad identificables. Antes de cualquier decisión comercial, operativa, financiera o regulatoria, deben validarse las preguntas pendientes mediante fuentes oficiales vigentes, evidencia de usuarios y revisión humana especializada.
   ```

6. Guarde el archivo.
7. Ejecute la comprobación final:

   ```powershell
   $LabPath = "C:\CopilotLabs\Batch1"
   $FinalEvidence = Join-Path $LabPath "05_escenarios_financieros_el_salvador.md"

   Write-Host "`nArchivo final:" -ForegroundColor Cyan
   Get-Item $FinalEvidence | Select-Object Name, Length, LastWriteTime

   Write-Host "`nSecciones encontradas:" -ForegroundColor Cyan
   Select-String -Path $FinalEvidence -Pattern `
     "^## Insumos integrados", `
     "^## Escenarios exploratorios", `
     "^## Visuales conceptuales", `
     "^## Evaluación comparativa", `
     "^## Escenario seleccionado", `
     "^## Preguntas de investigación", `
     "^## Conclusión" |
     Select-Object LineNumber, Line

   Write-Host "`nArchivos de evidencia disponibles:" -ForegroundColor Cyan
   Get-ChildItem -Path $LabPath -File |
     Where-Object { $_.Name -match "^(01_|02_|03_|04_|05_)" } |
     Select-Object Name, Length |
     Format-Table -AutoSize
   ```

**Expected output:**

Un documento final completo en Markdown que contiene escenarios, prompts visuales, evaluación comparativa, decisión justificada, condiciones mínimas y preguntas de investigación pendientes.

**Verification:**

La práctica está completa si el archivo `C:\CopilotLabs\Batch1\05_escenarios_financieros_el_salvador.md` incluye:

- Dos o tres escenarios exploratorios completos.
- Un horizonte temporal explícito en cada escenario.
- Usuarios, servicio o canal, beneficios, barreras, riesgos, actores, supuestos y señales de validación.
- Dos prompts visuales responsables o sus imágenes conceptuales asociadas.
- Una matriz de evaluación comparativa.
- Un escenario seleccionado con justificación.
- Cinco o más preguntas de investigación con método o fuente sugerida.
- Una conclusión que no presente escenarios como predicciones o hechos confirmados.

## Validación y Pruebas

Realice la siguiente validación final antes de entregar la evidencia.

| Prueba | Resultado esperado | Estado |
|---|---|---|
| Ubicación de la evidencia | El archivo final está en `C:\CopilotLabs\Batch1\`. | [ ] |
| Integración de artefactos | El documento menciona hallazgos de inclusión, pagos, perspectivas y competencia. | [ ] |
| Escenarios completos | Existen dos o tres escenarios con todos los campos requeridos. | [ ] |
| Lenguaje responsable | Se usan términos condicionales y se distinguen hipótesis de hechos. | [ ] |
| Validación humana | Los supuestos, fuentes pendientes y condiciones mínimas están documentados. | [ ] |
| Representación visual | Hay al menos dos prompts visuales responsables o visuales conceptuales asociados. | [ ] |
| Inclusión financiera | Se consideran conectividad, dispositivos, habilidades, costos, accesibilidad o soporte. | [ ] |
| Riesgo y protección | Se incluyen fraude, errores, reclamos, transparencia o exclusión potencial. | [ ] |
| Preguntas pendientes | Se registran cinco o más preguntas investigables. | [ ] |
| Información sensible | No se incluyeron datos reales de clientes, credenciales, cuentas ni documentos personales. | [ ] |

Ejecute también la siguiente prueba de contenido:

```powershell
$FinalEvidence = "C:\CopilotLabs\Batch1\05_escenarios_financieros_el_salvador.md"

$RequiredPhrases = @(
    "Escenarios exploratorios",
    "Horizonte temporal",
    "Señales de validación",
    "Supuestos",
    "Preguntas de investigación",
    "Conclusión"
)

foreach ($Phrase in $RequiredPhrases) {
    if (Select-String -Path $FinalEvidence -Pattern $Phrase -Quiet) {
        Write-Host "VALIDADO: $Phrase" -ForegroundColor Green
    } else {
        Write-Host "REVISAR: falta o no coincide -> $Phrase" -ForegroundColor Yellow
    }
}
```

Si falta una frase por diferencias de redacción, revise manualmente que la sección equivalente exista y que su contenido cumpla el objetivo.

## Solución de Problemas

1. **Síntoma:** Copilot responde con cifras, regulaciones, fechas de implementación o niveles de adopción sin enlaces oficiales claros, o presenta afirmaciones futuras como si fueran hechos.  
   **Causa probable:** El modelo generativo completó información plausible sin contar con evidencia verificable o actualizada.  
   **Corrección:** No copie la afirmación como hecho. Etiquétela como “requiere validación”, elimínela si no es necesaria o verifíquela mediante una fuente oficial vigente. Reformule el prompt con instrucciones explícitas como: “No inventes regulación, estadísticas ni adopción; separa hechos confirmados, supuestos y preguntas pendientes”.

2. **Síntoma:** La opción de generar imágenes no aparece en Copilot, la imagen tarda demasiado o el resultado incluye elementos inapropiados, marcas o mensajes que parecen promesas.  
   **Causa probable:** La disponibilidad de funciones visuales depende de la cuenta, región, políticas de la experiencia web o capacidad temporal del servicio; además, el prompt puede ser insuficientemente específico.  
   **Corrección:** Documente el prompt y una descripción visual detallada en el archivo Markdown; no es obligatorio generar una imagen para completar el análisis. Si vuelve a intentarlo, solicite explícitamente “ilustración conceptual”, “sin logotipos”, “sin datos personales”, “sin cifras inventadas” y “escenario sujeto a validación”.

## Limpieza

No elimine los archivos de evidencia requeridos, ya que forman parte del portafolio del batch. Cierre las pestañas de Copilot y Visual Studio Code cuando termine.

Si descargó imágenes temporales que no serán utilizadas, elimínelas solo después de confirmar que no son evidencia requerida. Conserve, como mínimo, los seis archivos obligatorios del batch y cualquier imagen conceptual que haya citado en el documento final.

Ejecute este comando para revisar los archivos que permanecerán:

```powershell
Get-ChildItem -Path "C:\CopilotLabs\Batch1" -File |
    Select-Object Name, Length, LastWriteTime |
    Sort-Object Name |
    Format-Table -AutoSize
```

No guarde credenciales, capturas con sesiones iniciadas, datos personales ni información real de clientes en el directorio del laboratorio.

## Resumen

En esta práctica creó escenarios visuales exploratorios sobre posibles evoluciones de los servicios financieros digitales en El Salvador. Integró oportunidades de inclusión, experiencias de pago, perspectivas de actores, riesgos y diferenciadores competitivos para comparar alternativas de manera responsable.

La evidencia principal es:

```text
C:\CopilotLabs\Batch1\05_escenarios_financieros_el_salvador.md
```

Recuerde que el valor del ejercicio no depende de acertar el futuro. Depende de hacer explícitos los supuestos, identificar riesgos y barreras, considerar perspectivas diversas, formular preguntas verificables y mantener revisión humana antes de tomar decisiones con implicaciones financieras, comerciales, regulatorias o legales.
