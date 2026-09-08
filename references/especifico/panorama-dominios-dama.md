# Panorama de los 12 dominios DAMA restantes — definición literal + razonamiento breve

> Tratamiento más liviano que `mapa-dama-dmbok.md` (mismo criterio que el Título VI de la Ley 21.719 en
> `proteccion-datos-personales-cl`): cada dominio trae su definición formal literal + 1-2 líneas de
> razonamiento aplicado. Para profundidad completa de cualquiera, el corpus íntegro está en
> `sources/especifico/dama-dmbok-2nd-edition.pdf.extracto/` (628 páginas, `INDICE.md` con el mapa completo
> de chunks) — se consulta bajo demanda, no se pre-sintetiza todo.

### Capítulo 1 — Data Management (marco general)
> **TEXTO LITERAL** (p.17-18) "Data management goals include: Understanding and supporting the
> information needs of the enterprise [...] Capturing, storing, protecting, and ensuring the integrity of
> data assets. Ensuring the quality of data and information. **Ensuring the privacy and confidentiality of
> stakeholder data.** Preventing unauthorized or inappropriate access [...]"

**Razonamiento aplicado:** confirma que privacidad/confidencialidad es un objetivo nombrado desde el
capítulo 1, no un añadido — la gestión de datos y la protección de datos personales están unidas desde la
base del marco, coherente con el Grafo hacia `proteccion-datos-personales-cl`.

### Capítulo 4 — Data Architecture
> **TEXTO LITERAL** (p.98) "Data Architecture is fundamental to data management. [...] An organization's
> Data Architecture is described by an integrated collection of master design documents at different
> levels of abstraction, including standards that govern how data is collected, stored, arranged, used,
> and removed."

**Razonamiento aplicado:** la arquitectura de datos es el plano/documento maestro — sin ella, cada
sistema nuevo (ej. cada notebook Python del pipeline SLEP) define su propia estructura sin relación con
las demás, generando exactamente el problema de inconsistencia que esta skill ya diagnostica.

### Capítulo 5 — Data Modeling and Design
> **TEXTO LITERAL** (p.124) "Definition: Data modeling is the process of discovering, analyzing, and
> scoping data requirements, and then representing and communicating these data requirements in a
> precise form called the data model."

**Razonamiento aplicado:** el modelo de datos (conceptual → lógico → físico) es insumo directo para
04-tyb-db-architect — esta skill se detiene en el "qué debe representar el modelo" (gobernanza), la
implementación física es de la otra skill.

### Capítulo 6 — Data Storage and Operations
> **TEXTO LITERAL** (p.170) "Definition: The design, implementation, and support of stored data to
> maximize its value."

**Razonamiento aplicado:** dominio mayormente técnico (DBA); el punto de gobierno relevante es el
listado de actividades que incluye "Manage Test Datasets" — regla de oro ya usada por esta skill
("mantener datos de producción fuera de entornos de no-producción") tiene aquí su anclaje formal.

### Capítulo 8 — Data Integration and Interoperability (DII)
> **TEXTO LITERAL** (p.270) "DII is dependent on these other areas of data management: Data Governance
> [...] Data Architecture [...] Data Security [...] Metadata: For tracking the technical inventory of
> data [...], the operational history and lineage of the data [...]"

**Razonamiento aplicado:** confirma textualmente que **linaje es una función de Metadatos aplicada a la
integración**, no un dominio aparte — el "Linaje de Datos" que esta skill trataba como dominio propio en
`base.md` es, según DAMA, una técnica dentro de Metadatos (Cap. 12) e Integración (Cap. 8) combinadas.

### Capítulo 9 — Document and Content Management
> **TEXTO LITERAL** (p.304) "Definition: Planning, implementation, and control activities for lifecycle
> management of data and information found in any form or medium. [...] To comply with legal obligations
> and customer expectations regarding Records management."

