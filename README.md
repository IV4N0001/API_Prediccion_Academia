🎓 API para predecir rendimiento academico
📄 Descripción
Esta API utiliza un modelo de regresión logística para predecir el rendimiento académico de estudiantes de ingeniería en función de diversas características como el promedio anterior, la escolaridad de los padres y las preferencias de estudio.

🗂️ Estructura del Proyecto
El proyecto contiene los siguientes archivos:

classify_students.py: Contiene la función classify_students que toma los datos de los estudiantes y devuelve las predicciones del rendimiento académico.
logistic_regression_model.py: Contiene el modelo de regresión logística (log_reg) y el codificador de etiquetas (label_encoder).
⚙️ Instalación
Para ejecutar este proyecto, necesitas instalar los siguientes paquetes:

bash
Copiar código
pip install numpy scikit-learn
🚀 Cómo Ejecutar
Clona este repositorio en tu máquina local:

bash
Copiar código
git clone https://github.com/usuario/academic-performance-api.git
Navega hasta el directorio del proyecto:

bash
Copiar código
cd academic-performance-api
Ejecuta el script principal con los datos de prueba:

bash
Copiar código
python classify_students.py
🔍 Requisitos de Paquetes
El proyecto requiere los siguientes paquetes:

numpy: para operaciones matemáticas y manipulación de arreglos.
scikit-learn: para el uso del modelo de regresión logística y la codificación de etiquetas.
✏️ Ejemplo de Uso
A continuación se muestra un ejemplo de cómo utilizar la función classify_students:

python
Copiar código
from classify_students import classify_students

# Datos de ejemplo de los estudiantes
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

# Clasificación de los estudiantes
predictions = classify_students(students_data)
print(f"Predicciones del rendimiento académico: {predictions}")
🛠️ Funciones Principales
classify_students(students_data):
Toma una lista de diccionarios con las características de cada estudiante.
Convierte los valores categóricos a texto y los codifica numéricamente.
Utiliza el modelo de regresión logística para predecir el rendimiento académico.
log_reg y label_encoder: Son importados desde el archivo logistic_regression_model.py y se encargan de la predicción y codificación de las características.
📚 Referencias
Scikit-Learn Documentation
NumPy Documentation
🧑‍💻 Autor
Iván Guadalupe Rivera Corral - Desarrollador de la API.
📜 Licencia
Este proyecto está licenciado bajo la MIT License - ver el archivo LICENSE para más detalles.