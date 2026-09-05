# Actividad 3 — Diagramas UML y Wireframes

**Ponderación en la rúbrica: 40%** (la de mayor peso y mayor riesgo técnico)

**Depende de:**
- [`decisiones.md`](../decisiones.md) — códigos originales de `guia-sgr.md`, sin renumerar.
- Actividad 1 → épicas, HU y códigos RF/RNF finales (no usar un subconjunto distinto al ya cerrado ahí).
- Actividad 2 → recursos de hardware/software mínimos y óptimos (deben coincidir con el diagrama de
  despliegue de este documento).

**Fuentes a consultar:** `fuentes/que-hacer-1-2-3.md` (sección Actividad 3, la más detallada),
`fuentes/audio-clase-2.md` (aclaraciones técnicas de include/extend y la discrepancia RF/RNF en la
trazabilidad — ver nota en la sección 6), `fuentes/guia-sgr.md` (entidades del dominio §8, arquitectura
§14.1).

---

## 1. Diagrama de Casos de Uso — Alto nivel

> Un diagrama general derivado directamente de las épicas. Debe representar el escenario global:
> actores involucrados y cómo se comunican con el sistema. Cada épica se traduce, a grandes rasgos, en
> un conjunto de casos de uso relacionados.

_(Insertar diagrama. Actores y épicas según lo cerrado en Actividad 1.)_

---

## 2. Diagrama(s) de Casos de Uso — Específicos

> Deben usar correctamente:
> - **`include`** → comportamiento obligatorio y reutilizable, que se gatilla siempre desde el caso de
>   uso principal (ej. "Validar Evidencia" incluido por distintos casos que suben evidencia).
> - **`extend`** → comportamiento opcional/condicional que extiende un caso base solo si se cumple una
>   condición (ej. "Generar Alerta" extiende "Revisar Avance").
>
> Punto de riesgo técnico común: confundir include/extend invierte la lógica y es un error clásico de
> evaluación.

_(Insertar diagrama(s) por módulo/funcionalidad.)_

---

## 3. Diagrama de Clases

> Estructurar lógicamente las entidades del dominio del sistema (ej. Funcionario, Actividad, Evidencia,
> Delegación, Meta, según el caso SGR). Incluir atributos, métodos relevantes y relaciones (asociación,
> composición, herencia si aplica).

_(Insertar diagrama.)_

---

## 4. Diagrama de Secuencia

> No aparece mencionado en las instrucciones ni en los audios, pero sí está explícito en la Rúbrica 2
> (dimensión "Análisis de los recursos...", 40%). Conviene incluirlo igual para no perder puntaje en esa
> dimensión. Típicamente uno por cada caso de uso principal.

_(Insertar diagrama, ej. "Registrar Actividad con Evidencia".)_

---

## 5. Diagrama de Componentes

> Enfocado en los componentes internos y consumos de servicios del software (ej. cómo el frontend
> consume la API, cómo la API consume la base de datos, servicios externos si los hay).

_(Insertar diagrama.)_

---

## 6. Diagrama de Despliegue

> Infraestructura física y lógica: hardware, software y consumos (nodos como servidor web, servidor BD,
> cliente; protocolos de comunicación entre ellos). **Debe vincularse directamente con los recursos de
> hardware/software mínimos y óptimos definidos en la Actividad 2** — no pueden ser inconsistentes entre
> sí.

_(Insertar diagrama. Verificar contra `actividad-2.md` sección 2 antes de dar por cerrado.)_

---

## 7. Diagrama de Requerimientos (en árbol)

> Representación jerárquica y en ramas: Requerimiento Funcional → Épica → Historia de Usuario → Tareas
> de desarrollo. Funciona como mapa visual del avance del proyecto, pensado para poder cruzarse con el
> estado real del tablero de trabajo (Actividad 1, sección 5).

_(Insertar diagrama.)_

---

## 8. Wireframes + Matriz de Trazabilidad

> Se exige una cadena de trazabilidad estricta y obligatoria, elemento por elemento:
>
> **Requerimiento (Funcional o No Funcional) → Épica → Historia de Usuario → Caso de Uso de Alto Nivel
> → Caso de Uso Específico → Wireframe**
>
> **Nota sobre una discrepancia real:** el enunciado escrito dice que la cadena parte de RF/RNF (ambos).
> En `fuentes/audio-clase-2.md` el profesor menciona en clase que parte de RNF específicamente. Si no se
> ha confirmado con el docente, la opción más segura es documentar la trazabilidad completa incluyendo
> tanto RF como RNF relevantes por cada wireframe, dejando explícito el criterio usado.

### 8.1 Wireframes

_(Insertar bocetos/diseño de las pantallas principales.)_

### 8.2 Matriz de trazabilidad

| Wireframe | RF/RNF | Épica | HU | CU alto nivel | CU específico |
|---|---|---|---|---|---|
| | | | | | |

_(Un renglón completo por cada wireframe presentado, no solo un ejemplo. El profesor dio como modelo
justificar la pantalla de login recorriendo la cadena completa de principio a fin.)_

---

## Checklist de cierre — Actividad 3

- [ ] Diagrama de Casos de Uso — alto nivel (desde épicas)
- [ ] Diagrama(s) de Casos de Uso específicos con include/extend correctos
- [ ] Diagrama de Clases del dominio
- [ ] Diagrama(s) de Secuencia (exigido por la rúbrica)
- [ ] Diagrama de Componentes (consumo de servicios)
- [ ] Diagrama de Despliegue (coherente con Actividad 2)
- [ ] Diagrama de Requerimientos en árbol
- [ ] Wireframes de las pantallas principales
- [ ] Trazabilidad completa por cada wireframe (RF/RNF→Épica→HU→CU alto nivel→CU específico→Wireframe)
- [ ] Verificado contra los códigos finales de Actividad 1 (sin inventar épicas/HU nuevas)
- [ ] Verificado contra los recursos de Actividad 2 (diagrama de despliegue consistente)
