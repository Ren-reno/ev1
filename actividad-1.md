# Actividad 1 — Técnicas para la toma de requerimientos

**Ponderación en la rúbrica: 25%**

**Depende de:** [`decisiones.md`](./decisiones.md) — usar los mismos códigos de `guia-sgr.md` (no
renumerar). **Alcance: MVP de `guia-sgr.md` §13.2** (decisión cerrada, ver `decisiones.md` § Alcance
del MVP) — se documentan únicamente las **22 HU marcadas P1** (de las 31 totales) y los RF/RNF que las
sustentan, más los RNF transversales. La sección 2 de este documento debe incluir solo esos RF/RNF, y
la sección 3 las 8 épicas (todas aparecen, aunque no todas con sus HU completas) con únicamente las 22
HU del MVP — ver la tabla completa de HU incluidas/excluidas en `decisiones.md`.

**Alimenta a:** Actividad 3 (los códigos de RF/RNF/EP/HU definidos aquí son los que se usan en los
diagramas de casos de uso, el diagrama de requerimientos en árbol, y la matriz de trazabilidad). Cualquier
cambio de nombre o alcance hecho después de cerrar esta actividad debe avisarse a quien trabaje la
Actividad 3.

**Fuentes a consultar:** `fuentes/que-hacer-1-2-3.md` (sección Actividad 1), `fuentes/guia-sgr.md`
(secciones de RF §5, RNF §6, épicas y HU §12 — **solo las 22 HU marcadas P1**, ver `decisiones.md` §
Alcance del MVP), `fuentes/audio-clase-1.md` y `fuentes/audio-clase-2.md` (aclaraciones sobre esfuerzo
y planificación), `fuentes/apuntes-cocreacion-patrones.md` (marco teórico: técnicas de cocreación y
levantamiento — entrevistas, talleres, encuestas, prototipos, mapeo de historias de usuario — y
clasificación de requerimientos no funcionales según Sommerville; usar solo como respaldo conceptual,
**no** como fuente de RF/RNF del caso SGR, eso viene únicamente de `guia-sgr.md`).

---

## 1. Técnicas e instrumentos de toma de requerimientos

> El caso SGR ya viene definido por el docente — esto no es "inventar" el problema, sino simular y
> documentar el proceso de levantamiento como si se hubiera hecho con el cliente (la Municipalidad).
> Los datos deben ser simulados/ficticios (no está permitido usar datos reales).

### 1.1 Técnica(s) elegida(s) y justificación

_(Elegir 1 o más: entrevista, encuesta, taller de co-creación, revisión documental, observación, etc.
Justificar por qué son adecuadas para este caso específico.)_

