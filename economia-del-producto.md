# Economía del producto — RutaSegura

- **Fecha, moneda y período:** 19/10/2026 · pesos argentinos (ARS) · valores mensuales. Tipo de cambio de referencia: $1.530 por dólar (oficial, Banco Nación, venta, 16/10/2026).
- **Usuario, valor y evidencia disponible:** empleados y estudiantes del AMBA que van o podrían ir en bici al trabajo. El valor es un puntaje de seguridad por ruta más una capa de puntos y beneficios. El MVP es una página con 3 rutas de ejemplo (Palermo → Microcentro) y datos de demostración; la prueba con otras personas sigue pendiente. No hay evidencia de disposición a pagar.
- **Quién pagaría y por qué (hipótesis, sin evidencia):** la empresa empleadora. Obtendría bienestar y retención de sus empleados, e impacto ambiental que le permitiría conseguir sellos y diferenciarse de otras empresas. Los premios los financia la empresa por su cuenta, fuera de lo que cobra RutaSegura.
- **Unidad económica:** empleado activo por mes (con al menos un viaje registrado en el mes).

## Números iniciales

| Concepto | Importe y unidad | Tipo | Fuente o motivo |
|---|---|---|---|
| Ingreso por unidad | $1.000 por empleado activo/mes | Estimación | Supuesto del equipo, sin referencia de mercado |
| Variable: consultas de mapas | ≈ $306 (40 consultas × US$5/1.000 × $1.530) | Estimación derivada | 40 consultas: supuesto del equipo. US$5 por 1.000: referencia, Google Routes (nivel Essentials, tramo 10.001–100.000 al mes; abril 2026). Puede aplicar Pro (US$10) |
| Variable: moderación de reportes | ≈ $326 (10 min × $1.956/hora) | Estimación derivada | 10 min: supuesto del equipo. $1.956/h: referencia, salario mínimo por hora, Res. 4/2026 (octubre 2026). Es un piso, no el costo real |
| Fijo por período: infraestructura | ≈ $38.250/mes (US$25) | Referencia | Supabase Pro (verificado jul–sep 2026). No incluye hosting web, dominio ni notificaciones |
| Inversión inicial | — | Pendiente | Construcción y puesta en marcha, sin estimar |

## Resultado y escenario

- **Costo variable por unidad (base):** $306 + $326 = **$632**.
- **Contribución por unidad (base):** $1.000 − $632 = **$368**.
- **Escenario exigente (cambia un solo supuesto: moderación de 10 a 20 min):** moderación $652, costo variable $958, contribución **$42**.

| Por empleado activo/mes | Base | Exigente |
|---|---:|---:|
| Ingreso | $1.000 | $1.000 |
| Costo variable | $632 | $958 |
| Contribución | $368 | $42 |
| Empleados activos para cubrir los $38.250 fijos | ≈ 104 | ≈ 911 |

- **Qué significa:** con estos supuestos, la contribución es muy sensible al tiempo de moderación. Con unos 21 minutos por empleado llegaría a cero. El precio mínimo para no tener contribución negativa sería $632 (base) o $958 (exigente).
- **Qué no demuestra:** la contribución no es ganancia neta y no prueba que haya demanda. Todas las cifras salen de estimaciones y referencias, no de datos observados. Los costos fijos adicionales y la inversión inicial no están incluidos.

## Primeros clientes

- **Canal, costo y esfuerzo previstos:** una empresa piloto conocida (contacto cercano). El costo en dinero sería bajo. El tiempo semanal de esfuerzo comercial está **pendiente de estimar**.
- **CAC / repago:** no calculables (cero clientes pagadores). Quedan como dato pendiente.

## Supuesto por comprobar

- **Supuesto elegido:** que una empresa pague $1.000 por empleado activo por mes.
- **Prueba, con quién, acción observable y registro:** entrevista de unos 30 minutos con quien decide el presupuesto (Recursos Humanos o Sostenibilidad) de la empresa piloto. Se muestra el MVP y se pregunta por presupuesto, decisor, plazos y rango de precio (primero el rango que diga la persona, después se menciona $1.000). Se registra por escrito el mismo día: si hay presupuesto, quién aprueba y en cuánto tiempo, rango mencionado, objeciones y si aceptaría un piloto. No demuestra pago efectivo.
- **Criterio previo y decisión según el resultado:**
  - *Favorable* (hay presupuesto, hay decisor y el rango llega a $1.000 o más): pasar a pedir un compromiso concreto (carta de intención o piloto con precio acordado).
  - *Intermedio* (hay interés, pero el rango es menor a $1.000): recalcular con ese precio y ver si el modelo sigue cerrando.
  - *Desfavorable* (sin presupuesto ni proceso, o rango máximo por debajo de $632): replantear el pagador o el mecanismo antes de seguir.
- **Responsable y fecha:** a definir por el equipo.
