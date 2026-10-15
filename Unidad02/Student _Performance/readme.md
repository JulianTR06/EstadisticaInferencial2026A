# Descripción de la base de datos: Student Performance Factors

## 1. Descripción general

La base de datos `StudentPerformanceFactors.csv` contiene información sobre factores que pueden estar relacionados con el rendimiento académico de los estudiantes. Incluye variables relacionadas con los hábitos de estudio, la asistencia a clases, el sueño, la motivación, el entorno familiar, los recursos educativos y las características de la escuela.

El conjunto de datos cuenta con **6,607 registros y 20 columnas**. Su variable principal de interés es `Exam_Score`, que representa la puntuación obtenida por los estudiantes en sus exámenes.

Esta información permite analizar la relación entre los hábitos personales, las condiciones socioeconómicas y los factores educativos con el desempeño académico.

## 2. Estructura de la base de datos

La base de datos está compuesta por las siguientes variables:

| Variable | Descripción | Tipo de dato |
|---|---|---|
| `Hours_Studied` | Número de horas dedicadas al estudio. | Entero |
| `Attendance` | Porcentaje de asistencia a clases. | Entero |
| `Parental_Involvement` | Nivel de participación de los padres en la educación. | Categórico |
| `Access_to_Resources` | Nivel de acceso a recursos educativos. | Categórico |
| `Extracurricular_Activities` | Indica si el estudiante participa en actividades extracurriculares. | Categórico |
| `Sleep_Hours` | Horas de sueño del estudiante. | Entero |
| `Previous_Scores` | Puntuaciones obtenidas anteriormente. | Entero |
| `Motivation_Level` | Nivel de motivación del estudiante. | Categórico |
| `Internet_Access` | Indica si el estudiante tiene acceso a internet. | Categórico |
| `Tutoring_Sessions` | Número de sesiones de tutoría recibidas. | Entero |
| `Family_Income` | Nivel de ingresos familiares. | Categórico |
| `Teacher_Quality` | Calidad percibida del docente. | Categórico |
| `School_Type` | Tipo de institución educativa, pública o privada. | Categórico |
| `Peer_Influence` | Influencia del entorno social y de los compañeros. | Categórico |
| `Physical_Activity` | Nivel de actividad física del estudiante. | Entero |
| `Learning_Disabilities` | Indica si se reportan dificultades de aprendizaje. | Categórico |
| `Parental_Education_Level` | Nivel educativo de los padres. | Categórico |
| `Distance_from_Home` | Distancia entre el hogar y la escuela, clasificada por categorías. | Categórico |
| `Gender` | Género registrado del estudiante. | Categórico |
| `Exam_Score` | Puntuación obtenida en el examen. | Entero |

## 3. Características de los datos

- **Número de registros:** 6,607 estudiantes.
- **Número de variables:** 20.
- **Variables numéricas:** 7.
- **Variables categóricas:** 13.
- **Variable objetivo:** `Exam_Score`.
- **Registros duplicados:** requieren una revisión específica para determinar si existen.
- **Valores faltantes:** se identifican datos ausentes en tres variables.

### Valores faltantes

| Variable | Valores faltantes |
|---|---:|
| `Teacher_Quality` | 78 |
| `Parental_Education_Level` | 90 |
| `Distance_from_Home` | 67 |
| **Total** | **235** |

Los 235 valores faltantes corresponden a aproximadamente el 0.18 % de todas las celdas de la base de datos. Antes de realizar un análisis, se recomienda evaluar cómo tratar estos datos ausentes.

## 4. Posibles aplicaciones

Esta base de datos puede utilizarse para desarrollar diferentes tipos de análisis:

1. **Análisis exploratorio:** identificar patrones y distribuciones en las variables académicas y
