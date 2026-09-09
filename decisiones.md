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

**Total MVP: 23 HU de 31** (las 23 marcadas P1 en `guia-sgr.md` §12). Quedan fuera del alcance: HU-03,
HU-08, HU-15, HU-19, HU-21, HU-22, HU-24 y HU-31 (todas P2 o P3).

> **Corrección de consistencia (detectada al cerrar Actividad 1):** esta línea decía antes "22 HU de
> 31", pero la tabla de arriba ya sumaba 23 códigos de HU al totalizar las 8 épicas
> (3+3+3+3+3+1+2+5 = 23) — el "22" era un error aritmético de esta misma sección, no una cifra
> distinta con otro respaldo. Se corrige aquí para que este archivo, que es la fuente de verdad del
> alcance del proyecto, no siga contradiciendo a `actividad-1.md` (que ya usa 23 y documenta el
> hallazgo en su nota de alcance inicial) ni a `actividad-3.md` (que ya lo señalaba como pendiente en
> su propia nota de consistencia).

### RF y RNF cubiertos por el MVP

Se incluyen los RF/RNF que sustentan directamente alguna de las 23 HU del MVP (columna "Requisitos
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
   únicamente las 23 HU P1 y los RF/RNF que las sustentan, no el documento completo de `guia-sgr.md`.
2. *MVP como entrega funcional demostrable al final del curso* (mencionado en `fuentes/audio-clase-1.md`,
   por la dinámica de "licitación" entre grupos, y en `actividad-2.md` §1.1) → es un concepto relacionado
   pero no idéntico: incluso dentro de las 23 HU del MVP de alcance, la entrega de software puede
   priorizarse de forma incremental dentro de los sprints (ver `guia-sgr.md` §13.3, ruta sugerida de
   desarrollo).

Cualquier IA o integrante que reciba una tarea de este proyecto debe asumir este alcance (23 HU P1, no
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
- Wireframe `wf-02-registrar-actividad.png` (Pantalla 2, "Registrar Actividad"): **resuelto**. Ya
  muestra los 4 selectores en cascada (tipo de actividad, servicio, atención, subatención), consistente
  con el diagrama de clases.
- HU-03 ("Registro de servicios entregados") **no** es el sustento de este cambio: es P2 y queda fuera
  del alcance del MVP (ver tabla de arriba). El respaldo es §8.1 + RF-004, ambos dentro del MVP.

Cualquier integrante o IA que reciba una tarea sobre el diagrama de clases o el wireframe de Registrar
Actividad debe asumir esta decisión ya cerrada, salvo que este archivo se actualice explícitamente
para decir lo contrario.

---

## Ajustes al diagrama de clases: responsable de Delegación, identificador de Auditoría, umbral colectivo

**Decisión cerrada, tras revisión de equipo sobre 4 observaciones:** se incorporan 3 cambios a
`clases-dominio.puml`; un cuarto punto propuesto (agregar un campo `item` a `Actividad`) se evalúa y
se descarta, porque ya está resuelto por la decisión de las 4 asociaciones con `ElementoCatalogo`
(sección anterior).

**1. `Delegacion.obtenerResponsable(): Funcionario` — agregado.** `guia-sgr.md` §8 dice que Delegación
tiene "identificador, nombre, estado, **responsables** y ámbito" (plural). Hoy la asociación
`Delegacion "1" -- "0..*" Funcionario : agrupa` no distingue rol dentro de esa colección; el método
encapsula el filtro por `Rol` (Delegado/Coordinador) que de otro modo se repetiría en cada lugar que
lo necesite (notificaciones, escalamiento de alertas, resumen de delegación).

**2. `Auditoria.identificador: String` — agregado.** `guia-sgr.md` §8 especifica "usuario, evento,
fecha, entidad, **identificador**, valor anterior y valor nuevo" para Auditoría. Sin este atributo, un
registro de auditoría dice qué entidad cambió (ej. "Actividad") pero no cuál fila específica.

**3. `Periodo.umbralColectivo: double` — agregado.** RN-006 define un umbral mínimo de cumplimiento
**colectivo** (80 % inicial, configurable por período o indicador), distinto de `umbralAmbar`
(RN-008), que es el corte de semáforo **individual** por Funcionario. Se decide ubicarlo en `Periodo`,
junto a `umbralAmbar`, en vez de en `Meta`/`Indicador`: ambos umbrales son parámetros configurables que
rigen a todos los vigentes en un período, mientras que `Meta` es una entidad por funcionario/cargo y no
calza con un umbral que mide al colectivo. RN-006 deja abierta la opción de asociarlo a "indicador" en
cambio de "período" — se prioriza `Periodo` por consistencia con el patrón ya existente de
`umbralAmbar`, no porque el documento base cierre la pregunta.

**4. Campo `item` en `Actividad` — evaluado y descartado.** Se propuso agregarlo porque RF-009 y los
criterios de aceptación de HU-01 dicen "ítem"/"indicador asociado" en singular. Ya existe una decisión
de equipo (sección anterior de este archivo) que resuelve exactamente esta redacción: §8.1 lista
"ítem, servicio, tipo y subtipo de atención" como cuatro categorías, y esas cuatro ya están modeladas
como las asociaciones con rol `tipoActividad`/`servicio`/`atencion`/`subatencion` hacia
`ElementoCatalogo`. Agregar un campo `item` adicional sería redundante con esas asociaciones y
reabriría una discusión ya cerrada.

**Impacto en otros artefactos:**
- `assets/actividad-3/clases-dominio.puml` y su SVG: actualizados con los 3 cambios.
- `actividad-3.md`, sección "Relaciones destacadas": documenta el porqué de cada uno.
- El SVG se regeneró con PlantUML 1.2024.7 (el `.puml` original no fija versión). El SVG previo en el
  repo fue generado con 1.2019.6; el layout y estilo (vía `style.cfg`) son equivalentes entre ambas
  versiones — se verificó renderizando ambos a PNG antes de regenerar — por lo que el cambio de
  versión de herramienta no afecta el contenido del diagrama.

Cualquier integrante o IA que reciba una tarea sobre el diagrama de clases debe asumir estos 4 puntos
como ya resueltos, salvo que este archivo se actualice explícitamente para decir lo contrario.

---

## Diagrama de clases: clase `Funcion` separada de `Cargo`, vigencia de HU-04 resuelta

**Decisión cerrada, tras retomar una tarea interrumpida (una sesión anterior se quedó sin tokens antes
de guardar los cambios que había narrado):** se incorporan 2 cambios a `clases-dominio.puml`.

**1. `Funcion` (clase nueva) + `Cargo "0..*" -- "0..*" Funcion : asigna` — agregado, reemplaza a
`Cargo.asignarFuncion(item: String)`.** `guia-sgr.md` §8 agrupa "Cargo y función" en un solo renglón
de la tabla de entidades ("ítems medibles, servicios, ponderaciones y vigencia" como datos mínimos),
pero un método que recibe un `String` sin estructura no permite listar, editar ni reutilizar las
funciones ya creadas, ni expresar que una misma función se repite en más de un cargo. Se modela como
clase propia (`nombre: String`, sin id) con asociación muchos a muchos.

**2. Vigencia de HU-04 Criterio 2 — resuelta sin nuevo atributo.** El criterio dice (`actividad-1.md`):
"dada una actualización de funciones, cuando se guarda, entonces rige desde su fecha de vigencia sin
alterar períodos ya cerrados." No se agrega `vigenciaDesde` a `Funcion` ni se mantiene en `Cargo`: la
vigencia pertenece a la asignación función–cargo para un período, no a la función como concepto ni al
cargo en sí — el mismo patrón que ya resuelve `Meta "0..*" -- "1" Periodo : vigente en`. PlantUML
admite una clase de asociación para esto, pero no hay precedente de esa técnica en el proyecto; se
apoya en el mecanismo `Meta`–`Periodo` ya existente por consistencia de estilo. La restricción de "no
alterar períodos ya cerrados" ya la cubre `Periodo.estado` junto con `reabrir(justificacion: String)`.

**Impacto en otros artefactos:**
- `assets/actividad-3/clases-dominio.puml` y su SVG: actualizados con los 2 cambios.
- `actividad-3.md`: conteo de entidades corregido a 13, sección "Atributos y métodos incorporados"
  documenta ambos puntos.
- **Corrección de numeración de la sesión interrumpida:** había quedado referenciado como "HU-04
  criterio 3" y como "pasa a 12 entidades" — ambos números eran incorrectos. `actividad-1.md` (ya
  cerrada) solo tiene Criterio 1 y Criterio 2 para HU-04; el "3" venía de contar los bullets de
  `guia-sgr.md` §12.2, que es la fuente cruda, no la HU ya aprobada. Y el `.puml` ya tenía 12 clases
  antes de este cambio (11 de `guia-sgr.md` §8 + `ElementoCatalogo`), por lo que sumar `Funcion` da 13,
  no 12.
- El SVG se regeneró con PlantUML 1.2020.02 vía `-config style.cfg` (la entrada anterior de este
  archivo usó 1.2024.7 y verificó equivalencia con 1.2019.6). Con esta versión, a diferencia del color
  de clase, `skinparam backgroundColor white` no queda explícito en el atributo `style` del `<svg>`
  raíz, así que se agregó `background:#FFFFFF;` ahí manualmente para igualar al resto de los diagramas
  del repo.

Cualquier integrante o IA que reciba una tarea sobre el diagrama de clases debe asumir estos 2 puntos
como ya resueltos, salvo que este archivo se actualice explícitamente para decir lo contrario.

---

## Diagrama de secuencia 4.1 (Registrar Actividad con Evidencia y Validación): rediseñado con objetos de dominio propios y `ConfiguracionSistema` incorporada

**Detectada al revisar el diagrama de secuencia 4.1.** Una versión anterior de
`sec-registrar-actividad-evidencia.puml` traía una nota indicando que la validación de formato de
evidencia "usa ConfiguracionSistema (RNF-017)", con la etiqueta `<<include>>` presente en ese momento
en las notas de HU-10 y HU-11 (esa parte de `<<include>>` en texto de nota ya se corrigió por separado,
ver la nota siguiente sobre EP-03).

**Decisión anterior (revertida): se había optado por no incluir `ConfiguracionSistema`.** Una primera
revisión de este diagrama concluyó que `ConfiguracionSistema` no debía traerse aquí porque el diagrama,
en ese momento, no modelaba `Evidencia` como participante propio — todo el flujo pasaba por llamadas
reflexivas de un único objeto `Sistema SGR`, y agregar `ConfiguracionSistema` sin separar antes
`Evidencia` habría sido inconsistente. Esa nota ya aclaraba, eso sí, que `ConfiguracionSistema` **sí
existe** como clase documentada, con atributos y métodos, en `assets/actividad-3/patron-singleton.puml`
(patrón Singleton, sección 3.1 de `actividad-3.md`) — nunca fue una clase inventada, solo no estaba
traída a este diagrama en particular.

**Decisión actual: se revierte lo anterior. El diagrama se rediseña con objetos de dominio propios, y
`ConfiguracionSistema` se incorpora.** En vez de una única caja `Sistema SGR` con llamadas reflexivas
para todo, el diagrama ahora separa `Actividad`, `Evidencia`, `Validacion` e `Indicador` como
participantes independientes, mostrando las interacciones reales entre ellos
(`Sistema -> Act: crear(datos)`, `Evi -> Act: adjuntarEvidencia(e)`, `Val -> Ind: recalcularAvance()`).
Con `Evidencia` ya como objeto propio, la razón para omitir `ConfiguracionSistema` deja de aplicar: se
agrega `Evi -> Config: obtenerFormatosYTamanoPermitido() (RNF-017)`, la misma relación ya documentada en
`patron-singleton.puml` (`Evidencia ..> ConfiguracionSistema : usa (formatos y tamaño permitido —
RNF-017)`) — este diagrama de secuencia solo la pone en acción en el tiempo, sin introducir ninguna
clase ni relación nueva.

**Relación con la nota de `include`/`extend` de EP-03 (siguiente en este archivo):** ese rediseño no
afecta la corrección de las notas HU-10/HU-11 (texto plano, sin `<<include>>`) ya aplicada sobre el
`.puml` anterior — solo cambia qué participantes existen y qué interacciones se muestran entre ellos.
Ambas correcciones conviven en la versión final del diagrama.

**Impacto en otros artefactos:**
- `assets/actividad-3/sec-registrar-actividad-evidencia.puml` y su SVG: reemplazados por completo.
- `actividad-3.md`, sección 4.1: segundo párrafo actualizado para describir el nuevo diagrama (el primer
  párrafo, sobre el `include` de EP-03, no se toca — pertenece a la nota siguiente).
- `assets/actividad-3/patron-singleton.puml` y `clases-dominio.puml`: sin cambios — `ConfiguracionSistema`
  ya estaba correctamente documentada ahí; este diagrama de secuencia solo la reutiliza. Sigue sin
  aparecer en `clases-dominio.puml` porque no es una entidad del dominio SGR, sino infraestructura de
  configuración del sistema (HU-25, RNF-013/014/015).

Cualquier integrante o IA que reciba una tarea sobre el diagrama de secuencia de Registrar Actividad, o
sobre `ConfiguracionSistema` en cualquier otro artefacto, debe asumir esta versión (con `Actividad`,
`Evidencia`, `Validacion`, `Indicador` y `ConfiguracionSistema` como participantes propios) como la
vigente, salvo que este archivo se actualice explícitamente para decir lo contrario.

---

## Nota de consistencia: relaciones `include`/`extend` de EP-03 (Validar Evidencia)

**Detectada en revisión entre pares de la Actividad 3.** El diagrama específico de EP-03
(`cu-ep03-evidencias-verificacion.puml`) usaba `<<include>>` desde Registrar Actividad (HU-01) y desde
Adjuntar Evidencia (HU-09) hacia Validar Evidencia (HU-11), siguiendo al pie de la letra el ejemplo del
profesor en `fuentes/audio-clase-2.md` ("Validar Evidencia" incluido por los casos que suben evidencia).
Un compañero de equipo detectó que eso invierte la lógica del dominio.

**Por qué se quitaron esos dos `<<include>>`:** RF-013 dice que la validación la ejecuta el Verificador
— un actor distinto — después y como decisión separada, no como paso obligatorio del mismo flujo de
Registrar Actividad o Adjuntar Evidencia. El propio objetivo de la épica lo dice explícito:
"Respaldar la ejecución y **separar el registro de la decisión de validación**" (`guia-sgr.md` §12.4).
El ejemplo del profesor sigue siendo válido como patrón general de `include` (una función común
reutilizada dentro del mismo flujo); simplemente no aplica tal cual a este caso porque el disparador es
un actor y un momento distintos. El diagrama de secuencia 4.1 ya representaba esa separación temporal
(bloques distintos + `...tiempo después...`), así que la corrección alinea el diagrama de casos de uso
con lo que el de secuencia ya mostraba.

**Reemplazo:** dos `<<extend>>` — Adjuntar Evidencia sobre Registrar Actividad (opcional, se dispara solo
si el Funcionario adjunta un archivo al registrar; RF-012) y la nueva Solicitar Corrección sobre Validar
Evidencia (1 de las 3 decisiones del Verificador: aprobar/rechazar/corregir; RF-013). Se agregó "Solicitar
Corrección (HU-11)" como caso de uso propio — antes no estaba modelado por separado — y una anotación
corta junto a cada `include`/`extend` con el RF que lo justifica y su condición (siempre / opcional / 1
de 3), a pedido de la misma revisión entre pares.

**Nota aparte — regresión encontrada de pasada:** la nota de consistencia anterior de este mismo archivo
("`ConfiguracionSistema` no aparece en...") ya había dejado registrado que se quitaba `<<include>>` de
`sec-registrar-actividad-evidencia.puml` por ser notación fuera de contexto en un diagrama de secuencia.
Al revisar los 5 `sec-*.puml` para esta corrección, las etiquetas `<<include>>` seguían presentes en
notas de **dos** de ellos — `sec-registrar-actividad-evidencia.puml` (HU-10 y HU-11) y también
`sec-avance-cumplimiento.puml` (HU-07, que ni siquiera es parte de EP-03) — no quedó claro cuándo ni por
qué volvieron. Se quitaron de nuevo en ambos, como texto plano sin comillas angulares. Los otros 3
(`sec-notificacion-alertas`, `sec-generar-informe`, `sec-administrar-delegaciones`) ya estaban limpios.
Aparte, se revisaron también `patron-observer.puml` (usa `<<extend>>` dos veces, pero solo como cita
textual a la relación ya existente del diagrama de casos de uso — no es un error, se dejó igual) y el
resto de `cu-ep0X.puml` (EP-02, EP-04, EP-05: sus `include`/`extend` sí son consistentes con sus RF; EP-06,
EP-07, EP-08 no declaran ninguna relación `include`/`extend`).

**Impacto en otros artefactos:**
- `assets/actividad-3/cu-ep03-evidencias-verificacion.puml` y su SVG: reemplazados los 2 `include`
  hacia Validar Evidencia por 2 `extend`; agregado el caso de uso Solicitar Corrección (HU-11); agregada
  una nota corta por cada relación con su RF y condición.
- `assets/actividad-3/cu-ep01-registro-gestion-actividades.puml` y su SVG: la nota bajo Registrar
  Actividad (UC1) ya no dice que dispara `<<include>>` hacia Validar Evidencia; ahora dice que es
  extendido opcionalmente por Adjuntar Evidencia, con referencia a la corrección de EP-03.
- `assets/actividad-3/sec-registrar-actividad-evidencia.puml` y su SVG: quitadas (de nuevo) las
  etiquetas `<<include>>` de las dos notas (HU-10 y HU-11), reemplazadas por texto plano. **Nota:** este
  mismo archivo fue rediseñado por completo después de esta corrección (ver la nota anterior en este
  archivo, "Diagrama de secuencia 4.1... rediseñado con objetos de dominio propios..."); las notas
  `note right:` de HU-10/HU-11 corregidas aquí ya no existen como tales en la versión vigente — el
  detalle de HU-10/HU-11 quedó implícito en los nombres de los métodos entre los nuevos participantes.
- `assets/actividad-3/sec-avance-cumplimiento.puml` y su SVG: mismo caso, quitada la etiqueta
  `<<include>>` de la nota de HU-07.
- `actividad-3.md`: sección 2.9 (tabla de relaciones y párrafo explicativo de la corrección), sección 4.1
  (texto actualizado: ya solo hay 1 `include` en EP-03, y aclaración de que Adjuntar/Validar Evidencia ya
  estaban separadas en el tiempo en el diagrama de secuencia), sección 8.2 (matriz de trazabilidad: las
  dos filas afectadas ahora muestran su relación `extend`).

Cualquier integrante o IA que reciba una tarea sobre el diagrama de casos de uso de EP-03, sobre el
diagrama de secuencia de Registrar Actividad, o sobre la matriz de trazabilidad de wireframes, debe
asumir esta nota como ya resuelta, salvo que este archivo se actualice explícitamente para decir lo
contrario.
