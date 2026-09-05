# Evaluación 2 — Proyecto SGR
## Qué hay que realizar en cada actividad

---

## Actividad 1 — Técnicas para la toma de requerimientos

### 1. Técnicas e instrumentos de toma de requerimientos

Como el caso SGR ya viene definido por el docente, esto no es "inventar" el problema ni simular un
instrumento aplicado a personas: es hacer la **bajada** del documento base (`guia-sgr.md`), que ya
trae la problemática, el análisis y los requerimientos resueltos. **No se simulan ni se inventan
datos de encuesta, taller u otro instrumento** (ni participantes, ni respuestas, ni porcentajes, ni
gráficos de resultados ficticios) — el docente lo aclaró explícitamente: eso no corresponde y no debe
figurar en el informe.

**Importante — esto no exime de tabular y analizar datos.** La Rúbrica 2 (criterio 2.1.1/2.1.2, 25 %
de la nota) exige explícitamente que el equipo **"aplica las técnicas necesarias"** y **"tabula y
analiza los datos obtenidos"** para definir los requerimientos; el enunciado pide lo mismo ("el
análisis de los datos y los resultados obtenidos"). Que no se simulen encuestas no significa dejar
esta parte vacía o solo descriptiva ("así se aplicaría la técnica"): el dato que se tabula y analiza
debe **existir y ser real**, tomado del propio `guia-sgr.md` (problemática, reglas de negocio,
entidades, atributos de calidad). Una sección 1 que solo describe el instrumento sin tabular ni
analizar nada concreto arriesga esa fila de la rúbrica igual que si hubiera usado datos inventados.

- Elegir 1 o más técnicas (entrevista, encuesta, taller de co-creación, revisión documental,
  observación, etc.) y **justificar técnicamente por qué esas técnicas** son adecuadas para este caso
  (qué tipo de información permiten levantar, por qué calzan con el escenario municipal descrito en
  `guia-sgr.md`).
- Presentar el **instrumento** que se usaría (ej. pauta de entrevista con preguntas, formulario de
  encuesta con sus ítems) como diseño metodológico — sin aplicarlo a datos simulados.
- Mostrar la **tabulación y el análisis de los datos**, entendiendo por "datos" la información que
  **ya está en `guia-sgr.md`** (problemática descrita, reglas de negocio, entidades, atributos de
  calidad): organizarla en tablas/resúmenes propios, analizarla y conectarla con la técnica elegida —
  este paso debe quedar tan visible como si fueran resultados de un instrumento aplicado, solo que
  construido sobre información real del documento base, no inventada.
- De ese análisis debe **derivarse explícitamente** la lista de requerimientos — no pueden aparecer
  los RF/RNF "de la nada", tienen que verse conectados a la información del documento base.

### 2. Requerimientos Funcionales (RF) y No Funcionales (RNF)

- Hacer la **bajada** desde el documento base SGR: seleccionar qué RF/RNF del documento aplican al alcance que el equipo decida cubrir (recomendable usar el MVP de la sección 13.2 como referencia, o un subconjunto de este).
- Redactarlos con formato propio del equipo (código, descripción, prioridad, etc.), no copiar/pegar tal cual del PDF.
- Deben quedar codificados de forma clara (ej. RF-01, RF-02… RNF-01, RNF-02…) porque **más adelante se necesitan para la trazabilidad** (Actividad 3): RF/RNF → Épica → HU → Caso de Uso → Wireframe.

### 3. Épicas, Historias de Usuario y Tareas

- **Épicas**: agrupaciones grandes de funcionalidad (ej. "Gestión de Actividades", "Agenda Colectiva", "Medición y Semáforo"). Cada épica debe alinearse con un bloque del alcance funcional del documento SGR.
- **Historias de Usuario (HU)** por cada épica, en formato estándar: *"Como [rol], quiero [acción], para [beneficio]"*, con sus **criterios de aceptación** (el documento SGR ya trae ejemplos en formato Dado/Cuando/Entonces que pueden servir de modelo).
- **Tareas** específicas dentro de cada HU (los pasos técnicos para implementarla: ej. "crear endpoint de registro", "diseñar tabla en BD", "validar formulario en frontend").

### 4. Estimación de esfuerzo — con justificación

- Asignar esfuerzo a cada tarea (o a nivel de HU, según lo que definan) usando un criterio explícito: story points, t-shirt sizing, horas estimadas, etc.
- **No basta con poner el número.** Hay que explicar el criterio usado para llegar a esa estimación: complejidad técnica, dependencias con otras tareas, incertidumbre, tamaño del equipo (3 personas), etc.

