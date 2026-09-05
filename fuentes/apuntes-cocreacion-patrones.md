# Cocreación, Patrones y Requerimientos del Software

## Tabla de CONTENIDOS

Introducción.................................................... 03

**Introducción a los ciclos de vida y metodologías de desarrollo de software**
- Ciclos de vida de un proyecto de software...... 04
- Ciclo de vida del producto de software........... 04
- Metodologías de desarrollo de software......... 04
- Selección de una metodología y ciclo de vida................................................................. 05
- Recursos complementarios............................ 05
- Cierre............................................................... 06
- Ideas fuerza..................................................... 06

**Técnicas de levantamiento de requerimientos y cocreación con el cliente**
- ¿Qué es un requerimiento?............................ 07
- Tipos de requerimientos................................ 08
- Requerimientos del software.......................... 08
- Técnicas de cocreación y levantamiento de requerimientos.............................................. 09
- Actores del proceso....................................... 09
- Recursos complementarios............................ 10
- Cierre............................................................... 10
- Ideas fuerza..................................................... 10

**Patrones de diseño en software**
- Patrones de diseño de software: singleton, factory, observer y adapter............................... 12
- Recursos complementarios............................ 14
- Cierre............................................................... 14
- Ideas fuerza..................................................... 14

**Diagramas UML para modelado de sistemas**
- ¿Qué es un diagrama UML?............................ 15
- Tipos de diagramas UML................................ 16
- Recursos complementarios............................ 17
- Cierre............................................................... 17
- Ideas fuerza..................................................... 17

**Estándares de calidad en software**
- Principales estándares de calidad en software........................................................... 18
- Relación entre estándares y metodologías de desarrollo........................................................ 18
- Cascada y modelos tradicionales................... 19
- Híbridos.......................................................... 19
- Recursos complementarios............................ 20
- Cierre............................................................... 20
- Ideas fuerza..................................................... 20

**Integración y revisión de proyecto**
- Selección de metodología y ciclo de vida....... 21
- Recursos complementarios............................ 22

---

## Introducción

En este recurso, analizarás los ciclos de vida de los proyectos de software y las metodologías de desarrollo, comparando enfoques ágiles y tradicionales. Comenzarás profundizando en el concepto de ciclo de vida de desarrollo de software y comprenderás las fases comunes que lo componen, tales como la recopilación de requisitos, el diseño, la implementación, las pruebas, el despliegue y el mantenimiento.

Discutirás cómo los ciclos de vida de un producto y un proyecto están estrechamente relacionados, destacando la importancia de realizar todas las actividades necesarias para obtener productos de calidad y facilitar nuevos desarrollos.

Además, te enfocarás en los estándares de calidad en software, fundamentales para asegurar que los productos y servicios cumplan con las expectativas.

Explorarás los principales estándares internacionales de calidad aplicables al desarrollo de software, incluyendo ISO/IEC 12207, que abarca los procesos de ciclo de vida del software, y ISO/IEC 33000 (SPICE), que se centra en la evaluación y mejora de la capacidad y madurez de los procesos.

También analizarás ISO 9001, un estándar globalmente reconocido para la gestión de la calidad, y ISO/IEC 25000 (SQuaRE), que proporciona un marco para evaluar la calidad del producto de software.

Discutirás cómo estos estándares pueden integrarse con metodologías de desarrollo ágil y tradicionales para optimizar el levantamiento y cocreación de requerimientos, asegurando que los procesos sean eficientes y los productos finales de alta calidad. Profundizarás en la integración y evaluación de proyectos, reforzando el conocimiento previamente adquirido sobre metodologías de desarrollo.

Explorarás la selección de metodologías y ciclos de vida. Profundizarás en el diseño con diagramas UML, incluyendo diagramas de clases, casos de uso y secuencia, así como la integración de patrones de diseño para mejorar la estructura del sistema. Además, abordarás diversas técnicas de cocreación y levantamiento de requerimientos.

---

## Introducción a los ciclos de vida y metodologías de desarrollo de software

### Ciclos de vida de un proyecto de software

Un ciclo de vida de desarrollo de software es un marco que describe las fases y actividades involucradas en la creación de un sistema de software. Este ciclo de vida proporciona una guía detallada para gestionar el desarrollo de software desde la concepción inicial hasta su retiro, asegurando que el producto final cumpla con los requisitos del cliente y los estándares de calidad.

### Ciclo de vida del producto de software

Los ciclos de vida de un producto y un proyecto se encuentran estrechamente relacionados; cualquier idea vinculada con un producto de software tiene que ser conducida por un proyecto asociado. Durante la ejecución del proyecto deberán realizarse todas las actividades que contemplan las diversas fases por las que atraviesa, de esa forma se obtendrán productos de calidad y darán paso a nuevos desarrollos.

### Metodologías de desarrollo de software

**1. Metodologías tradicionales**

