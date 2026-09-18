# Práctica. Diferentes perspectivas ante la evolución de los servicios financieros digitales

## Metadatos

| Duration | Complexity | Bloom level |
|---|---|---|
| 15 minutos | Media | Aplicar |

## Descripción General

En esta práctica analizará la evolución de un servicio de pagos digitales desde cinco perspectivas: usuario potencialmente excluido, pequeño comercio, institución financiera, regulador y organización de protección al consumidor. Usará Microsoft Copilot para generar argumentos contrastantes, diferenciando claramente entre perspectivas, hipótesis, riesgos y hechos verificables. El resultado será un mapa estructurado de perspectivas que servirá como insumo para el Laboratorio 04-00-01.

## Objetivos de Aprendizaje

- [ ] Analizar un servicio financiero digital desde las perspectivas de cinco partes interesadas.
- [ ] Diferenciar opiniones, necesidades percibidas e hipótesis de hechos que requieren evidencia verificable.
- [ ] Identificar coincidencias, tensiones y riesgos relacionados con inclusión, seguridad, privacidad, confianza y regulación.
- [ ] Usar Microsoft Copilot de forma responsable para estructurar argumentos contrastantes sin presentar contenido generado como evidencia oficial.
- [ ] Crear y guardar el archivo `03_mapa_perspectivas_servicios_financieros.md` en el directorio de evidencias establecido.

## Prerrequisitos

**Conocimientos requeridos**

- Haber completado el Laboratorio 02-00-01 y contar con la comparación de experiencias de pagos digitales.
- Reconocer la diferencia entre:
  - **Hecho verificable:** afirmación que puede confirmarse con una fuente oficial, un documento normativo, una política publicada o datos confiables.
  - **Perspectiva u opinión:** valoración, preocupación o expectativa de una parte interesada.
  - **Hipótesis:** posibilidad que requiere investigación, validación o evidencia adicional.
- Comprender que las respuestas de Copilot pueden contener errores, información incompleta o referencias no actualizadas.

**Acceso requerido**

