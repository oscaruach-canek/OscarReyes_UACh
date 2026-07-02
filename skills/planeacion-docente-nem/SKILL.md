# Skill: Planeacion Docente NEM

Skill de Claude que genera borradores de planeacion didactica para docentes de educacion basica bajo el marco de la Nueva Escuela Mexicana (NEM).

## Que hace esta skill?

Guia al docente paso a paso para producir un borrador completo de planeacion didactica NEM, incluyendo:

- Campos formativos y ejes articuladores aplicables
- Contenidos, procesos de desarrollo del aprendizaje (PDA) y progresiones
- Momentos didacticos (apertura, desarrollo, cierre)
- Sugerencias de evaluacion formativa
- Dashboard de seguimiento grupal (3 pestanas: planeacion, seguimiento, recursos)

## Flujo de uso

1. Recopilar datos: Claude pregunta grado, asignatura/campo formativo, eje articulador, caracteristicas del grupo y tiempo disponible.
2. Redactar contenido: Genera la planeacion con lenguaje NEM autentico (campos formativos, PDA, situaciones de aprendizaje).
3. Llenar el dashboard: Clona la plantilla assets/dashboard_template.html e inserta los datos de la sesion.
4. Cierre: Invita al docente a personalizar y adaptar segun las necesidades reales del grupo.

## Principios que siempre respeta

- Nunca inventa caracteristicas del grupo; siempre pregunta antes de asumir.
- Advierte que la evaluacion sumativa requiere criterios adicionales del docente.
- Marca todo como borrador (la planeacion es un punto de partida, no un producto definitivo).
- Usa terminologia NEM oficial (campos formativos, ejes articuladores, PDA, progresiones).

## Archivos de la skill

- SKILL.md: Este archivo (flujo, principios e instrucciones de uso)
- references/marco_nem.md: Marco conceptual NEM
- assets/dashboard_template.html: Plantilla del dashboard con 3 pestanas

## Instalacion rapida

1. Clona este repositorio o descarga la carpeta skills/planeacion-docente-nem/
2. En Claude Desktop, ve a Configuracion -> Skills -> Importar y selecciona la carpeta.
3. Activa la skill y empieza con: "Ayudame a planear una clase de [campo formativo] para [grado]"

## Aviso

Esta skill es una herramienta de apoyo pedagogico. Las planeaciones generadas son borradores que el docente debe revisar, adaptar y validar conforme al contexto real de su grupo y los lineamientos de su centro escolar. No sustituye el juicio profesional del docente.

Parte del repositorio OscarReyes_UACh - Dr. Oscar Ivan Reyes Maya, UACh.
