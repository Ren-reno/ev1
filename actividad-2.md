# Actividad 2 — Selección y justificación de la metodología

**Ponderación en la rúbrica: 35%**

**Depende de:**
- [`decisiones.md`](./decisiones.md) — metodología elegida: **Scrum**. Falta definir la
  segunda metodología de comparación (candidatas sugeridas: Kanban, Cascada, o XP). Alcance del
  proyecto: MVP de 22 HU (ver `decisiones.md` § Alcance del MVP).
- Actividad 1 → el volumen del backlog del MVP (22 HU de 31, con sus RF/RNF asociados, ver
  `decisiones.md` § Alcance del MVP) es evidencia técnica a favor de la metodología elegida: úsalo en
  la sección 1.4 (comparación técnica) en vez de razonar en abstracto sobre "un proyecto típico". Si
  Actividad 1 todavía no cerró sus códigos finales, ese número puede citarse como aproximado, pero debe
  revisarse antes de dar por cerrada esta actividad.

**Alimenta a:** Actividad 3 (los recursos de hardware/software mínimos y óptimos definidos aquí en la
sección 3 deben coincidir exactamente con lo que se represente en el diagrama de despliegue — no pueden
ser inconsistentes entre sí).

**Fuentes a consultar:** `fuentes/que-hacer-1-2-3.md` (sección Actividad 2), `fuentes/audio-clase-1.md` y
`fuentes/audio-clase-2.md` (énfasis en no aceptar cuadros simples de ventajas/desventajas), `fuentes/guia-sgr.md`
§14.1 (arquitectura sugerida, como referencia para los recursos de despliegue), `fuentes/apuntes-cocreacion-patrones.md`
(marco teórico de metodologías tradicionales vs. ágiles y criterios de selección — tamaño del proyecto,
recursos disponibles, requisitos del cliente, plazos y presupuesto; útil para dar fundamento académico a
la sección 1, no reemplaza el análisis técnico específico del caso SGR).

---

## 1. Metodologías a comparar

> Categorías admisibles: estructurada (ej. cascada), ágil, híbrida o incremental.
> **Espiral queda explícitamente excluida** — ni se menciona como opción a comparar.
> **No se acepta un cuadro simple de ventajas/desventajas** — la comparación debe conectar
> características técnicas de cada metodología (ciclos de retroalimentación, manejo del cambio,
> artefactos que produce, roles, cadencia de entregas, forma de gestionar riesgo) con las condiciones
> reales del proyecto.

> Apoyo teórico disponible en `fuentes/apuntes-cocreacion-patrones.md` (sección "Selección de una
> metodología y ciclo de vida"): los 4 criterios de análisis — tamaño del proyecto, recursos
> disponibles, requisitos del cliente (claros/estables vs. cambiantes), y plazos/presupuesto — mapean
> directamente con las condiciones reales del punto 1.1 y sirven de estructura para argumentar 1.2–1.4
> sin caer en un cuadro simple de ventajas/desventajas.

### 1.1 Condiciones reales del proyecto (referencia obligatoria para el análisis)

- Equipo de 4 personas
- Plazo acotado: 9 días para esta etapa, semestre completo como restricción mayor
- Requerimientos ya definidos por el docente, con margen de ajuste ("bajada")
- Alcance ya fijado al MVP de `guia-sgr.md` §13.2 (22 HU de 31, ver `decisiones.md` § Alcance del MVP);
  esto refuerza la necesidad de una metodología que permita entregar valor de forma incremental dentro
  del propio MVP, ya priorizado por sprints en `guia-sgr.md` §13.3

### 1.2 Metodología 1: Scrum

_(Ciclos de retroalimentación, manejo del cambio, artefactos, roles, cadencia de entregas, gestión de
riesgo — y cómo cada uno de estos puntos responde a las condiciones del proyecto listadas arriba.)_

### 1.3 Metodología 2: [pendiente de definir]

_(Mismo nivel de análisis técnico que el punto anterior.)_

### 1.4 Comparación técnica y elección final

_(De la comparación anterior debe derivarse y justificarse cuál metodología se elige finalmente. Ya
está decidido que es Scrum — aquí se argumenta técnicamente por qué, no solo se declara.)_

---

## 2. Recursos de Hardware y Software

> Especificar mínimos y óptimos, separando etapa de desarrollo vs. etapa de producción/operación. Estos
> recursos se conectarán después con el diagrama de despliegue (Actividad 3) — conviene definirlos
> pensando ya en qué nodos/infraestructura se van a representar ahí (servidor web, servidor BD, cliente,
> etc.).

### 2.1 Etapa de desarrollo

| Recurso | Mínimo | Óptimo |
|---|---|---|
| Hardware | | |
| Software | | |

### 2.2 Etapa de producción/operación

| Recurso | Mínimo | Óptimo |
|---|---|---|
| Hardware | | |
| Software | | |

---

## 3. Recursos Humanos

> Definir roles, perfiles y organización del equipo de trabajo, para desarrollo y para operación.

### 3.1 Roles y organización del equipo (desarrollo)

| Rol | Perfil | Responsabilidad |
|---|---|---|
| | | |

### 3.2 Roles y organización del equipo (operación)

| Rol | Perfil | Responsabilidad |
|---|---|---|

### 3.3 Justificación de perfiles según la metodología elegida (Scrum)

_(Si en algún punto se considera un rol o práctica más exigente en experiencia — como ocurriría con XP
por el pair programming — abordar aquí la tensión entre lo que pide la metodología y que el equipo real
tiene 4 integrantes probablemente todos estudiantes.)_

---

## Checklist de cierre — Actividad 2

- [ ] Mínimo 2 metodologías comparadas (sin espiral)
- [ ] Comparación con fundamento técnico de ingeniería (no cuadro pro/contra)
- [ ] Metodología elegida (Scrum), justificada según condiciones reales del proyecto
- [ ] Recursos de Hardware/Software mínimos (desarrollo)
- [ ] Recursos de Hardware/Software óptimos (desarrollo)
- [ ] Recursos de Hardware/Software mínimos (operación)
- [ ] Recursos de Hardware/Software óptimos (operación)
- [ ] Roles y organización del equipo humano
- [ ] Justificación de perfiles según la metodología elegida
- [ ] Recursos comunicados a quien trabaje el diagrama de despliegue en Actividad 3
