# 🛡️ GRC Toolkit — ENS · ISO 27001 · NIS2

> Herramienta de auto-diagnóstico de cumplimiento normativo en ciberseguridad.  
> Evalúa tu organización frente al **Esquema Nacional de Seguridad**, **ISO 27001:2022** y la **Directiva NIS2** — por separado o en modo cruzado.  
> También útil como herramienta de aprendizaje y estudio.

---

## ¿Qué es este proyecto?

Durante mis estudios de ciberseguridad y mi acercamiento al mundo del **GRC (Governance, Risk & Compliance)**, comprendí la importancia de que las organizaciones conozcan y se adapten al marco normativo que les aplica — algo que, en la práctica, muchas veces se desconoce o se aborda demasiado tarde.

Este toolkit nació como proyecto de autoaprendizaje para familiarizarme con estas normativas de forma práctica, y lo comparto por si puede ser útil a otras personas en el mismo camino.

Tiene dos secciones principales:
- **Cuestionarios de diagnóstico** — preguntas sobre cada normativa que simulan las áreas que se evaluarían en una auditoría real a una empresa u organización.
- **Flashcards de estudio** — para aprender y repasar los controles de forma progresiva.

> ⚠️ **Importante**: estos cuestionarios no sustituyen en ningún caso una auditoría real, que debe ser realizada por una empresa o profesional certificado y autorizado para ello. Esta herramienta tiene un fin orientativo: ayudar a reflexionar sobre las necesidades de adaptación normativa de tu organización y servir como recurso de aprendizaje.

---

## Demo

Abre el archivo `index.html` directamente en cualquier navegador. No requiere servidor, base de datos ni dependencias externas.

---

## ⚙️ Funcionalidades

### 01 · ENS — Esquema Nacional de Seguridad
- **75 medidas** basadas en el RD 311/2022
- Lógica de **niveles Básico, Medio y Alto** — solo se muestran las medidas aplicables a la categoría del sistema
- Resultado con puntuación de cumplimiento, GAP analysis priorizado y plan de acción con remediaciones concretas

### 02 · ISO 27001:2022
- **93 controles** del Anexo A (versión 2022)
- Organizados en **4 dominios**: Controles Organizativos, de Personas, Físicos y Tecnológicos
- Mismo sistema de diagnóstico: cumple / parcial / no cumple

### 03 · NIS2 — Directiva UE 2022/2555
- **30 controles** estructurados en **10 áreas de obligación**
- Referencias explícitas a los artículos de la directiva (Art.20, Art.21)
- Especialmente orientado a entidades esenciales e importantes

### 04 · Evaluación Cruzada 
- Un solo cuestionario que evalúa las **tres normativas simultáneamente**
- Cada pregunta muestra qué controles específicos cubre en ENS, ISO 27001 y NIS2
- Resultado con **tres porcentajes independientes** (uno por normativa) y análisis de solapamientos
- Identifica qué gaps afectan a múltiples marcos normativos a la vez

### 05 · Flashcards de estudio
- Más de **200 tarjetas** (75 ENS + 93 ISO + 30 NIS2)
- Filtros por normativa, dominio y prioridad
- Sistema de seguimiento: "Lo sé / Repasar / Saltar"
- Diseñado para aprender los controles mientras usas la herramienta

---

## Cobertura normativa

| Normativa | Controles | Versión | Áreas |
|---|---|---|---|
| ENS | 75 medidas | RD 311/2022 | 15 familias |
| ISO 27001 | 93 controles | ISO/IEC 27001:2022 | 4 dominios |
| NIS2 | 30 controles | Directiva UE 2022/2555 | 10 áreas |

---

## Stack técnico

```
HTML5 · CSS3 · JavaScript vanilla
Sin dependencias externas
Sin backend — todo corre en el navegador
Un único archivo HTML autocontenido
```

La decisión de no usar frameworks fue intencionada: el objetivo era que cualquier persona pueda descargar el archivo y usarlo directamente, sin npm, sin instalaciones, sin configuración.

---

## Estructura del proyecto

```
grc-toolkit/
├── index.html        # Aplicación completa (único archivo)
└── README.md               # Este archivo

    
```

---

## Casos de uso

- **Consultor GRC**: primera reunión con un cliente para detectar el estado de partida antes del proyecto de adecuación
- **CISO / Responsable de Seguridad**: diagnóstico rápido interno para priorizar inversiones en seguridad
- **Auditor**: checklist de referencia durante una revisión de cumplimiento
- **Estudiante de ciberseguridad**: aprender las normativas de forma práctica y aplicada

---

## Cómo interpretar los resultados

| Puntuación | Nivel | Significado |
|---|---|---|
| ≥ 75% | BUENO | Cumplimiento sólido. Revisar gaps residuales |
| 45–74% | MEJORABLE | Gaps importantes. Priorizar controles de prioridad ALTA |
| < 45% | INSUFICIENTE | Riesgo elevado. Iniciar plan de adecuación urgente |

> ⚠️ **Aviso importante**: Esta herramienta es un instrumento de auto-diagnóstico orientativo. No sustituye a una auditoría formal realizada por un organismo certificador o consultor especializado.

---

## Roadmap

- [ ] Exportar informe en PDF con ReportLab (Python backend)
- [ ] Añadir mapeo completo ENS ↔ ISO 27001 ↔ NIS2 en modo cruzado
- [ ] Guardar y comparar evaluaciones en el tiempo (localStorage)
- [ ] Añadir guías CCN-STIC como referencia por medida ENS
- [ ] Versión multiidioma (inglés)
- [ ] Incluir RGPD / ENS-RGPD como cuarta normativa

---

## Referencias normativas

- [RD 311/2022 — Esquema Nacional de Seguridad](https://www.boe.es/eli/es/rd/2022/05/03/311)
- [ISO/IEC 27001:2022](https://www.iso.org/standard/27001)
- [Directiva NIS2 — UE 2022/2555](https://eur-lex.europa.eu/legal-content/ES/TXT/?uri=CELEX%3A32022L2555)
- [CCN-CERT — Guías CCN-STIC](https://www.ccn-cert.cni.es/es/guias/guias-series-ccn-stic.html)
- [INCIBE — Centro de Ciberseguridad Nacional](https://www.incibe.es)

---

## Autor

Proyecto desarrollado como parte de mi portfolio en **GRC y ciberseguridad**.  

---

## Licencia

MIT License — puedes usar, modificar y distribuir libremente con atribución.

---

*Si este proyecto te ha resultado útil, considera darle una ⭐ en GitHub.*
