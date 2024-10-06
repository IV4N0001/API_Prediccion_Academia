# API para predecir rendimiento academico utilizando regresión logística
## Descripción

Esta API utiliza un modelo de regresión logística para predecir el rendimiento académico de estudiantes de ingeniería en función de diversas características como el promedio anterior, la escolaridad de los padres y las preferencias de estudio.

## Estructura del Proyecto

El proyecto contiene los siguientes archivos:

classify_students.py: Contiene la función classify_students que toma los datos de los estudiantes y devuelve las predicciones del rendimiento académico.

logistic_regression_model.py: Contiene el modelo de regresión logística (log_reg) y el codificador de etiquetas (label_encoder).

## Instalación
Para ejecutar este proyecto primero necesitas instalar los siguientes paquetes:

    pip install numpy scikit-learn

Despues ejecuta: 

    python classify_students.py

## Datos de ejemplo de los estudiantes
    students_data = [
        {
            'father_education': 2,
            'mother_education': 1,
            'family_income': 2,
            'high_school_GPA': 3,
            'current_GPA': 8.2,
            'study_preference': 1,
            'preference_academic_activities': 3,
            'study_frequency': 2
        }
    ]
