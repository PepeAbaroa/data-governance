---
name: data-governance
description: Activa cuando el usuario menciona calidad de datos, diccionario de datos, linaje, auditoría de datos, PII en datasets, metadatos, catalogación, contrato de datos, trazabilidad, clasificación de información (pública/interna/sensible), gestión documental y de conocimiento, o hay que definir qué datos son confiables. NO activa para generar documentación legal de cumplimiento (compliance-cl) ni para diseño físico de bases de datos (db-architect).
---

# Gobernanza de datos, información y conocimiento — router

**Profundidad completa en `references/base.md`.**

## Tabla de decisión
| La tarea trata de… | Ir a |
|---|---|
| Calidad: completitud, consistencia, exactitud de un dataset | base.md §Calidad de Datos |
| Linaje / de dónde viene este número | base.md §Linaje |
| Diccionario / glosario de columnas | base.md §Diccionario de Datos |
| PII: detectar y proteger en datasets | base.md §Gestión de PII (+ compliance-cl si hay que documentar legalmente) |
| Clasificar información y conocimiento organizacional | base.md §AMPLIACIÓN Gobernanza de información y conocimiento |
| Implementación técnica (esquemas, ETL) | skill db-architect |

## Reglas de oro (sin abrir base)
1. Clasificar SIEMPRE antes de mover: pública / interna / sensible (21.719) / crítica — la clasificación decide dónde vive y si entra a un prompt.
2. Dato sin dueño ni linaje = dato no confiable para auditoría, aunque "se vea bien".
3. Toda decisión metodológica durable va a memoria del proyecto; todo entregable lleva su "cómo se generó".

## Grafo
complementa: compliance-cl, db-architect, data-scientist-phd · deriva-a: redactor-experto (documentar), bpm-procesos-cl (proceso documental) · nunca-junto-con: declarar confiable un dato sin verificar fuente