- Cuenta personal de Microsoft activa.
- Acceso a Microsoft Copilot en [https://copilot.microsoft.com/](https://copilot.microsoft.com/).
- Acceso al archivo o imagen generado en el Laboratorio 02:
  - `02_comparacion_pagos_digitales.md`
  - `02_comparacion_pagos_digitales.png`
- Permisos de escritura en `C:\CopilotLabs\Batch1\`.

> **Uso responsable:** No ingrese datos reales de clientes, números de cuenta, documentos de identidad, contraseñas, información bancaria confidencial ni información interna de una institución financiera.

## Entorno de Laboratorio

| Componente | Especificación de referencia |
|---|---|
| Sistema operativo | Windows 11 Pro 23H2 o Windows 11 24H2 |
| Navegador | Microsoft Edge 128.0.2739.79 o versión compatible |
| Herramienta principal | Microsoft Copilot, experiencia web |
| Editor de archivos | Visual Studio Code 1.93.1 o editor de texto equivalente |
| Cuenta requerida | Cuenta Microsoft personal |
| Conectividad | Internet estable de al menos 10 Mbps de descarga y 2 Mbps de carga |
| Directorio obligatorio | `C:\CopilotLabs\Batch1\` |
| Contexto geográfico | El Salvador |

Abra Windows Terminal, PowerShell o Símbolo del sistema y ejecute los siguientes comandos para verificar el directorio de trabajo y los archivos previos:

```powershell
New-Item -ItemType Directory -Force -Path "C:\CopilotLabs\Batch1"
Set-Location "C:\CopilotLabs\Batch1"
Get-ChildItem
```

Debe identificar, cuando estén disponibles, los siguientes archivos del laboratorio anterior:

```text
02_comparacion_pagos_digitales.md
02_comparacion_pagos_digitales.png
```

El archivo de evidencia principal de esta práctica será:

```text
C:\CopilotLabs\Batch1\03_mapa_perspectivas_servicios_financieros.md
```

## Instrucciones Paso a Paso

### Paso 1: Revisar la comparación previa y seleccionar el servicio a analizar

**Objetivo:** Definir un servicio financiero digital concreto y mantener consistencia con la comparación realizada en el Laboratorio 02.

**Instrucciones:**

1. Abra el Explorador de archivos y navegue a:

   ```text
   C:\CopilotLabs\Batch1\
   ```

2. Abra `02_comparacion_pagos_digitales.md` o visualice `02_comparacion_pagos_digitales.png`.

3. Identifique el servicio de pagos digitales que será analizado. Use el mismo servicio comparado en el Laboratorio 02.

4. Si su comparación previa incluyó más de un servicio, seleccione uno como foco principal. Ejemplos aceptables:
   - Billetera digital para pagos en comercios.
   - Aplicación móvil de transferencias entre personas.
   - Pago mediante código QR.
   - Pago sin contacto con tarjeta o teléfono.
   - Plataforma de cobros digitales para pequeños comercios.

5. Anote una descripción neutral de una o dos líneas. Evite afirmaciones no verificadas.

   Ejemplo de descripción neutral:

   ```text
   Servicio analizado: billetera digital que permite a personas realizar pagos y transferencias desde un teléfono móvil, potencialmente utilizable en comercios que acepten pagos digitales.
   ```

6. Abra Microsoft Edge e ingrese a:

   ```text
   https://copilot.microsoft.com/
   ```

7. Inicie sesión con su cuenta Microsoft personal, si Copilot lo solicita.

**Resultado esperado:**

Debe contar con un servicio financiero digital definido y una descripción neutral basada en el trabajo del Laboratorio 02.

**Verificación:**

Confirme que puede responder las siguientes preguntas antes de continuar:

- ¿Cuál es el servicio digital seleccionado?
- ¿Qué necesidad de pago o transferencia busca resolver?
- ¿La descripción evita asegurar que el servicio cumple una regulación específica o que está disponible para todas las personas?
- ¿El servicio coincide con la comparación previa?

---

### Paso 2: Solicitar a Copilot un análisis inicial de las cinco perspectivas

**Objetivo:** Obtener una primera propuesta de argumentos contrastantes sin confundir contenido generado con evidencia comprobada.

**Instrucciones:**

1. En Copilot, cree una conversación nueva para separar esta actividad de consultas anteriores.

2. Copie y adapte el siguiente prompt. Sustituya el texto entre corchetes por el servicio seleccionado.

   ```text
   Actúa como asistente de análisis de partes interesadas para un ejercicio académico en El Salvador.

   Analiza el siguiente servicio financiero digital:
   [describa aquí el servicio seleccionado]

   Presenta cinco perspectivas separadas:
   1. Usuario potencialmente excluido, por ejemplo una persona con conectividad limitada, baja alfabetización digital, discapacidad, ingresos variables o distancia de puntos de atención.
   2. Pequeño comercio.
   3. Institución financiera o proveedor del servicio.
   4. Regulador o autoridad supervisora.
   5. Organización de protección al consumidor.

   Para cada perspectiva, incluye:
   - necesidades o intereses;
   - beneficios percibidos;
   - preocupaciones;
   - riesgos;
   - evidencia que sería necesaria para respaldar las afirmaciones.

   Reglas:
   - Distingue explícitamente entre perspectiva, hipótesis y hecho verificable.
   - No inventes leyes, cifras, regulaciones, instituciones ni requisitos de El Salvador.
   - Si se menciona regulación, indica que debe verificarse en fuentes oficiales vigentes.
   - Usa lenguaje claro y una tabla en español.
   - No presentes recomendaciones legales.
   ```

3. Revise la respuesta de Copilot. No la copie automáticamente como evidencia final.

4. Identifique al menos una afirmación de cada tipo:
   - Una **perspectiva**, por ejemplo: “un pequeño comercio puede valorar la rapidez del cobro”.
   - Una **hipótesis**, por ejemplo: “la adopción podría disminuir si la conectividad es inestable”.
   - Un **hecho que requeriría verificación**, por ejemplo: “el servicio debe cumplir determinados requisitos regulatorios”.

5. Si Copilot presenta una ley, entidad reguladora, estadística o requisito específico sin fuente clara, márquelo como:

   ```text
   Pendiente de validación con fuente oficial vigente.
   ```

6. Solicite una mejora breve si la respuesta mezcla opiniones con hechos. Puede usar este prompt:

   ```text
   Reorganiza tu respuesta en una tabla. Etiqueta cada afirmación como:
   - Perspectiva o necesidad percibida
   - Hipótesis o riesgo por investigar
   - Hecho verificable pendiente de fuente oficial

   No agregues datos, leyes o estadísticas no verificadas.
   ```

**Resultado esperado:**

Debe disponer de un borrador generado por Copilot con cinco perspectivas diferenciadas y con advertencias claras sobre la necesidad de validar hechos, normas y datos.

**Verificación:**

Compruebe que la respuesta incluye los cinco actores requeridos:

- Usuario potencialmente excluido.
- Pequeño comercio.
- Institución financiera.
- Regulador.
- Organización de protección al consumidor.

También confirme que ninguna respuesta de Copilot se considere automáticamente una fuente oficial.

---

### Paso 3: Identificar coincidencias, tensiones y decisiones responsables

**Objetivo:** Comparar los argumentos de las partes interesadas para reconocer acuerdos y conflictos relevantes.

**Instrucciones:**

1. En la misma conversación de Copilot, solicite una comparación crítica usando el siguiente prompt:

   ```text
   Con base en las cinco perspectivas anteriores, identifica:

   1. Tres coincidencias o intereses compartidos.
   2. Tres tensiones o conflictos entre actores.
   3. Decisiones que una institución financiera o proveedor debería revisar antes de ampliar el servicio en El Salvador.

   Incluye como mínimo estas tensiones:
   - conveniencia frente a privacidad;
   - innovación frente a protección al consumidor;
   - reducción de costos frente a brecha digital.

   Para cada punto, indica:
   - actores involucrados;
   - posible impacto;
   - tipo de afirmación: perspectiva, hipótesis o hecho verificable;
   - evidencia o fuente que se debería revisar.

   No afirmes cumplimiento regulatorio ni des recomendaciones legales definitivas.
   ```

2. Revise si Copilot identifica conflictos realistas. Algunos ejemplos que pueden aparecer son:
   - El usuario busca rapidez y facilidad, pero también necesita protección de sus datos.
   - El comercio busca reducir manejo de efectivo, pero puede preocuparse por comisiones, fallas técnicas o costos de aceptación.
   - La institución busca escalar el servicio, pero debe gestionar fraude, seguridad y soporte.
   - El regulador busca innovación responsable, estabilidad, transparencia y mecanismos de supervisión.
   - La organización de protección al consumidor busca información clara, reclamos accesibles y prevención de prácticas abusivas.

3. Seleccione al menos:
   - Tres coincidencias.
   - Tres tensiones.
   - Tres decisiones o acciones de revisión.

4. Para cada decisión, determine qué evidencia sería necesaria. Ejemplos:
   - Términos y condiciones publicados por el proveedor.
   - Tarifario vigente.
   - Política de privacidad.
   - Canales de reclamo y atención al cliente.
   - Documentos oficiales de autoridades competentes.
   - Información sobre accesibilidad, cobertura, conectividad o asistencia al usuario.
   - Datos verificables sobre incidentes, fraude, tiempos de atención o disponibilidad.

5. Mantenga una postura crítica: que una característica sea conveniente no significa que sea segura, accesible, justa o conforme a disposiciones vigentes.

**Resultado esperado:**

Debe contar con una lista de coincidencias, tensiones y decisiones que conecte cada argumento con los actores involucrados y con la evidencia requerida.

**Verificación:**

Verifique que sus tensiones incluyan, como mínimo, los siguientes pares de intereses:

| Tensión requerida | Ejemplo de pregunta crítica |
|---|---|
| Conveniencia frente a privacidad | ¿Qué datos se recopilan, para qué se usan y cómo puede el usuario conocer o controlar ese uso? |
| Innovación frente a protección al consumidor | ¿Qué mecanismos existen para informar comisiones, resolver reclamos y atender operaciones no reconocidas? |
| Reducción de costos frente a brecha digital | ¿Quién puede quedar excluido por falta de teléfono, conectividad, habilidades digitales o accesibilidad? |

---

### Paso 4: Construir el mapa de perspectivas en Markdown

**Objetivo:** Crear un registro estructurado, verificable y reutilizable para el Laboratorio 04.

**Instrucciones:**

1. Abra Visual Studio Code o un editor de texto.

2. Cree el archivo:

   ```text
   C:\CopilotLabs\Batch1\03_mapa_perspectivas_servicios_financieros.md
   ```

3. Copie la siguiente estructura. Reemplace los ejemplos por hallazgos adaptados a su servicio seleccionado.

   ```markdown
   # Mapa de perspectivas sobre servicios financieros digitales

   ## Servicio analizado

   **Servicio:** [nombre o descripción neutral del servicio]

   **Contexto:** El Salvador.

   **Descripción neutral:** [descripción de una o dos líneas, sin afirmar cumplimiento legal ni disponibilidad universal.]

   **Fuente de partida:** Comparación elaborada en el Laboratorio 02:
   - `02_comparacion_pagos_digitales.md`
   - `02_comparacion_pagos_digitales.png`

   ## Criterio de lectura

   - **Perspectiva:** necesidad, interés, expectativa o preocupación atribuida a un actor.
   - **Hipótesis o riesgo:** posibilidad que debe investigarse antes de tomar una decisión.
   - **Hecho verificable:** afirmación que requiere fuente oficial, documento publicado o evidencia confiable.
   - El contenido generado con Copilot es un apoyo de análisis y no sustituye fuentes oficiales, asesoría legal ni validación humana.

   ## Mapa de perspectivas

   | Actor | Necesidades o intereses | Beneficios percibidos | Preocupaciones | Riesgos o hipótesis por investigar | Evidencia requerida |
   |---|---|---|---|---|---|
   | Usuario potencialmente excluido | Acceso simple, costos comprensibles, asistencia y alternativas de uso. | Puede reducir traslados o facilitar pagos cotidianos. | Falta de conectividad, dificultad de uso, miedo a fraude o cargos no entendidos. | Algunas personas podrían quedar excluidas por falta de teléfono, datos móviles, habilidades digitales o accesibilidad. | Información de accesibilidad, requisitos técnicos, canales de apoyo, costos publicados, estudios o datos verificables de acceso. |
   | Pequeño comercio | Cobro rápido, costos previsibles, disponibilidad y soporte. | Menor manejo de efectivo y posibilidad de atender más medios de pago. | Comisiones, fallas de conexión, devoluciones, conciliación y fraude. | El beneficio económico puede variar según volumen de ventas, tarifas y conectividad. | Tarifario vigente, términos de aceptación, tiempos de liquidación, política de contracargos y soporte. |
   | Institución financiera o proveedor | Escalabilidad, seguridad, sostenibilidad operativa y confianza. | Mayor uso digital, eficiencia operativa y nuevos servicios. | Fraude, incidentes de ciberseguridad, reputación y costos de soporte. | Un crecimiento acelerado sin controles adecuados podría aumentar reclamos o pérdidas por fraude. | Políticas de seguridad publicadas, procedimientos de gestión de incidentes, indicadores internos validados y requisitos regulatorios vigentes. |
   | Regulador o autoridad supervisora | Transparencia, estabilidad, cumplimiento aplicable, prevención de riesgos y trato justo. | La digitalización puede ampliar opciones y trazabilidad cuando se implementa responsablemente. | Riesgo sistémico, fraude, publicidad engañosa, protección de datos y exclusión. | La innovación puede generar riesgos no cubiertos por procesos tradicionales de supervisión. | Normativa oficial vigente, comunicados institucionales, requisitos aplicables y documentación del proveedor. |
   | Organización de protección al consumidor | Información clara, mecanismos de reclamo, reparación y trato no discriminatorio. | Mayor variedad de opciones y potencial acceso a servicios. | Cláusulas difíciles de entender, cobros no transparentes y barreras para reclamar. | Los usuarios con menor alfabetización digital podrían tener mayor exposición a engaños o errores no detectados. | Contratos, política de privacidad, tarifarios, registros de reclamos, canales de atención y material educativo verificable. |

   ## Coincidencias entre perspectivas

   | Coincidencia | Actores relacionados | Clasificación | Evidencia o revisión necesaria |
   |---|---|---|---|
   | Necesidad de confianza y seguridad en las transacciones. | Todos los actores. | Perspectiva compartida. | Políticas de seguridad, mecanismos de autenticación, canales de reporte y documentación verificable. |
   | Necesidad de información clara sobre costos y condiciones. | Usuario, comercio, regulador y protección al consumidor. | Perspectiva compartida. | Tarifarios, contratos, términos y condiciones, material informativo vigente. |
   | Necesidad de continuidad operativa y soporte accesible. | Usuario, comercio e institución financiera. | Perspectiva compartida. | Acuerdos de servicio, canales de soporte, reportes de disponibilidad y procedimientos de contingencia. |

   ## Tensiones y conflictos

   | Tensión | Actores involucrados | Posible impacto | Clasificación | Evidencia requerida |
   |---|---|---|---|---|
   | Conveniencia frente a privacidad. | Usuario, institución financiera, regulador y protección al consumidor. | Una experiencia rápida puede requerir recolección o tratamiento de datos que el usuario no comprenda. | Riesgo e hipótesis por investigar. | Política de privacidad, consentimiento, finalidad del tratamiento y controles publicados. |
   | Innovación frente a protección al consumidor. | Institución financiera, regulador y organización de protección al consumidor. | Una función nueva puede avanzar más rápido que la comprensión del usuario o que los controles de reclamo. | Riesgo e hipótesis por investigar. | Información oficial vigente, términos del producto, mecanismos de reclamo y documentación de controles. |
   | Reducción de costos frente a brecha digital. | Comercio, usuario potencialmente excluido, institución financiera y regulador. | La reducción de efectivo puede beneficiar al comercio, pero excluir a personas sin conectividad o habilidades digitales. | Perspectiva y riesgo por investigar. | Datos de acceso, alternativas de atención, pruebas de accesibilidad y cobertura disponible. |

   ## Decisiones responsables que requieren revisión humana

   | Decisión o pregunta | Actores afectados | Evidencia mínima requerida | Estado |
   |---|---|---|---|
   | ¿El servicio comunica de forma clara costos, límites, tiempos y condiciones de uso? | Usuario, comercio y protección al consumidor. | Tarifario, términos y condiciones, comunicaciones vigentes. | Pendiente de validación. |
   | ¿Existen alternativas o apoyos para usuarios con barreras de conectividad, alfabetización digital o accesibilidad? | Usuario potencialmente excluido, regulador y organización de protección al consumidor. | Material de accesibilidad, canales alternativos, soporte y datos verificables. | Pendiente de validación. |
   | ¿Cómo se reportan y resuelven operaciones no reconocidas, errores o fraudes? | Usuario, comercio, institución financiera y regulador. | Procedimiento oficial, canales de reporte, tiempos de respuesta y documentación publicada. | Pendiente de validación. |

   ## Hechos pendientes de validación

   | Afirmación por verificar | Por qué no debe asumirse como hecho | Fuente prioritaria |
   |---|---|---|
   | Requisitos regulatorios aplicables al servicio. | Las disposiciones pueden cambiar y dependen del tipo de entidad, producto y operación. | Fuente oficial vigente de la autoridad competente en El Salvador. |
   | Tarifas, comisiones, límites y tiempos de liquidación. | Pueden variar por proveedor, producto, canal, fecha o perfil de cliente. | Tarifario y términos oficiales vigentes del proveedor. |
   | Cobertura, disponibilidad y accesibilidad efectiva. | La experiencia puede variar por zona, dispositivo, conectividad y condiciones del usuario. | Información publicada por el proveedor y evidencia verificable de pruebas o cobertura. |

   ## Conclusión

   El análisis muestra que un mismo servicio financiero digital puede ser conveniente para algunos actores y generar barreras o riesgos para otros. Antes de adoptar, promover o comparar el servicio, se requiere validar hechos con fuentes oficiales y documentación vigente, especialmente cuando existan implicaciones regulatorias, de privacidad, seguridad o protección al consumidor.
   ```

4. Revise que el contenido de la tabla sea específico para el servicio seleccionado. No deje frases genéricas si puede relacionarlas con características observables del servicio.

5. Si utiliza una afirmación obtenida de Copilot, manténgala como perspectiva, hipótesis o asunto pendiente de verificación, salvo que haya consultado una fuente confiable y actualizada.

6. Guarde el archivo con codificación UTF-8.

**Resultado esperado:**

Debe existir el archivo `03_mapa_perspectivas_servicios_financieros.md` con un mapa de cinco perspectivas, coincidencias, tensiones, decisiones responsables y hechos pendientes de validación.

**Verificación:**

En PowerShell, ejecute:

```powershell
Test-Path "C:\CopilotLabs\Batch1\03_mapa_perspectivas_servicios_financieros.md"
Get-Content "C:\CopilotLabs\Batch1\03_mapa_perspectivas_servicios_financieros.md" -TotalCount 25
```

El primer comando debe devolver:

```text
True
```

El segundo comando debe mostrar el título, la descripción del servicio y el inicio de la estructura del mapa.

---

### Paso 5: Realizar la revisión final de calidad y trazabilidad

**Objetivo:** Validar que el mapa sea útil para una decisión responsable y pueda reutilizarse en el siguiente laboratorio.

**Instrucciones:**

1. Abra nuevamente `03_mapa_perspectivas_servicios_financieros.md`.

2. Compruebe que aparecen exactamente los cinco actores requeridos:
   - Usuario potencialmente excluido.
   - Pequeño comercio.
   - Institución financiera o proveedor.
   - Regulador o autoridad supervisora.
   - Organización de protección al consumidor.

3. Revise que cada actor tenga información en las cinco categorías:
   - Necesidades o intereses.
   - Beneficios percibidos.
   - Preocupaciones.
   - Riesgos o hipótesis por investigar.
   - Evidencia requerida.

4. Confirme que el documento contiene al menos:
   - Tres coincidencias.
   - Tres tensiones.
   - Tres decisiones responsables que requieren revisión humana.
   - Tres hechos pendientes de validación.

5. Busque expresiones absolutas que deban moderarse, por ejemplo:
   - “El servicio cumple con toda la regulación.”
   - “Todos los usuarios tendrán acceso.”
   - “La aplicación es completamente segura.”
   - “No existen costos.”
   - “El regulador autoriza este producto.”

6. Reemplace afirmaciones absolutas no verificadas por redacción responsable. Ejemplos:

   | Redacción no adecuada | Redacción responsable |
   |---|---|
   | “El servicio cumple con la normativa.” | “El cumplimiento aplicable debe validarse con fuentes oficiales vigentes y documentación del proveedor.” |
   | “La aplicación protege todos los datos.” | “Las medidas de privacidad y seguridad deben revisarse en políticas, términos y evidencia técnica disponible.” |
   | “La billetera incluye a toda la población.” | “La inclusión potencial depende de conectividad, costos, accesibilidad, habilidades digitales y canales alternativos.” |

7. Guarde los cambios finales.

**Resultado esperado:**

El archivo final debe distinguir de manera visible las perspectivas de los hechos verificables y debe registrar qué fuentes se necesitan antes de adoptar una conclusión comercial, operativa o regulatoria.

**Verificación:**

Use esta lista de comprobación final:

- [ ] El archivo está guardado en `C:\CopilotLabs\Batch1\`.
- [ ] El nombre del archivo es exactamente `03_mapa_perspectivas_servicios_financieros.md`.
- [ ] El servicio analizado coincide con el servicio comparado en el Laboratorio 02.
- [ ] Se incluyen los cinco actores solicitados.
- [ ] Se incluyen necesidades, beneficios, preocupaciones, riesgos y evidencia requerida para cada actor.
- [ ] Se documentan tres coincidencias y tres tensiones.
- [ ] Se incluyen las tensiones de privacidad, protección al consumidor y brecha digital.
- [ ] Las afirmaciones regulatorias, tarifas y datos no verificados se marcan como pendientes de validación.
- [ ] No se incluyen datos reales de clientes ni información confidencial.
- [ ] El documento puede utilizarse como insumo para responder una afirmación competitiva en el Laboratorio 04.

## Validación y Pruebas

Ejecute la siguiente validación en PowerShell desde el directorio de trabajo:

```powershell
Set-Location "C:\CopilotLabs\Batch1"

$requiredFile = "03_mapa_perspectivas_servicios_financieros.md"
$requiredTerms = @(
    "Usuario potencialmente excluido",
    "Pequeño comercio",
    "Institución financiera",
    "Regulador",
    "protección al consumidor",
    "Coincidencias",
    "Tensiones",
    "Evidencia requerida",
    "Pendiente de validación"
)

if (-not (Test-Path $requiredFile)) {
    Write-Host "ERROR: No se encontró $requiredFile" -ForegroundColor Red
}
else {
    Write-Host "Archivo encontrado: $requiredFile" -ForegroundColor Green

    $content = Get-Content $requiredFile -Raw

    foreach ($term in $requiredTerms) {
        if ($content -match [regex]::Escape($term)) {
            Write-Host "OK: Se encontró '$term'" -ForegroundColor Green
        }
        else {
            Write-Host "REVISAR: No se encontró '$term'" -ForegroundColor Yellow
        }
    }
}
```

La validación técnica es satisfactoria si:

1. El archivo existe en el directorio obligatorio.
2. El archivo contiene referencias a los cinco actores.
3. El contenido incluye secciones de coincidencias, tensiones y evidencia requerida.
4. El documento incorpora el concepto de validación pendiente.

La validación académica es satisfactoria si:

| Criterio | Evidencia esperada |
|---|---|
| Análisis de perspectivas | Cada actor presenta intereses, beneficios, preocupaciones y riesgos diferenciados. |
| Pensamiento crítico | El documento muestra que una misma característica puede producir beneficios y riesgos distintos según el actor. |
| Uso responsable de IA | Copilot se utiliza como apoyo para organizar ideas, no como fuente oficial ni como asesor legal. |
| Trazabilidad | Las afirmaciones relevantes indican qué tipo de evidencia o fuente se debe consultar. |
| Aplicación al contexto | El escenario se relaciona con servicios financieros digitales y condiciones de inclusión en El Salvador. |

## Solución de Problemas

**Problema 1: Copilot presenta leyes, entidades, cifras o requisitos específicos sin una fuente verificable.**

- **Síntomas:** La respuesta menciona una norma, una estadística, una autorización o una obligación como si fuera un hecho definitivo, pero no muestra una fuente oficial vigente o la referencia parece poco clara.
- **Causa:** Los modelos generativos pueden producir información desactualizada, incompleta o incorrecta, especialmente en temas regulatorios y financieros.
- **Solución:** No copie la afirmación como hecho. Regístrela en la sección **Hechos pendientes de validación** y señale la fuente prioritaria que debería revisarse. Reformule el contenido como hipótesis o pregunta de revisión, por ejemplo: “Los requisitos regulatorios aplicables deben confirmarse con fuentes oficiales vigentes”.

**Problema 2: El archivo Markdown no aparece en el directorio obligatorio o se guardó con otro nombre.**

- **Síntomas:** El comando `Test-Path` devuelve `False`, el archivo se encuentra en Descargas, Documentos u otra carpeta, o tiene un nombre como `mapa_perspectivas.md.txt`.
- **Causa:** El editor utilizó una ubicación predeterminada diferente, ocultó extensiones conocidas o agregó automáticamente `.txt`.
- **Solución:** En el editor, use **Guardar como** y seleccione exactamente `C:\CopilotLabs\Batch1\03_mapa_perspectivas_servicios_financieros.md`. En el cuadro de guardado, seleccione el tipo **Todos los archivos** si está disponible. Después ejecute:

  ```powershell
  Get-ChildItem "C:\CopilotLabs\Batch1\03_mapa_perspectivas_servicios_financieros*"
  ```

  Si existe un archivo con extensión incorrecta, cámbiele el nombre cuidadosamente para que termine en `.md`.

## Limpieza

1. Guarde y cierre `03_mapa_perspectivas_servicios_financieros.md`.
2. Mantenga en `C:\CopilotLabs\Batch1\` todos los archivos de evidencia creados en este batch; no elimine el archivo del Laboratorio 02 ni el mapa creado en esta práctica.
3. Cierre las pestañas de Copilot que contengan borradores si ya no las necesita.
4. Cierre sesión de Microsoft Copilot únicamente si utiliza un equipo compartido autorizado para prácticas.
5. Verifique que no haya guardado información real de clientes, capturas con datos sensibles ni credenciales en el directorio de evidencias.

## Resumen

En esta práctica construyó un mapa de perspectivas sobre un servicio financiero digital en El Salvador. El análisis incorporó las necesidades y preocupaciones de usuarios potencialmente excluidos, pequeños comercios, instituciones financieras, reguladores y organizaciones de protección al consumidor.

El producto principal es:

```text
C:\CopilotLabs\Batch1\03_mapa_perspectivas_servicios_financieros.md
```

El documento será utilizado en el Laboratorio 04-00-01 para elaborar una respuesta fundamentada ante una afirmación competitiva relacionada con servicios financieros digitales. Antes de utilizar cualquier conclusión sobre regulación, seguridad, costos, privacidad o protección al consumidor, valide la información con fuentes oficiales y documentación vigente.
