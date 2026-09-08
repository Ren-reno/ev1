# Decisiones

Base común que las 3 actividades deben respetar. Cuando alguien redacte su parte, estas son las
decisiones ya cerradas por el equipo — no hay que volver a discutirlas ni improvisar una distinta.

**Alimenta a:** [`actividad-1.md`](./actividad-1.md), [`actividad-2.md`](./actividad-2.md) y
[`actividad-3.md`](./actividad-3.md) — las tres leen este documento antes de empezar. Cualquier cambio
aquí (alcance, metodología, nomenclatura) debe avisarse a quien esté trabajando cada actividad, porque
puede invalidar contenido ya redactado.

---

## Alcance del MVP

**Decisión cerrada: se usa el "Alcance mínimo recomendado (MVP)" de `guia-sgr.md` §13.2**, no el
documento completo. A continuación se traduce cada punto de §13.2 a códigos concretos de RF/RNF/Épica/HU,
usando como base la columna "ALCANCE MÍNIMO" de la tabla de épicas (§12) y la prioridad P1 de cada
historia.

### Épicas cubiertas (las 8, de forma parcial)

Las **8 épicas** (EP-01 a EP-08) están representadas en el MVP, pero **no todas sus HU**: solo se
documentan las historias marcadas **P1** en `guia-sgr.md` §12, que son las que §13.2 agrupa como
"alcance mínimo recomendado". Las HU marcadas P2 o P3 quedan fuera del MVP y no se documentan en la
Actividad 1 ni se diagraman en la Actividad 3.

| Épica | Nombre | HU incluidas en el MVP (P1) | HU excluidas (P2/P3) |
|---|---|---|---|
| EP-01 | Registro y gestión de actividades | HU-01, HU-02, HU-04 | HU-03 (P2) |
| EP-02 | Medición y desempeño | HU-05, HU-06, HU-07 | HU-08 (P2) |
| EP-03 | Evidencias y verificación | HU-09, HU-10, HU-11 | — (las 3 HU de esta épica son P1) |
| EP-04 | Agenda colectiva y compromisos | HU-12, HU-13, HU-14 | HU-15 (P2) |
| EP-05 | Monitoreo y control de gestión | HU-16, HU-17, HU-18 | HU-19 (P2) |
| EP-06 | Reportabilidad y toma de decisiones | HU-20 | HU-21 (P2), HU-22 (P3) |
| EP-07 | Plataforma colaborativa | HU-23, HU-25 | HU-24 (P2) |
| EP-08 | Administración, seguridad y trazabilidad | HU-26, HU-27, HU-28, HU-29, HU-30 | HU-31 (P2) |

**Total MVP: 22 HU de 31** (las 22 marcadas P1 en `guia-sgr.md` §12). Quedan fuera del alcance: HU-03,
HU-08, HU-15, HU-19, HU-21, HU-22, HU-24 y HU-31 (todas P2 o P3).

### RF y RNF cubiertos por el MVP

