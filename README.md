# 🧠 Claude Skills — Administración & Comercio

> **Skills para Claude orientadas a estudiantes y profesionales de administración, negocios y comercio, basadas en documentos oficiales y legislación vigente.**

## ¿Qué es este repositorio?

Este repositorio contiene una colección de **Skills personalizadas para Claude** (Anthropic) diseñadas específicamente para el ámbito de la **administración de empresas, contabilidad, derecho mercantil y comercio**. Cada skill encapsula instrucciones, prompts estructurados y marcos de referencia que orientan a Claude para responder con precisión, profundidad y apego a la normativa oficial vigente.

Las skills están pensadas para dos perfiles:

- 🎓 **Estudiantes universitarios** de licenciaturas en Administración, Contaduría, Comercio Internacional, Negocios y áreas afines.
- 💼 **Profesionales y consultores** que requieren apoyo concreto y fundamentado en tareas operativas, análisis jurídico-administrativo y toma de decisiones.

---

## ✨ Características principales

- 📜 **Basadas en fuentes oficiales**: Cada skill referencia legislación, normas y documentos gubernamentales vigentes (DOF, SAT, IMSS, INFONAVIT, Código de Comercio, LISR, LIVA, LSS, entre otros).
- 🏗️ **Estructuradas y reproducibles**: Siguen el formato estándar de skills de Claude, listas para instalar y usar desde Claude Desktop o la API de Anthropic.
- 🇲🇽 **Contexto mexicano**: Enfoque primario en el marco jurídico y prácticas comerciales de México, con posibilidad de adaptación a otros países hispanohablantes.
- 🔄 **Actualizables**: Diseñadas para mantenerse alineadas con reformas fiscales, laborales y mercantiles.
- 🧩 **Modulares**: Cada skill aborda un dominio específico y puede usarse de forma independiente o en combinación.

---

## 📦 Skills incluidas

| Skill | Descripción | Fuentes clave |
|---|---|---|
| `rh-mexico-nomina` | Cálculo de nómina, IMSS, INFONAVIT e ISR para pequeñas empresas | LSS, LISR, Resolución Miscelánea Fiscal |
| `contratos-mercantiles` | Redacción y revisión de contratos civiles y mercantiles | Código Civil Federal, Código de Comercio |
| `constitucion-empresa` | Guía paso a paso para constituir personas morales en México | LGSyM, SAT, RPC |
| `regimenes-fiscales` | Orientación sobre régimen fiscal aplicable según actividad económica | LISR, LIVA, CFF |
| `comercio-exterior` | Procedimientos de importación/exportación, aranceles e Incoterms | Ley Aduanera, TIGIE, SHCP |
| `analisis-financiero` | Interpretación de estados financieros con base en NIF mexicanas | NIF A-1 a NIF B-15, CINIF |
| `prestaciones-ley` | Cálculo de aguinaldo, vacaciones, PTU y liquidaciones | LFT, Ley del IMSS |
| `normas-informacion-financiera` | Aplicación de NIF en registro contable y presentación de información | NIF México (CINIF) |
| `uach-evaluacion-investigacion` | Evaluación de productos de investigación conforme a la norma UACh 2025 | Norma DGIPS-UACh mayo 2025 |

> 🔧 Se añaden nuevas skills regularmente. ¡Contribuciones bienvenidas!

---

## 🚀 Instalación y uso

### Requisitos

- Cuenta activa en [Claude.ai](https://claude.ai) (plan Pro, Team o Enterprise) **o** acceso a la API de Anthropic.
- Para uso en flujos de trabajo avanzados: [Claude Desktop](https://claude.ai/download) con soporte MCP.

### Instalación rápida (Claude Desktop / MCP)

1. Clona el repositorio:
   ```bash
   git clone https://github.com/TU_USUARIO/claude-skills-admin-comercio.git
   ```

2. Copia la carpeta de la skill deseada a tu directorio de skills:
   ```bash
   cp -r claude-skills-admin-comercio/skills/rh-mexico-nomina ~/.claude/skills/
   ```

3. Recarga Claude Desktop y la skill estará disponible en tu sesión.

### Uso directo (sin MCP)

Cada skill incluye un archivo `SKILL.md` con instrucciones de activación. Puedes copiar el contenido del `system_prompt` directamente en una conversación de Claude o usarlo como system prompt en la API.

```python
import anthropic

with open("skills/rh-mexico-nomina/system_prompt.txt") as f:
    system = f.read()

client = anthropic.Anthropic()
message = client.messages.create(
    model="claude-opus-4-5",
    max_tokens=1024,
    system=system,
    messages=[{"role": "user", "content": "¿Cuánto pago de IMSS por un trabajador con salario de $8,000 mensuales?"}]
)
print(message.content)
```

---

## 🗂️ Estructura del repositorio

```
claude-skills-admin-comercio/
├── README.md
├── LICENSE
├── skills/
│   ├── rh-mexico-nomina/
│   │   ├── SKILL.md          # Descripción, triggers y metadatos
│   │   ├── system_prompt.txt # Instrucciones del sistema
│   │   └── ejemplos/         # Casos de uso y prompts de prueba
│   ├── contratos-mercantiles/
│   ├── constitucion-empresa/
│   ├── regimenes-fiscales/
│   ├── comercio-exterior/
│   ├── analisis-financiero/
│   ├── prestaciones-ley/
│   ├── normas-informacion-financiera/
│   └── uach-evaluacion-investigacion/
└── docs/
    ├── guia-de-uso.md
    ├── fuentes-legales.md
    └── contribuir.md
```

---

## ⚠️ Aviso legal

Las skills de este repositorio son **herramientas de apoyo educativo y profesional**. Las respuestas generadas por Claude con estas skills **no constituyen asesoría legal, fiscal o contable formal**. Para decisiones de alto impacto, siempre consulta a un profesional certificado (Contador Público, Abogado, etc.) y verifica la vigencia de las disposiciones normativas en el [Diario Oficial de la Federación (DOF)](https://www.dof.gob.mx).

---

## 👨‍🏫 Autor

**Dr. Óscar Iván Reyes Maya**
Profesor-Investigador · Universidad Autónoma Chapingo (UACh)
Departamento de Ingeniería Agroindustrial / CIDAM

[![ORCID](https://img.shields.io/badge/ORCID-0000--0002--5381--883X-brightgreen?logo=orcid)](https://orcid.org/0000-0002-5381-883X)

Este repositorio forma parte de un esfuerzo por integrar herramientas de inteligencia artificial generativa en la enseñanza y práctica de la administración, con rigor académico y apego a fuentes oficiales.

---

## 🤝 Contribuciones

¿Quieres agregar una skill, mejorar una existente o actualizar una referencia legal? Lee la [guía de contribución](docs/contribuir.md).

Los tipos de contribuciones bienvenidas son:

- Nuevas skills para áreas no cubiertas (finanzas bursátiles, auditoría, negocios internacionales, etc.)
- Actualización de prompts ante reformas fiscales o laborales
- Traducción o adaptación a otros marcos jurídicos (Colombia, España, Argentina, etc.)
- Casos de uso y ejemplos en la carpeta `ejemplos/`

---

## ⭐ Si este repositorio te es útil…

Dale una estrella ⭐ para ayudar a que más estudiantes y profesionales lo encuentren. Compártelo con tu comunidad académica o de trabajo.

---

## 📄 Licencia

Distribuido bajo licencia [MIT](LICENSE). Puedes usar, modificar y redistribuir libremente con atribución al autor original.
