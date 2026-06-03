Asesor de Recursos Humanos para micro empresas en México. Calcula nómina, retenciones ISR, cuotas IMSS/INFONAVIT, prestaciones de ley y genera visualizadores interactivos — todo fundamentado en los textos legales vigentes.

Base normativa
LeyÚltima reforma incorporadaLey Federal del Trabajo (LFT)DOF 14-05-2026Ley del Seguro Social (LSS)DOF 07-06-2024Ley del Impuesto sobre la Renta (LISR)DOF 01-04-2024

Los PDFs oficiales de las tres leyes fueron procesados directamente para construir esta skill. Las tablas numéricas (tarifa ISR Art. 96, cuotas LSS, subsidio al empleo) provienen de los textos originales de la Cámara de Diputados.


¿Qué hace esta skill?

Nómina: calcula percepciones, deducciones IMSS obrero e ISR, y neto al trabajador
Costo patrón: desglosa cuotas IMSS + INFONAVIT por rama (Arts. 106, 107, 147, 168 LSS)
Prestaciones anuales: aguinaldo (Art. 87 LFT), vacaciones (Art. 76 LFT), prima vacacional (Art. 80 LFT), PTU (Art. 117 LFT)
Finiquitos y liquidaciones: cálculo por tipo de contrato (Art. 50 LFT)
Contratos: plantilla por tiempo determinado con cláusulas del Art. 25 LFT
Visualizadores interactivos: dashboards React con sliders para modificar salario, antigüedad y prima de riesgo en tiempo real


Estructura del repositorio
rh-mexico-asesoria/
├── SKILL.md                          # Definición principal de la skill
└── references/
    ├── cuotas-imss.md                # Tablas completas LSS con tasas escalonadas por SBC
    ├── isr-tablas.md                 # Tarifa Art. 96 LISR + subsidio al empleo
    ├── nomina-ejemplo.md             # Nómina quincenal completa paso a paso
    ├── contratos.md                  # Plantilla contrato por tiempo determinado
    └── checklist-patron.md          # Obligaciones del patrón: al contratar, durante y al terminar

Instalación

Descarga el archivo rh-mexico-asesoria.skill
En claude.ai ve a Configuración → Skills
Selecciona Instalar skill y sube el archivo


Ejemplos de uso
"Voy a contratar a alguien con $18,000 al mes, ¿cuánto le retengo de ISR?"

"Genera un visualizador interactivo de nómina para modificar el salario"

"Mi empleado lleva 3 años, ¿cuántos días de vacaciones le corresponden?"

"¿Cuánto me cuesta en total tener un empleado con salario de $12,000?"

"Calcula el finiquito si termina el contrato en diciembre"

"¿Cuáles son mis obligaciones al dar de alta a un trabajador en el IMSS?"

Valores vigentes 2025
ConceptoValorSalario Mínimo General$278.80 MXN/díaUMA diaria$108.57 MXNTope SBC (25 UMA)$2,714.25 MXN/día

Fuentes: CONASAMI · INEGI (UMA)


Cuándo actualizar
Qué cambiaCuándoQué actualizarSalario mínimoEnero de cada añoSKILL.md — tabla de valores vigentesUMAFebrero de cada añoSKILL.md y references/cuotas-imss.mdTarifa ISR Art. 96Cuando inflación acumulada > 10% (Art. 152 LISR)references/isr-tablas.mdCuotas IMSSCon reformas a la LSSreferences/cuotas-imss.mdDías de vacacionesCon reformas a la LFTSKILL.md — tabla Art. 76

Cobertura y limitaciones
✅ Zona salarial general (todo México excepto frontera norte)
✅ Contratos por tiempo determinado e indeterminado
✅ Micro y pequeña empresa (1–50 empleados)
✅ Personas físicas con actividad empresarial como patrón
⚠️ No cubre zona frontera norte (SMG diferente)
⚠️ No incluye contratos colectivos ni tabuladores sindicales
⚠️ PTU requiere conocer la renta gravable declarada al SAT
⚠️ Prima de riesgo de trabajo varía por empresa (usar SIRT del IMSS)

Advertencia legal
Esta skill proporciona orientación general con base en los textos legales vigentes. No sustituye la asesoría de un contador certificado (CP) o abogado laboral para situaciones específicas, procesos ante el IMSS, litigios laborales o declaraciones fiscales formales.

Autor
Óscar Reyes · Universidad Autónoma Chapingo (UACh)
Skill construida con Claude · Base legal: Cámara de Diputados del H. Congreso de la Unión
