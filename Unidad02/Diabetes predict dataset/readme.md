# Descripción de la base de datos: Diabetes Prediction Dataset

## 1. Descripción general

La base de datos `diabetes_prediction_dataset.csv` contiene información relacionada con características demográficas, antecedentes médicos y factores de salud de diferentes personas, con el propósito de analizar los factores asociados con la presencia de diabetes.

El conjunto de datos cuenta con **100,000 registros y 9 columnas**. Incluye variables como género, edad, hipertensión, enfermedades cardíacas, historial de tabaquismo, índice de masa corporal, nivel de hemoglobina glucosilada y nivel de glucosa en sangre.

La variable principal de interés es `diabetes`, que indica si una persona presenta diabetes o no.

## 2. Estructura de la base de datos

La base de datos está compuesta por las siguientes variables:

| Variable | Descripción | Tipo de dato |
|---|---|---|
| `gender` | Género de la persona. | Categórico |
| `age` | Edad de la persona en años. | Numérico |
| `hypertension` | Indica si la persona presenta hipertensión. | Binario |
| `heart_disease` | Indica si la persona presenta alguna enfermedad cardíaca. | Binario |
| `smoking_history` | Historial de consumo de tabaco. | Categórico |
| `bmi` | Índice de masa corporal de la persona. | Numérico |
| `HbA1c_level` | Nivel de hemoglobina glucosilada en sangre. | Numérico |
| `blood_glucose_level` | Nivel de glucosa en sangre. | Numérico |
| `diabetes` | Indica si la persona presenta diabetes. | Binario |

## 3. Características de los datos

- **Número de registros:** 100,000 personas.
- **Número de variables:** 9.
- **Variables numéricas:** 5.
- **Variables categóricas:** 2.
- **Variables binarias:** 2.
- **Variable objetivo:** `diabetes`.
- **Valores faltantes:** no se identificaron valores nulos.
- **Registros duplicados:** requieren una revisión específica.

### Distribución de las variables principales

| Variable | Valores o rango |
|---|---|
| `gender` | Female, Male, Other |
| `age` | 0.08 a 80 años |
| `hypertension` | 0 = No, 1 = Si |
| `heart_disease` | 0 = No, 1 = Si |
| `smoking_history` | never, No Info, current, former, ever, not current |
| `bmi` | 10.01 a 95.69 |
| `HbA1c_level` | 3.5 a 9.0 |
| `blood_glucose_level` | 80 a 300 |
| `diabetes` | 0 = No, 1 = Si |

### Distribución de la variable objetivo

La variable `diabetes` permite identificar la presencia o ausencia de diabetes:

- **0:** personas que no presentan diabetes.
- **1:** personas que presentan diabetes.

En el conjunto de datos, aproximadamente el 8.5 % de los registros corresponde a personas con diabetes, mientras que el 91.5 % corresponde a personas sin diabetes.

## 4. Posibles aplicaciones

Esta base de datos puede utilizarse para desarrollar diferentes tipos de análisis:

1. **Análisis exploratorio:** identificar patrones y distribuciones en las características de salud de las personas.
2. **Análisis de correlación:** estudiar la relación entre la edad, el índice de masa corporal, la glucosa y la diabetes.
3. **Análisis de factores de riesgo:** explorar la asociación de la hipertensión, las enfermedades cardíacas y el tabaquismo con la presencia de diabetes.
4. **Visualización de datos:** crear histogramas, diagramas de dispersión y gráficos comparativos.
5. **Aprendizaje automático:** desarrollar modelos de clasificación para predecir la presencia de diabetes.
6. **Identificación de patrones:** analizar qué características presentan mayor asociación con la variable objetivo.

## 5. Consideraciones para el análisis

Antes de utilizar
