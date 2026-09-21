# Práctica. ¿Qué responder cuando un cliente afirma que la competencia tiene una mejor opción?

Esta práctica utiliza información pública y actualizada para contrastar la Cuenta de Ahorro Digital de Bancoagrícola con una alternativa digital de otra institución financiera. El objetivo es construir una respuesta equilibrada y sustentada, diferenciando lo que puede demostrarse de lo que todavía requiere información adicional.

## Metadatos

| Campo | Detalle |
|---|---|
| Duración | 17 min |
| Complejidad | Media |
| Nivel de Bloom | Evaluar |
| Tipo de actividad | Investigación, contraste de evidencia y respuesta al cliente |
| Aplicaciones | Microsoft Copilot Chat |
| Modalidad | Individual, guiada |
| Insumos previos | Ninguno |
| Resultado | Comparación sustentada y respuesta equilibrada al cliente |

## Distribución de tiempo

| Fase | Actividad | Tiempo |
|---|---|---:|
| 1 | Identificar la alternativa y las fuentes oficiales | 4 min |
| 2 | Contrastar la afirmación del cliente | 8 min |
| 3 | Construir una respuesta equilibrada | 5 min |
| **TOTAL** |  | **17 min** |

## Descripción general

El cliente afirma que una alternativa digital de otra institución financiera es más conveniente que la Cuenta de Ahorro Digital de Bancoagrícola. Usarás Copilot para encontrar información pública vigente de ambos productos, comparar características, beneficios, requisitos y posibles limitaciones, y distinguir qué argumentos pueden respaldarse con fuentes oficiales.

## Objetivos de aprendizaje

- Investigar información pública vigente priorizando fuentes oficiales.
- Contrastar argumentos a favor y en contra de una afirmación.
- Identificar cuándo la evidencia disponible es insuficiente para sostener una conclusión.
- Redactar una respuesta equilibrada sin presentar ventajas no demostradas como hechos.

## Escenario de la práctica

Un cliente compara la Cuenta de Ahorro Digital de Bancoagrícola con una alternativa digital ofrecida por otra institución financiera y afirma que la opción de la competencia es más conveniente. La alternativa competidora no está definida previamente: debe seleccionarse durante la práctica entre productos que puedan verificarse mediante información pública vigente.

## Prerrequisitos

- Conocimientos básicos de Copilot y prompting.
- Acceso a Internet y Microsoft Copilot Chat.
- No se requiere Microsoft 365 Copilot Premium.

## Preparación del entorno

1. Abre `https://copilot.cloud.microsoft/chat` o el acceso equivalente de tu organización.
2. Confirma que Copilot puede consultar información pública de la Web.
3. Inicia una conversación nueva.
4. No introduzcas datos reales de clientes.

## Desarrollo de la práctica

### Fase 1 - Identificar la alternativa y las fuentes oficiales

**Tiempo:** 4 min  
**Aplicación:** Microsoft Copilot Chat  
**Objetivo:** establecer qué dos productos se compararán y con qué evidencia.

### Paso 1. Localiza las fuentes

> **PROMPT 1 - LOCALIZAR PRODUCTOS Y FUENTES OFICIALES**

```text
Necesito comparar la Cuenta de Ahorro Digital de Bancoagrícola con una alternativa digital ofrecida por otra institución financiera y disponible para clientes en El Salvador. La alternativa debe ser razonablemente comparable por propósito de uso y contar con información pública suficiente.

1. Localiza la página oficial vigente de la Cuenta de Ahorro Digital de Bancoagrícola.
2. Identifica hasta 2 alternativas de otras instituciones financieras que puedan compararse razonablemente con ese producto.
3. Para cada alternativa incluye el enlace oficial y confirma si la fuente indica que está disponible en El Salvador.
4. No uses blogs, comparadores comerciales ni publicaciones de terceros como fuente principal.
5. Si la disponibilidad o vigencia no puede confirmarse, indícalo como “pendiente de confirmar”.

No realices todavía la comparación detallada.
```

### Paso 2. Selecciona la alternativa

Elige una alternativa con fuente oficial vigente y disponibilidad suficientemente clara. Si ninguna cumple, pide a Copilot una nueva búsqueda.

**Criterio de finalización:** tienes dos enlaces oficiales: uno para Bancoagrícola y otro para la alternativa seleccionada.

### Fase 2 - Contrastar la afirmación del cliente

**Tiempo:** 8 min  
**Aplicación:** Microsoft Copilot Chat  
**Objetivo:** reunir evidencia a favor y en contra de la afirmación “la competencia es más conveniente”.

### Paso 3. Ejecuta la comparación basada en evidencia

> **PROMPT 2 - CONTRASTAR LA AFIRMACIÓN**

