# Registro del experimento — RutaSegura

> Este documento reúne el punto de partida, el instrumento construido y el registro de ejecución del experimento mínimo definido en la Caja 8 del Lean Product Canvas. El archivo de trabajo (`instrumento-rutasegura.xlsx`) se sube junto a este `.md` en el repositorio.

---

## 1. Punto de partida

- **Hipótesis priorizada (comportamiento):** Creemos que los empleados usarán la app de forma recurrente para ganar puntos por commutes sostenibles. Lo sabremos si registran viajes de forma repetida durante el piloto.
- **Pregunta de aprendizaje:** ¿Los empleados usarán la app de forma recurrente para registrar sus viajes en bicicleta y ganar puntos?
- **Experimento mínimo:** Concierge / Wizard of Oz — formulario manual + planilla simulando el sistema de puntos, con una empresa piloto.
- **Métrica:** % de participantes que registran 3 o más viajes en bici en 2 semanas.
- **Criterio de éxito:** ≥ 50% de los participantes.

## 2. Posición inicial en la curva de la verdad

- **Evidencia disponible:** Ninguna evidencia de comportamiento real todavía; todo el canvas está marcado como Supuesto. Solo hay datos oficiales de infraestructura/seguridad vial (Clase 2), no de adopción de gamificación.
- **Incertidumbre pendiente:** Si empleados reales, con un incentivo real, registran viajes de forma recurrente usando un proceso 100% manual.
- **Inversión autorizada:** Formulario simple + planilla de cálculo de puntos manual. Sin app, sin backend, sin score de seguridad real.

## 3. Instrumento construido por la IA

- **Tipo de instrumento:** Wizard of Oz — planilla Excel con formulario de carga manual y cálculo automático de puntos.
- **Archivo:** `instrumento-rutasegura.xlsx`

### Estructura del instrumento

**Hoja "Instrucciones"**
Explica la hipótesis, la métrica, el criterio de éxito, los límites del experimento y la leyenda de celdas editables (fondo amarillo = completar; el resto son fórmulas).

**Hoja "Registro de viajes" (el formulario)**
El equipo carga una fila cada vez que un empleado reporta un viaje.

| Columna | Contenido | Editable |
|---|---|---|
| ID_Empleado | Código asignado (P01–P12) | Sí |
| Fecha | Fecha del viaje | Sí |
| Modo | Bici / Otro (lista desplegable) | Sí |
| Origen (barrio aprox.) | Dato complementario, no exacto por privacidad | Sí |
| Destino (barrio aprox.) | Dato complementario, no exacto por privacidad | Sí |
| Puntos | `=IF(Modo="Bici",10,0)` | No (fórmula) |

La fila 2 es un ejemplo marcado explícitamente (ID ficticio `EJ-00`), no cuenta para ningún participante real.

**Hoja "Sistema de puntos" (agregación por empleado)**

| Columna | Fórmula / contenido |
|---|---|
| ID_Empleado | P01 a P12, precargado |
| Nombre | Editable por el equipo |
| Viajes en bici registrados | `=COUNTIFS('Registro de viajes'!A:A, ID, 'Registro de viajes'!Modo:Modo, "Bici")` |
| Puntos totales | `=SUMIFS('Registro de viajes'!Puntos:Puntos, 'Registro de viajes'!A:A, ID)` |
| Cumple criterio (3+ viajes) | `=IF(Viajes>=3,"Sí","No")` |

**Hoja "Resumen del piloto" (cálculo automático del resultado)**

| Indicador | Fórmula |
|---|---|
| Participantes activos | `=COUNTA('Sistema de puntos'!Nombre)` |
| Participantes con 3+ viajes | `=COUNTIF('Sistema de puntos'!Cumple,"Sí")` |
| % de cumplimiento | Participantes con 3+ viajes / Participantes activos |
| Criterio de éxito | 50% (fijo, no se modifica durante la ejecución) |
| Resultado | `=IF(Activos=0,"Inconclusa",IF(%Cumplimiento>=Criterio,"Respaldada","No respaldada"))` |

### Qué quedó fuera (a propósito)

App móvil, score de seguridad real, login, notificaciones, cualquier UI de producto. Es un instrumento descartable: responde una sola pregunta (adopción recurrente), no entrega una experiencia de producto completa.

---

## 4. Ejecución

- Fecha y contexto: _Pendiente — completar al correr el piloto._
- Participantes, escenarios, fuentes o datos: _Pendiente._
- Tarea realizada: _Pendiente._
- Resultados obtenidos: _Pendiente._
- Anomalías observadas: _Pendiente._

## 5. Evidencia

- A favor: _Pendiente._
- En contra: _Pendiente._
- Interpretación del equipo: _Pendiente._
- Limitaciones: El piloto dura solo 2 semanas y usa un proceso manual — no representa condiciones de producto real ni comportamiento a largo plazo. No mide precisión del score de seguridad ni disposición a pagar.

## 6. Aprendizajes

- Qué aprendimos: _Pendiente._
- Qué continúa siendo un supuesto: _Pendiente._
- Cambios realizados o propuestos: _Pendiente._

## 7. Estado de la evidencia y próxima iteración

- Respaldada, no respaldada o inconclusa: _Pendiente — lo calcula automáticamente la hoja "Resumen del piloto" del Excel una vez cargados los datos reales._
- Comparación con el criterio: _Pendiente._
- Decisión de iteración: _Pendiente._
- Justificación: _Pendiente._
- Próxima incertidumbre por reducir: _Pendiente._

## 8. Nueva posición en la curva de la verdad

- Evidencia incorporada: _Pendiente._
- Inversión que se justifica ahora: _Pendiente._
- Qué todavía no se justifica construir: _Pendiente._
