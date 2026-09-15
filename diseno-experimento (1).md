# Diseño del experimento — RutaSegura (Clase 5)

> Este documento reúne la evidencia de partida, el contrato experimental, el instrumento construido y las instrucciones de armado. Las imágenes (`trayecto1_sin_score.png`, etc.) se suben junto a este `.md` en la carpeta `experimento-clase5-mapas/`.

---

## 1. Evidencia de partida

- **Problema respaldado (Clase 2, fuentes oficiales):** las personas evitan la bici cuando no perciben el recorrido completo como seguro y continuo.
- **Estado de la hipótesis de comportamiento (Clase 4):** en validación mediante piloto Concierge de 2 semanas — resultado aún pendiente, no se usa como insumo de este experimento.
- **Incertidumbres abiertas identificadas en el pre-mortem (Clase 3):** calidad del dato de seguridad, sostenibilidad del compromiso de recompensas, privacidad de ubicación.
- **Incertidumbre elegida para este experimento:** calidad/valor del score de seguridad — ¿influye en la preferencia de ruta declarada?

## 2. Pregunta de aprendizaje

¿Las personas cambian de ruta preferida cuando ven un score de seguridad+continuidad, comparado con solo ver el mapa sin score?

(Descartadas para esta vuelta: B — confianza/privacidad al compartir ubicación; C — sostenibilidad del compromiso de recompensa del empleador. Quedan disponibles como próximas incertidumbres.)

## 3. Experimento elegido y alternativas descartadas

**Elegido: Comparación A/B con mapas estáticos.**

| Alternativa | Por qué se descartó |
|---|---|
| Wizard of Oz conversacional | Da evidencia más rica, pero no escala en el tiempo disponible (5-8 personas máx.) |
| Prototipo navegable (Figma) | Agrega construcción innecesaria para esta pregunta; riesgo de convertirse en MVP |

## 4. Contrato experimental

| Campo | Definición |
|---|---|
| Hipótesis | Creemos que mostrar un score de seguridad+continuidad sobre el mapa cambia la ruta que las personas dicen preferir, comparado con ver solo el mapa sin score. |
| Participantes/escenarios | 15–20 personas que usan o considerarían usar bici en AMBA. 3 trayectos predefinidos. |
| Acción/resultado observable | Para cada trayecto, la persona elige Ruta 1 o Ruta 2 — una vez viendo el mapa sin score, otra vez viendo el mapa con score. |
| Métrica | % de elecciones donde la persona prefiere la ruta más segura (más tramos verdes) cuando esa ruta es distinta a la que eligió sin score. |
| Criterio de éxito | ≥60% de las elecciones muestran preferencia por la ruta más segura al ver el score. *(Umbral propuesto por la IA sin evidencia previa que lo respalde — aceptado como arbitrario por el equipo.)* |
| Duración / regla de fin | Corte a las 15 respuestas completas o a los 3 días de enviado, lo que ocurra primero. |
| Limitaciones conocidas | Preferencia declarada, no comportamiento real en la calle. Score simulado a mano, no calculado con datos reales de incidentes. No mide si después usarían efectivamente la bici. Posible sesgo de orden (ver sección 6). |

## 5. Partes reales y simuladas

| Elemento | Real | Simulado |
|---|---|---|
| Elección de la persona | ✅ | |
| Trazado de las rutas (calles) | | ✅ esquemático, no es un mapa geográfico real |
| Score de seguridad por tramo | | ✅ asignado a mano por el equipo, no calculado con datos |
| Cantidad y variedad de participantes | ✅ si se ejecuta con personas reales | |

## 6. Alcance mínimo

**Imprescindible:** 3 trayectos con mapa base, score simulado superpuesto, formulario de elección A/B, exposición al mapa sin score antes que al mapa con score.
**Simulable/opcional:** pregunta abierta de "por qué elegiste esa ruta".
**Fuera de alcance:** datos demográficos, login, cálculo real del score, prototipo interactivo.

## 7. Instrumento construido

6 imágenes esquemáticas (carpeta `experimento-clase5-mapas/`): por cada uno de los 3 trayectos, una versión sin score (rutas en azul/naranja, sin indicar seguridad) y una versión con score (tramos coloreados verde/amarillo/rojo según seguridad simulada).

### Cómo armar el formulario (Google Forms)

**Sección 1 — Sin score** (mostrar siempre primero)

1. ![Trayecto 1 sin score](experimento-clase5-mapas/trayecto1_sin_score.png)
   "¿Qué ruta elegirías para este trayecto?" → Ruta 1 / Ruta 2

2. ![Trayecto 2 sin score](experimento-clase5-mapas/trayecto2_sin_score.png)
   misma pregunta

3. ![Trayecto 3 sin score](experimento-clase5-mapas/trayecto3_sin_score.png)
   misma pregunta

**Sección 2 — Con score** (mostrar después)

4. ![Trayecto 1 con score](experimento-clase5-mapas/trayecto1_con_score.png)
   misma pregunta

5. ![Trayecto 2 con score](experimento-clase5-mapas/trayecto2_con_score.png)
   misma pregunta

6. ![Trayecto 3 con score](experimento-clase5-mapas/trayecto3_con_score.png)
   misma pregunta

**Pregunta final (opcional):** "¿Por qué elegiste esas rutas?" → respuesta corta.

**Pasos de carga:** crear el Form → por cada pregunta, insertar la imagen correspondiente → agregar debajo la opción múltiple Ruta 1 / Ruta 2 → compartir el link → exportar respuestas a Sheets al llegar a 15 o pasar 3 días.

### Limitación de orden

Google Forms no randomiza fácil el orden de secciones, así que "sin score" queda siempre primero. Esto es un sesgo de orden posible (la persona ya vio las rutas antes de ver el score) — documentado, no resuelto. Una mejora futura sería armar dos versiones del form e intercalar a quién le llega cada una.

### Cómo leer los resultados (cuando existan)

Por cada persona y cada trayecto, comparar la elección "sin score" vs "con score":
- Cambió hacia la ruta con más tramos verdes → a favor de la hipótesis.
- No cambió, o cambió hacia la ruta con más tramos rojos → en contra.
- % a favor sobre el total de elecciones → comparar contra el criterio de 60%.

## 8. Decisiones humanas registradas

- Paso 1: síntesis de evidencia confirmada sin cambios.
- Paso 2: se eligió la pregunta A (valor del score) sobre B (privacidad) y C (compromiso del empleador).
- Paso 3: se eligió Comparación A/B con mapas estáticos sobre Wizard of Oz y prototipo navegable.
- Paso 4: contrato confirmado sin ajustes, incluyendo el criterio de éxito de 60%.
- Paso 5: alcance mínimo aprobado sin cambios.
- Paso 6: instrumento construido y verificado; pendiente de piloto interno.

---

## 9. Estado de avance y lo que falta

Este documento cubre los Pasos 1 a 6 de la skill `ejecutar-experimento-producto` (síntesis, pregunta, comparación de experimentos, contrato, alcance, construcción). **No incluye** los Pasos 7 a 10 (piloto interno, ejecución con participantes reales, registro de resultados, clasificación como Respaldada/No respaldada/Inconclusa) porque esos pasos requieren correr el formulario con personas reales — algo que no se puede simular sin fabricar evidencia.

Cuando el equipo tenga respuestas reales del formulario, se completa `registro-experimento.md` de esta clase con los resultados, la evidencia a favor/en contra y la decisión de iteración.
