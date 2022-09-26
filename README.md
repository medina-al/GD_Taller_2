# Taller 2 Gestión de datos
## Integrantes
- Laura Carolina Tinjacá Cristancho
- Andrés Leonardo Medina Quijano
# Colección seleccionada
Escogimos la colección denominada "movies" de la base de datos "sample_mflix", dicha colección contiene diversa información de películas de todos los géneros, países, directores, épocas y gustos en general.
Algunas datos de la colección:
- Tiene 23530 documentos
- Cuenta con varios campos de tipo objeto/array como países, géneros, directores, premios o reparto
- Los datos en general están muy completos y estandarizados, por lo que el esfuerzo en tareas de calidad de datos es muy bajo

## Datos seleccionados

Los siguientes son los campos del documento que escogimos, algunos son de tipo array por lo que después se presenta la estructura de datos final a la que se deseó llegar:
- ID
- Nombre 
- Año
- Cantidad de nominaciones a premios
- Cantidad de premios ganados
- Géneros (Array)
- Países (Array)
- Puntuación en IMDB
- Puntuación en Rotten Tomatoes

### Estructura de datos

#### Movies 

| Campo       | Tipo de dato |
| ----------- | ------------ |
| _id        | int          |
| title       | varchar(100) |
| year        | date         |
| nominations | int          |
| winnings    | int          |
| runtime     | int          |

#### Genres

| Campo     | Tipo de dato  |
| --------- | ------------- |
| id_movie  | int           |
| genre     | varchar (100) |

#### Countries

| Campo     | Tipo de dato  |
| --------- | ------------- |
| id_movie | int            |
| country   | varchar (100) |

#### Raitings

| Campo            | Tipo de dato |
| ---------------- | ------------ |
| id_movie        | int           |
| rating_imdb     | float         |
| rating_tomatoes | float         |

# Análisis

## Preguntas de negocio

Las siguientes son las preguntas que se pretenden responder con la información extraída:
1. ¿Cuáles son las 5 mejores y las 5 peores películas para la crítica?
2. ¿Cuál es el promedio de duración de las películas por cada género?
3. ¿Cuántas películas se hacen cada año en cada país? ¿Es equitativa la distribución?
4. ¿Cualés son las películas más nominadas y más ganadores de premios en la historia?

# Resultados

## ¿Cuáles son las 5 mejores y las 5 peores películas para la crítica?
Las cinco mejores películas puntuadas por la audiencia son Frozen Planet, The Shawshank Redemption, The Shawshank Redemption, The War, Baseball. 
Por otro lado, las cinco peores películas puntuadas por la audiencia son Krampus: The Christmas Devil, Starship, Gunday, Dragon Fighter, The Hounds


## ¿Cuál es el promedio de duración de las películas por cada género?
El promedio de duración para cada película y cortometraje oscila entre los 128 minutos y 18 minutos para los cortometrajes.


## ¿Cuántas películas se hacen cada año en cada país? ¿Es equitativa la distribución?
USA es el país que presenta mayor cantidad de películas por año. Por lo tanto, no es equitativa su distribución.


## ¿Cualés son las películas más nominadas y más ganadores de premios en la historia?
Las películas con mayor número de nominaciones obtuvieron la mayor cantidad de veces ganadas, entre ellas se encuentran las siguientes películas. Gravity, The Grand Budapest Hotel, 12 Years a Slave, Precious, Birdman: Or (The Unexpected Virtue of Ignorance)
