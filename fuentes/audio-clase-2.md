# Notas de la Evaluación 2 — Proyecto SGR
### Aclaraciones adicionales (más allá de la guía formal)

---

## Actividad 1 — Requerimientos

- El caso ya viene dado (SGR), así que el trabajo no es "inventar" el problema sino hacer la **bajada**: seleccionar del documento base qué RF/RNF aplican al alcance que el equipo decida cubrir (probablemente el MVP de la sección 13.2), y ajustarlos/redactarlos con formato propio.
- **Épicas → HU → Tareas** con esfuerzo estimado y **justificación** del esfuerzo (no basta con poner "3 días"; hay que explicar el criterio: complejidad, dependencias, tamaño, etc. — story points, t-shirt sizing, horas con supuestos, lo que elijan, pero justificado).
- La gestión de esto en GitHub Projects ("GCAP") o un plan de trabajo probablemente sea **evidencia aparte** (capturas del tablero, board), no solo texto en el informe. Vale la pena confirmar con el docente si esto va dentro del informe como anexo/capturas o es un entregable paralelo.

---

## Actividad 2 — Metodología

- Mínimo 2 metodologías, de las categorías: **estructurada, ágil, híbrida o incremental**. Espiral queda **explícitamente descartada** — ni siquiera mencionarla como opción a comparar.
- **No sirve un cuadro de ventajas/desventajas.** Esto es clave: hay que argumentar con fundamento de ingeniería — por ejemplo, relacionar características del proyecto (equipo de 3, plazo corto, requerimientos parcialmente estables por venir de un caso ya definido, necesidad de entregas incrementales verificables) con las propiedades técnicas de cada metodología (ciclos de retroalimentación, gestión de cambio, artefactos, roles, cadencia de entrega) y de ahí derivar la elección.
- Recursos: separar claramente **mínimos vs óptimos**, y **software/hardware** vs **recursos humanos**. Si eligen algo como XP, tienen que justificar por qué el equipo (pair programming, roles) tiene sentido con solo 3 integrantes — este es un caso donde la teoría choca con la realidad del equipo, así que conviene anticiparlo.

---

## Actividad 3 — UML, Wireframes, Trazabilidad

Este es el núcleo con más riesgo de errores técnicos:

1. **Casos de Uso**: primero un diagrama de alto nivel derivado de las épicas (una épica ≈ un conjunto de casos de uso relacionados), luego diagramas específicos con **include/extend** bien usados:
   - `include` = comportamiento obligatorio y reutilizable (el profesor lo enfatiza como "función modular" — ej. "Validar Evidencia" incluido por varios casos de uso que suben evidencia).
   - `extend` = comportamiento opcional/condicional que extiende un caso base (ej. "Generar Alerta" extiende "Revisar Avance" solo si se cumple una condición).

2. **Clases**: estructurar entidades (Funcionario, Actividad, Evidencia, Delegación, Meta, etc., según el SGR), con atributos, métodos clave y relaciones (asociación, composición, herencia si aplica).

3. **Componentes**: foco en **consumos del sistema** — probablemente se refiere a cómo los componentes consumen servicios/APIs entre sí (frontend consume API, API consume BD, servicios externos si los hay).

4. **Despliegue**: infraestructura física/lógica — nodos (servidor web, servidor BD, cliente), protocolos de comunicación, y "consumos físicos/lógicos" probablemente se refiere a especificar qué corre en qué nodo y cómo se comunican.

5. **Diagrama de Requerimientos**: en **árbol jerárquico** (no el diagrama SysML tradicional necesariamente, sino una jerarquía visual tipo mapa), que funcione como mapa de avance del tablero de trabajo — esto sugiere que debería poder cruzarse visualmente con el estado de las HU en GitHub Projects.

6. **Trazabilidad**: la cadena completa y obligatoria es:

   **RNF → Épica → HU → Caso de Uso alto nivel → Caso de Uso específico → Wireframe**

   Nota que aquí el profesor parte de **RNF** (no RF como decía la guía escrita) — vale la pena confirmar esto con el docente porque es una discrepancia real entre el documento oficial y lo que dijo en clase. Si la duda no se resuelve, lo más seguro es documentar la trazabilidad completa incluyendo tanto RF como RNF relevantes por cada wireframe, dejando explícito el criterio usado.