En el modelo tradicional o metodología *waterfall*, o en cascada, se divide el proyecto en distintas fases. En este modelo es necesario terminar y validar cada una de las fases antes de pasar a la siguiente. Con esta metodología se previenen errores, aunque esto implique más en el tiempo la entrega final del proyecto.

**2. Metodologías ágiles**

En las metodologías ágiles de desarrollo de proyectos o metodologías *scrum*, cada una de las fases, las divides en fases aún más pequeñas que llamarás *sprints*.

Cada uno de estos *sprints* se puede completar de manera independiente a la fase en la que se encuentra, y abrirá las puertas a comenzar con otras fases, aunque la suya propia no esté terminada de forma completa.

Brinda mayor versatilidad ya que distintos equipos trabajarán a la vez en distintas fases del proyecto y puedes ir iterando y saltando entre los distintos *sprints*.

**¿Cuál es la diferencia entre una metodología tradicional y ágil?**

La principal diferencia entre las metodologías tradicionales o *waterfall* y las metodologías ágiles o scrum radica en que, en las primeras, el proceso es lineal y secuencial, mientras que en las segundas el proceso es repetitivo.

En las metodologías en cascada, los requisitos son bien definidos desde el principio, mientras que, en las metodologías ágiles, los requisitos se toman de una manera más dinámica.

### Selección de una metodología y ciclo de vida

**Análisis de necesidades y recursos**

A continuación, profundizarás en las necesidades principales:

- **Tamaño del proyecto:** es para proyectos grandes que pueden beneficiarse de metodologías tradicionales, mientras que proyectos pequeños y medianos pueden ser más adecuados para metodologías ágiles.
- **Recursos disponibles:** se requiere considerar la experiencia del equipo y las herramientas disponibles.
- **Requisitos del cliente:** se debe determinar si los requisitos son claros y estables o si es probable que cambien.
- **Plazos y presupuesto:** se requiere evaluar la urgencia y las restricciones financieras del proyecto.

### Recursos complementarios

*YouTube*
**OPM Integral**
Metodologías ÁGILES vs TRADICIONALES | Metodologías Ágiles de Gestión de Proyectos
Ver video: https://www.youtube.com/watch?v=s19iuO4QRv8

### Cierre

La selección adecuada de una metodología y ciclo de vida de desarrollo de software es crucial para el éxito del proyecto.

Has explorado los diferentes ciclos de vida de un proyecto de software y las metodologías de desarrollo, tanto ágiles como tradicionales. Adicionalmente, has aprendido que cada enfoque tiene sus ventajas y desventajas, y que la elección de la metodología adecuada depende de varios factores, incluyendo el tamaño del proyecto, los recursos disponibles y los requisitos del cliente. Es fundamental analizar y comprender estas variables para tomar decisiones informadas que aseguren la calidad y el éxito del proyecto.

### Ideas fuerza

**1. Importancia de la metodología adecuada**
- La metodología seleccionada impacta directamente en la eficiencia y calidad del desarrollo del software.
- Un enfoque adecuado puede prevenir errores y mejorar la satisfacción del cliente.
- La elección debe basarse en un análisis detallado de las necesidades y recursos del proyecto.

**2. Comparación entre metodologías ágiles y tradicionales**
- Las metodologías ágiles son flexibles y adaptativas, ideales para proyectos con requisitos cambiantes.
- Las metodologías tradicionales, como el modelo en cascada, son más estructuradas y adecuadas para proyectos con requisitos bien definidos desde el inicio.
- Cada enfoque tiene sus propias ventajas y desventajas que deben ser consideradas.

**3. Fases del ciclo de vida del software**
- Requisitos: recopilación y análisis de las necesidades del cliente.
- Diseño: planificación de la estructura del software.
- Implementación: codificación del software.
- Pruebas: verificación y validación del software.
- Despliegue y mantenimiento: implementación y mejora continua del software.

**4. Relación entre ciclo de vida del producto y del proyecto**
- Los ciclos de vida de un producto y un proyecto están estrechamente relacionados.
- La ejecución del proyecto debe contemplar todas las actividades necesarias para obtener productos de calidad.
- Un enfoque integral asegura el éxito y la continuidad del desarrollo.

**5. Gestión del riesgo y flexibilidad**
- Las metodologías ágiles permiten una identificación y mitigación continua de riesgos.
- Las metodologías tradicionales gestionan los riesgos en fases específicas del proyecto.
- La flexibilidad en la gestión del proyecto es clave para adaptarse a cambios y nuevos desafíos.

---

## Técnicas de levantamiento de requerimientos y cocreación con el cliente

### ¿Qué es un requerimiento?

De acuerdo con Ian Sommerville (2020), los requerimientos son la "descripción de los servicios que ofrece un sistema y sus restricciones operativas. También reflejan las necesidades de los clientes."

Sommerville y Pete Sawyer definen el proceso de obtención de requisitos como "la forma de descubrir los requisitos de un sistema a través de la comunicación con los clientes, los usuarios y otras personas interesadas en el desarrollo del sistema."

### Tipos de requerimientos

