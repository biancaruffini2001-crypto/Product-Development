# Nuestro primer MVP

> Versión exploratoria. Usa datos de demostración y todavía no fue probada con personas reales. No valida el producto.

- **Usuario y situación:** empleado o estudiante del AMBA que va, o podría ir, en bicicleta al trabajo o a estudiar. Antes de salir no sabe si todo su recorrido es seguro y continuo, y por eso duda o descarta la bici.
- **Valor y acción central:** reducir la incertidumbre sobre la seguridad del recorrido. La acción central es consultar el puntaje de seguridad de una ruta, compararlo con otra y elegir cuál tomaría.
- **Acceso o forma de ejecución:** página web publicada como artefacto de Claude: https://claude.ai/artifact/Vqh7b56DjMFrfjxAJDNQ6q (visible solo para quien la creó hasta que decida compartirla).
- **Recorrido:** elegir una de 3 rutas de un trayecto de ejemplo (Palermo → Microcentro) → ver puntaje, tramos, puntos y beneficios → comparar con otra ruta → elegir cuál tomaría → "¡Que comience el recorrido!" con mapa simulado, tramo por tramo.

## Funciona / manual o simulado / fuera de alcance

| Funciona hoy | Manual o simulado | Fuera de alcance |
|---|---|---|
| Elegir ruta y ver puntaje (0 a 100, verde / amarillo / rojo) y detalle de tramos | Rutas, puntajes y tramos: datos de demostración inventados | Mapa real con GPS y ubicación en vivo |
| Comparar dos rutas y registrar la elección | Puntos (10 por km en ciclovía protegida) y beneficio de empresa (vale de comida): ejemplos, sin acuerdo real | Integración real con Waze o Google Maps (solo mencionada como posible versión futura) |
| Mensajes claros si falta elegir ruta o se repite la misma | Mapa del recorrido: imagen esquemática que simula ser en vivo | Cuentas de usuario, panel de la empresa, canje real de puntos |
| Registro de consultas, comparaciones, elecciones, recorridos y puntos (en el navegador) | Recorridos terminados: simulados, no son viajes reales | Datos reales de seguridad y ciclovías |

## Evidencia disponible y duda pendiente

- **Evidencia disponible:** solo fuentes institucionales de la Clase 2 (datos oficiales sobre ciclovías, seguridad vial y conectividad). No hay entrevistas ni resultados de experimentos con personas reales. Los experimentos de Clase 4 (piloto de comportamiento) y Clase 5 (A/B de mapas) están diseñados y todavía sin datos.
- **Duda pendiente:** si ver el puntaje de seguridad cambia la ruta que elige la persona, y si los puntos y beneficios de la empresa influyen en el uso recurrente.
- **Qué medimos:** usuarios que intentan y completan la acción (consultan una ruta, comparan, eligen) y resultado útil observado (ruta elegida y recorrido iniciado). Por ahora el conteo se hace a mano con el registro de la página.

## Prueba e iteración

### Ciclo 1

- **Quién probó (rol) y tarea:** integrante del equipo (prueba interna, no es un usuario del segmento). Tarea: elegir una ruta, compararla con otra y elegir una.
- **Qué ocurrió y cómo lo sabemos:** eligió la ruta más segura tras comparar dos opciones. Lo sabemos por su relato. No es evidencia de comportamiento de usuarios reales.
- **Devolución concreta que dimos a la IA:** agregar un mapa en vivo con indicaciones de cómo ir; mostrar beneficios al lado de cada ruta; tras elegir, mostrar "¡Que comience el recorrido!" con el mapa.
- **Cambio realizado y resultado de la nueva prueba:** se agregaron beneficios por ruta y la pantalla de recorrido con mapa esquemático y guía por tramos. El mapa en vivo real no se incluyó: requiere datos reales de calles y ciclovías y permisos de ubicación. Nueva prueba: **pendiente**.

### Ciclo 2

- **Quién probó (rol) y tarea:** integrante del equipo. Tarea: revisar opciones de ruta con puntos y beneficios de empresa y el mapa simulado.
- **Devolución concreta que dimos a la IA:** incluir los beneficios que los trabajadores obtendrían en sus empresas o los puntos acumulados por elegir cada ruta; usar una imagen de mapa que simule ser en vivo y aclarar que podría asociarse con aplicaciones de tránsito como Waze o Google Maps.
- **Cambio realizado y resultado de la nueva prueba:** cada ruta muestra puntos y un beneficio de ejemplo; el mapa simulado incluye la aclaración sobre Waze y Google Maps. Nueva prueba: **pendiente**.

### Prueba entre pares

- **Pendiente:** que otra persona complete la tarea sin instrucciones paso a paso. Registrar resultado, obstáculos y ayudas necesarias. Una prueba entre compañeros no equivale a validación con usuarios del segmento.

### Próximo ajuste

- Registrar los resultados de la prueba entre pares y corregir una prioridad por ciclo.
- Probar con usuarios reales del segmento (empleados y estudiantes del AMBA) cuando el MVP esté terminado y completar las secciones de resultados de los experimentos de Clase 4 y 5.
