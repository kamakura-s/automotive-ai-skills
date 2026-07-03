# Vehicle Maintenance Planner (Planificador de Mantenimiento)

[English](./README.md) | [日本語](./README.ja.md) | **Español**

Una habilidad de IA que construye y gestiona calendarios de mantenimiento preventivo adaptados a tu vehículo, kilometraje, clima y patrón de conducción.

## Descripción

El Planificador de Mantenimiento convierte el consejo genérico de "cada 10.000 km" en un plan personalizado. Considera condiciones de servicio severo (trayectos cortos, remolque, calor o frío extremo, caminos polvorientos), distingue lo que vence ahora de lo que vence pronto, te ayuda a presupuestar y explica *por qué* importa cada servicio para que decidas con criterio.

**Audiencia:** Todo propietario de vehículo — desde el primer coche hasta gestores de flotas.

## Capacidades

- Generar un calendario completo de mantenimiento a partir de año, marca, modelo, motor y kilometraje actual
- Ajustar intervalos por servicio severo: trayectos cortos, tráfico denso, remolque, uso en pista, climas extremos, polvo
- Explicar en qué consiste cada servicio y la consecuencia de saltárselo
- Priorizar lo vencido por riesgo (seguridad primero, luego longevidad del motor, luego confort)
- Estimar rangos de coste (piezas en bricolaje vs. precio típico de taller)
- Distinguir servicios aptos para bricolaje de los que requieren taller (equipamiento, residuos, calibración)
- Planificar mantenimiento estacional: preparación de invierno, sistema de refrigeración antes del verano, cambio de neumáticos
- Construir planes de puesta al día para vehículos con historial desconocido o descuidado
- Gestionar fluidos y consumibles: aceite, refrigerante, líquido de frenos, transmisión, diferenciales, filtros, correas, bujías, neumáticos, batería
- Asesorar sobre el registro de mantenimiento y qué documentación preserva el valor de reventa

## Prompts de ejemplo

```text
Acabo de comprar un Mazda CX-5 2017 con 130.000 km y sin historial de
mantenimiento. Hazme un plan de puesta al día ordenado por prioridad.
```

```text
Conduzco 6 km al trabajo en clima frío. ¿Cómo debería cambiar eso mi
intervalo de cambio de aceite y por qué?
```

```text
¿Qué mantenimiento toca entre 150.000 y 190.000 km en una Toyota Hilux
2016, y cuánto costaría aproximadamente en taller vs. bricolaje?
```

```text
Crea un calendario de mantenimiento de 12 meses para mis dos coches: un
Honda CR-V 2020 (40.000 km) y una furgoneta 2011 (220.000 km).
```

```text
¿El aceite de transmisión "de por vida" es realmente de por vida?
¿Cuándo debería cambiarlo en realidad?
```

## Flujo de trabajo recomendado

1. **Proporciona los datos del vehículo:** año, marca, modelo, motor, tipo de transmisión y kilometraje.
2. **Describe tu conducción:** kilometraje anual, longitud de trayectos, clima, remolque, terreno.
3. **Comparte el historial conocido:** servicios recientes y lo que sabes que se omitió.
4. **Pide un plan priorizado:** ahora / 3 meses / 12 meses.
5. **Decide bricolaje o taller por ítem:** pide dificultad y herramientas necesarias.
6. **Actualiza en cada servicio:** kilometraje e ítems completados para mantener el plan vigente.

## Limitaciones

- **El calendario de fábrica tiene prioridad.** El manual del propietario es la autoridad; los intervalos del asistente son estimaciones informadas.
- **Los costes son rangos, no presupuestos:** la mano de obra varía mucho por región.
- **Sin memoria persistente entre sesiones** (salvo que tu cliente la soporte) — lleva tu propio registro y pégalo al inicio.
- **Los requisitos de garantía son estrictos:** en garantía, sigue el calendario de fábrica al pie de la letra y guarda los recibos.
- **No puede inspeccionar el vehículo:** frenos y neumáticos requieren medición física; el plan solo dice cuándo revisarlos.

## Habilidades relacionadas

- [Used Car Inspector](../used-car-inspector/README.es.md) — evaluar el estado antes de planificar un vehículo recién comprado
- [Mechanic Assistant](../mechanic-assistant/README.es.md) — ejecutar los servicios de bricolaje del plan
- [EV Assistant](../ev-assistant/) — los calendarios de VE difieren sustancialmente (inglés/japonés)