**1. Requerimientos funcionales**

Son declaraciones de los servicios que debe proporcionar el sistema, de la manera en que éste debe reaccionar a entradas particulares. O también pueden declarar explícitamente lo que el sistema no debe hacer. Es importante que describa el ¿qué?

**2. Requerimientos no funcionales**

Son restricciones de los servicios o funciones ofrecidos por el sistema. Incluyen restricciones de tiempo, sobre el proceso de desarrollo y estándares. Dentro de estos requerimientos encontramos todo lo referente a fiabilidad, el tiempo de respuesta y la capacidad de almacenamiento. Características que de una u otra forma pueden limitar al sistema.

Sommerville también clasifica los requerimientos no funcionales en tres tipos: Requerimientos de producto, Requerimientos organizacionales, Requerimientos externos.

**Figura 1.** Tipos de requerimientos no funcionales.

```
Requerimientos no funcionales
├── Requerimientos del producto
│   ├── Requerimientos de usabilidad
│   ├── Requerimientos de eficiencia
│   │   ├── Requerimientos de rendimiento
│   │   └── Requerimientos de espacio
│   └── Requerimientos de fiabilidad
│   └── Requerimientos de portabilidad
├── Requerimientos organizacionales
│   ├── Requerimientos de entrega
│   ├── Requerimientos de implementación
│   └── Requerimientos de estándares
└── Requerimientos externos
    ├── Requerimientos interoperabilidad
    ├── Requerimientos éticos
    └── Requerimientos legislativos
        ├── Requerimientos de privacidad
        └── Requerimientos de seguridad
```

**Fuente.** Elaboración propia.

### Requerimientos del software

Un requisito de software es una **propiedad** que debe ser exhibida por algo, con el fin de **resolver** algún **problema en el mundo real**.

Se puede tratar de automatizar parte de una tarea dirigida a alguien que permita apoyar los procesos de negocio de una organización, para corregir defectos de software existente o para controlar un dispositivo, por nombrar solo algunos de los muchos problemas que son posibles de solucionar gracias a los *softwares*.

### Técnicas de cocreación y levantamiento de requerimientos

- **Entrevistas:** reuniones estructuradas o semiestructuradas con *stakeholders* para obtener información detallada sobre sus necesidades y expectativas, ya sean individuales o grupales.
- **Talleres de cocreación:** sesiones colaborativas donde desarrolladores y clientes generan ideas y soluciones, fomentando la creatividad y asegurando la participación de todas las partes interesadas.
- **Encuestas y cuestionarios:** herramientas para recopilar información de muchos usuarios, obteniendo datos cuantitativos y cualitativos sobre sus necesidades y preferencias.
- **Observación:** estudio del entorno y actividades del usuario para comprender mejor sus necesidades e interacción con el sistema, ya sea de forma directa o mediante grabaciones.
- **Prototipos:** versiones preliminares del sistema que permiten a los clientes visualizar y probar funcionalidades antes de la implementación final, facilitando la retroalimentación temprana y la validación de los requerimientos.
- **Mapeo de historias de usuario:** técnica que organiza las historias de usuario en un mapa visual, mostrando sus relaciones y ayudando a priorizar funcionalidades y entender el flujo del sistema.
- **Análisis de documentación:** revisión de documentos existentes para extraer información relevante sobre los requerimientos del sistema.
- **Focus groups:** reuniones con un grupo de usuarios representativos para discutir sus necesidades y obtener retroalimentación sobre ideas y prototipos, explorando diferentes perspectivas y obteniendo *insights* valiosos.

### Actores del proceso

Es importante conocer las funciones de las personas que participan en el proceso de requerimientos. Este proceso **es fundamentalmente interdisciplinario**, y el especialista de requerimientos tiene que mediar entre el dominio de la parte interesada y la del ingeniero del software.

Generalmente hay muchas personas involucradas, además del especialista de requerimientos, cada uno de los cuales tiene una participación en el software. Las partes interesadas podrán variar a través de proyectos, pero siempre incluirán los usuarios, operadores y clientes.

A continuación, profundizarás en ejemplos típicos de las partes interesadas de software:

- **Usuarios:** este grupo comprende los que van a operar el software. A menudo es un grupo heterogéneo que involucra a personas con diferentes roles y necesidades.
- **Clientes:** este grupo comprende a los que han encargado el software o que representan el mercado objetivo de software.
- **Los analistas de mercado:** un producto de mercado masivo no tendrá un cliente al momento de la puesta en marcha, así que a menudo la gente de *marketing* es necesaria para establecer las necesidades del mercado y para actuar como clientes de prueba o filtro.
- **Reguladores:** muchos campos de aplicación, como la banca y el transporte público, están regulados. El software en estos dominios debe cumplir con los requerimientos de las autoridades reguladoras.
- **Los ingenieros de software:** estos individuos tienen un interés legítimo en sacar provecho de desarrollo del software, por ejemplo, la reutilización de componentes o de otros productos.

