# Clase 8 · Pruebas y mejoras del MVP

> **Estado: borrador en modo anticipación.** El plan de medición está definido como propuesta para que el equipo lo confirme. El registro de pruebas, la comparación y la prioridad quedan **sin completar** hasta tener participantes reales. No hay resultados inventados.

## Contexto

- **Equipo:** por completar
- **Fecha:** 19/10/2026 (inicio del documento)
- **Usuario y problema:** empleado o estudiante del AMBA que va, o podría ir, en bicicleta al trabajo o a estudiar. Antes de salir no sabe si todo su recorrido es seguro y continuo, y por eso duda o descarta la bici.
- **MVP:** página web publicada como artefacto de Claude: https://claude.ai/artifact/Vqh7b56DjMFrfjxAJDNQ6q
- **Versión a probar:** `V2` (Ciclo 2 de `mvp.md`: beneficios y puntos por ruta, mapa esquemático simulado). Si se cambia, se etiqueta `V3`, etc.
- **Pendiente antes de probar:** el enlace es visible solo para quien creó el artefacto. Esto bloqueó la Ronda 0. Hay que compartirlo y verificar, desde otra cuenta o dispositivo, que se abra.

## Tarea, finalización y ayuda

**Tarea (sin indicar botones ni pasos):**
"Mañana tenés que ir de Palermo al Microcentro en bici y querés decidir por qué ruta ir."

- **Inicio:** la persona abre la página sin ninguna explicación del recorrido.
- **Resultado observable (tarea completada):** la persona elige una ruta y la elección queda registrada en la página.
- **Qué se observa por separado (no define el éxito):** si consultó el puntaje, si comparó dos rutas y si pudo explicar por qué eligió esa.
- **Qué cuenta como ayuda:** cualquier indicación del equipo sobre dónde mirar, tocar o qué significa algo (incluso un gesto o una pista). Aclarar el contexto o la consigna al inicio no cuenta como ayuda.
- **Cierre del intento:** éxito (elige ruta), abandono (la persona dice que no puede o no quiere seguir) o límite de 5 minutos *(a confirmar por el equipo)*.

## Qué es real, manual o simulado

| Real / funcional | Manual o simulado |
|---|---|
| Elegir ruta, ver puntaje 0–100 con colores, detalle de tramos, comparar dos rutas, mensajes de error | Rutas, puntajes y tramos: datos de demostración inventados |
| Registro de consultas, comparaciones y elecciones en el navegador | Puntos, beneficio de empresa y mapa del recorrido: ejemplos y simulación |
| | "Recorridos terminados": simulados, no son viajes reales |

**Consecuencia para la medición:** la prueba puede mostrar si la persona entiende y usa la interfaz. No puede mostrar que ande más en bici, que se sienta más segura en la calle ni que los puntos o beneficios la motiven. Los datos de seguridad no son reales, así que el puntaje no es información confiable para decidir un recorrido real.

## Plan de medición

> Los criterios son una propuesta exploratoria, no una regla. El equipo debe confirmarlos o ajustarlos **antes** de probar.

| Métrica | Fórmula / unidad | Fuente y momento | Criterio exploratorio (propuesto) | Decisión que informa |
|---|---|---|---|---|
| **Éxito** | Participantes que completan la tarea / participantes que la intentan (primer intento por persona y versión). | Observación directa durante la prueba, confirmada con el registro de la página. | Al menos 4 de 5 completan. | Si pocos completan: revisar qué impide llegar a elegir ruta (acceso, consigna, interfaz) antes de agregar funciones. |
| **Autonomía** | Participantes que completan sin ayuda / participantes que intentan. | Observación; cada ayuda se anota con el momento y la causa. | Al menos 4 de 5 completan sin ayuda. | Si muchos necesitan ayuda: mejorar textos, orden o señales de la pantalla donde se pidió. |
| **Valor** (proxy) | Participantes que dicen que, con el puntaje, saben qué ruta elegir y por qué: valor 1–5 a "¿qué tan seguro/a estás de tu elección de ruta?" + respuesta a "¿qué ruta habrías elegido sin el puntaje?". | Pregunta oral al terminar la tarea, anotada por quien registra. | Exploratorio: al menos 4 de 5 contestan 4 o 5 y explican la elección con el puntaje o los tramos. | Si el puntaje no explica la elección: revisar si se entiende o si pesan otros factores (tiempo, beneficios). |
| **Valor real** (no medido) | Cambio en la ruta elegida o en viajes en bici reales por semana. | Prueba posterior en contexto real (pilotos de Clase 4 y 5). | Se define cuando existan datos reales de rutas. | Si el puntaje cambia la decisión en contexto real, justificar construir datos reales. Hoy: **no medido**. |

**Reglas de registro**

- Se cuenta el primer intento por persona y versión; los reintentos se anotan aparte.
- Se incluyen abandonos y fallas. Si nadie intentó se escribe "no medido", no 0 %.
- Se informa como "3 de 5", sin generalizar a todos los usuarios.
- La respuesta de valor es un **proxy** basado en lo que la persona dice. No es una medida de comportamiento.

## Registro de pruebas

