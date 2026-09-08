# Mapa DAMA-DMBOK 2nd Edition — texto literal + razonamiento aplicado

> Verificado contra `sources/especifico/dama-dmbok-2nd-edition.pdf.extracto/` (628 páginas físicas,
> integridad confirmada). El libro tiene 17 capítulos — dado su tamaño (más de 10x cualquier ley ya
> tratada en esta arquitectura), este archivo da tratamiento completo (TEXTO LITERAL + Razonamiento
> aplicado) a los **5 capítulos que sostienen el trabajo real de esta skill** (Gobierno de Datos, Calidad,
> Metadatos, Seguridad, Ética) y trata el resto en `panorama-dominios-dama.md` a nivel de definición y
> puntero al `INDICE.md` — no es omitir contenido, es la misma lógica ya aplicada al Título VI de la Ley
> 21.719 (profundidad proporcional a lo que realmente se consulta).
>
> **Formato**: `TEXTO LITERAL` (cita exacta) + `Razonamiento aplicado` (interpretación, nunca mezclado).

---

## 1. Marco general — DAMA-DMBOK2 Data Management Framework

> **TEXTO LITERAL** (Cap. 3, p.67, `chunk_070.md`)
> "Data Governance (DG) is defined as the exercise of authority and control (planning, monitoring, and
> enforcement) over the management of data assets. All organizations make decisions about data,
> regardless of whether they have a formal Data Governance function. [...] The Data Governance function
> guides all other data management functions."

**Razonamiento aplicado:** el "rueda" DAMA-DMBOK2 tiene 11 dominios (Gobierno de Datos en el centro,
rodeado de: Calidad, Metadatos, Arquitectura, Modelado y Diseño, Almacenamiento y Operaciones,
Seguridad, Integración e Interoperabilidad, Documentos y Contenido, Datos Maestros/Referencia,
Warehousing/BI) — **el Gobierno de Datos no es un dominio más, es el que gobierna a todos los demás**.
Cualquier trabajo de "calidad" o "metadatos" sin gobierno detrás es técnica aislada, no gestión de datos
real — coincide con la crítica ya validada en esta skill: "gobernanza decorativa" vs. gobernanza que
funciona.

---

## 2. Gobierno de Datos (Capítulo 3)

> **TEXTO LITERAL** (Definición formal, p.69, `chunk_072.md`)
> "Definition: The exercise of authority, control, and shared decision-making (planning, monitoring, and
> enforcement) over the management of data assets."

> **TEXTO LITERAL** (Alcance típico de un programa, p.68, `chunk_071.md`)
> "Strategy: Defining, communicating, and driving execution of Data Strategy and Data Governance
> Strategy · Policy: Setting and enforcing policies related to data and Metadata management, access,
> usage, security, and quality · Standards and quality: Setting and enforcing Data Quality and Data
> Architecture standards · Oversight: Providing hands-on observation, audit, and correction [...] (often
> referred to as stewardship) · Compliance: Ensuring the organization can meet data-related regulatory
> compliance requirements · Issue management [...] · Data management projects [...] · Data asset
> valuation: Setting standards and processes to consistently define the business value of data assets."

**Razonamiento aplicado:** 8 componentes, no uno solo — un programa que solo hace "políticas" (lo más
común en la práctica) sin *oversight/stewardship* activo, sin gestión de issues, y sin valuación de
activos de datos está incompleto por definición del propio DAMA, aunque tenga documentos bien escritos.
Para SLEP/cliente educativo: el componente "Compliance" es el puente directo hacia
`proteccion-datos-personales-cl` — el gobierno de datos no reemplaza el cumplimiento legal, lo sostiene
operativamente (sin RAT/linaje no se puede demostrar cumplimiento, ver
`~/.claude/skills/proteccion-datos-personales-cl/references/complementario/criterios-rat-eipd-mpi.md`).

> **TEXTO LITERAL** (Actividades formales, p.69, `chunk_072.md`)
> "Activities: 1. Define Data Governance for the Organization (P) [...] 2. Define the Data Governance
> Strategy (P) [...] 3. Implement Data Governance (O): Sponsor Data Standards and Procedures, Develop a
> Business Glossary, Co-ordinate with Architecture Groups, Sponsor Data Asset Valuation. 4. Embed Data
> Governance (C,O)."

