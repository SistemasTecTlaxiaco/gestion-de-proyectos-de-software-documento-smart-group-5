# Documento detallado: Objetivo SMART y Análisis de Viabilidad

**Proyecto:** Plataforma comunitaria para la preservación y transmisión de la lengua materna de Santa María Cuquila (ProyectoLM), dentro de Open Hub Tec
**Organización cliente:** Comité Comunitario de Cultura y Lengua de Santa María Cuquila. Representante: María López García
**Asignatura:** Gestión de Proyectos de Software (SCG-1009), Unidad 3: Planificación del proyecto, Sprint 3
**Docente / Product Owner:** José Alfredo Román Cruz
**Institución:** Tecnológico Nacional de México, Campus Tlaxiaco
**Periodo:** Agosto–Diciembre 2026
**Fecha:** 13 de octubre de 2026

**Equipo eduScrum**

| Integrante | Rol permanente | Rol en el Sprint 3 |
|---|---|---|
| Yaretzy Montesinos López | Documentadora | **eduScrum Master** |
| Elisa Sánchez Coronel | Investigadora | Integrante |
| Diego Ernesto López Vásquez | eduScrum Master del Sprint 1 | Integrante |
| Daisy Ortiz López | Responsable del Backlog | Integrante |

---

## Índice

1. [Contexto y problemática](#1-contexto-y-problemática)
2. [Insumos de los Sprints 1 y 2 (trazabilidad)](#2-insumos-de-los-sprints-1-y-2-trazabilidad)
3. [Estimación de tiempo y costo](#3-estimación-de-tiempo-y-costo)
4. [Objetivo SMART](#4-objetivo-smart)
5. [Viabilidad técnica](#5-viabilidad-técnica)
6. [Viabilidad operativa](#6-viabilidad-operativa)
7. [Viabilidad financiera Web3](#7-viabilidad-financiera-web3)
8. [Dictamen Go / No-Go](#8-dictamen-go--no-go)
9. [Autogestión eduScrum](#9-autogestión-eduscrum)
10. [Referencias](#10-referencias)

---

## 1. Contexto y problemática

Santa María Cuquila pertenece al municipio de Heroica Ciudad de Tlaxiaco, Oaxaca. El INALI ubica a la comunidad en la variante **tu'un savi (mixteco del suroeste central)**, y el INPI conserva material bilingüe sobre su historia y tradición. El conocimiento existe, pero está disperso y depende sobre todo de la transmisión oral de las personas mayores.

El equipo no parte de afirmar que la lengua haya desaparecido. Lo que identifica es una oportunidad: **fortalecer la documentación, la consulta, el aprendizaje y la transmisión** de la lengua con una herramienta digital ligera, validada por la propia comunidad.

**Problemática seleccionada:** *PROB-01: Preservación y transmisión de la lengua y memoria cultural de Santa María Cuquila*. En el Sprint 1 aparecía como PROB-03 entre tres candidatas (residuos, agua y lengua). Tras la comparación de alternativas quedó en estado **ELEGIDA** y en el Acta de Criterios de Aceptación se renumeró como PROB-01.

---

## 2. Insumos de los Sprints 1 y 2 (trazabilidad)

### 2.1 Historias de usuario validadas con el cliente (Sprint 1)

Las historias vienen del **Acta de Criterios de Aceptación** firmada con el Comité Comunitario el 31 de agosto de 2026. Antes de la firma pasaron por la auditoría con IA, que revisó la estructura Como/Quiero/Para, el rol real, el alcance y que los criterios fueran verificables.

| HU | Historia | Dictamen del cliente | Modificación acordada |
|---|---|---|---|
| HU-01 | Consultar palabras y expresiones | Aceptado | — |
| HU-02 | Escuchar pronunciaciones | Modificado | Conservar la fuente y la fecha del audio |
| HU-03 | Aportar conocimiento | Aceptado | Mantener la revisión antes de publicar |
| HU-04 | Consultar memoria cultural | Modificado | Agregar contexto, fuente y fecha |
| HU-05 | Validar contenido | Aceptado | — |
| HU-06 | Escuchar pronunciaciones asociadas al término | Modificado | Mostrar el término durante la reproducción |

El acta dictaminó el proyecto como **viable con ajustes** en accesibilidad, conectividad, validación comunitaria, procedencia del contenido, almacenamiento de audios y facilidad de uso. Este documento retoma esos ajustes como requisitos.

### 2.2 Costo de la Calidad (Sprint 2)

Datos del **Plan de Calidad** (`COSTO-CALIDAD-HISTORIAS.md` y `METRICAS-CALIDAD.md`), con una tarifa de práctica de **$150 MXN por hora**:

| HU | Prevención | Evaluación | Corrección | Costo de calidad | j = Hp/Hc |
|---|---:|---:|---:|---:|---:|
| HU-01 | 4 h | 2 h | 3 h | $1,350 | 1.33 |
| HU-02 | 5 h | 3 h | 5 h | $1,950 | 1.00 |
| HU-03 | 6 h | 3 h | 8 h | $2,550 | 0.75 |
| HU-04 | 6 h | 3 h | 7 h | $2,400 | 0.86 |
| HU-05 | 5 h | 3 h | 6 h | $2,100 | 0.83 |
| HU-06 | 4 h | 3 h | 5 h | $1,800 | 0.80 |
| **Total** | **30 h** | **17 h** | **34 h** | **$12,150** | **0.88** |

### 2.3 Auditoría del repositorio (Sprint 2)

La lista de verificación con el auditor automático (`AUDITAR-REPOSITORIO.ps1`) dio estos resultados: **10 de 10 criterios cumplidos (100 %)**, **0 hallazgos críticos o altos** e **insignia Oro provisional**.

### 2.4 Qué insumo se usa en cada sección

| Insumo | Dónde se usa |
|---|---|
| HU-01 a HU-06 y sus dictámenes | Elección de las historias del módulo y de su alcance (3.1) |
| Horas de prevención y corrección por HU | Se copian tal cual en la tabla de horas (3.2) |
| Tarifa de $150 MXN/h | La misma para todo el equipo y todas las historias (3.5) |
| j por historia y meta j ≥ 1.00 | Elección del módulo y metas del objetivo SMART (4) |
| Metas de usabilidad y conectividad (≥ 90 %) | Indicadores del objetivo SMART (4) |
| Contexto comunitario del acta | Viabilidad técnica y operativa (5 y 6) |
| `FINANCIAMIENTO.md` e informe Stellar/Drips | Viabilidad financiera (7) |

---

## 3. Estimación de tiempo y costo

Se sigue la receta de cuatro pasos vista en clase (*Estimación de tiempo y costo, Sprint 3*):

| Paso | Pregunta | Fórmula |
|---|---|---|
| 1 | ¿Cuántas horas lleva cada historia? | Construir + prevenir + corregir. Construir = (Bien + Normal × 4 + Falla) ÷ 6 |
| 2 | ¿Cuánto colchón dejamos? | Horas × 10, 15 o 20 %, según la matriz de riesgos |
| 3 | ¿Cuántas semanas? | Horas ÷ horas que el equipo trabaja de verdad por semana |
| 4 | ¿Cuánto dinero? | Horas × tarifa + gastos |

### 3.1 Historias del módulo

El módulo que se estima es **"Consulta y pronunciación"**, formado por **HU-01** (consultar palabras y expresiones) y **HU-02** (escuchar pronunciaciones). Se eligieron estas dos por tres razones:

- Son el núcleo de la preservación: sin consulta ni audio, la plataforma no transmite la lengua.
- Son las únicas con **j ≥ 1.00** en el Sprint 2 (1.33 y 1.00). Es decir, ya tienen más prevención que corrección y son las de menor riesgo de retrabajo.
- Ambas fueron aceptadas por el cliente: HU-01 sin cambios y HU-02 con el criterio de fuente y fecha del audio.

### 3.2 Paso 1: horas por historia

**Horas de construcción (estimación de tres puntos):**

| Historia | Si todo va bien | Lo normal | Si algo falla | Construir = (B + N × 4 + F) ÷ 6 |
|---|---:|---:|---:|---:|
| HU-01 Consultar palabras | 10 h | 16 h | 28 h | (10 + 64 + 28) ÷ 6 = **17 h** |
| HU-02 Escuchar pronunciaciones | 8 h | 12 h | 16 h | (8 + 48 + 16) ÷ 6 = **12 h** |

Razones de cada caso:

- **HU-01:** en el caso "si algo falla" se consideran las variantes de escritura del tu'un savi, porque la búsqueda debe encontrar la palabra aunque se escriba distinto.
- **HU-02:** en el caso "si algo falla" se consideran los audios que haya que volver a grabar o comprimir para que carguen con señal débil.

**Total por historia:**

| Historia | Construir · hoy | Prevenir · Sprint 2 | Corregir · Sprint 2 | Total |
|---|---:|---:|---:|---:|
| HU-01 · Consultar palabras | 17 h | 4 h | 3 h | 17 + 4 + 3 = **24 h** |
| HU-02 · Escuchar pronunciaciones | 12 h | 5 h | 5 h | 12 + 5 + 5 = **22 h** |
| **Las dos historias** | **29 h** | **9 h** | **8 h** | 24 + 22 = **46 h** |

Las columnas de prevenir y corregir se copian sin cambios de la tabla de Costo de la Calidad del Sprint 2. Las 2 h y 3 h de evaluación de esa tabla quedan dentro de "construir", porque son las pruebas funcionales de cada historia.

En HU-02, **10 de 22 horas** se dedican a prevenir y corregir. La calidad es parte del trabajo, no un extra.

### 3.3 Paso 2: reserva por riesgos

**Matriz de riesgos del módulo:**

| Riesgo | Probabilidad | Impacto | Nivel |
|---|---|---|---|
| R1. Pocos hablantes disponibles para grabar (temporada agrícola, horarios comunitarios) | Media | Alto | **Alto** |
| R2. Falla de conectividad en Cuquila durante las pruebas con usuarios | Alta | Medio | **Alto** |
| R3. Variantes de escritura que complican la búsqueda | Media | Medio | Medio |
| R4. Retrasos por la carga académica de otras materias | Media | Medio | Medio |
| R5. Desacuerdo comunitario sobre el uso de las grabaciones | Baja | Alto | Medio |

Hay **dos riesgos altos** (R1 y R2), así que la reserva es del **15 %**:

> 46 h × 15 % = 6.9 ≈ **7 h**  →  46 h + 7 h = **53 horas**

La reserva se registra en el Tablero como un issue propio, «[PLAN] Reserva por riesgos (15 %)», para que sus horas aparezcan en la suma.

### 3.4 Paso 3: tiempo

| Dato | Cálculo | Resultado |
|---|---|---|
| Horas del equipo | 4 personas × 5 h por semana | 20 h por semana |
| Horas que sí rinden | 20 h × 75 % | **15 h por semana** |
| Semanas necesarias | 53 h ÷ 15 h | **3.5 semanas** |
| Semanas disponibles | Semanas 12 a 16 de la instrumentación (5 semanas × 15 h) | 75 h |
| **Holgura** | 75 h − 53 h | **22 h: sí alcanza** |

**Distribución por semana:**

| Semana | Horas | Trabajo |
|---|---:|---|
| 12 | 15 h | Casos de prueba (prevención), estructura de datos y búsqueda de HU-01. **Visita 1:** grabación |
| 13 | 15 h | Ficha de palabra de HU-01 y reproductor de HU-02 con fuente y fecha del audio |
| 14 | 15 h | Modo sin conexión, compresión de audios y correcciones. **Visita 2:** pruebas con usuarios |
| 15 | 8 h | Uso de la reserva, cierre de defectos y publicación v1.0 |
| 16 | 0 h | Holgura (sobran 22 h para imprevistos o para adelantar HU-06) |

### 3.5 Paso 4: costo

| Concepto | Cálculo | Costo (MXN) |
|---|---|---:|
| Trabajo | 53 h × $150 | $7,950 |
| Pasajes Tlaxiaco–Cuquila | 2 visitas × 4 personas × $50 ida y vuelta | $400 |
| Datos móviles | 2 recargas de $100 | $200 |
| Hospedaje (GitHub Pages) y repositorio (GitHub) | Plan gratuito | $0 |
| **Costo total del módulo** | 53 h × $150 + $600 de gastos | **$8,550** |

### 3.6 Resumen

| 1 · Horas | 2 · Colchón | 3 · Tiempo | 4 · Costo |
|:---:|:---:|:---:|:---:|
| **46 h** | **53 h** | **3.5 semanas** | **$8,550** |
| 24 + 22, de las dos historias | 46 + 7 h de reserva (15 %) | 53 ÷ 15 h por semana | 53 × $150 + $600 de gastos |

### 3.7 Proyección del proyecto completo

Con la misma receta, para dimensionar el financiamiento de la sección 7:

| Historia | Bien | Normal | Falla | Construir | Prevenir | Corregir | Total |
|---|---:|---:|---:|---:|---:|---:|---:|
| HU-01 | 10 | 16 | 28 | 17 | 4 | 3 | 24 h |
| HU-02 | 8 | 12 | 16 | 12 | 5 | 5 | 22 h |
| HU-03 | 12 | 20 | 34 | 21 | 6 | 8 | 35 h |
| HU-04 | 9 | 14 | 25 | 15 | 6 | 7 | 28 h |
| HU-05 | 12 | 18 | 30 | 19 | 5 | 6 | 30 h |
| HU-06 | 4 | 8 | 12 | 8 | 4 | 5 | 17 h |
| **Seis historias** | | | | **92** | **30** | **34** | **156 h** |

- **Colchón:** 156 h × 15 % = 23 h, para un total de **179 h**.
- **Tiempo:** 179 h ÷ 15 h = **11.9 semanas**. No cabe en las 5 semanas del semestre, así que se recorta el alcance (ver 3.8).
- **Costo:** 179 h × $150 + $1,800 de gastos (6 visitas × 4 × $50 y 6 recargas de $100) = **$28,650**.

### 3.8 Regla de alcance

Las seis historias suman 179 h y solo hay 75 h en el semestre. Por eso **no se estira el semestre: se recorta el alcance**.

| Fase | Historias | Horas | Cuándo |
|---|---|---:|---|
| Módulo 1 | HU-01, HU-02 | 53 h | Este semestre (semanas 12–16) |
| Módulo 2 | HU-05, HU-06 | 54 h | Siguiente periodo |
| Módulo 3 | HU-03, HU-04 | 72 h | Siguiente periodo |

Mientras HU-05 no esté construida, el Comité valida el contenido **fuera de la plataforma**: revisa la lista de palabras y los audios antes de cargarlos. Así se cumple el acuerdo del acta de no publicar nada sin validar.

### 3.9 Supuestos escritos

- Tarifa: $150 MXN por hora, la misma del Sprint 2 y para todo el equipo.
- 5 h por persona a la semana, entre clase y tarea.
- 75 % de enfoque: de cada 4 horas, 3 rinden de verdad.
- Reserva del 15 %, por los dos riesgos altos (R1 y R2).
- Pasaje de $50 ida y vuelta por persona, Tlaxiaco–Cuquila. **Confirmar con el pasaje real.**
- Construcción del módulo en las semanas 12 a 16 de la instrumentación.
- Tipo de cambio de referencia: $18.50 MXN por USD.

---

## 4. Objetivo SMART

> **Para el cierre de la semana 16 del semestre (diciembre de 2026), el equipo publicará en un repositorio abierto de GitHub el módulo "Consulta y pronunciación" de la plataforma comunitaria de Santa María Cuquila (HU-01 y HU-02).**
>
> **El módulo tendrá al menos 100 palabras y expresiones en tu'un savi validadas por el Comité Comunitario de Cultura y Lengua, y al menos 50 de ellas con pronunciación grabada por hablantes de la comunidad, con fuente y fecha.**
>
> **Se validará con 10 usuarios de la comunidad. Las metas son: que al menos el 90 % consulte y escuche una palabra sin ayuda, que al menos el 90 % de las pruebas con conexión limitada sean exitosas y que el indicador de calidad se mantenga en j ≥ 1.00.**
>
> **El presupuesto es de 53 horas y $8,550 MXN.**

| Dimensión | Cómo se cumple |
|---|---|
| **Específico** | Define el módulo, las dos historias, el contenido en tu'un savi, al cliente (el Comité) y al responsable (el equipo). |
| **Medible** | Seis indicadores numéricos: 100 entradas, 50 audios, 10 usuarios, 90 % de usabilidad, 90 % de éxito con conexión limitada y j ≥ 1.00. Las metas del 90 % y de j ≥ 1.00 son las mismas del Plan de Calidad del Sprint 2. |
| **Alcanzable** | Las 53 h caben en las 75 h disponibles, con 22 h de holgura. La infraestructura es gratuita y no se depende de financiamiento externo. |
| **Relevante** | Atiende PROB-01 con las dos funciones centrales que aceptó el cliente. Además, el módulo publicado es el requisito previo para Drips y para el SCF (sección 7). |
| **Temporal** | Semanas 12 a 16, con avance semanal (3.4) y publicación al final de la semana 15. |

---

## 5. Viabilidad técnica

### 5.1 Arquitectura propuesta

| Componente | Solución | Por qué |
|---|---|---|
| Aplicación | Aplicación web progresiva (PWA) en HTML, CSS y JavaScript | Funciona en el navegador de cualquier celular, sin tienda de aplicaciones. |
| Hospedaje | GitHub Pages | Es gratuito, está integrado al repositorio y no hay servidor que mantener. |
| Datos | Archivos JSON versionados en Git: palabra, significado, fuente, fecha y estado de validación | Cada cambio queda auditado. Cumple el acuerdo de "conservar fuente y fecha" (HU-02). |
| Audio | Grabación con celular, comprimida a Opus o MP3 de 32 kbps (unos 10–20 KB por palabra) | 50 audios pesan menos de 1 MB: se escuchan con señal débil y gastan pocos datos. |
| Sin conexión | *Service worker* con **paquetes de contenido descargables** | Es la alternativa que propuso el equipo en el acta: se descarga una vez y se consulta sin internet. |
| Calidad | Auditor automático del Sprint 2, pruebas de `PRUEBAS-CALIDAD.md` y revisión cruzada | Mantiene la insignia Oro y los criterios de ISO/IEC 25010 y WCAG 2.2 del Plan de Calidad. |

### 5.2 Restricciones de infraestructura en la Mixteca

| Restricción (sección 13 del acta) | Impacto | Solución técnica |
|---|---|---|
| Conectividad variable en Cuquila | La página no carga o se interrumpe | Paquetes sin conexión y sincronización cuando haya señal |
| Costo de los datos móviles | La gente evita usar la plataforma | Módulo de menos de 3 MB en total, sin videos y con audio comprimido |
| Celulares de gama baja | Lentitud o fallas | Sin *frameworks* pesados; pruebas en al menos 3 celulares distintos |
| Alfabetización digital desigual | Usuarios que no saben buscar | Botones grandes, íconos y la búsqueda en la pantalla principal (WCAG 2.2) |
| Escritura no estandarizada del tu'un savi | Una palabra no aparece por escribirse distinto | Búsqueda que ignora tildes y acepta las variantes de escritura registradas |

### 5.3 Blockchain

El módulo **no necesita** Stellar ni Soroban para cumplir su función. El informe Stellar/Drips del Sprint 2 lo dejó claro: *"no se utilizará blockchain únicamente porque sea una tecnología moderna"*. Integrar Soroban exige Rust, Stellar CLI, el *target* `wasm32v1-none` y pruebas en Testnet, conocimientos que el equipo todavía no tiene. Forzar esa integración en 75 h pondría en riesgo la fecha.

**Conclusión técnica: VIABLE.** Se usan tecnologías conocidas, la infraestructura no cuesta nada y el diseño parte de la conectividad real de la comunidad.

---

## 6. Viabilidad operativa

### 6.1 Operación con la comunidad

- **Validación lingüística.** El Comité Comunitario, por medio de María López García o de quien ella designe, revisa la lista de palabras y los audios antes de cargarlos. Ninguna palabra se publica sin esa revisión.
- **Consentimiento y reconocimiento.** Cada hablante autoriza el uso de su voz y se le reconoce como fuente, como pide el acta. Solo se guardan su nombre o seudónimo y la fecha.
- **Propiedad cultural.** El código usa licencia MIT. Para el contenido lingüístico se propondrá al Comité una licencia que no permita el uso comercial sin permiso, por ejemplo CC BY-NC-SA 4.0.
- **Temporada agrícola y horarios.** Las dos visitas se agendan con el Comité y en fin de semana (riesgo R1).

### 6.2 Operación del equipo (eduScrum)

| Restricción | Mitigación |
|---|---|
| Solo 5 h a la semana por persona | Alcance de 2 historias, 22 h de holgura y capacidad calculada al 75 % |
| No todos pueden viajar a la comunidad | Dos integrantes van a campo y dos desarrollan; se rota en cada visita |
| Dependencia de una sola persona técnica | Revisión cruzada en cada *pull request*, como en el Sprint 2 (`REVISION-SEGUNDO-INTEGRANTE.md`) |
| Conexión limitada para coordinarse | Tablero eduScrum en GitHub y acuerdos por escrito en `ACUERDO.md` |

**Conclusión operativa: VIABLE**, con una dependencia crítica: que el Comité participe en la validación. El acta lo advierte: sin ella, *"el equipo tendría dificultades para determinar si los contenidos representan correctamente el conocimiento comunitario"*.

---

## 7. Viabilidad financiera Web3

### 7.1 Costo frente a las fuentes de financiamiento

| Criterio | Stellar Community Fund (Build Award) | Drips Protocol |
|---|---|---|
| Tipo de apoyo | Premio por tramos ligados a entregables | Flujo continuo (*streaming*), donación (*giving*) y reparto (*splitting*) |
| Monto | Hasta 150,000 USD en XLM (unos $2,775,000 MXN) | Variable: depende de quién patrocine |
| Costo del módulo ($8,550) | 0.3 % del tope | Equivale a unos 13 meses de un *stream* de $660/mes |
| Proyecto completo + 1 año de operación ($36,550) | 1.3 % del tope | El mantenimiento anual ($7,900) pide unos $660 MXN al mes |
| Requisitos clave | *Use of Stellar*, *Integration Plan*, *Ready to Build*, presupuesto por tramos | Repositorio público, dirección EVM, `FUNDING.json` y ETH para el gas |
| Lo que ya tiene el proyecto | Necesidad validada con el cliente, presupuesto por tramos (7.2), repositorio con calidad Oro | Repositorio público con licencia MIT |
| Lo que le falta | Módulo publicado, un uso de Stellar con valor real, prototipo en Testnet y wallet | Wallet multisig, `FUNDING.json` y reclamar el repositorio |
| Momento adecuado | Con el producto completo, y solo si aparece un uso real de Stellar | Al publicar el módulo 1, para sostener la operación |

Las comisiones de Stellar son de fracciones de centavo y no cambian el total.

### 7.2 Presupuesto por tramos (formato del SCF)

| Tramo | Entregable verificable | Horas | Costo (MXN) | Fuente |
|---|---|---:|---:|---|
| 1. Módulo de consulta y pronunciación | v1.0 con HU-01 y HU-02, 100 entradas validadas y 50 audios | 53 h | $8,550 | Recursos propios y académicos |
| 2. Validación y audio asociado | HU-05 y HU-06 en la plataforma | 54 h | $8,700 | Propios / postulación SCF |
| 3. Aportaciones y memoria cultural | HU-03 y HU-04; prototipo en Soroban solo si aporta valor (p. ej., registro verificable del reconocimiento a colaboradores) | 72 h | $11,400 | Postulación SCF |
| 4. Operación del primer año | Mantenimiento (4 h/mes × 12 × $150), dominio y gas de Drips | 48 h | $7,900 | Drips (*stream* de patrocinadores) |
| **Total** | | **227 h** | **$36,550 (unos 1,976 USD)** | |

Gastos de los tramos 2 y 3: $600 cada uno ($400 de pasajes y $200 de datos). Tramo 4: $7,200 de mantenimiento, $300 de dominio y $400 de gas.

### 7.3 Análisis

1. **El monto no es el obstáculo.** El módulo cuesta $8,550 MXN, casi todo en horas del equipo, y no requiere dinero externo. El proyecto completo es apenas el 1.3 % del tope del SCF.
2. **La elegibilidad sí lo es.** Hoy el proyecto saldría mal evaluado en *Use of Stellar* y *Ready to Build*. Postular ahora obligaría a inventar un uso de blockchain que la comunidad no necesita, algo que el equipo ya descartó en el Sprint 2.
3. **Drips es el camino natural para sostener el proyecto.** La entrada es barata (unos $400 MXN de gas), no condiciona el diseño y encaja con un repositorio abierto y bien documentado. La calidad Oro del Sprint 2 da confianza a los patrocinadores: *calidad → confianza → sostenibilidad → financiamiento*.
4. **El orden importa.** Primero el módulo 1 con recursos propios, después Drips para la operación y, al final, el SCF si aparece un uso de Stellar con beneficio real.

---

## 8. Dictamen Go / No-Go

| Decisión | Dictamen | Fundamento |
|---|---|---|
| Construir el módulo 1 (HU-01 y HU-02) en las semanas 12–16 | ✅ **GO** | **Tiempo:** 53 h caben en 75 h y sobran 22 h. **Dinero:** $8,550 cubiertos con recursos propios. **Calidad:** las dos historias tienen j ≥ 1.00 y el repositorio tiene insignia Oro. **Cliente:** dictamen "viable con ajustes". |
| HU-03, HU-04, HU-05 y HU-06 este semestre | ⏸️ **Fuera de alcance** | Las seis historias suman 179 h y no caben en las 75 h disponibles. Se recorta alcance, no se estira el semestre. |
| Postular al Stellar Community Fund ahora | ⛔ **NO-GO** | No se cumplen *Use of Stellar*, *Integration Plan* ni *Ready to Build*. Se reevalúa con el producto publicado. |
| Reclamar el repositorio en Drips | 🟡 **GO condicionado** | Al publicar la v1.0, una vez creados la wallet multisig del equipo y el `FUNDING.json`. |

### Dictamen general: **GO**

El proyecto avanza con el módulo 1 sin depender de fondos externos. El financiamiento Web3 entra por etapas y solo cuando se cumplen los requisitos de cada fuente. Así se cierran las brechas declaradas en "El hueco honesto" de `FINANCIAMIENTO.md`.

**Condiciones para mantener el GO** (se revisan en cada retrospectiva):

1. El Comité confirma su participación en la validación antes de la semana 12.
2. Al final de la semana 13, HU-01 está terminada. Si no, la meta de audios baja de 50 a 25.
3. Las horas reales no superan la reserva de 7 h. Si la superan, el eduScrum Master replantea el alcance con el equipo.

---

## 9. Autogestión eduScrum

### 9.1 Evidencia en el Tablero de GitHub

Siguiendo los cinco pasos vistos en clase, el Project del equipo tiene:

1. Cuatro campos numéricos: **Construcción, Prevención, Corrección y Estimación** (en horas).
2. Los issues de HU-01 y HU-02 con sus campos llenos y el total escrito a mano (24 h y 22 h).
3. El issue **«[PLAN] Reserva por riesgos (15 %)»**, con 7 h.
4. La vista agrupada por Iteración, con la suma de campos activada: **53 h**.
5. El issue **«[PLAN] Estimación de tiempo y costo»**, con la tabla, el tiempo, el costo y los supuestos de la sección 3.9.

El eduScrum Master mueve el issue de estimación a *Hecho* solo después de que el Product Owner lo revisa.

### 9.2 Distribución del trabajo

| Sección | Responsable | Revisor |
|---|---|---|
| Coordinación, Tablero y revisión final | Yaretzy Montesinos López (eduScrum Master del Sprint 3) | Todo el equipo |
| Estimación de tiempo y costo, y viabilidad financiera Web3 | Elisa Sánchez Coronel | Diego |
| Viabilidad técnica | Diego Ernesto López Vásquez | Daisy |
| Trazabilidad con el backlog, matriz de riesgos y viabilidad operativa | Daisy Ortiz López | Elisa |
| Estimación "normal" de cada historia | Todo el equipo (cada quien dijo su número a la vez, como en *planning poker*) | eduScrum Master |
| Objetivo SMART y dictamen | Todo el equipo, por consenso (`ACUERDO.md` §8) | eduScrum Master |

> Ajusten esta tabla si el reparto real fue distinto. Debe coincidir con los *commits* del repositorio.

### 9.3 Prácticas del equipo

- **Rotación del eduScrum Master:** Diego (Sprint 1), Elisa (Sprint 2), Yaretzy (Sprint 3) y Daisy (Sprint 4), según `ACUERDO.md`.
- **Definición de Hecho:** otro integrante revisó la sección, se integró al repositorio y el auditor automático no reporta fallas.
- **Reunión breve al inicio de cada sesión:** qué hice, qué haré y qué me bloquea.
- **Retrospectiva** al cierre del sprint, donde se revisan las condiciones del dictamen GO.

---

## 10. Referencias

1. Román Cruz, J. A. (2026). *Estimación de tiempo y costo, Sprint 3* [diapositivas de clase]. Gestión de Proyectos de Software, TecNM Campus Tlaxiaco.
2. Project Management Institute. (2021). *Guía del PMBOK®* (7.ª ed.). Estimación de tres puntos y reservas de contingencia.
3. Stellar Development Foundation. (2026). *Stellar Community Fund: Build Awards.* https://communityfund.stellar.org/awards
4. Drips Network. (2026). *Drips Documentation.* https://docs.drips.network/
5. Drips Network. (2026). *Claim your open-source project.* https://docs.drips.network/get-support/claim-your-repository/
6. Instituto Nacional de Lenguas Indígenas. *Catálogo de las Lenguas Indígenas Nacionales: Mixteco.* https://www.inali.gob.mx/sitios/clin-inali/html/v_mixteco.html
7. Instituto Nacional de los Pueblos Indígenas. *Santa María Cuquila, Tlaxiaco, Oaxaca: Historia y tradición de una comunidad mixteca.* https://dili.inpi.gob.mx/santa-maria-cuquila-tlaxiaco-oaxaca/
8. Equipo. (2026). *Backlog y tablero eduScrum del Hub* (Sprint 1).
9. Equipo. (2026). *Acta de Criterios de Aceptación con Clientes* (Sprint 1).
10. Equipo. (2026). *Repositorio e infraestructura financiera*: `FINANCIAMIENTO.md`.
11. Equipo. (2026). *Plan de Calidad*: `COSTO-CALIDAD-HISTORIAS.md` y `METRICAS-CALIDAD.md` (Sprint 2).
12. Equipo. (2026). *Informe Stellar/Drips* y *Lista de verificación* (Sprint 2).
13. Delhij, A., van Solingen, R. y Wijnands, W. (2015). *The eduScrum Guide.*
