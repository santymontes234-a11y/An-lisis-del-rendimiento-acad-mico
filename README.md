# Análisis del rendimiento académico

Análisis exploratorio del desempeño de estudiantes en matemáticas, lectura y escritura, con el fin de identificar patrones relacionados con el curso de preparación, el nivel educativo de los padres y otras variables demográficas.

## Dataset

- **Nombre:** Students Performance in Exams
- **Fuente:** Kaggle — https://www.kaggle.com/datasets/spscientist/students-performance-in-exams
- **Descripción:** 1000 registros de estudiantes con variables demográficas (género, grupo étnico, nivel educativo de los padres, tipo de almuerzo, curso de preparación) y sus calificaciones en matemáticas, lectura y escritura.

## Objetivo

Realizar un análisis exploratorio del dataset para identificar patrones en el rendimiento académico de los estudiantes, evaluando el efecto del curso de preparación, el nivel educativo de los padres y otras variables sobre sus calificaciones, y clasificar a los estudiantes según su desempeño general.

## Requisitos

- Python 3
- Las dependencias incluidas en `requirements.txt`

## Instalación

Clonar el repositorio:

```bash
git clone https://github.com/santymontes234-a11y/An-lisis-del-rendimiento-acad-mico.git
```

Entrar al proyecto:

```bash
cd An-lisis-del-rendimiento-acad-mico
```

Crear el entorno:

```bash
python -m venv .venv
```

Activarlo e instalar dependencias:

```bash
source .venv/bin/activate
pip install -r requirements.txt
```

## Ejecución

```bash
jupyter notebook src/analisis_rendimiento_academico.ipynb
```

Y ejecutar las celdas en orden desde el inicio.

## Análisis realizados

1. Exploración inicial del dataset (registros, columnas, tipos de datos, valores faltantes, duplicados, estadísticas descriptivas).
2. Limpieza y preprocesamiento de los datos.
3. Creación de la variable `average_score` (promedio de matemáticas, lectura y escritura).
4. Clasificación del rendimiento académico en tres categorías: Bajo, Medio y Alto.
5. Identificación del área con el promedio más alto.
6. Comparación del desempeño entre estudiantes que tomaron el curso de preparación y quienes no.
7. Análisis del rendimiento según el nivel educativo de los padres.
8. Distribución porcentual de estudiantes por categoría de rendimiento.
9. Comparación del rendimiento entre grupos étnicos (`race/ethnicity`).
10. Visualizaciones de los hallazgos principales.

## Resultados y conclusiones

- La lectura es el área con mejor desempeño promedio y matemáticas la más débil, de forma consistente entre los distintos subgrupos analizados.
- El curso de preparación para el examen está asociado a un mejor desempeño: quienes lo completaron obtienen en promedio varios puntos más que quienes no lo tomaron.
- El nivel educativo de los padres influye en el desempeño: a mayor nivel educativo de los padres, mayor tiende a ser el promedio de los estudiantes, con maestría y licenciatura a la cabeza y "some high school" en el último lugar.
- La mayoría de los estudiantes se concentra en la categoría de rendimiento Medio, con proporciones menores y similares entre Bajo y Alto.
- Existen diferencias notables entre grupos étnicos, con el grupo E mostrando el promedio más alto y el grupo A el más bajo.
- En conjunto, los resultados sugieren que factores externos al estudiante —preparación previa y contexto familiar— están relacionados con su desempeño académico, más allá de diferencias por género, que resultan menos marcadas.