**Razonamiento aplicado:** secuencia de 4 fases (Definir → Estrategia → Implementar → Incorporar/
Embeber) — "Embed" es la fase que casi siempre se salta en la práctica: un programa de gobierno que
nunca llega a "incorporarse" a la operación diaria queda como iniciativa de proyecto, no como función
permanente. El **Business Glossary** (glosario de negocio) aparece como entregable explícito de la fase
de implementación — es exactamente el "Diccionario de Datos" que ya tenía esta skill como dominio propio,
ahora con anclaje textual.

---

## 3. Calidad de Datos (Capítulo 13)

> **TEXTO LITERAL** (Definición, p.454, `chunk_458.md`)
> "Data is of high quality to the degree that it meets the expectations and needs of data consumers. That
> is, if the data is fit for the purposes to which they want to apply it. It is of low quality if it is not
> fit for those purposes. Data quality is thus dependent on context and on the needs of the data
> consumer."

**Razonamiento aplicado:** calidad NO es una propiedad absoluta del dato — es relativa al uso. Un dataset
"de mala calidad" para un análisis financiero de precisión puede ser perfectamente adecuado para un
reporte agregado de tendencia. Antes de auditar calidad hay que preguntar primero "¿calidad para qué uso
específico?", no aplicar un estándar único.

> **TEXTO LITERAL** (Las 6 dimensiones DAMA UK, p.457, `chunk_461.md` — fuente exacta del "las 6
> dimensiones" que esta skill ya usaba sin cita)
> "In 2013, DAMA UK produced a white paper describing six core dimensions of data quality: Completeness:
> The proportion of data stored against the potential for 100%. Uniqueness: No entity instance (thing)
> will be recorded more than once based upon how that thing is identified. Timeliness: The degree to
> which data represent reality from the required point in time. Validity: Data is valid if it conforms to
> the syntax (format, type, range) of its definition. Accuracy: The degree to which data correctly
> describes the 'real world' object or event being described. Consistency: The absence of difference,
> when comparing two or more representations of a thing against a definition."

**Razonamiento aplicado — esto es exactamente lo que `SKILL.md` anterior citaba sin fuente**: las 6
dimensiones (Completitud, Unicidad, Oportunidad, Validez, Exactitud, Consistencia) vienen textualmente
del white paper DAMA UK 2013, referenciado dentro del propio DMBOK2 — no eran una lista inventada, pero
tampoco estaban citadas. Ahora sí quedan ancladas a la fuente exacta.

> **TEXTO LITERAL** (Dato crítico, p.454, `chunk_458.md`)
> "Master Data is critical by definition. Data sets or individual data elements can be assessed for
> criticality based on the processes that consume them, the nature of the reports they appear in, or the
> financial, regulatory, or reputational risk to the organization if something were to go wrong with the
> data."

**Razonamiento aplicado:** criterio operativo para decidir QUÉ auditar primero cuando no hay tiempo para
auditar todo: datos maestros (ej. RBD, tabla de establecimientos, tabla de funcionarios) son críticos
"por definición" — no hace falta justificar caso a caso por qué se prioriza su calidad, DAMA ya lo
establece como regla general.

---

## 4. Metadatos (Capítulo 12)

> **TEXTO LITERAL** (Definición y analogía, p.417-418, `chunk_420.md`-`chunk_421.md`)
> "The most common definition of Metadata, 'data about data,' is misleadingly simple. [...] To understand
> Metadata's vital role in data management, imagine a large library, with hundreds of thousands of books
> and magazines, but no card catalog. [...] An organization without Metadata is like a library without a
> card catalog. [...] Without reliable Metadata, an organization does not know what data it has, what the
> data represents, where it originates, how it moves through systems, who has access to it, or what it
> means for the data to be of high quality."

**Razonamiento aplicado:** la frase final es la justificación textual de por qué "linaje" y "diccionario
de datos" (dominios que esta skill ya trabajaba) son en realidad sub-componentes de Metadatos, no
categorías paralelas — sin metadata no se puede saber de dónde viene el dato (linaje) ni qué significa
cada campo (diccionario). Confirma también el vínculo con seguridad: *"Metadata is necessary to ensure an
organization can identify private or sensitive data"* — el catálogo de metadatos es la herramienta que
permite saber DÓNDE está el PII antes de poder protegerlo, conectando directo con
`proteccion-datos-personales-cl` (Art. 14 ter, RAT).

---

## 5. Seguridad de Datos (Capítulo 7)

> **TEXTO LITERAL** (Definición, p.217, `chunk_220.md`)
> "Data Security includes the planning, development, and execution of security policies and procedures to
> provide proper authentication, authorization, access, and auditing of data and information assets. [...]
> the goal of data security practices is the same: To protect information assets in alignment with
> privacy and confidentiality regulations, contractual agreements, and business requirements."

**Razonamiento aplicado:** DAMA vincula explícitamente seguridad de datos con "privacy and
confidentiality regulations" — es el puente directo hacia `infraestructura-ciberseguridad` (el control
técnico) y `proteccion-datos-personales-cl` (la obligación legal, Art. 14 quinquies) — esta skill aporta
la capa de gobernanza/proceso entre ambas, no reemplaza a ninguna.

