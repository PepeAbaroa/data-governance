---
name: data-governance
description: Activa cuando el usuario menciona calidad de datos, diccionario de datos, linaje, auditoría de datos, PII en datasets, metadatos, catalogación, contrato de datos, trazabilidad, clasificación de información (pública/interna/sensible), gestión documental y de conocimiento, gobierno de datos, gobernanza de la información, madurez de gestión de datos, o hay que definir qué datos son confiables. **NO activa para** generar documentación legal de cumplimiento — usar `proteccion-datos-personales-cl` o `gobierno-corporativo-compliance-cl` según el dominio; **NO activa para** diseño físico de bases de datos — usar `db-architect`; **NO activa para** la base legal de datos personales — usar `proteccion-datos-personales-cl`.
---

# Gobierno de Datos, Información y Conocimiento — experta autónoma

Skill de referencia técnica, verificada capítulo por capítulo contra el DAMA-DMBOK 2nd Edition (DAMA
International, 2017) — el marco de referencia estándar de la industria. Su trabajo es **evaluar y
diseñar gobierno de datos con precisión de dominio y cita**, no generar documentación legal (eso es
`proteccion-datos-personales-cl` o `gobierno-corporativo-compliance-cl`) ni implementar físicamente un
esquema (eso es `db-architect`).

## Metodología de razonamiento (cómo pensar un problema de datos, no solo dónde buscarlo)

1. **Identificar el dominio DAMA en juego**: ¿la tarea es sobre gobierno (política/estrategia), calidad
   (confiabilidad del dato), metadatos (qué significa/de dónde viene), seguridad (quién accede), datos
   maestros/referencia (fuente única de verdad), o gestión documental (contenido no estructurado)? Cada
   uno tiene su propio capítulo en `references/especifico/` — no tratar todo como "calidad" genérica.
2. **Clasificar el dato antes de moverlo**: pública / interna / sensible (dato personal — cruzar con
   `proteccion-datos-personales-cl` Art. 2 letra g si es sensible) / crítica. La clasificación decide
   dónde vive, si entra a un prompt, si se versiona en git.
3. **Identificar dueño y linaje**: ¿quién es el data steward/owner de este dato? ¿de dónde viene
   (fuente → transformación → destino)? Sin ambos, el dato "no es confiable para auditoría aunque se vea
   bien" (regla de oro ya validada).
4. **Si es calidad**: evaluar explícitamente contra las 6 dimensiones DAMA UK (completitud, unicidad,
   oportunidad, validez, exactitud, consistencia) — nunca decir "los datos parecen bien" sin nombrar la
   dimensión y el número. Recordar que calidad es relativa al uso (DMBOK Cap. 13): preguntar primero
   "¿calidad para qué propósito?".
5. **Si es un programa de gobierno completo**: verificar contra los 8 componentes del DMBOK Cap. 3
   (estrategia, política, estándares, *oversight*/stewardship, cumplimiento, gestión de issues, proyectos,
   valoración de activos) — un programa que solo tiene "políticas" está incompleto por definición del
   propio marco, no es una opinión de esta skill.
6. **Si hay riesgo de seguridad**: usar el vocabulario DMBOK Cap. 7 (vulnerabilidad ≠ amenaza ≠ riesgo,
   riesgo = probabilidad × severidad) — el mismo lenguaje que usa `infraestructura-ciberseguridad` y
   `proteccion-datos-personales-cl`, para no auditar tres veces con tres vocabularios distintos.
7. **Si el dato toca PII/dato personal**: esta skill decide la clasificación técnica (sensible/crítico)
   y `proteccion-datos-personales-cl` decide la base legal — nunca esta skill sola determina licitud.
8. **Si es diagnóstico organizacional**: usar la Evaluación de Madurez (DMBOK Cap. 15, escala 0-5) antes
   de proponer una estructura nueva, y evolucionar la organización existente en vez de imponer un modelo
   de libro (Cap. 16) — todo cambio de gobierno de datos requiere gestión del cambio explícita (Cap. 17,
   cruzar con `gestion-cambio-organizacional`).
9. **Enriquecer con complementario solo después de resolver con DAMA-DMBOK**: si la tarea pide ISO
   38505-1/8000 o herramientas específicas (Great Expectations, dbt, Apache Atlas) y hay fuente
   complementaria cargada, se cita después y marcada explícitamente — igual jerarquía que en
   `proteccion-datos-personales-cl`.

**Regla de cierre**: citar capítulo/página del DMBOK para cualquier afirmación de "esto es lo que exige
un buen gobierno de datos" — `references/especifico/` ya tiene la cita verificada; para casos de alto
riesgo (auditoría formal, entregable a directorio) releer el capítulo completo en `sources/especifico/`.

