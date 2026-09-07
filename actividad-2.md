# Actividad 2 — Selección y justificación de la metodología

**Ponderación en la rúbrica: 35%**

**Depende de:**
- [`decisiones.md`](./decisiones.md) — metodología elegida: **Scrum**. Segunda metodología de
  comparación: **Cascada** (categoría estructurada, la que ofrece el contraste técnico más claro
  frente a Scrum para un caso con fases de análisis/diseño/construcción bien identificables). Alcance
  del proyecto: MVP de 22 HU (ver `decisiones.md` § Alcance del MVP).
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

Scrum organiza el trabajo en iteraciones cortas y de duración fija llamadas *sprints*, dentro de las
cuales el equipo diseña, construye y prueba un incremento potencialmente utilizable del producto.

- **Ciclos de retroalimentación:** Scrum define eventos formales de inspección y adaptación —
  planificación de sprint, reunión diaria, revisión de sprint y retrospectiva— que generan puntos de
  control cada pocos días en vez de esperar al cierre del proyecto completo. Con un plazo de 9 días
  para esta etapa y el semestre completo como restricción mayor, contar con puntos de control tan
  frecuentes permite detectar desviaciones de alcance o de estimación de forma temprana, cuando aún es
  barato corregirlas.
- **Manejo del cambio:** el *Product Backlog* es una lista viva y priorizable; sus ítems pueden
  reordenarse o ajustarse entre sprints sin invalidar el trabajo ya completado en sprints anteriores.
  Esto encaja con que los requerimientos de este proyecto ya vienen definidos por el docente pero con
  margen de ajuste ("bajada"): ese ajuste se absorbe actualizando el backlog, sin necesidad de
  reabrir trabajo ya cerrado.
- **Artefactos:** Product Backlog, Sprint Backlog e Incremento. Son artefactos que se construyen de
  forma incremental y verificable, lo que calza directamente con las 22 HU del MVP fijadas en
  `decisiones.md`: pueden organizarse como un único Product Backlog priorizado, siguiendo la misma
  lógica de la ruta de sprints sugerida en `guia-sgr.md` §13.3 (Sprint 0 a Sprint 4, cada uno con un
  foco funcional distinto).
- **Roles:** Product Owner, Scrum Master y equipo de desarrollo multifuncional, sin jerarquías internas
  rígidas. En un equipo de 4 personas estos roles pueden combinarse o rotar (ver §3.3) sin necesitar
  especialistas dedicados de tiempo completo a un único rol.
- **Cadencia de entregas:** incrementos funcionales al cierre de cada sprint, en lugar de una entrega
  única al final del proyecto. Esto es relevante porque el proyecto necesita llegar a un MVP funcional
  demostrable al término del curso: Scrum permite mostrar avance ejecutable sprint a sprint, reduciendo
  el riesgo de una entrega "todo o nada" al final del semestre.
- **Gestión de riesgo:** al inspeccionarse el incremento al cierre de cada sprint, los riesgos técnicos
  (una historia más compleja de lo previsto, un supuesto de diseño equivocado) se detectan y mitigan
  tempranamente, en vez de descubrirse recién en una fase de pruebas tardía.

### 1.3 Metodología 2: Cascada

Cascada organiza el proyecto en fases secuenciales (análisis de requerimientos, diseño,
implementación, pruebas, mantenimiento), donde cada fase debe cerrarse y validarse formalmente antes
de iniciar la siguiente.

- **Ciclos de retroalimentación:** la validación real con el interesado (en este caso, el docente)
  ocurre al cierre de cada fase o, más comúnmente, recién en la fase de pruebas. Con un plazo de 9 días
  para esta etapa, un esquema que solo permite corregir un malentendido de alcance al final de una fase
  larga deja muy poco margen de reacción.
- **Manejo del cambio:** Cascada asume requisitos estables desde el inicio; un ajuste de alcance obliga
  a retroceder a las fases de análisis y diseño y volver a documentarlas. El margen de ajuste que el
  docente deja explícitamente sobre los requerimientos del caso SGR es, precisamente, el escenario que
  más penaliza este modelo.
- **Artefactos:** documentación extensa por fase (especificación de requisitos, documento de diseño,
  plan de pruebas), pensada para fijar trazabilidad completa antes de programar. Es una fortaleza en
  proyectos regulados, pero compite directamente por tiempo con los 9 días disponibles para esta etapa.