Meta: 3 a 5 participantes por ronda, con roles de facilitación, observación y registro. Si son menos, anotar cuántos y la limitación. Identificar a las personas como U1, U2, etc., sin datos personales.

### Ronda 0 · V2 · acceso bloqueado

Tres personas de 19 años intentaron probar el MVP y no pudieron usarlo porque el artefacto era privado. El feedback que dieron está pendiente de registrar textual.

| ID | ¿Pertenece al segmento? | Versión | ¿Intentó? | ¿Completó? | ¿Sin ayuda? | Valor (1–5 y ruta sin puntaje) / no medido | Dificultad y ayuda recibida |
|---|---|---|---|---|---|---|---|
| R0-U1 | Por confirmar | V2 | Sí | No | No | No medido | No pudo acceder (artefacto privado). Feedback: por completar |
| R0-U2 | Por confirmar | V2 | Sí | No | No | No medido | No pudo acceder (artefacto privado). Feedback: por completar |
| R0-U3 | Por confirmar | V2 | Sí | No | No | No medido | No pudo acceder (artefacto privado). Feedback: por completar |

**Resumen Ronda 0:** éxito 0 de 3, autonomía 0 de 3, valor no medido. La causa registrada es de acceso, no de diseño: no dice nada todavía sobre si la tarea es comprensible ni si el puntaje sirve.

### Ronda 1 · tras corregir el acceso

| ID | ¿Pertenece al segmento? | Versión | ¿Intentó? | ¿Completó? | ¿Sin ayuda? | Valor (1–5 y ruta sin puntaje) / no medido | Dificultad y ayuda recibida |
|---|---|---|---|---|---|---|---|
| R1-U1 | Por completar | V3 | Por completar | Por completar | Por completar | Por completar | Por completar |
| R1-U2 | Por completar | V3 | Por completar | Por completar | Por completar | Por completar | Por completar |
| R1-U3 | Por completar | V3 | Por completar | Por completar | Por completar | Por completar | Por completar |

**Preguntas al terminar:** ¿Qué esperabas encontrar? ¿Qué te resultó confuso? ¿Qué te hizo elegir esa ruta?

**Límites a recordar:** los compañeros fuera del segmento sirven para detectar dificultades de uso. No muestran demanda ni valor para empleados y estudiantes que van en bici. Las pruebas con IA o datos sintéticos verifican funcionamiento y no cuentan como participantes.

## Aprendizaje e iteración

> Se completa con el registro real.

- **Hechos observados:** en la Ronda 0, 3 de 3 personas de 19 años intentaron y ninguna pudo acceder al MVP porque el artefacto era privado. Feedback de ese intento: por completar.
- **Posibles causas (a comprobar):** el acceso quedó configurado como privado; no se verificó antes de la prueba que otra persona pudiera abrir el enlace.
- **Dificultad priorizada y justificación:** acceso al MVP. Bloquea la tarea completa, apareció en 3 de 3 intentos y es de bajo esfuerzo de corregir. Decisión del equipo: por confirmar.
- **Pedido a la IA y alternativas discutidas:** por completar
- **Decisión del equipo:** por completar
- **Cambio realizado y versión (con punto de recuperación):** por completar
- **Verificación técnica** (recorrido principal + un caso de error): por completar

**Aspectos a mirar durante la prueba** (no son hallazgos, solo puntos a observar):

- Si la persona entiende qué significa el puntaje y los colores sin explicación.
- Si distingue "elegir una ruta" de "iniciar el recorrido" y qué espera que pase después.
- Si los mensajes de error (falta elegir, misma ruta repetida) se entienden.
- Si puntos y beneficios aparecen antes que el puntaje o lo opacan.

## Comparación antes / después

| Métrica | Antes (n y resultado) | Después (n y resultado) | Interpretación y límites |
|---|---|---|---|
| Éxito | 0 de 3 (Ronda 0, V2) | Por completar (Ronda 1, V3) | Antes: falla de acceso, no de uso. Comparar con cuidado. |
| Autonomía | 0 de 3 (Ronda 0, V2) | Por completar (Ronda 1, V3) | Igual que éxito. |
| Valor (proxy) | No medido | Por completar / no medido | Nadie vio el puntaje en la Ronda 0. |

**Condiciones de la segunda ronda:** misma tarea y mismas definiciones, con personas nuevas del mismo perfil. Si participan las mismas, indicar que ya conocen el recorrido. Registrar cambios de dispositivo, segmento o instrucciones. La comparación es exploratoria y no prueba que el cambio causó el resultado.

## Próximo paso

- **Incertidumbre pendiente:** si el puntaje de seguridad cambia la ruta que elige la persona y si eso ocurre con datos reales.
- **Acción más barata:** correr la primera ronda con 3 a 5 personas (idealmente del segmento) usando la tarea definida.
- **Responsable y momento:** por completar
- **Qué observar y qué decidir según el resultado:**
  - Si la mayoría completa sin ayuda y el puntaje explica la elección: pasar a una prueba más exigente con datos reales de una ruta concreta.
  - Si no completan o necesitan ayuda: priorizar una dificultad de uso y repetir la prueba.
  - Si no aparecen dificultades relevantes: justificar mantener la versión y ampliar la prueba de valor.