### Recursos complementarios

*YouTube*
**Ingeniería de Software de Élite**
Cómo deleitar a tus usuarios - Ingeniería de Requerimientos, La Serie
Ver video: https://www.youtube.com/watch?v=LPM1ehPDpSc&list=PLCVGhLzsMEq8-Q7Mrvq5Q6jrHo4nDJpod

### Cierre

El levantamiento de requerimientos y la cocreación son esenciales para el éxito de los proyectos de software.

A lo largo de este recurso, has explorado diversas técnicas para capturar y validar los requerimientos del cliente, asegurando que el producto final cumpla con sus expectativas. Además, profundizaste en la importancia de la participación del cliente y la validación continua, así como las funciones de las diferentes partes interesadas en el proceso de desarrollo de software.

### Ideas fuerza

La correcta aplicación de técnicas de levantamiento de requerimientos y cocreación, junto con la validación y participación del cliente, es fundamental para el desarrollo de software de alta calidad que satisfaga las necesidades del usuario.

**1. Técnicas de levantamiento de requerimientos**
- Entrevistas, talleres de cocreación, encuestas y observación son métodos clave.
- Permiten obtener información detallada y precisa sobre las necesidades del cliente.
- Facilitan la identificación de requerimientos específicos y relevantes.

**2. Prototipos y feedback iterativo**
- Los prototipos permiten la visualización y prueba temprana de funcionalidades.
- El feedback iterativo asegura ajustes continuos basados en la retroalimentación del cliente.
- Mejora la calidad del producto final y la satisfacción del cliente.

**3. Documentación clara y accesible**
- Mantener una documentación detallada y actualizada es crucial.
- Facilita la comprensión común del proyecto entre todas las partes interesadas.
- Ayuda a evitar malentendidos y asegura la coherencia en el desarrollo.

**4. Participación del cliente**
- La participación del cliente en revisiones periódicas y feedback es esencial.
- Asegura que los requerimientos capturados sean precisos y completos.
- Fomenta una relación de confianza y colaboración entre el equipo de desarrollo y el cliente.

**5. Roles de las partes interesadas**
- Identificar y comprender los roles de usuarios, clientes, analistas de mercado, reguladores e ingenieros de software.
- Cada grupo aporta perspectivas y necesidades únicas que deben ser equilibradas.
- La negociación de compensaciones es clave para satisfacer las necesidades de todas las partes interesadas.

---

## Patrones de diseño en software

Los patrones de diseño se derivaron de ideas planteadas por Christopher Alexander, quien sugirió que había ciertos patrones comunes de diseño de construcción que eran relativamente agradables y efectivos. El patrón es una **descripción del problema** y la **esencia de su solución**, de modo que la solución puede reutilizarse en diferentes configuraciones. El patrón no es una especificación detallada. Más bien, puede considerarla como una **descripción de sabiduría y experiencia acumuladas**, una solución bien probada a un problema común (Alexander et al., 1977, pp. 189–190).

Los patrones de diseño más conocidos fueron descritos en su libro de patrones (Gamma et al., 1995). Los elementos esenciales de los patrones de diseño, definidos en este libro, son:

**Figura 2.** Elementos esenciales de los patrones de diseño.

1. Un nombre que sea una referencia significativa al patrón.
2. Una descripción del área problemática que enuncie cuándo puede aplicarse el patrón.
3. Una descripción de la solución de las partes de la solución de diseño, sus relaciones y responsabilidades.
4. Un estado de las consecuencias, los resultados y las negociaciones, al aplicar el patrón.

**Fuente.** Elaboración propia.

### Patrones de diseño de software: singleton, factory, observer y adapter

**Patrón *singleton***

Es un patrón de diseño que restringe la creación a un único objeto la creación de objetos pertenecientes a una clase y **asegura que solo haya esta instancia única**.

Además de garantizar que una clase solo tenga una instancia, proporciona un punto de acceso global a ella.

**Patrón *factory***

Consiste en utilizar una clase constructora (al estilo del *abstract factory*) abstracta con unos cuantos métodos definidos y otro(s) abstracto(s): el dedicado a la construcción de objetos de un subtipo de un tipo determinado.

Asimismo, es una simplificación del *abstract factory*, en la que la clase abstracta tiene métodos concretos que usan algunos de los abstractos; según usemos una u otra hija de esta clase abstracta, tendremos uno u otro comportamiento.

Este patrón pretende **resolver problemas recurrentes** con un diseño flexible y reusable para *software* orientado a objetos. Específicamente, el método *factory* resuelve cómo un objeto puede ser creado haciendo que las subclases puedan decidir qué clases instanciar y cómo una clase puede diferir la instanciación de subclases.

**Patrón *observer***

Es un patrón de diseño de comportamiento que permite **definir un mecanismo** de suscripción para notificar a varios objetos sobre cualquier evento que le suceda al objeto que están observando.

**Patrón *adapter***

Es un patrón de diseño estructural que permite la colaboración entre objetos con interfaces incompatibles.