> **TEXTO LITERAL** (Vocabulario esencial, p.223, `chunk_226.md`)
> "A vulnerability is a weaknesses or defect in a system that allows it to be successfully attacked and
> compromised [...] A threat is a potential offensive action that could be taken against an organization.
> [...] The term risk refers both to the possibility of loss and to the thing or condition that poses the
> potential loss. Risk can be calculated for each possible threat using the following factors: Probability
> [...], the type and amount of damage [...], the effect damage will have on revenue or business
> operations, the cost to fix the damage [...], the cost to prevent the threat [...], the goal or intent of
> the probable attacker."

**Razonamiento aplicado:** este vocabulario (vulnerabilidad ≠ amenaza ≠ riesgo) es el mismo que exige
`infraestructura-ciberseguridad` y coincide con la metodología riesgo = probabilidad × severidad ya usada
en `proteccion-datos-personales-cl/references/complementario/criterios-rat-eipd-mpi.md` §3 — es el mismo
lenguaje de riesgo repetido en 3 dominios distintos (datos, ciberseguridad, protección de datos), lo que
confirma que debería ser una sola matriz de riesgo compartida, no tres auditorías separadas con
terminología distinta.

---

## 6. Ética del manejo de datos (Capítulo 2)

> **TEXTO LITERAL** (Modelo de riesgo ético, p.64, `chunk_067.md`)
> "Data professionals involved in Business Intelligence, analytics, and Data Science are often responsible
> for data that describes: Who people are [...] What people do [...] Where people live [...] How people
> are treated, including outcomes of analysis, such as scoring and preference tracking that will tag them
> as ultimately privileged or not for future business. This data can be misused and counteract the
> principles underlying data ethics: respect for persons, beneficence, and justice."

> **TEXTO LITERAL** (Vínculo con gobierno, p.64, `chunk_068.md`)
> "Oversight for the appropriate handling of data falls under both data governance and legal counsel.
> [...] Data Governance must set standards and policies for and provide oversight of data handling
> practices. [...] Data Governance has a particular oversight requirement to review plans and decisions
> proposed by BI, analytics and Data Science studies."

**Razonamiento aplicado:** la ética de datos no es un capítulo aislado de filosofía — DAMA la ata
formalmente a Gobierno de Datos como función de supervisión obligatoria sobre cualquier proyecto de
BI/analytics/Data Science. Para un sistema tipo "alerta de riesgo de deserción escolar" (ya analizado en
`proteccion-datos-personales-cl` bajo el Art. 8 bis y 15 ter), el Gobierno de Datos tiene, según DAMA, la
responsabilidad explícita de revisar ese tipo de proyecto ANTES de implementarlo — no es solo un requisito
legal (EIPD), es también una función de gobierno de datos por diseño del propio marco DAMA.

---

## Grafo
Se combina con `proteccion-datos-personales-cl` (PII, base legal), `infraestructura-ciberseguridad`
(control técnico de seguridad), 04-tyb-db-architect (implementación física). Ver `panorama-dominios-dama.md`
para los 12 capítulos restantes del libro (arquitectura, modelado, storage, integración, documentos,
datos maestros, warehousing/BI, big data, madurez, organización, gestión del cambio).
