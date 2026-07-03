# Mechanic Assistant (Asistente de Mecánica)

[English](./README.md) | [日本語](./README.ja.md) | **Español**

Una habilidad de IA de propósito general que apoya a mecánicos profesionales y aficionados serios durante los trabajos de reparación — desde la evaluación inicial de síntomas hasta pares de apriete, guías de procedimiento y verificación posreparación.

## Descripción

El Asistente de Mecánica actúa como una segunda opinión experta en el taller. Te ayuda a razonar trabajos poco familiares, recordar procedimientos y especificaciones, planificar secuencias de reparación y evitar errores comunes. Está diseñado para **complementar** — no reemplazar — los manuales de servicio de fábrica, los boletines técnicos del fabricante y el criterio práctico.

**Audiencia:** Técnicos profesionales, aprendices de mecánica y aficionados con experiencia.

## Capacidades

- Guiar procedimientos de reparación paso a paso (correa de distribución, rodamientos de rueda, junta de culata)
- Explicar el funcionamiento de los sistemas del vehículo (encendido, alimentación, refrigeración, carga, frenos, climatización, transmisión)
- Sugerir estrategias de diagnóstico cuando un síntoma tiene múltiples causas posibles
- Indicar rangos típicos de pares de apriete y secuencias, con el recordatorio de verificar contra el manual de fábrica
- Recomendar las herramientas correctas, incluidas herramientas especiales y sustitutos aceptables
- Identificar fallos típicos de marcas, modelos y familias de motores concretas
- Ayudar a interpretar el lenguaje de los manuales, los diagramas eléctricos y los boletines técnicos
- Estimar la dificultad del trabajo, rangos de tiempo de mano de obra y si es apropiado para bricolaje
- Asesorar sobre repuestos: OEM vs. alternativo, reconstruido vs. nuevo, qué reemplazar "ya que estás ahí"

## Prompts de ejemplo

```text
Voy a cambiar la correa de distribución de un Subaru Outback 2.5 de 2012.
Guíame por el procedimiento y dime qué más debería reemplazar de paso.
```

```text
¿Cuál es la secuencia y el enfoque de apriete correcto para los tornillos
de culata en un bloque de aluminio? Explica por qué importa la secuencia.
```

```text
El coche de un cliente tiene un zumbido que varía con las RPM del motor
pero no con la velocidad. ¿Qué sistemas reviso primero?
```

```text
Necesito sacar un tornillo gripado del soporte de la pinza de freno.
¿Cuáles son mis opciones, de la menos a la más agresiva?
```

```text
Explica cómo falla un volante bimasa y cómo saber si necesita reemplazo
durante un cambio de embrague.
```

## Flujo de trabajo recomendado

1. **Describe el vehículo con precisión.** Año, marca, modelo, motor, transmisión y kilometraje.
2. **Indica el trabajo o el síntoma,** incluyendo lo que ya revisaste o reemplazaste.
3. **Pide un plan antes de tocar nada:** procedimiento completo, herramientas y lista de piezas.
4. **Verifica las especificaciones críticas** contra el manual de fábrica antes de aplicarlas.
5. **Trabaja de forma iterativa:** informa lo que encuentras en cada paso y deja que el plan se ajuste.
6. **Confirma la reparación:** pide una lista de verificación posreparación (fugas, reaprendizajes, criterios de prueba en carretera).

## Limitaciones

- **No sustituye la documentación de fábrica.** Pares, capacidades y procedimientos varían por mercado y fecha de producción. Verifica siempre los valores críticos de seguridad.
- **No puede ver, oír ni medir.** La calidad del diagnóstico depende de la precisión de tus descripciones y mediciones.
- **El conocimiento tiene fecha de corte.** Modelos muy recientes, llamadas a revisión y boletines pueden no estar cubiertos.
- **Sin responsabilidad por el resultado.** Frenos, dirección, suspensión, airbags (SRS) y sistemas de combustible son críticos: ante la duda, acude a un profesional certificado.
- **Variación regional:** las especificaciones y normativas difieren entre mercados (América, Europa, Japón).

## Habilidades relacionadas

- [OBD-II Diagnostic Assistant](../obd2-diagnostic-assistant/README.es.md) — diagnóstico electrónico basado en códigos de falla
- [Vehicle Troubleshooting](../vehicle-troubleshooting/) — triaje por síntomas antes de reparar (inglés/japonés)
- [Motorcycle Mechanic](../motorcycle-mechanic/) — el equivalente para motocicletas (inglés/japonés)
