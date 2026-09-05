# Evaluación 2 — Proyecto SGR

Índice de contexto para trabajar con Claude sin repetir los documentos completos en cada prompt.

**Antes de dividir el trabajo por actividad, lean [`decisiones.md`](./decisiones.md).**
Las 3 actividades dependen de las mismas decisiones base (alcance, metodología, nomenclatura). Si cada quien
arranca sin eso definido, las épicas/HU de la Actividad 1 no van a calzar con los diagramas de la Actividad 3.

**Alcance (decisión cerrada, no releer transcripciones antiguas de esto):** el proyecto cubre el
**MVP de `guia-sgr.md` §13.2** — 22 de las 31 HU (las marcadas P1 en §12), con sus RF/RNF asociados más
los RNF transversales. No se cubre el documento completo. El detalle exacto de qué HU/RF/RNF entran y
cuáles quedan fuera está en `decisiones.md` § Alcance del MVP — consultarlo antes de escribir cualquier
lista de RF/RNF/HU para no incluir un ítem fuera de alcance.

## Carpeta `fuentes/`

Los 7 documentos originales, sin modificar. Guía de cuándo pegar cada uno en un prompt:

| Archivo | Qué es | Úsalo para | NO lo uses para |
|---|---|---|---|
| `guia-sgr.md` | Caso base: RF-001 a RF-038, RNF-001 a RNF-018, reglas de negocio RN-001 a RN-013, 8 épicas (EP-01 a EP-08), 31 HU, entidades, arquitectura sugerida, MVP §13.2 | Actividad 1 (bajada de RF/RNF/HU **del MVP**, ver `decisiones.md` § Alcance del MVP), diagrama de clases (entidades §8), diagrama de despliegue (arquitectura §14.1) | Nunca hace falta pegarlo completo — es largo (1053 líneas). Copien solo la sección numerada que necesiten (ej. "§5.3 Agenda colectiva" o "§12.5 EP-04") |
| `ppt-original.md` | Transcripción cruda de las diapositivas de la Municipalidad: planillas reales con nombres de funcionarios | Casi nunca. Solo si necesitan ver "cómo se ve hoy" el proceso en Google Sheets para justificar una decisión de UX en un wireframe | **Nunca lo peguen para generar RF/RNF/HU ni datos de ejemplo** — tiene nombres reales de personas y la guía prohíbe usar datos reales. La versión ya formalizada y segura de esto es `guia-sgr.md` |
| `enunciado-y-rubrica.md` | Enunciado oficial de la evaluación + Rúbrica 2 con ponderaciones (25% / 35% / 40%) | Confirmar qué se califica exactamente, fechas, formato del informe (portada, tercera persona, APA) | No sirve como fuente del caso SGR — no tiene RF ni HU |
| `que-hacer-1-2-3.md` | Desglose propio ya combinado (guía + audios), con checklists por actividad | El más denso y accionable. Punto de partida por defecto para cualquier actividad | — |
| `audio-clase-1.md` | Transcripción de clase: aclaraciones sobre logística, licitación entre grupos, liderazgo rotativo | Dudas sobre formato de entrega o dinámica de evaluación | Contenido técnico de diagramas (ver `audio-clase-2.md` para eso) |
| `audio-clase-2.md` | Transcripción de clase: aclaraciones técnicas sobre include/extend, trazabilidad, y **una discrepancia real** (el profesor dice que la cadena de trazabilidad parte de RNF, el enunciado escrito dice RF) | Actividad 3 — especialmente antes de armar la matriz de trazabilidad | — |
| `apuntes-cocreacion-patrones.md` | Material teórico del ramo (no es del caso SGR): ciclos de vida y metodologías, técnicas de cocreación/levantamiento de requerimientos, tipos de requerimientos según Sommerville, patrones de diseño GoF (singleton, factory, observer, adapter), tipos de diagramas UML, estándares de calidad (ISO/IEC 12207, ISO/IEC 33000 SPICE, ISO 9001, ISO/IEC 25000 SQuaRE) | Actividad 1 (marco teórico de técnicas de levantamiento y clasificación de RNF), Actividad 2 (criterios de selección de metodología y comparación cascada vs. ágil), Actividad 3 (aplicar patrones de diseño al diagrama de clases/componentes, y como referencia de qué es cada tipo de diagrama UML) | No reemplaza a `guia-sgr.md` — es teoría general citable (Sommerville, Gamma et al., ISO), no contiene RF/RNF/HU del caso SGR ni define el MVP (eso viene solo de `guia-sgr.md` §13.2) |

## Documentos de trabajo por actividad

Cada actividad tiene su propio archivo, para que los 4 integrantes puedan trabajar en ramas separadas sin
generar conflictos de merge entre sí. Cada uno enlaza a `decisiones.md` y señala de qué otro documento
depende o a cuál alimenta — revisar esa cabecera antes de dar por cerrada la actividad.

- **[`actividad-1.md`](./actividad-1.md)** (25%) — Técnicas de requerimientos, RF/RNF, épicas, HU, tareas,
  esfuerzo, planificación. Fuentes: `que-hacer-1-2-3.md` (sección Actividad 1) + secciones de RF/RNF/HU
  de `guia-sgr.md` que correspondan al **MVP ya fijado en `decisiones.md` § Alcance del MVP** (22 HU,
  no las 31) + `apuntes-cocreacion-patrones.md` (marco teórico de técnicas de cocreación y clasificación
  de RNF, usar solo como respaldo conceptual).
- **[`actividad-2.md`](./actividad-2.md)** (35%) — Comparación de metodologías, elección justificada
  (Scrum), recursos de hardware/software y humanos. Fuentes: `que-hacer-1-2-3.md` (sección Actividad 2).
  No hace falta releer `guia-sgr.md` completo, solo §14.1 (arquitectura) para los recursos.
  `apuntes-cocreacion-patrones.md` aporta los criterios de selección de metodología (tamaño, recursos,
  requisitos, plazos) para reforzar la comparación técnica.
- **[`actividad-3.md`](./actividad-3.md)** (40%, la de mayor peso y riesgo) — Diagramas UML, wireframes,
  matriz de trazabilidad. Fuentes: `que-hacer-1-2-3.md` (sección Actividad 3) + `audio-clase-2.md` (por
  la discrepancia RF/RNF) + los códigos exactos que se cierren en `actividad-1.md` y `actividad-2.md`
  (recordar: solo las 22 HU del MVP, no las 31). `apuntes-cocreacion-patrones.md` aporta los patrones de
  diseño GoF (singleton, factory, observer, adapter) a evaluar en el diagrama de clases/componentes.

**Orden de dependencia:** Actividad 1 y Actividad 2 pueden avanzar en paralelo, pero Actividad 3 necesita
que ambas estén con sus códigos y recursos ya cerrados antes de darse por terminada — no antes de
empezar a redactar, pero sí antes del merge final.
