# Evaluación 2 — Proyecto SGR

Índice de contexto para trabajar con Claude sin repetir los documentos completos en cada prompt.

**Antes de dividir el trabajo por actividad, lean [`decisiones.md`](./decisiones.md).**
Las 3 actividades dependen de las mismas decisiones base (alcance, metodología, nomenclatura). Si cada quien
arranca sin eso definido, las épicas/HU de la Actividad 1 no van a calzar con los diagramas de la Actividad 3.

## Carpeta `fuentes/`

Los 6 documentos originales, sin modificar. Guía de cuándo pegar cada uno en un prompt:

| Archivo | Qué es | Úsalo para | NO lo uses para |
|---|---|---|---|
| `guia-sgr.md` | Caso base: RF-001 a RF-038, RNF-001 a RNF-018, reglas de negocio RN-001 a RN-013, 8 épicas (EP-01 a EP-08), 31 HU, entidades, arquitectura sugerida, MVP §13.2 | Actividad 1 (bajada de RF/RNF/HU), diagrama de clases (entidades §8), diagrama de despliegue (arquitectura §14.1) | Nunca hace falta pegarlo completo — es largo (1053 líneas). Copien solo la sección numerada que necesiten (ej. "§5.3 Agenda colectiva" o "§12.5 EP-04") |
| `ppt-original.md` | Transcripción cruda de las diapositivas de la Municipalidad: planillas reales con nombres de funcionarios | Casi nunca. Solo si necesitan ver "cómo se ve hoy" el proceso en Google Sheets para justificar una decisión de UX en un wireframe | **Nunca lo peguen para generar RF/RNF/HU ni datos de ejemplo** — tiene nombres reales de personas y la guía prohíbe usar datos reales. La versión ya formalizada y segura de esto es `guia-sgr.md` |
| `enunciado-y-rubrica.md` | Enunciado oficial de la evaluación + Rúbrica 2 con ponderaciones (25% / 35% / 40%) | Confirmar qué se califica exactamente, fechas, formato del informe (portada, tercera persona, APA) | No sirve como fuente del caso SGR — no tiene RF ni HU |
| `que-hacer-1-2-3.md` | Desglose propio ya combinado (guía + audios), con checklists por actividad | El más denso y accionable. Punto de partida por defecto para cualquier actividad | — |
| `audio-clase-1.md` | Transcripción de clase: aclaraciones sobre logística, licitación entre grupos, liderazgo rotativo | Dudas sobre formato de entrega o dinámica de evaluación | Contenido técnico de diagramas (ver `audio-clase-2.md` para eso) |
| `audio-clase-2.md` | Transcripción de clase: aclaraciones técnicas sobre include/extend, trazabilidad, y **una discrepancia real** (el profesor dice que la cadena de trazabilidad parte de RNF, el enunciado escrito dice RF) | Actividad 3 — especialmente antes de armar la matriz de trazabilidad | — |

## Documentos de trabajo por actividad

Cada actividad tiene su propio archivo, para que los 4 integrantes puedan trabajar en ramas separadas sin
generar conflictos de merge entre sí. Cada uno enlaza a `decisiones.md` y señala de qué otro documento
depende o a cuál alimenta — revisar esa cabecera antes de dar por cerrada la actividad.

- **[`actividad-1.md`](./actividad-1.md)** (25%) — Técnicas de requerimientos, RF/RNF, épicas, HU, tareas,
  esfuerzo, planificación. Fuentes: `que-hacer-1-2-3.md` (sección Actividad 1) + secciones de RF/RNF/HU
  de `guia-sgr.md` que correspondan al alcance elegido.
- **[`actividad-2.md`](./actividad-2.md)** (35%) — Comparación de metodologías, elección justificada
  (Scrum), recursos de hardware/software y humanos. Fuentes: `que-hacer-1-2-3.md` (sección Actividad 2).
  No hace falta releer `guia-sgr.md` completo, solo §14.1 (arquitectura) para los recursos.
- **[`actividad-3.md`](./actividad-3.md)** (40%, la de mayor peso y riesgo) — Diagramas UML, wireframes,
  matriz de trazabilidad. Fuentes: `que-hacer-1-2-3.md` (sección Actividad 3) + `audio-clase-2.md` (por
  la discrepancia RF/RNF) + los códigos exactos que se cierren en `actividad-1.md` y `actividad-2.md`.

**Orden de dependencia:** Actividad 1 y Actividad 2 pueden avanzar en paralelo, pero Actividad 3 necesita
que ambas estén con sus códigos y recursos ya cerrados antes de darse por terminada — no antes de
empezar a redactar, pero sí antes del merge final.