- **Roles:** roles especializados y secuenciales (analista, diseñador, programador, tester), que
  normalmente no se solapan en el tiempo. Con solo 4 integrantes, este esquema fuerza a que las mismas
  personas esperen a que una fase completa cierre antes de poder avanzar en la siguiente, sin poder
  paralelizar el trabajo.
- **Cadencia de entregas:** una entrega única al cierre del proyecto o de cada fase larga, sin
  incrementos funcionales demostrables antes de eso. Esto choca con la necesidad de exhibir un MVP
  funcional de forma progresiva durante el semestre.
- **Gestión de riesgo:** los riesgos de diseño o de interpretación de requerimientos se detectan tarde,
  típicamente en la fase de pruebas, cuando corregirlos puede implicar retrabajo de fases ya cerradas.

Cascada seguiría siendo la opción más adecuada si los requerimientos estuvieran completamente cerrados
y no fueran a cambiar, si existiera una exigencia contractual o regulatoria de documentación exhaustiva
previa a programar, o si el dominio fuera de muy bajo riesgo técnico. Ninguna de esas tres condiciones
describe completamente a este proyecto: el alcance tiene margen de ajuste, no hay una exigencia
contractual de ese tipo, y el equipo (compuesto por estudiantes) está a la vez aprendiendo el propio
proceso de desarrollo, lo que introduce incertidumbre técnica que Cascada gestiona peor que Scrum.

### 1.4 Comparación técnica y elección final

El análisis siguiente no yuxtapone columnas de ventajas y desventajas: para cada una de las seis
dimensiones técnicas ya usadas en 1.2 y 1.3, se explica cómo la resuelve cada metodología y, de
inmediato, qué condición real del proyecto (§1.1) inclina la balanza hacia una u otra.

- **Ciclos de retroalimentación.** Scrum inspecciona el trabajo cada pocos días, mediante revisión y
  retrospectiva de sprint; Cascada solo lo hace al cierre de una fase completa o en la fase de pruebas.
  Con 9 días para esta etapa y el semestre completo como restricción mayor, un ciclo de inspección de
  días es la única frecuencia compatible con el plazo: en Cascada, un malentendido de alcance recién se
  descubriría cuando ya no quedara tiempo para corregirlo sin comprometer la entrega.
- **Manejo del cambio.** El Product Backlog de Scrum se reordena entre sprints sin invalidar el trabajo
  ya cerrado; en Cascada, un cambio de alcance obliga a reabrir las fases de análisis y diseño ya
  documentadas. Los requerimientos de este proyecto vienen definidos por el docente pero con margen de
  ajuste explícito ("bajada"): ese margen es justamente el escenario que Cascada penaliza con más
  retrabajo y que Scrum absorbe sin fricción.
- **Artefactos.** Scrum construye Product Backlog, Sprint Backlog e Incremento de forma progresiva;
  Cascada exige especificación, diseño y plan de pruebas extensos antes de escribir una sola línea de
  código. Las 22 HU del MVP ya vienen secuenciadas por sprint en `guia-sgr.md` §13.3 (Sprint 0 a Sprint
  4): ese plan de origen ya asume artefactos incrementales, no una especificación monolítica previa.
- **Roles.** Scrum trabaja con un equipo multifuncional donde los roles se combinan o rotan; Cascada
  separa analista, diseñador, programador y tester en fases que no se solapan en el tiempo. Con 4
  integrantes, la secuencialidad de Cascada dejaría a la mayoría del equipo sin tareas paralelas
  posibles durante buena parte de cada fase, algo que un equipo tan reducido no puede permitirse en 9
  días.
- **Cadencia de entregas.** Scrum entrega un incremento funcional al cierre de cada sprint; Cascada
  entrega una sola vez, al final del proyecto o de una fase larga. El proyecto necesita mostrar un MVP
  funcional de forma verificable durante el semestre y no solo al final, lo que exige poder exhibir algo
  ejecutable sprint a sprint, cadencia que Cascada no ofrece por diseño.