**Tabla 1.** Comparación de patrones de diseño.

| Patrón | Descripción | Cuando usarlo | Ventajas | Desventajas |
|---|---|---|---|---|
| **Singleton** | Garantiza que una clase tenga solo una instancia y proporciona un punto global de acceso a ella. | Cuando se necesita exactamente una instancia global de una clase, como en manejadores de configuración o logging. | Fácil acceso a la instancia; controla el acceso centralizado. | Puede dificultar las pruebas unitarias y romper el principio de responsabilidad única. |
| **Factory** | Proporciona una interfaz para crear objetos sin especificar las clases concretas que se instanciarán. | Cuando el proceso de creación de objetos es complejo o depende de condiciones que varían en tiempo de ejecución. | Facilita la extensibilidad y abstrae el proceso de creación. | Puede aumentar la complejidad del código debido a las múltiples subclases o métodos de fábrica. |
| **Observer** | Define una relación de dependencia 1 a muchos, notificando a todos los dependientes cuando cambia un estado. | Cuando varios objetos necesitan estar informados de cambios en el estado de otro objeto, como en sistemas de eventos. | Desacopla emisores y receptores; simplifica la comunicación entre objetos. | Puede generar problemas de rendimiento si hay demasiados observadores o si no se gestionan adecuadamente. |
| **Adapter** | Permite que dos interfaces incompatibles trabajen juntas al envolver una clase en otra. | Cuando necesitas usar una clase existente cuya interfaz no coincide con la requerida por el cliente. | Facilita la reutilización de código existente sin modificarlo; mejora la interoperabilidad entre componentes. | Puede aumentar la complejidad si se abusa o si hay múltiples adaptadores necesarios. |

**Fuente.** Elaboración propia.

### Recursos complementarios

*Blog*
**Refactoring Guru**
Observer
Leer blog: https://refactoring.guru/es/design-patterns/adapter

*YouTube*
**BettaTech**
FACTORY | PATRONES de DISEÑO
Ver video: https://www.youtube.com/watch?v=lLvYAzXO7Ek

### Cierre

Los patrones de diseño como *singleton, factory, observer y adapter* son esenciales para crear sistemas flexibles y escalables.

Estos patrones proporcionan soluciones reutilizables para problemas comunes en el desarrollo de software, facilitando la creación de aplicaciones robustas y mantenibles. Los diagramas UML ayudan a visualizar la estructura y el comportamiento de estos patrones, mejorando la comprensión y la implementación en proyectos reales.

### Ideas fuerza

Los patrones de diseño son herramientas fundamentales que permiten a los desarrolladores crear software eficiente y adaptable, promoviendo buenas prácticas de programación y facilitando la resolución de problemas recurrentes.

**1. Patrón singleton**
- Garantiza una única instancia de una clase.
- Proporciona un punto de acceso global.
- Controla el ciclo de vida del objeto.

**2. Patrón factory**
- Encapsula la creación de objetos.
- Permite a las subclases decidir qué clase instanciar.
- Mejora la cohesión y facilita el mantenimiento.

**3. Patrón observer**
- Define una relación de suscriptor/publicador.
- Facilita la comunicación entre objetos sin acoplamiento fuerte.
- Promueve el bajo acoplamiento y la implementación de sistemas en tiempo real.

**4. Patrón adapter**
- Permite que dos interfaces incompatibles trabajen juntas.
- Facilita la reutilización de código existente.
- Promueve la interoperabilidad entre sistemas.

---

## Diagramas UML para modelado de sistemas

### ¿Qué es un diagrama UML?

Es una herramienta clave para visualizar sistemas y *software* mediante el UML. Este lenguaje permite a los ingenieros de *software* **representar diseños, arquitectura de código** e **implementaciones propuestas de sistemas complejos** de forma visual y comprensible.

Además, los diagramas UML son útiles para modelar flujos de trabajo y procesos empresariales, simplificando conceptos técnicos mediante un estándar visual. Facilitan la **comprensión de relaciones** y **jerarquías** en grandes **proyectos de programación**, ayudando a ingenieros y partes interesadas a coordinar esfuerzos y descomponer componentes críticos de un sistema.

### Tipos de diagramas UML

**1. Diagramas estructurales**

Representan la estructura estática del sistema. Estos diagramas muestran relaciones jerárquicas, atributos y métodos de las clases.

**Figura 3.** Pasos para construir un diagrama de clases.

1. Identificación de objetos y clases
2. Identificación de atributos y funciones
3. Identificación de los asociaciones y agregaciones
4. Identificación de las relaciones de herencia

**Fuente.** Elaboración propia.

**2. Diagramas de comportamiento**

Describen el comportamiento y la dinámica del sistema. Permiten observar cómo **interactúan los componentes en un contexto específico**.

**Figura 4.** Diagrama de casos de uso detallado.

Módulo de registro de hospedaje — Actor: Recepcionista