Se incluyen los RF/RNF que sustentan directamente alguna de las 22 HU del MVP (columna "Requisitos
relacionados" de cada HU en `guia-sgr.md` §12.2 a §12.9):

- **RF incluidos:** RF-001 a RF-014, RF-016 a RF-029, RF-031 a RF-033, RF-036, RF-037, RF-038.
- **RF excluidos del MVP:** RF-015 (asociado solo a HU-03, P2), RF-030 (asociado solo a HU-19, P2),
  RF-035 (asociado solo a HU-24, P2). RF-034 sí se cubre porque sustenta a HU-23, que es P1.
- **RNF incluidos como citados directamente:** RNF-003, RNF-004, RNF-005, RNF-008, RNF-017 (aparecen en
  la columna "Requisitos relacionados" de alguna HU P1).
- **RNF-001, RNF-002, RNF-006, RNF-007, RNF-009 a RNF-016, RNF-018:** no aparecen citados directamente
  en ninguna HU P1, pero **se incluyen igualmente como RNF transversales del MVP** (disponibilidad,
  rendimiento, confidencialidad, integridad, privacidad, respaldo, usabilidad, accesibilidad,
  compatibilidad, escalabilidad, mantenibilidad, interoperabilidad, monitoreo) porque aplican a
  cualquier subconjunto de funcionalidades que se implemente, no solo a un RF puntual.

**Regla de trazabilidad para la Actividad 1, sección 1.4:** no se simulan datos de encuesta, taller
u otro instrumento (el docente lo aclaró explícitamente: eso no corresponde). El análisis de la
sección 1.4 se hace sobre la información real ya contenida en `guia-sgr.md` (problemática, reglas de
negocio, entidades). Si un RF/RNF del MVP no tiene un punto de la problemática o análisis que lo
sustente de forma puntual, se marca como **"incluido por completitud del MVP (§13.2)"** en la tabla de
la sección 1.4, en vez de forzar una conexión artificial que no está en el documento base.

### Nota para no confundir dos usos distintos de la palabra "MVP" en este proyecto

1. *MVP como recorte de alcance de requerimientos* (esta decisión) → aplica: la Actividad 1 documenta
   únicamente las 22 HU P1 y los RF/RNF que las sustentan, no el documento completo de `guia-sgr.md`.
2. *MVP como entrega funcional demostrable al final del curso* (mencionado en `fuentes/audio-clase-1.md`,
   por la dinámica de "licitación" entre grupos, y en `actividad-2.md` §1.1) → es un concepto relacionado
   pero no idéntico: incluso dentro de las 22 HU del MVP de alcance, la entrega de software puede
   priorizarse de forma incremental dentro de los sprints (ver `guia-sgr.md` §13.3, ruta sugerida de
   desarrollo).

Cualquier IA o integrante que reciba una tarea de este proyecto debe asumir este alcance (22 HU P1, no
el documento completo), salvo que este archivo se actualice explícitamente para decir lo contrario.

---

## Trazabilidad requerimiento → información base (Actividad 1, sección 1.4)

No se simulan hallazgos de encuesta, taller u otro instrumento aplicado a personas: el docente aclaró
explícitamente que no corresponde. Esto **no exime** de cumplir la Rúbrica 2 (criterio 2.1.1/2.1.2,
25 % de la nota), que exige "aplica las técnicas" y "tabula y analiza los datos obtenidos" — la
sección 1.3/1.4 debe mostrar contenido real y concreto, no solo declarar la técnica sin tabular nada.
Con alcance de MVP, la mayoría de los RF/RNF incluidos sí deberían poder sustentarse en algún punto
concreto de la problemática, las reglas de negocio o el análisis que ya trae `guia-sgr.md`, porque el
MVP ya es un subconjunto acotado y priorizado. Aun así, para los RNF transversales (ver lista arriba)
que no responden a un punto puntual del documento base sino a buenas prácticas generales de la
aplicación, se marca la etiqueta **"incluido por completitud del MVP (§13.2)"** en la tabla de la
sección 1.4 en vez de forzar una relación artificial que el documento base no sostiene.

## Metodología

**Scrum.**

**Segunda metodología de comparación (Actividad 2, §1.3): Cascada.** Categoría estructurada, elegida
por ser la que ofrece el contraste técnico más claro frente a Scrum para un caso con fases de
análisis/diseño/construcción bien identificables (se descarta Espiral, excluida explícitamente de
las categorías admisibles).

## Nomenclatura y codificación

Se mantienen los mismos códigos de `guia-sgr.md` (RF-001, RNF-001, EP-01, HU-01, etc.), sin renumerar.
Los RF/RNF/HU que quedan fuera del MVP (ver tabla de arriba) **no se renumeran ni se reutilizan sus
códigos** — simplemente no aparecen en la documentación de este proyecto.

---

## Relación Actividad–ElementoCatalogo en el diagrama de clases (Actividad 3)

**Decisión cerrada: la asociación entre `Actividad` y `ElementoCatalogo` se modela como 4 asociaciones
independientes con rol** (`tipoActividad`, `servicio`, `atencion`, `subatencion`), no como una sola.
No se toca la redacción de ningún RF/RNF/HU para llegar a esto — es una decisión de diseño del
diagrama, no una corrección del documento base.

**Por qué:** `guia-sgr.md` §8.1 ("Campos mínimos del registro de actividad") enumera textualmente
"ítem, servicio, tipo y subtipo de atención" como parte de un mismo registro, y RF-004 ya administra
esas cuatro categorías como entidades separadas del catálogo ("tipos de actividad, servicio, atención
y subatención por área"). Con una sola asociación `Actividad -- ElementoCatalogo`, una actividad solo
puede clasificarse en una de las cuatro categorías a la vez, lo que no permite representar un caso
real del dominio (ej. una visita a terreno por poda de árboles, registrada simultáneamente como
atención comunitaria y como reclamo).

**Nota sobre RF-009:** RF-009 dice "ítem" en singular, y los criterios de aceptación de HU-01 también
hablan de "indicador asociado" en singular. Esa redacción no se cambia. La lectura del equipo es que
§8.1 (que sí lista las cuatro categorías) y RF-009 (resumen corto del mismo requisito) no son
contradictorios entre sí, sino que §8.1 da el detalle que RF-009 resume — por eso el modelo de 4
asociaciones no reinterpreta RF-009, solo traduce a UML lo que §8.1 ya especifica.

**Impacto en otros artefactos de la Actividad 3:**
- `assets/actividad-3/clases-dominio.puml` y su SVG: ya actualizados con las 4 asociaciones.
- Wireframe `wf-02-registrar-actividad.png` (Pantalla 2, "Registrar Actividad"): **pendiente**. Hoy
  muestra un único dropdown "Ítem / Categoría"; debería pasar a 4 selectores. Es una imagen sin fuente
  editable versionada en el repo, por lo que no se regenera junto con el diagrama de clases — queda
  anotado en `actividad-3.md` (Pantalla 2) para quien la actualice.
- HU-03 ("Registro de servicios entregados") **no** es el sustento de este cambio: es P2 y queda fuera
  del alcance del MVP (ver tabla de arriba). El respaldo es §8.1 + RF-004, ambos dentro del MVP.

Cualquier integrante o IA que reciba una tarea sobre el diagrama de clases o el wireframe de Registrar
Actividad debe asumir esta decisión ya cerrada, salvo que este archivo se actualice explícitamente
para decir lo contrario.