- **Gestión de riesgo.** Scrum expone los riesgos técnicos al cierre de cada sprint, cuando corregirlos
  es barato; Cascada los expone recién en la fase de pruebas, cuando corregirlos puede implicar
  retrabajo de fases ya cerradas. Un equipo de estudiantes que está aprendiendo a la vez la propia
  disciplina de desarrollo concentra más incertidumbre técnica que un equipo profesional experimentado,
  precisamente el escenario donde detectar errores temprano importa más, no menos.

En las seis dimensiones, la metodología que mejor resuelve las condiciones reales del proyecto —equipo
de 4 personas, plazo de 9 días con el semestre como restricción mayor, requerimientos con margen de
ajuste y un alcance ya secuenciado por sprints— es Scrum. Por eso el equipo confirma su elección: no
como una preferencia declarada de antemano, sino como la que se sostiene dimensión por dimensión frente
a la alternativa estructurada más comparable.

---

## 2. Recursos de Hardware y Software

> Especificar mínimos y óptimos, separando etapa de desarrollo vs. etapa de producción/operación. Estos
> recursos se conectarán después con el diagrama de despliegue (Actividad 3) — conviene definirlos
> pensando ya en qué nodos/infraestructura se van a representar ahí (servidor web, servidor BD, cliente,
> etc.).

> La arquitectura de referencia (`guia-sgr.md` §14.1) separa interfaz web, API/servicios, dominio y
> datos/archivos. Los recursos siguientes se definen pensando ya en esos cuatro bloques, para que
> Actividad 3 pueda representarlos como nodos del diagrama de despliegue sin inconsistencias.

### 2.1 Etapa de desarrollo

| Recurso | Mínimo | Óptimo |
|---|---|---|
| Hardware | Un equipo por integrante: procesador tipo i5/Ryzen 5 o equivalente, 8 GB de RAM, 256 GB de almacenamiento SSD, conexión a internet estable (≥ 10 Mbps) | Procesador tipo i7/Ryzen 7 o equivalente, 16 GB de RAM, 512 GB SSD, segundo monitor, conexión ≥ 50 Mbps |
| Software | Editor/IDE gratuito, cliente Git y cuenta en un repositorio remoto con tablero Scrum integrado (backlog e historias del MVP), motor de base de datos relacional en versión local, runtime del lenguaje de backend elegido, navegador actualizado para pruebas manuales, herramienta de wireframing con plan gratuito | Suite de pruebas automatizadas (unitarias e integración, alineadas con `guia-sgr.md` §14.3), integración continua para ejecutar esas pruebas en cada entrega, entorno en contenedores para que todo el equipo trabaje sobre la misma configuración, plan colaborativo de la herramienta de wireframing |

### 2.2 Etapa de producción/operación