**Razonamiento aplicado:** cubre explícitamente contenido no estructurado (documentos, correos, redes
sociales) — relevante para la gestión documental de un SLEP más allá de las bases de datos estructuradas,
y conecta con obligaciones legales de retención de registros.

### Capítulo 10 — Reference and Master Data
> **TEXTO LITERAL** (p.348) "Definition: Managing shared data to meet organizational goals, reduce risks
> associated with data redundancy, ensure higher quality, and reduce the costs of data integration."

**Razonamiento aplicado:** datos maestros (ej. tabla única de establecimientos/RBD) — ya identificados en
`mapa-dama-dmbok.md` §3 como "críticos por definición"; este capítulo da el proceso completo (identificar
fuente autoritativa única, gobernarla, publicarla para consumo de otros sistemas).

### Capítulo 11 — Data Warehousing and Business Intelligence
> **TEXTO LITERAL** (p.382) "Definition: Planning, implementation, and control processes to provide
> decision support data and support knowledge workers engaged in reporting, query, and analysis."

**Razonamiento aplicado:** entregable explícito "Lineage Dictionary" — el linaje documentado es
condición de entrada para cualquier reporte Power BI/TMDL que esta skill ya rastrea en el pipeline SLEP.

### Capítulo 14 — Big Data and Data Science
> **TEXTO LITERAL** (p.498) "As importantly, the speed and volume of data present challenges that
> require different approaches to critical aspects of data management, such as integration, Metadata
> Management, and Data Quality assessment."

**Razonamiento aplicado:** Big Data no exime de gobierno de datos — exige lo mismo (integración,
metadatos, calidad) pero con métodos distintos (ELT en vez de ETL). Puente hacia 04-tyb-data-scientist-phd para
la parte de modelado, y hacia `gobernanza-ia-cl` (pendiente de crear) cuando el uso es específicamente IA.

### Capítulo 15 — Data Management Maturity Assessment
> **TEXTO LITERAL** (p.531-532) "A Data Management Maturity Assessment (DMMA) can be used to evaluate
> data management overall, or it can be used to focus on a single Knowledge Area [...] Regulation:
> Regulatory oversight requires minimum levels of maturity in data management."

**Razonamiento aplicado:** da el instrumento formal para responder "¿qué tan maduro está el gobierno de
datos de este cliente?" con una escala reconocida (CMM-like, 0-5), no una impresión cualitativa —
aplicable como diagnóstico inicial de cualquier consultoría de gobierno de datos.

### Capítulo 16 — Data Management Organization and Role Expectations
> **TEXTO LITERAL** (p.552) "A Data Management Organization should align with a company's organizational
> hierarchy and resources. [...] it makes sense to evolve these organizations, rather than imposing
> radical changes."

**Razonamiento aplicado:** advertencia explícita contra el error común de imponer una estructura de
gobierno de datos "de libro" sin adaptarla a la cultura/jerarquía existente — coherente con
02-ges-cambio-organizacional (evolución, no revolución).

### Capítulo 17 — Data Management and Organizational Change Management
> **TEXTO LITERAL** (p.574) "Organizations don't change, people change [...] People don't resist change.
> They resist being changed [...] Change requires Change Agents, people who pay attention to the people
> and not just the systems."

**Razonamiento aplicado:** aplica el modelo de 8 errores/8 etapas de Kotter (ya cubierto en
02-ges-cambio-organizacional) específicamente a proyectos de datos — confirma que ningún programa de
gobierno de datos sobrevive sin gestión del cambio explícita, sin importar cuán bien diseñado esté
técnicamente.

## Grafo
Complementa `mapa-dama-dmbok.md` (los 5 capítulos centrales) y deriva hacia 04-tyb-db-architect (Caps. 4-6),
02-ges-bpm-procesos-cl (Cap. 9, gestión documental), 04-tyb-data-scientist-phd (Cap. 14), 02-ges-cambio-organizacional
(Caps. 16-17).
