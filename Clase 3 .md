# Lean Product Canvas — RutaSegura

> Este canvas contiene hipótesis. La evidencia surgirá de observar y experimentar.
> Las entrevistas reales todavía no fueron realizadas: todo el contenido no
> validado con usuarios se marca explícitamente como **Supuesto**.

---

## 1. Problema de negocio

Jóvenes y adultos del AMBA evitan usar la bicicleta en sus traslados
cotidianos porque no perciben que el recorrido completo (no solo
tramos aislados) sea seguro y continuo, lo que reduce la adopción de
un medio de transporte sostenible y limita el impacto de las
inversiones en infraestructura ciclista ya realizadas.

**Lo sabemos por:** datos oficiales de siniestralidad (86% de los
incidentes fatales de ciclistas ocurre fuera de la red de
infraestructura) y por los criterios de diseño de conectividad
declarados por el GCBA.

**Supuesto todavía no validado:** que la discontinuidad de la
infraestructura pesa más que otras barreras (costo, tiempo,
comodidad general) en la decisión individual de usar o no bicicleta.
Esto debe confirmarse con entrevistas reales.

---

## 2. Resultados de negocio

- Aumentar la cantidad de viajes registrados por medios de transporte
  sostenibles (bicicleta u otros) entre los empleados de empresas
  clientes, como parte de sus métricas de sostenibilidad/ESG, desde
  pendiente de medir hasta un objetivo a definir, en un plazo a definir.

- Como resultado de soporte: aumentar el porcentaje de empleados que
  adoptan un medio sostenible para su traslado cotidiano al trabajo,
  desde pendiente de medir hasta un objetivo a definir, en el mismo plazo.

---

## 3. Usuarios y clientes

- **Usuario y cliente:** el empleado o estudiante que se traslada
  cotidianamente y paga por la solución para adoptar un medio de
  transporte más sostenible.

- **Decisor:** la empresa, que decide si habilita, promueve o integra
  la solución dentro de sus iniciativas de sostenibilidad (sin ser
  quien paga la solución en sí). Supuesto: la empresa podría aportar
  beneficios indirectos (descuentos, reconocimiento interno, métricas
  ESG) — todavía no validado.

- **Influenciador:** pendiente de investigación. Posibles candidatos:
  compañeros de trabajo, campañas internas de sostenibilidad, o el
  área de RRHH/Sostenibilidad de la empresa.

---

## 4. Necesidades y resultados del usuario

Cuando planeo mi recorrido diario al trabajo o estudio, quiero saber
si puedo completarlo de forma segura y continua en bicicleta, para
no tener que volver a un medio menos sostenible por miedo o
incertidumbre.

**Supuesto:** esta necesidad todavía no fue confirmada con entrevistas
reales; surge de evidencia institucional (siniestralidad fuera de
la red de ciclovías) e interpretación del equipo.

---

## 5. Ideas de solución

### RutaSegura — Mapa de continuidad con recompensas corporativas

- **Propuesta:** app que puntúa rutas ciclistas por continuidad y
  seguridad, y convierte los trayectos sostenibles en puntos dentro
  de un ranking interno de la empresa del usuario, canjeables por
  beneficios (bonos, comida, reconocimiento, día libre).
- **Valor para el usuario:** decide con anticipación qué tramos son
  seguros y continuos, suma motivación social/competitiva y obtiene
  beneficios tangibles de su propia empresa.
- **Tecnología central:** ruteo + scoring de continuidad/seguridad +
  capa de gamificación + panel de configuración para la empresa.
- **Datos necesarios:** datos abiertos de ciclovías, ubicación/tracking
  de trayectos (con consentimiento), pertenencia a empresa/equipo,
  catálogo de recompensas definido por cada empresa.
- **Riesgo principal:** dilución del incentivo con el tiempo; depende
  de que la empresa se comprometa a entregar recompensas reales.
- **Prototipo inicial:** mockup navegable (Figma) o Wizard of Oz con
  cálculo manual de puntos para un grupo piloto chico.
- **Dependencias:** compromiso de RRHH de la empresa para definir y
  entregar recompensas (dependencia secundaria, no física).