### 5. Planificación y gestión

- El avance de esta evaluación debe estar **gestionado en una herramienta de control**: GitHub Projects ("GCAP") **o** un plan de trabajo/**carta Gantt**.
- Las HU y tareas deben quedar reflejadas en un tablero, no solo en el informe como texto.
- **Pendiente de confirmar con el docente**: si esto va como capturas/anexo dentro del mismo informe, o si es un entregable separado (ej. link al repositorio/proyecto).

### Checklist Actividad 1

| Debe incluir | ¿Listo? |
|---|---|
| Técnica(s) de levantamiento justificada(s) | ☐ |
| Instrumento presentado (pauta/encuesta), como diseño metodológico | ☐ |
| Tabulación y análisis con datos reales y concretos de `guia-sgr.md` (no solo mencionar la fuente; debe verse tabla/resumen y análisis, no un instrumento aplicado a datos simulados) | ☐ |
| Lista de RF codificados | ☐ |
| Lista de RNF codificados | ☐ |
| Épicas definidas | ☐ |
| HU por épica con criterios de aceptación | ☐ |
| Tareas por cada HU | ☐ |
| Esfuerzo estimado + justificación del criterio | ☐ |
| Evidencia de tablero (GitHub Projects / carta Gantt) | ☐ |

---

## Actividad 2 — Selección y Justificación de la Metodología

### 1. Análisis técnico comparativo de al menos 2 metodologías

- Deben ser **viables y aplicables al alcance concreto** del proyecto SGR (no un análisis genérico de metodologías en abstracto).
- Categorías admisibles: **estructuradas** (ej. cascada), **ágiles**, **híbridas** o **incrementales**.
- **Espiral queda explícitamente excluida** — ni se menciona como opción a comparar, por las limitaciones de tiempo del semestre.

### 2. Nivel de profundidad exigido (esto es lo más importante y lo que más se repite)

- **No se acepta un cuadro simple de ventajas/desventajas.** El docente lo dice de forma explícita y enfática en ambos audios.
- La justificación debe basarse en **fundamentos de ingeniería de software**, es decir, conectar características técnicas de cada metodología (ciclos de retroalimentación, manejo del cambio, artefactos que produce, roles, cadencia de entregas, forma de gestionar riesgo) con las **condiciones reales del proyecto**:
  - Equipo de 3 personas.
  - Plazo acotado (9 días para esta etapa, y el semestre completo como restricción mayor).
  - Requerimientos ya definidos por el docente pero con margen de ajuste ("bajada").
  - Necesidad de llegar a un **MVP funcional** demostrable al final del curso.
- De esa comparación técnica debe **derivarse y justificarse** cuál metodología se elige finalmente para el desarrollo.

### 3. Definición detallada de recursos

**a) Hardware y Software**
- Especificar requisitos **mínimos y óptimos**.
- Separar **etapa de desarrollo** vs **etapa de producción/operación**.
- Detalle nuevo del audio: estos recursos **se conectarán después con el diagrama de despliegue** (Actividad 3), así que conviene definirlos pensando ya en qué nodos/infraestructura se van a representar ahí (servidor web, servidor BD, cliente, etc.).

**b) Recursos Humanos**
- Definir **roles, perfiles y organización del equipo** de trabajo (para desarrollo y para operación).
- Si se elige una metodología como **XP**, hay que justificar técnicamente el tipo de profesionales requeridos — el docente da la pista explícita de que **XP típicamente exige desarrolladores con más experiencia, no solo perfiles junior**, dado el pair programming y la disciplina técnica que exige. Esto es relevante porque el equipo real tiene solo 3 integrantes (probablemente estudiantes), así que conviene anticipar y abordar esa tensión en el informe en vez de ignorarla.

### Checklist Actividad 2

| Debe incluir | ¿Listo? |
|---|---|
| Mínimo 2 metodologías comparadas (sin espiral) | ☐ |
| Comparación con fundamento técnico de ingeniería (no cuadro pro/contra) | ☐ |
| Metodología elegida, justificada según condiciones reales del proyecto | ☐ |
| Recursos de Hardware/Software mínimos (desarrollo) | ☐ |
| Recursos de Hardware/Software óptimos (desarrollo) | ☐ |
| Recursos de Hardware/Software mínimos (operación) | ☐ |
| Recursos de Hardware/Software óptimos (operación) | ☐ |
| Roles y organización del equipo humano | ☐ |
| Justificación de perfiles según la metodología elegida | ☐ |

---

## Actividad 3 — Diagramas UML y Wireframes

Esta es la actividad con más peso en la rúbrica (**40%**) y la de mayor riesgo técnico, porque exige varios diagramas correctamente vinculados entre sí.

### 1. Diagrama de Casos de Uso — dos niveles obligatorios

**a) Alto nivel**
- Un diagrama general **derivado directamente de las épicas**.
- Debe representar el **escenario global**: actores involucrados y cómo se comunican con el sistema.
- Cada épica se traduce, a grandes rasgos, en un conjunto de casos de uso relacionados.

**b) Específicos**
- Diagramas más detallados por módulo/funcionalidad.
- Deben usar correctamente:
  - **`include`** → comportamiento **obligatorio y reutilizable**, que se gatilla siempre desde el caso de uso principal. El profesor lo compara con una "función" que varios casos de uso consumen (ej. "Validar Evidencia" incluido por distintos casos que suben evidencia).
  - **`extend`** → comportamiento **opcional/condicional** que extiende un caso base solo si se cumple una condición (ej. "Generar Alerta" extiende "Revisar Avance").
- Este es un punto de riesgo técnico común: confundir include/extend invierte la lógica y es un error clásico de evaluación.

### 2. Diagrama de Clases

- Estructurar lógicamente las **entidades del dominio** del sistema (ej. Funcionario, Actividad, Evidencia, Delegación, Meta, según el caso SGR).
- Incluir atributos, métodos relevantes y relaciones (asociación, composición, herencia si aplica).

### 3. Diagrama de Secuencia — **agregado por la rúbrica**

- No aparece mencionado en las instrucciones ni en los audios, pero **sí está explícito en la Rúbrica 2** (dimensión "Análisis de los recursos de acuerdo a los principios de desarrollo", 40%): pide Caso de Uso, Clase, **secuencia**, componentes y despliegue.
- Conviene incluirlo igual para no perder puntaje en esa dimensión — típicamente se hace uno por cada caso de uso principal (ej. secuencia de "Registrar Actividad con Evidencia").

### 4. Diagrama de Componentes

- Enfocado en los **componentes internos y consumos de servicios** del software (ej. cómo el frontend consume la API, cómo la API consume la base de datos, servicios externos si los hay).

### 5. Diagrama de Despliegue

- Infraestructura **física y lógica**: hardware, software y consumos (nodos como servidor web, servidor BD, cliente; protocolos de comunicación entre ellos).
- **Debe vincularse directamente** con los recursos de hardware/software mínimos y óptimos definidos en la Actividad 2 — no pueden ser inconsistentes entre sí.

### 6. Diagrama de Requerimientos (en árbol)

- Representación **jerárquica y en ramas**: Requerimiento Funcional → Épica → Historia de Usuario → Tareas de desarrollo.
- Funciona como **mapa visual del avance del proyecto**, pensado para poder cruzarse con el estado real del tablero de trabajo (GitHub Projects o carta Gantt de la Actividad 1).

### 7. Wireframes + Matriz de Trazabilidad — el punto más exigente

- Los wireframes son bocetos/diseño de pantallas del sistema (interfaz, no funcionalidad backend).
- Se exige una **cadena de trazabilidad estricta y obligatoria**, elemento por elemento:

  **Requerimiento (Funcional o No Funcional) → Épica → Historia de Usuario → Caso de Uso de Alto Nivel → Caso de Uso Específico → Wireframe**

- La cadena parte de "Requerimiento Funcional/No Funcional" (ambos, no solo uno).
- El profesor da un ejemplo concreto: **justificar la pantalla de login recorriendo la cadena completa de principio a fin** — esto sirve como plantilla de cómo debe verse cada trazabilidad documentada (uno por cada wireframe presentado, no solo uno de ejemplo).

### Checklist Actividad 3

| Debe incluir | ¿Listo? |
|---|---|
| Diagrama de Casos de Uso — alto nivel (desde épicas) | ☐ |
| Diagrama(s) de Casos de Uso específicos con include/extend correctos | ☐ |
| Diagrama de Clases del dominio | ☐ |
| Diagrama(s) de Secuencia (exigido por la rúbrica) | ☐ |
| Diagrama de Componentes (consumo de servicios) | ☐ |
| Diagrama de Despliegue (coherente con Actividad 2) | ☐ |
| Diagrama de Requerimientos en árbol | ☐ |
| Wireframes de las pantallas principales | ☐ |
| Trazabilidad completa por cada wireframe (RF/RNF→Épica→HU→CU alto nivel→CU específico→Wireframe) | ☐ |