```text
Compara la Cuenta de Ahorro Digital de Bancoagrícola con la alternativa seleccionada usando prioritariamente las páginas oficiales encontradas.

Analiza:
- características principales;
- beneficios publicados;
- requisitos de apertura o elegibilidad;
- costos, comisiones o montos mínimos cuando la fuente los publique;
- canales de uso disponibles;
- posibles limitaciones o condiciones relevantes;
- cualquier información pública que sea necesaria para interpretar la conveniencia del producto.

Organiza el resultado en 3 secciones:

A. Evidencia que podría respaldar la afirmación del cliente de que la alternativa resulta más conveniente.
B. Evidencia que podría matizar o contradecir esa afirmación.
C. Información que no puede determinarse con las fuentes públicas disponibles y que sería necesario confirmar.

Para cada afirmación incluye:
- producto al que se refiere;
- dato o condición;
- enlace de la fuente oficial;
- fecha de consulta o fecha de publicación cuando esté disponible;
- estado: “respaldado por fuente” o “requiere información adicional”.

Reglas:
- No inventes tasas, costos, requisitos, promociones ni disponibilidad.
- No conviertas lenguaje promocional de una institución en una ventaja objetiva sin explicarlo.
- No concluyas que un producto es mejor en términos generales.
```

### Paso 4. Verifica la evidencia

Abre al menos los dos enlaces principales y comprueba que las páginas respaldan los datos más importantes de la comparación. Si un dato no aparece en la fuente, pide a Copilot que lo elimine o lo marque como pendiente.

**Criterio de finalización:** la comparación contiene evidencia tanto a favor como para matizar la afirmación y separa claramente los puntos que requieren información adicional.

### Fase 3 - Construir una respuesta equilibrada

**Tiempo:** 5 min  
**Aplicación:** Microsoft Copilot Chat  
**Objetivo:** transformar la comparación en una respuesta útil para la conversación con el cliente.

### Paso 5. Redacta la respuesta

> **PROMPT 3 - RESPUESTA AL CLIENTE**

```text
A partir únicamente de la comparación anterior, redacta una respuesta para un cliente que afirma: “la competencia tiene una mejor opción”.

La respuesta debe:
- reconocer la afirmación sin desacreditar a la competencia;
- mencionar 2 o 3 diferencias que sí estén respaldadas por fuentes públicas;
- explicar que la conveniencia depende de los criterios que el cliente valore;
- señalar de forma transparente cualquier información que no pueda confirmarse;
- incluir 2 preguntas breves para entender qué significa “más conveniente” para ese cliente;
- evitar recomendaciones financieras personalizadas;
- evitar afirmar superioridad cuando la evidencia no la demuestra.

Extensión máxima: 140 palabras.
```

### Paso 6. Haz la revisión final

Asegúrate de que cada diferencia mencionada en la respuesta pueda rastrearse a la comparación anterior. Elimina cualquier ventaja no sustentada.

**Criterio de finalización:** existe una respuesta breve que orienta la conversación con evidencia y reconoce sus límites.

## Validación y pruebas finales

| # | Criterio | Estado |
|---|---|---|
| 1 | Se compara la Cuenta de Ahorro Digital de Bancoagrícola con una alternativa real identificada durante la práctica. | ☐ |
| 2 | Hay una fuente oficial para cada producto. | ☐ |
| 3 | La comparación incluye características, beneficios, requisitos y posibles limitaciones. | ☐ |
| 4 | Se presentan argumentos que respaldan y que matizan la afirmación del cliente. | ☐ |
| 5 | Los vacíos de información están marcados como pendientes. | ☐ |
| 6 | La respuesta final no supera 140 palabras. | ☐ |
| 7 | La respuesta incluye exactamente 2 preguntas para aclarar la necesidad del cliente. | ☐ |
| 8 | No se presenta una ventaja no demostrada como hecho. | ☐ |

## Solución de problemas

| Situación | Qué hacer |
|---|---|
| Copilot no encuentra una alternativa con fuente oficial. | Pide otras opciones y exige una página oficial que confirme disponibilidad y características. |
| Una página oficial no muestra un costo o requisito. | No lo infieras; márcalo como información adicional requerida. |
| Copilot declara que un producto es “mejor”. | Pide que sustituya el juicio general por una explicación condicionada a criterios concretos. |
| La respuesta al cliente incluye una ventaja no presente en la comparación. | Elimina esa frase o vuelve a solicitar la redacción limitándola a la evidencia validada. |

## Limpieza y conservación

- Conserva la conversación si se utilizará durante la demostración.
- No es necesario crear archivos adicionales.
- No introduzcas información personal o confidencial de clientes.

## Resumen de la práctica

Investigaste dos productos mediante fuentes oficiales, contrastaste evidencia a favor y en contra de la afirmación del cliente y construiste una respuesta equilibrada que diferencia hechos verificables de información aún no confirmada.