- **Estado:** idea no validada.

**Filtro digital aplicado:**

| Criterio | Evaluación |
|---|---|
| Valor | Ayuda a decidir con anticipación y con seguridad + motivación por incentivos. |
| Centralidad digital | Ruteo, scoring y gamificación son el corazón del valor. |
| Evidencia | Continuidad/seguridad respaldada por datos oficiales; gamificación es Supuesto. |
| Prototipabilidad | Sí, con mockup navegable o Wizard of Oz. |
| Datos | Ciclovías (dato abierto), ubicación (requiere consentimiento), recompensas (a definir). |
| Riesgo | Dilución del incentivo; compromiso incierto de la empresa. |
| Dependencias | Compromiso de gestión de RRHH (secundaria, no bloquea el valor digital). |

---

## 6. Hipótesis principales

### Hipótesis de problema

Creemos que jóvenes y adultos del AMBA evitan usar la bicicleta para
ir al trabajo/estudio porque no perciben que puedan completar el
recorrido de forma segura y continua.

Lo sabremos si: en entrevistas, la mayoría de los usuarios menciona
espontáneamente la discontinuidad o falta de seguridad del recorrido
(y no solo costo o comodidad) como motivo para no usar bicicleta.

### Hipótesis de valor

Creemos que mostrar un mapa con scoring de continuidad/seguridad
ayudará a los usuarios a decidir con más confianza si pueden hacer
su trayecto en bicicleta.

Lo sabremos si: al probar el prototipo, la mayoría de los usuarios
dice que el mapa cambia o refuerza su decisión de intentar el
trayecto en bici (comparado con no tener esa información).

### Hipótesis de comportamiento

Creemos que los empleados usarán la app de forma recurrente si
pueden ganar puntos canjeables por beneficios de su empresa.

Lo sabremos si: en un piloto, un porcentaje relevante de usuarios
registra viajes más de una vez por semana durante el período de
prueba (no solo una vez para "probar").

### Hipótesis de factibilidad

Creemos que podemos calcular un score de continuidad/seguridad
razonable combinando los datos abiertos de ciclovías con reportes
simples de usuarios, sin necesitar infraestructura de datos compleja.

Lo sabremos si: logramos generar el score para al menos un recorrido
real de prueba usando solo datos públicos + un formulario simple de
reportes, sin depender de fuentes que no tengamos acceso.

---

## 7. Lo más importante por aprender

¿Los empleados usarán la app de forma recurrente para registrar sus
trayectos sostenibles a cambio de puntos canjeables por beneficios
de su empresa?

| Hipótesis | Incertidumbre (1-5) | Impacto (1-5) | Prioridad | Justificación |
|---|---:|---:|---:|---|
| Problema | 3 | 5 | 2 | Hay evidencia institucional, pero no confirmamos si es *la* barrera principal. |
| Valor | 3 | 4 | 3 | Es razonable pensar que más información ayuda, pero no sabemos si cambia el comportamiento. |
| Comportamiento | 5 | 5 | 1 | No hay evidencia de que los puntos/beneficios generen uso recurrente. Sin esto, no hay producto. |
| Factibilidad | 2 | 2 | 4 | Datos abiertos ya existen; técnicamente alcanzable para un prototipo estudiantil. |

### Pre-mortem

Imaginando que RutaSegura fracasó a los 6 meses de lanzarse, el
equipo priorizó estos tres riesgos:

1. **Datos insuficientes/mala calidad:** el score de continuidad
   podría no reflejar la seguridad real percibida por los usuarios.
   Señal temprana: rutas bien puntuadas que los usuarios reportan
   como inseguras. Experimento: comparar el score calculado contra
   percepción real con 5-10 usuarios en rutas conocidas.

2. **Modelo de negocio:** las empresas podrían no comprometerse a
   sostener recompensas en el tiempo. Señal temprana: abandono del
   programa de recompensas por parte de empresas piloto en pocos
   meses. Experimento: entrevistas con RRHH/Sostenibilidad de 2-3
   empresas para validar disposición real (no solo interés declarado).

