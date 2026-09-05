La primera evaluación formal del proyecto se estructurará detalladamente bajo un formato de informe y una rúbrica específica que abarca las siguientes pautas, actividades y entregables:

### Aspectos Generales y Logística de la Entrega
* **Fecha y hora límite de entrega:** El plazo máximo es el **10 de septiembre hasta las 23:00 horas**. Para ello, se dispondrá de **9 días de trabajo** en total.
* **Modalidad de trabajo:** Las actividades se desarrollarán en **grupos** para fomentar el trabajo colaborativo, aunque se permite la opción de trabajar de manera **individual**.
* **Liderazgo del proyecto:** Cada grupo debe definir a un representante que actúe como **líder de proyecto**, quien será el único interlocutor válido entre el docente y el equipo. Se requiere que este rol de líder **vaya cambiando o rotando** a medida que se avanza en las distintas fases del proyecto (por ejemplo, según se requiera un enfoque técnico o de planificación).
* **Dinámica de "Licitación":** Debido a que hay aproximadamente 20 grupos desarrollando el mismo sistema, la evaluación operará bajo un **modo de licitación**. La idea planteada es competir para que se seleccione la mejor propuesta con miras a obtener un **Producto Mínimo Viable (MVP)** al finalizar la asignatura.

---

### Actividad 1: Técnicas para la Toma de Requerimientos
Aunque el docente proporciona un documento base que ya define la problemática y cuenta con una captura inicial de requerimientos, los estudiantes deberán realizar una bajada de dicha información y adecuar ciertos aspectos. Esta sección del informe debe contener:
1. **Justificación de técnicas:** Indicar y justificar técnicamente las herramientas y técnicas utilizadas para la captura y análisis de los datos.
2. **Requerimientos estructurados:** Definir y detallar tanto los **requerimientos funcionales** como los **no funcionales**.
3. **Épicas e Historias de Usuario:** Desglosar las épicas y detallar cada una de las historias de usuario con sus respectivas tareas específicas.
4. **Asignación de esfuerzos:** Documentar la estimación de esfuerzo de cada tarea, lo cual consiste en asignar y justificar técnicamente **cuánto tiempo demorará cada una de ellas**.
5. **Planificación y Gestión:** El trabajo y avance de esta evaluación debe estar debidamente planificado y gestionado a través de herramientas de control como **GitHub ("GCAP")** o un plan de trabajo/carta Gantt.

---

### Actividad 2: Selección y Justificación de la Metodología
Los equipos deben realizar una propuesta metodológica propia y formal para el desarrollo del proyecto. Los requisitos de esta sección son:
1. **Análisis técnico riguroso:** Se debe realizar un análisis técnico comparativo de **al menos dos metodologías** que sean viables y aplicables al alcance del proyecto. Las opciones admisibles incluyen metodologías estructuradas (como cascada), ágiles, híbridas o incrementales.
2. **Exclusión de la metodología en espiral:** Esta metodología queda **explícitamente descartada** debido a las limitaciones de tiempo del semestre.
3. **Prohibición de cuadros simples:** El docente enfatiza que **no se aceptará un cuadro básico de ventajas y desventajas**; la elección de la metodología debe justificarse exclusivamente con sólidos fundamentos de ingeniería de software.
4. **Definición detallada de recursos:**
   * **Hardware y Software:** Especificar los requisitos técnicos **mínimos y óptimos** tanto para la etapa de desarrollo como para la puesta en producción/operación (los cuales posteriormente se conectarán con la arquitectura física en el diagrama de despliegue).
   * **Recursos Humanos:** Definir los roles, perfiles y la organización del equipo de trabajo. Por ejemplo, si se opta por un marco ágil como XP (Extreme Programming), se debe justificar técnicamente el tipo de profesionales a integrar (mencionando que XP usualmente requiere desarrolladores con mayor experiencia y no solo juniors).

---

### Actividad 3: Desarrollo de Diagramas UML y Wireframes
El modelado de la solución informática exige el desarrollo y vinculación de múltiples diagramas bajo el estándar UML, así como las interfaces de usuario:

1. **Diagramas de Casos de Uso:**
   * **De alto nivel:** Un diagrama general derivado directamente de las **épicas** que represente el escenario global, los actores involucrados y cómo se comunican dentro del sistema.
   * **Específicos:** Diagramas detallados que incorporen y utilicen de forma correcta las relaciones de obligatoriedad (**include**) y extensión (**extend**). Los *includes* representan comportamientos obligatorios que se gatillan desde un caso de uso principal y que están diseñados para ser reutilizados por múltiples interfaces del programa (funcionando conceptualmente como funciones de software que consumen los distintos módulos).
2. **Diagramas de Clases:** Para estructurar lógicamente las entidades del dominio del sistema.
3. **Diagramas de Componentes:** Enfocados en identificar los componentes internos y consumos de servicios del software.
4. **Diagramas de Despliegue:** Para detallar la infraestructura física y lógica de hardware, software y consumos, vinculándose con los requerimientos de infraestructura definidos en la Actividad 2.
5. **Diagramas de Requerimientos (en árbol):** Representar de manera jerárquica y en ramas el requerimiento funcional, la épica, la historia de usuario y las tareas de desarrollo. Este diagrama sirve como un mapa visual o línea de trabajo para controlar el avance del proyecto.
6. **Wireframes y Matriz de Trazabilidad:** Diseño de pantallas o bocetos del sistema (los cuales son de carácter no funcional/diseño de interfaz). Se exige una **trazabilidad estricta y obligatoria** que conecte cada elemento en una cadena lógica clara: 
   \\[\text{Requerimiento Funcional/No Funcional} \rightarrow \text{Épica} \rightarrow \text{Historia de Usuario} \rightarrow \text{Caso de Uso de Alto Nivel} \rightarrow \text{Caso de Uso Específico} \rightarrow \text{Wireframe (Interfaz)}.\\]
   *Un ejemplo de esto es justificar el diseño de la pantalla de inicio de sesión (login) recorriendo de principio a fin cada uno de estos niveles trazables.*

---

📋 ¿Te gustaría que prepare una plantilla estructurada en formato markdown para que comiences a redactar los puntos de la **Actividad 1** y la **Actividad 2** basándonos en la problemática de las delegaciones municipales?
