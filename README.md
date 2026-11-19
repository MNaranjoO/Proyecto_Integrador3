# Proyecto Integrador 2 — Sistema de Notas y Asistencias

## Integrantes

- **Luis Miguel Naranjo Ocampo** — CC 1040049580
- **Daniel Alejandro Martínez Ardila** — CC 1036949511
- **Diego Andrés Castañeda Villada** — CC 1036942350
- **Jhonatan Arley Arias Higuita** — CC 1036964562

---

## Descripción del proyecto

Este proyecto corresponde a la maquetación web estática en **HTML5** y **CSS3** de un **Sistema de Notas y Asistencias** académico, estructurado a partir de nuestro Modelo Entidad-Relación (MER) y Modelo Relacional (MR) de 7 tablas normalizadas.

El sistema se divide en **dos entornos funcionales**:

1. **Portal Público (acceso general y estudiantes):**
   - `index.html`: Página de inicio con la presentación del sistema, guía de perfiles y acceso directo a todos los módulos.
   - `consulta.html`: Portal de consulta donde el estudiante visualiza su resumen consolidado por materia, el desglose individual de calificaciones por actividad y el historial detallado de asistencias con fechas exactas.
   - `login.html`: Formulario de ingreso para profesores con validación HTML5.

2. **Panel del Profesor (gestión académica):**
   - `estudiantes.html`: Registro y listado de estudiantes (`id_estudiante`, `nombre`, `apellido`, `correo`).
   - `profesores.html`: Registro y listado de docentes (`id_profesor`, `nombre`, `apellido`, `correo`).
   - `materias.html`: Registro y catálogo de asignaturas (`id_materia`, `nombre`, `descripcion`).
   - `profesores_materias.html`: Tabla intermedia (`id_profesor_materia`, `id_profesor`, `id_materia`) que permite asignar múltiples materias a un mismo profesor.
   - `matriculas.html`: Inscripción de estudiantes en materias por periodo (`id_matricula`, `id_estudiante`, `id_materia`, `anio_periodo`).
   - `notas.html`: Registro de calificaciones asociadas a una matrícula (`id_nota`, `id_matricula`, `descripcion`, `valor_nota`).
   - `asistencias.html`: Control de asistencia por matrícula y fecha (`id_asistencia`, `id_matricula`, `fecha`, `estado`).
   - `resumen.html`: Tablero general con el conteo de registros de las 7 tablas del modelo y el consolidado académico por matrícula.

---

## Estructura de archivos

```text
Proyecto_Integrador2/
├── index.html                 # Página principal
├── consulta.html              # Consulta detallada de notas y asistencias
├── login.html                 # Inicio de sesión para profesores
├── estudiantes.html           # Gestión de estudiantes
├── profesores.html            # Gestión de profesores
├── materias.html            # Gestión de materias
├── profesores_materias.html   # Asignación de materias a profesores
├── matriculas.html            # Gestión de matrículas
├── notas.html                 # Registro de calificaciones
├── asistencias.html           # Registro de asistencias
├── resumen.html               # Resumen general y consolidado por matrícula
├── style.css                  # Hoja de estilos única para todo el proyecto
└── README.md                  # Documentación e instrucciones de ejecución