3. **Privacidad/confianza:** los usuarios podrían no querer compartir
   su ubicación/trayectos con su empleador. Señal temprana: baja
   aceptación de permisos de ubicación en el piloto. Experimento:
   preguntar explícitamente en entrevistas si compartirían su
   recorrido con su empleador.

Estos riesgos refuerzan que la hipótesis de comportamiento sigue
siendo la prioritaria, pero el experimento debe poner a prueba
específicamente el mecanismo de puntos + uso de ubicación + compromiso
real de la empresa, no solo el uso general de la app.

---

## 8. Experimento mínimo

- **Hipótesis que prueba:** Comportamiento — ¿los empleados usarán la
  app de forma recurrente para registrar trayectos sostenibles a
  cambio de puntos canjeables por beneficios de su empresa?

- **Objetivo:** observar si un grupo de empleados de una empresa piloto
  registra sus trayectos de forma recurrente (no solo una vez) durante
  el período de prueba, cuando hay un beneficio real de por medio.

- **Tipo de experimento:** Concierge / Wizard of Oz + landing de registro.

- **Herramienta:** formulario simple (Google Forms o Typeform) para que
  el usuario registre cada viaje (fecha, medio usado, tramo recorrido);
  planilla manual (Google Sheets) donde el equipo calcula los puntos
  "a mano" simulando el sistema automático.

- **Participantes:** 8-12 empleados de una sola empresa piloto (idealmente
  ya conversada previamente con RRHH/Sostenibilidad para conseguir al
  menos una recompensa real y chica, ej. vale de café o reconocimiento
  interno).

- **Duración:** 2 semanas.

- **Tarea:** cada vez que el usuario haga un trayecto sostenible al
  trabajo, completa el formulario. El equipo actualiza manualmente
  un ranking visible (planilla compartida o print semanal) y al final
  entrega la recompensa acordada a quien más puntos sumó.

- **Datos necesarios:** registros de viaje (fecha, medio, tramo),
  consentimiento explícito de los usuarios para compartir su recorrido
  (probando así también, de forma liviana, la barrera de privacidad
  detectada en el pre-mortem).

- **Métrica:** cantidad de registros por usuario durante las 2 semanas.

- **Criterio de éxito:** al menos el 50% de los participantes registra
  3 o más trayectos en las 2 semanas (evidencia de uso recurrente,
  no solo prueba única).

- **Criterio de fracaso:** la mayoría de los participantes registra 1
  trayecto o menos después de la primera semana, o menos del 30%
  acepta compartir su recorrido.

- **Aprendizaje esperado:** si el mecanismo de puntos + recompensa
  genera uso recurrente real, y si la barrera de privacidad es
  significativa o no.

- **Limitaciones:** la recompensa es simulada/manual y a pequeña escala;
  el resultado con una sola empresa no necesariamente se replica en
  otras; el score de continuidad del mapa no se está probando en este
  experimento (eso quedaría para un experimento posterior sobre la
  hipótesis de valor).

---

## Cierre del equipo

**La solución digital que decidimos explorar es:** RutaSegura, un mapa
de continuidad/seguridad ciclista con gamificación y recompensas
corporativas.

**La evidencia más fuerte que la respalda es:** el 86% de los
incidentes fatales de ciclistas en la Ciudad ocurre fuera de la red
de ciclovías, y los criterios oficiales de diseño de infraestructura
ya priorizan la conectividad.

**El supuesto más riesgoso es:** que los empleados usarán la app de
forma recurrente motivados por puntos canjeables por beneficios de
su empresa.

**Lo más importante que necesitamos aprender es:** si el mecanismo de
puntos + recompensa genera uso recurrente real, más allá de la
curiosidad inicial.

**El experimento que realizaremos es:** un piloto de 2 semanas con
8-12 empleados de una empresa, usando un formulario de registro y un
ranking manual con una recompensa real chica.

**Abandonaremos o cambiaremos la propuesta si:** menos del 50% de los
participantes registra 3 o más trayectos en las 2 semanas, o si menos
del 30% acepta compartir su ubicación/recorrido.