- Asignar habitación **«extend»** Verificar disponibilidad
- Liberar habitación **«extend»** Verificar reservación
- Realizar corte **«include»** Generar nota/factura

**Fuente.** Elaboración propia.

### Recursos complementarios

*YouTube*
**Lucid Software Español**
Tutorial - Diagrama de Clases UML
Ver video: https://www.youtube.com/watch?v=Z0yLerU0g-Q

*YouTube*
**Universitat Politècnica de València – UPV**

### Cierre

Has explorado los diagramas UML y su importancia en el modelado de sistemas de software.

Aprendiste sobre los diferentes tipos de diagramas UML, incluyendo los diagramas de caso de uso, de clases y de secuencia. Cada uno de estos diagramas ofrece una perspectiva única y complementaria para entender y diseñar sistemas de software complejos.

Además, has discutido las técnicas recomendadas para crear estos diagramas y cómo pueden facilitar la comunicación entre desarrolladores y *stakeholders*.

### Ideas fuerza

Los diagramas UML son herramientas esenciales para el diseño y la documentación de sistemas de software. Su uso adecuado puede mejorar significativamente la comprensión y la comunicación en los equipos de desarrollo.

**1. Diagramas de caso de uso:**
- Representan las interacciones entre los actores y el sistema.
- Facilitan la identificación de los requisitos funcionales.
- Son fáciles de entender por todos los *stakeholders*.

**2. Diagramas de clases:**
- Muestran la estructura estática del sistema.
- Incluyen relaciones jerárquicas y asociativas.
- Ayudan en la implementación del código.

**3. Diagramas de secuencia:**
- Describen el flujo de mensajes entre objetos en orden cronológico.
- Son ideales para detallar escenarios específicos.
- Facilitan la comprensión de la lógica dinámica del sistema.

**4. Importancia de UML:**
- Facilita la visualización de sistemas complejos.
- Mejora la comunicación entre desarrolladores y *stakeholders*.
- Ayuda a mantener la coherencia en el diseño del sistema.

---

## Estándares de calidad en software

### Principales estándares de calidad en software

Son varias las organizaciones internacionales que se dedican a redactar estándares de calidad para unificar las buenas prácticas en torno a la industria del software. Este caso, profundizarás en:

**ISO** – Organización Internacional de Normalización *(International Organization for Standardization)*. Sus normas especifican requerimientos para **garantizar que los productos y/o servicios cumplen con su objetivo**.

**IEC** – Comisión Electrotécnica Internacional *(International Electrotechnical Commission)*. Sus normas son documentos técnicos que **ayudan a diseñadores y fabricantes a garantizar la seguridad**.

### Relación entre estándares y metodologías de desarrollo

Los estándares de calidad pueden integrarse con metodologías de desarrollo ágil y tradicionales para optimizar el levantamiento y cocreación de requerimientos como:

**Desarrollo ágil:** prioriza la entrega rápida de valor al cliente mediante iteraciones cortas, enfoque en la colaboración y flexibilidad en los procesos. Sin embargo, la calidad no puede ser sacrificada en favor de la rapidez. Algunas metodologías incluyen:

- ***Scrum y kanban:*** estas metodologías, al centrarse en entregas incrementales, pueden beneficiarse de la aplicación de estándares como ISO/IEC 25000 para definir los **criterios de aceptación** en las historias de usuario.
- **Integración de estándares:** en *scrum*, los eventos como la planificación del sprint y la retrospectiva pueden utilizarse para validar la conformidad de los entregables con estándares de calidad.

### Cascada y modelos tradicionales

El modelo cascada se caracteriza por su enfoque secuencial, lo que lo hace ideal para proyectos con requisitos claros y bien definidos desde el inicio. Algunas características incluyen:

- **Estándares alineados:** ISO/IEC 12207 se adapta perfectamente al modelo Cascada porque define procesos detallados para cada etapa del ciclo de vida del software. La documentación extensa, una característica inherente al modelo Cascada, también facilita la aplicación de ISO 9001, garantizando que se cumplan los requisitos organizacionales.
- **Requerimientos y calidad:** ISO/IEC 25000 puede emplearse para evaluar los requisitos iniciales bajo criterios de calidad (funcionalidad, fiabilidad, mantenibilidad, etc.), asegurando que el software cumpla con los objetivos previstos al final del desarrollo.

### Híbridos

Los enfoques híbridos combinan lo mejor de las metodologías tradicionales y ágiles para adaptarse a las necesidades cambiantes del proyecto. Esto permite una mayor flexibilidad en los procesos, mientras se mantienen niveles elevados de trazabilidad y calidad. Algunas características incluyen:

- **Definición y adaptación:** al integrar ISO/IEC 33000 en procesos híbridos, las organizaciones pueden realizar evaluaciones periódicas de la madurez de los procesos, ajustándolos según las necesidades del proyecto. Por ejemplo, la fase de levantamiento de requerimientos puede utilizar técnicas iterativas propias del enfoque ágil, complementadas con revisiones exhaustivas propias del enfoque en cascada.
- **Optimización continua:** la mejora continua, uno de los principios fundamentales de ISO 9001, puede integrarse para refinar los ciclos de iteración, asegurando que cada entrega incrementa la calidad global del producto.
- **Criterios claros y medibles:** los atributos de calidad definidos en ISO/IEC 25000 pueden emplearse como guía tanto en las entregas iterativas como en los hitos clave del proyecto, garantizando que cada fase cumpla con los requisitos esperados.

### Recursos complementarios

*YouTube*
**AENOR**
ISO/IEC 33000 - Certificación de desarrollo de software
Ver video: https://www.youtube.com/watch?v=QxBCXlOp6Es

*YouTube*
**Sebastian Marroquin**
UPV Normas ISO // calidad en desarrollo de software
Ver video: https://www.youtube.com/watch?v=FSCIACtKUxA

### Cierre

La implementación de estándares de calidad en el desarrollo de software asegura productos de alta calidad y mejora los procesos internos.

Integrar estándares como ISO/IEC 12207, ISO/IEC 33000, ISO 9001 e ISO/IEC 25000 en el levantamiento y cocreación de requerimientos no solo garantiza la calidad del producto final, sino que también fomenta una cultura de mejora continua dentro de la organización.

Estos estándares proporcionan un marco estructurado que ayuda a las organizaciones a cumplir con los objetivos organizacionales y satisfacer las expectativas de los usuarios.

### Ideas fuerza

La adopción de estándares de calidad en el desarrollo de software es fundamental para asegurar productos consistentes y de alta calidad, además de optimizar los procesos internos y fomentar una cultura de mejora continua.

**1. ISO/IEC 12207: procesos de ciclo de vida del software**
- Establece un marco completo para los procesos involucrados en el ciclo de vida del software.
- Incluye procesos primarios, de soporte y organizativos.
- Enfatiza la gestión de requerimientos claros, trazables y validados.

**2. ISO/IEC 33000 (SPICE): evaluación de procesos**
- Proporciona una base para evaluar la capacidad y madurez de los procesos de software.
- Incluye niveles de madurez y un modelo de referencia.
- Mejora la eficiencia del levantamiento de requerimientos a través de evaluaciones continuas.

**3. ISO 9001: gestión de la calidad**
- Enfocado en la satisfacción del cliente y la mejora continua.
- Alinea los requerimientos con las expectativas del cliente.
- Fomenta la mejora de las metodologías usadas para la captura y validación de requerimientos.

**4. ISO/IEC 25000 (SQuaRE): calidad del producto de software**
- Define modelos de calidad y métricas para evaluar productos de software.
- Evalúa características como funcionalidad, fiabilidad, usabilidad y mantenibilidad.
- Proporciona criterios para definir requisitos funcionales y no funcionales basados en atributos de calidad.

Implementar estos estándares no solo asegura productos de alta calidad, sino que también mejora los procesos internos y fomenta una cultura de mejora continua.

---

## Integración y revisión de proyecto

### Selección de metodología y ciclo de vida

A continuación, se detallan los pasos esenciales para seleccionar la metodología adecuada para un proyecto:

- **Análisis de necesidades y recursos:** antes de seleccionar una metodología, se debe analizar exhaustivamente los requisitos del proyecto (características, funcionalidad, objetivos de rendimiento), las limitaciones de tiempo, el presupuesto, el tamaño y las habilidades del equipo, y las expectativas de participación del cliente.

Además, se considera factores como la **complejidad del proyecto**, la **disponibilidad del cliente** para **recibir comentarios** y la **necesidad de flexibilidad**.

- **Selección de la metodología:** en función del análisis, hay una metodología adecuada. Existen diversos enfoques, se encuentran los enfoques tradicionales (cascada) y los ágiles (*scrum, kanban*). A continuación, profundizarás en sus ventajas:
  - **Cascada:** es adecuado para proyectos con requisitos claramente establecidos.
  - **Ágil:** es más adaptable a los requisitos cambiantes y permite un desarrollo iterativo. Adicional, es excelente para proyectos en los que la opinión del cliente es fundamental y los requisitos pueden evolucionar con el tiempo. *Scrum* y *kanban* son marcos de trabajo ágiles populares, cada uno de los cuales ofrece ventajas únicas.

- **Ciclo de vida**

Este ciclo incluye fases como:
  - Recopilación de requisitos.
  - Diseño.
  - Pruebas.
  - Implementación.
  - Mantenimiento.

Para la metodología ágil, esto se traduce en iteraciones *(sprints)* con ciclos de retroalimentación continuos.

El diseño con diagramas UML incluye el uso de diagramas de clases, casos de uso y secuencia para modelar la estructura y comportamiento del sistema. Los patrones de diseño como *singleton, factory, observer* y *adapter* ayudan a abordar desafíos específicos en el desarrollo. Las técnicas de cocreación y levantamiento de requerimientos, como entrevistas, talleres, encuestas, prototipos y mapeo de historias de usuario, aseguran una comprensión y validación exhaustivas de las necesidades del cliente.

