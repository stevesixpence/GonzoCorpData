# GonzoCorpData
Repositorio para DataScience Coderhouse

El dataset esta compuesto de una carpeta de archivos en formato CSV conteniendo informacion de usuarios de USA que realizan reservaciones en AirBnB para diferentes paises. Dicho Dataset puede descargarse de kaggle (solo despues de un muy engorroso proceso de alta de usuario) en la siguiente liga:

__https://www.kaggle.com/competitions/airbnb-recruiting-new-user-bookings/data__

El sitio web describe el Dataset con el siguiente parrafo:

''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
Dataset Description'''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''

In this challenge, you are given a list of users along with their demographics, web session records, and some summary statistics. You are asked to predict which country a new user's first booking destination will be. All the users in this dataset are from the USA.

There are 12 possible outcomes of the destination country: 'US', 'FR', 'CA', 'GB', 'ES', 'IT', 'PT', 'NL','DE', 'AU', 'NDF' (no destination found), and 'other'. Please note that 'NDF' is different from 'other' because 'other' means there was a booking, but is to a country not included in the list, while 'NDF' means there wasn't a booking.

The training and test sets are split by dates. In the test set, you will predict all the new users with first activities after 7/1/2014 (note: this is updated on 12/5/15 when the competition restarted). In the sessions dataset, the data only dates back to 1/1/2014, while the users dataset dates back to 2010. ''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''

El dataset consta de 5 archivos en formato CSV que contienen unformacion de los usuarios y reservaciones en la plataforma AirBnb. Los archivos son los siguientes:

1. **age_gender_bkts**: contiene info. de la edad, pais, genero, ID y anyo de registro de los usuarios
2. **countries**: describe los paises destino de los diferentes usuarios, describe la ubicacion con latitud y longitud, distancia en km, descripcion del destino en km2, lenguaje del pais destino y distancia levenshtein del lenguaje
3. **sessions**: contiene informacion de sesion del usuario, userID, accion ejecutada, tipo de accion, detalle de accion, tipo de dispositivo y segundos transcurridos. Este archivo se omite dentro de este repositorio, pues es bastante pesado.
4. **test_users**: dataset de 15 columnas con informacion de los regtistros como user ID, fecha de creacion del usuario, timestamp de actividad, fecha de la primera reserva, genero, edad, metodo de registro, flujo de registro, idioma, canal afiliado, proveedor afiliado, primer afiliado reconocido, tipo de aplicacion de registro y primer browser. Se usa para probar el modelo predictivo.
5. **train_users_2**: dataset de 16 columnas con informacion de los regtistros como user ID, fecha de creacion del usuario, timestamp de actividad, fecha de la primera reserva, genero, edad, metodo de registro, flujo de registro, idioma, canal afiliado, proveedor afiliado, primer afiliado reconocido, tipo de aplicacion de registro, primer browser y pais de destino. 

El objetivo de todo el dataset es que el programador se dedique a disenyar y entrenar un modelo predictivo para lograr saber cual es el siguiente pais que visitara un usuario registrado.