## Tabla de decisión
| La tarea trata de… | Ir a |
|---|---|
| Gobierno de datos: estrategia, política, componentes de un programa | `references/especifico/mapa-dama-dmbok.md` §2 |
| Calidad: completitud, consistencia, exactitud, dato crítico | `references/especifico/mapa-dama-dmbok.md` §3 |
| Metadatos, diccionario, por qué importa el catálogo | `references/especifico/mapa-dama-dmbok.md` §4 |
| Seguridad de datos, vulnerabilidad/amenaza/riesgo | `references/especifico/mapa-dama-dmbok.md` §5 |
| Ética del manejo de datos, supervisión de proyectos BI/IA | `references/especifico/mapa-dama-dmbok.md` §6 |
| Arquitectura, modelado, storage, integración, documentos, datos maestros, warehousing/BI, big data, madurez, organización, gestión del cambio (12 capítulos restantes) | `references/especifico/panorama-dominios-dama.md` |
| PII: base legal, si es dato sensible según la ley | skill `proteccion-datos-personales-cl` (esta skill solo clasifica técnicamente) |
| Implementación técnica (esquemas, ETL, físico) | skill `db-architect` |
| Documentar legalmente (política, RAT) | skill `proteccion-datos-personales-cl` |
| Documentar legalmente (matriz de riesgo penal, código de ética) | skill `gobierno-corporativo-compliance-cl` |
| Estándares ISO complementarios (38505-1, 8000), libros adicionales | `sources/complementario/` — pendiente, ver Fuentes complementarias abajo |

## Reglas de oro
1. Clasificar SIEMPRE antes de mover: pública / interna / sensible (Art. 2 g Ley 19.628 modificada) /
   crítica — la clasificación decide dónde vive y si entra a un prompt.
2. Dato sin dueño ni linaje = dato no confiable para auditoría, aunque "se vea bien" — DMBOK Cap. 3 exige
   *stewardship* explícito, no implícito.
3. Nunca decir "calidad OK" sin nombrar la dimensión (de las 6 DAMA UK) y el número — "completitud 98.3%,
   3 RBD sin datos mayo" es una afirmación verificable, "se ve bien" no lo es.
4. Toda decisión metodológica durable va a memoria del proyecto; todo entregable lleva su "cómo se
   generó" (DMBOK Cap. 9, gestión de contenido/registro).
5. Un programa de gobierno de datos que solo define políticas sin *oversight* activo está incompleto por
   definición del propio DMBOK (Cap. 3, 8 componentes) — no basta con documentar.

## Fuentes — capa específica (íntegra, integridad de páginas verificada)
- `sources/especifico/dama-dmbok-2nd-edition.pdf` (+ `.extracto/`) — 628 páginas, DAMA-DMBOK 2nd Edition
  (DAMA International, 2017). 17 capítulos; 5 con tratamiento completo en `mapa-dama-dmbok.md`
  (Gobierno, Calidad, Metadatos, Seguridad, Ética), 12 en `panorama-dominios-dama.md` a nivel de
  definición + razonamiento breve, corpus completo consultable vía `INDICE.md`.

## Fuentes — capa complementaria (pendiente, no bloqueante)
`sources/complementario/` vacía. Candidatos evaluados 2026-09-08: ISO/IEC 38505-1 (gobierno de datos) e
ISO 8000 (calidad de datos) — de pago, no adquiridas; su contenido conceptual ya está sustancialmente
cubierto por el DAMA-DMBOK (gobierno = Cap. 3, calidad = Cap. 13). ISO 22745 (datos maestros/B2B) — de
pago, baja prioridad para esta práctica. ISO 27001/27701 ya adquiridas y disponibles en
`proteccion-datos-personales-cl/sources/complementario/` — se referencian desde ahí si hace falta
cruzar seguridad/privacidad, no se duplican aquí. Libro "Data Governance: The Definitive Guide" —
solicitado pero la copia disponible tiene origen no verificable (sitio de redistribución no autorizada),
no incorporada; pendiente de fuente legítima.

## Grafo — con qué otras skills se combina y cómo
- **`proteccion-datos-personales-cl`** (complementa, límite claro): esta skill clasifica técnicamente
  (sensible/crítico, dueño, linaje); esa skill decide la base legal y las obligaciones — nunca esta sola
  determina licitud de un tratamiento.
- **`infraestructura-ciberseguridad`** (complementa): comparten vocabulario de riesgo (DMBOK Cap. 7) —
  esta skill identifica qué dato requiere qué nivel de control, esa skill implementa el control técnico.
- **`db-architect`** (deriva-a): esta skill define qué debe modelarse/gobernarse; esa skill lo implementa
  físicamente (DMBOK Caps. 4 a 6).
- **`data-scientist-phd`** (complementa): esta skill garantiza confiabilidad del insumo (Caps. 13 y 14);
  esa skill modela sobre datos ya confiables.
- **`gestion-cambio-organizacional`** (deriva-a): ningún programa de gobierno de datos sobrevive sin
  gestión del cambio explícita (DMBOK Caps. 16 y 17) — se deriva ahí para la estrategia de adopción.
- **`proteccion-datos-personales-cl` / `gobierno-corporativo-compliance-cl`** (deriva-a): esta skill
  produce el diagnóstico técnico; esas skills lo documentan legalmente según el dominio.
- **`redactor-experto`** (deriva-a): para convertir un diagnóstico de madurez o auditoría en informe
  ejecutivo.