La implementación de estándares de calidad, como ISO/IEC 12207, ISO/IEC 33000 (SPICE), ISO 9001 e ISO/IEC 25000 (SQuaRE), se integra con la metodología seleccionada para garantizar un proceso de desarrollo robusto y exitoso, gestionando requisitos y mejorando procesos continuamente.

### Recursos complementarios

*Blog*
**Hack(io)**
UML: el lenguaje universal para el modelado de sistemas que tienes que conocer
Ver video: https://www.hackio.com/blog/uml-el-lenguaje-universal-para-el-modelado-de-sistemas

*YouTube*
**MitoCode**
Curso de Patrones de diseño - 2 Singleton
Ver video: https://www.youtube.com/watch?v=gocJeOHtj9w

*Blog*
**Ambit BTS**
Normas ISO. ¿Qué son y cuáles son las más importantes?
Leer blog: https://www.ambit-bst.com/blog/normas-iso.-qu%C3%A9-son-y-cu%C3%A1les-son-las-m%C3%A1s-importantes

---

## Bibliografía

Alexander, C., Ishikawa, S., Silverstein, M., Jacobson, M., Fiksdahl-King, I., & Angel, S. (1977). *A pattern language: Towns, buildings, construction*. Oxford University Press.

Beck, K., & Andres, C. (2004). *Extreme programming explained: Embrace change* (2nd ed.). Addison-Wesley.

Beck, K., Beedle, M., Van Bennekum, A., Cockburn, A., Cunningham, W., Fowler, M., & Thomas, D. (2001). *Manifesto for Agile Software Development*. Agile Alliance. https://agilemanifesto.org

Booch, G., Rumbaugh, J., & Jacobson, I. (2005). *The Unified Modeling Language user guide*. Addison-Wesley.

Cohn, M. (2005). *Agile estimating and planning*. Prentice Hall.

Fowler, M. (2004). *UML distilled: A brief guide to the standard object modeling language* (3rd ed.). Addison-Wesley.

Gamma, E., Helm, R., Johnson, R., & Vlissides, J. (1994). *Design patterns: Elements of reusable object-oriented software.* Addison-Wesley.

Gamma, E., Helm, R., Johnson, R., & Vlissides, J. (1995). *Design patterns: Elements of reusable object-oriented software.* Addison-Wesley.

INACAP. (s.f.). *Material de profundización: Software como solución de negocio* [PDF].

International Organization for Standardization. (2008). *Sistemas y software de ingeniería: Procesos del ciclo de vida del software* (ISO/IEC 12207:2008).

International Organization for Standardization. (2014). *Sistemas y software de ingeniería: Requisitos y evaluación de calidad (SQuaRE)* (ISO/IEC 25000:2014).

International Organization for Standardization. (2015). *ISO 9001:2015 Quality management systems—Requirements*. ISO.

International Organization for Standardization. (2015). *ISO/IEC 25000:2014 Systems and software engineering—Systems and software quality requirements and evaluation (SQuaRE)—Guide to SQuaRE*. ISO.

International Organization for Standardization. (2015). *ISO/IEC 33000:2015 Information technology—Process assessment—Concepts and terminology*. ISO.

International Organization for Standardization. (2017). *ISO/IEC 12207:2017 Systems and software engineering—Software life cycle processes.* ISO.

Larman, C. (2004). *Agile and iterative development: A manager's guide*. Addison-Wesley.

Poppendieck, M., & Poppendieck, T. (2003). *Lean software development: An agile toolkit*. Addison-Wesley.

Pressman, R. S. (2014). *Ingeniería de software: Un enfoque práctico* (7ª ed.). McGraw-Hill.

Pressman, R. S., & Maxim, B. R. (2020). *Ingeniería de software: Un enfoque práctico* (8ª ed.). McGraw-Hill.

Refactoring Guru. (2014). *Adapter*. https://refactoring.guru/es/design-patterns/adapter

Royce, W. W. (1970). *Managing the development of large software systems*. Proceedings of IEEE WESCON, 1–9. https://doi.org/10.1109/WESCON.1970.45

Schwaber, K., & Sutherland, J. (2020). *The Scrum guide: The definitive guide to Scrum: The rules of the game*. Scrum.org. https://scrumguides.org

Schwaber, K., & Sutherland, J. (2020). *The Scrum Guide: The definitive guide to Scrum: The rules of the game*. Scrum.org. https://www.scrumguides.org/

Sommerville, I. (2020). *Engineering Software Products: An Introduction to Modern Software Engineering*. Pearson.

Sommerville, I. (2016). *Ingeniería de software* (10.a ed.). Pearson.

Sommerville, I. (2016). *Software engineering* (10th ed.). Pearson Education.

Universidad Oberta de Catalunya. (n.d.). *Introducción al lenguaje de modelado unificado (UML)*. Open Access UOC. https://openaccess.uoc.edu