> Apoyo teórico disponible en `fuentes/apuntes-cocreacion-patrones.md` (sección "Técnicas de
> cocreación y levantamiento de requerimientos"): entrevistas, talleres de cocreación, encuestas y
> cuestionarios, observación, prototipos, mapeo de historias de usuario, análisis de documentación y
> focus groups. Útil para justificar con fundamento académico por qué se elige cada técnica, y para
> citar a Sommerville al definir qué es un requerimiento y el proceso de obtención de requisitos.

### 1.2 Instrumento aplicado

_(Presentar el instrumento en sí: pauta de entrevista con preguntas, formulario de encuesta con sus
ítems, etc.)_

### 1.3 Tabulación y análisis de los datos

_(Datos simulados pero presentados como resultados reales de aplicar el instrumento: tablas, gráficos
simples, hallazgos.)_

### 1.4 Derivación de requerimientos

_(Explicar cómo, a partir del análisis anterior, se llega a la lista de RF/RNF de la sección 2 — no
deben aparecer "de la nada".)_

---

## 2. Requerimientos Funcionales y No Funcionales

> Bajada desde `guia-sgr.md`: incluir **solo** los RF/RNF del MVP fijado en `decisiones.md` § Alcance
> del MVP (los que sustentan alguna de las 22 HU marcadas P1, más los RNF transversales). No copiar
> RF/RNF que solo aparezcan asociados a una HU P2/P3 excluida del MVP. Redactar con formato propio del
> equipo (no copiar/pegar tal cual). Código según `decisiones.md` (numeración original de `guia-sgr.md`,
> sin renumerar). Cada RF/RNF debe poder rastrearse hasta la tabla de la sección 1.4, ya sea con un
> hallazgo real o con la etiqueta "incluido por completitud del MVP (§13.2)".

### 2.1 Requerimientos Funcionales

| Código | Descripción | Prioridad |
|---|---|---|
| RF-XXX | | |

### 2.2 Requerimientos No Funcionales

> Para clasificar o justificar cada RNF puede usarse la taxonomía de `fuentes/apuntes-cocreacion-patrones.md`
> (Sommerville): requerimientos de producto (usabilidad, eficiencia, fiabilidad, portabilidad),
> organizacionales (entrega, implementación, estándares) y externos (interoperabilidad, éticos,
> legislativos — privacidad y seguridad). No es obligatorio anotar la categoría en la tabla, pero sirve
> como respaldo si la rúbrica pide fundamentar el tipo de cada RNF.

| Código | Descripción | Prioridad |
|---|---|---|
| RNF-XXX | | |

---

## 3. Épicas, Historias de Usuario y Tareas

### 3.1 Épicas cubiertas

_(Las 8 épicas de `guia-sgr.md` §12 aparecen representadas, pero solo con sus HU marcadas P1 —ver la
tabla completa de HU incluidas/excluidas por épica en `decisiones.md` § Alcance del MVP. No agregar
HU-03, HU-08, HU-15, HU-19, HU-21, HU-22, HU-24 ni HU-31: quedan fuera del MVP.)_

| Código | Nombre | RF/RNF relacionados |
|---|---|---|
| EP-XX | | |

### 3.2 Historias de Usuario por épica

_(Formato: "Como [rol], quiero [acción], para [beneficio]", con criterios de aceptación en formato
Dado/Cuando/Entonces.)_

#### EP-XX — [nombre de la épica]

**HU-XX:** Como [rol], quiero [acción], para [beneficio].
- Criterio de aceptación (Dado/Cuando/Entonces): ...

### 3.3 Tareas por Historia de Usuario

_(Pasos técnicos para implementar cada HU: ej. "crear endpoint de registro", "diseñar tabla en BD",
"validar formulario en frontend".)_

| HU | Tarea |
|---|---|
| HU-XX | |

---

## 4. Estimación de esfuerzo

> No basta con poner el número — explicar el criterio usado: complejidad técnica, dependencias con
> otras tareas, incertidumbre, tamaño del equipo (4 personas).

**Criterio elegido:** _(story points / t-shirt sizing / horas estimadas, etc.)_

| Tarea | Esfuerzo | Justificación |
|---|---|---|
| | | |

---

## 5. Planificación y gestión

> Evidencia de tablero: GitHub Projects ("GCAP") o carta Gantt. Pendiente de definir en `decisiones.md`
> punto 4 (herramienta de gestión) — si se usa GitHub Projects del mismo repo, adjuntar aquí capturas o
> el link al tablero.

_(Adjuntar evidencia cuando esté disponible.)_

---

## Checklist de cierre — Actividad 1

- [ ] Alcance verificado contra `decisiones.md` § Alcance del MVP (solo las 22 HU P1, sin agregar HU-03/08/15/19/21/22/24/31)
- [ ] Técnica(s) de levantamiento justificada(s)
- [ ] Instrumento aplicado (pauta/encuesta)
- [ ] Tabulación y análisis de datos (aunque simulados)
- [ ] Lista de RF codificados
- [ ] Lista de RNF codificados
- [ ] Épicas definidas
- [ ] HU por épica con criterios de aceptación
- [ ] Tareas por cada HU
- [ ] Esfuerzo estimado + justificación del criterio
- [ ] Evidencia de tablero (GitHub Projects / carta Gantt)
- [ ] Códigos finales comunicados a quien trabaje la Actividad 3