| Recurso | Mínimo | Óptimo |
|---|---|---|
| Hardware | 1 instancia AWS EC2 tipo c2 (cuenta AWS Academy Learner Lab, presupuesto de 50 USD en créditos) con AMI de Linux, alojando en el mismo nodo la API y la base de datos; equipos cliente de los funcionarios municipales sin requisitos especiales (cualquier PC o notebook con navegador compatible, cumpliendo RNF-013) | Misma instancia EC2 c2 (sin escalar a un tipo mayor ni a múltiples instancias, para no exceder el crédito disponible), agregando una réplica de la base de datos para continuidad ante fallos; certificado SSL válido |
| Software | AMI de Linux, Python 3.x, Django (framework de backend), Gunicorn como servidor WSGI de producción (Django por sí solo no está pensado para servir tráfico real), motor de base de datos relacional *(por definir — pendiente elegir entre PostgreSQL u otra opción, y si corre en la misma instancia o en una separada)*, certificado HTTPS básico y respaldos programados (RNF-010: RPO 24 h / RTO 4 h como línea base) | Mismo software del mínimo, más certificado HTTPS reforzado (ej. Let's Encrypt con renovación automática), backups automatizados con mayor frecuencia y retención definida, y configuración de réplica de base de datos (streaming replication) para la continuidad indicada en la columna Hardware |

---

## 3. Recursos Humanos

> Definir roles, perfiles y organización del equipo de trabajo, para desarrollo y para operación.

### 3.1 Roles y organización del equipo (desarrollo)

Equipo: Reinaldo Codoceo, Constanza Vergara, Maricel Videla y Valentina Ferreira. Consistente con la
justificación de §3.3, el Product Owner y el Scrum Master rotan entre los 4 integrantes cada sprint en
vez de fijarse en una sola persona durante todo el proyecto.

| Rol | Perfil | Responsabilidad |
|---|---|---|
| Product Owner (rotativo) | En cada sprint, uno de los 4 integrantes asume el rol; se prioriza a quien tenga mayor familiaridad con el bloque funcional de ese sprint (ver `guia-sgr.md` §13.3) | Gestionar y priorizar el Product Backlog (las 22 HU del MVP), resolver dudas de alcance y aceptar o rechazar el incremento al cierre de su sprint |
| Scrum Master (rotativo) | En cada sprint, uno de los 4 integrantes distinto de quien ejerce de Product Owner ese mismo sprint | Facilitar las ceremonias Scrum, remover impedimentos del equipo y cuidar que el proceso se cumpla sin sobrecargar a nadie |
| Equipo de desarrollo | Los 4 integrantes, incluidos quienes ejercen PO o SM ese sprint | Diseñar, construir, probar e integrar las historias asignadas en cada sprint; participar en la estimación de esfuerzo y en las ceremonias |

### 3.2 Roles y organización del equipo (operación)

| Rol | Perfil | Responsabilidad |
|---|---|---|
| Administrador del sistema / soporte técnico | Perfil técnico; en el contexto académico puede recaer en uno de los integrantes del equipo de desarrollo | Mantener el servidor, aplicar actualizaciones, gestionar respaldos y monitorear la disponibilidad del sistema (RNF-001, RNF-010) |
| Administrador funcional | Funcionario municipal con rol de coordinación (ej. encargado de delegación), no necesariamente técnico | Administrar catálogos, períodos, metas, usuarios y roles dentro del sistema (HU-26 a HU-28); primer punto de contacto ante incidencias funcionales |
| Usuario final | Funcionario de delegación | Registrar actividades y evidencias, gestionar compromisos de la agenda colectiva y consultar su propio desempeño |

### 3.3 Justificación de perfiles según la metodología elegida (Scrum)

A diferencia de otras metodologías ágiles como XP, Scrum no exige perfiles con años de experiencia
profesional ni prácticas técnicas de alta disciplina como el *pair programming* constante o el
desarrollo guiado por pruebas estricto en cada línea de código. Los roles de Scrum (Product Owner,
Scrum Master, equipo de desarrollo) son roles de proceso, no cargos que requieran certificación o
antigüedad, lo que los hace compatibles con un equipo de 4 integrantes que, siendo estudiantes, están
a la vez aprendiendo la propia disciplina de desarrollo.

Esto es relevante porque XP fue descartada precisamente por esta tensión: su exigencia de pair
programming constante y refactorización disciplinada típicamente requiere desarrolladores más senior,
algo difícil de sostener con un equipo de 4 personas sin experiencia profesional previa y en un plazo
de 9 días para esta etapa. Cascada, en cambio, sí admite perfiles junior, pero a costa de secuenciar el
trabajo (nadie puede programar hasta que el diseño esté cerrado por completo), desaprovechando la
capacidad de paralelizar tareas que un equipo pequeño y multifuncional sí tiene bajo Scrum.

Por esta misma razón conviene que el rol de Scrum Master rote entre integrantes a lo largo de los
sprints: con solo 4 personas, ninguna debería quedar fija y exclusivamente en un rol de facilitación
sin aportar también al desarrollo, y la rotación permite que todos adquieran experiencia gestionando
el proceso sin restar tiempo efectivo de construcción al equipo.

---

## Checklist de cierre — Actividad 2

- [x] Mínimo 2 metodologías comparadas (sin espiral) — Scrum y Cascada
- [x] Comparación con fundamento técnico de ingeniería (no cuadro pro/contra)
- [x] Metodología elegida (Scrum), justificada según condiciones reales del proyecto
- [x] Recursos de Hardware/Software mínimos (desarrollo)
- [x] Recursos de Hardware/Software óptimos (desarrollo)
- [x] Recursos de Hardware/Software mínimos (operación)
- [x] Recursos de Hardware/Software óptimos (operación)
- [x] Roles y organización del equipo humano
- [x] Justificación de perfiles según la metodología elegida
- [ ] Recursos comunicados a quien trabaje el diagrama de despliegue en Actividad 3 — pendiente de
      coordinación humana con quien redacte esa parte, no se puede cerrar solo con este documento
