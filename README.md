
# 🏘️ Homie 

Homie is an app focused on the search of living places for rent globally.
You can find the possibility of filtering these places by city, condition, category or bedrooms.

## 🖥️ technologies
React, MongoDB, Express, Node, Postman.
Some libraries like Mongoose, Axios, Bootstrap, AntDesign were also used during this process of 2 hard weeks of work at Ironhack Madrid.

### Endpoints

| Method   | Auth               | Route                             |   Description  |
| :---     |   :---:            |          ---:                     |           ---: |
| POST     |  Public            | ‘/signup’                         |  Mandar datos Registro                                |
| POST     |  Public            | ‘/login’                          |  Mandar datos de inicio de sesion|
| GET      |  Is authenticated  | ‘/logout’                         |  Cerrar sesion|
| GET      |  Is authenticated  | ‘/account:id’                     |  Obtener datos de cuenta de usuario logueado|
| PATCH    |  Is authenticated  | ‘/account/:id/edit’               |  Mandar datos para editar cuenta de usuario logueado|
| GET      |  Public            | ‘/living-places?city=Madrid’      |  Obtener listado de viviendas|
| POST     |  Is authenticated  | ‘/living-places/create’           |  Mandar datos para crear vivienda|
| GET      |  Public            | ‘/living-places/:id’              |  Obtener datos de detalle vivienda|
| PATCH    |  Is Owner          | ‘/living-places/:id’         |  Mandar datos para editar vivienda|
| DELETE   |  Is Owner          | ‘/living-places/:id’              |  Borrar de la base de datos una vivienda|
|POST      |  Public            | ‘/living-places/:id/message’      |  Formulario de contacto|


#### Screenshots


![homie-screenshot1](https://user-images.githubusercontent.com/95500908/159767471-448591d1-aec2-45d3-8d64-b19765540aa2.jpg)
![homie-screenshot2](https://user-images.githubusercontent.com/95500908/159767491-bdae3414-85c9-4972-9c14-4695d3399fb1.jpg)
![homie-screenshot3](https://user-images.githubusercontent.com/95500908/159767929-fe6138cd-e3ee-4ebe-a4d5-99347f228a1a.jpg)
![homie-screenshot4](https://user-images.githubusercontent.com/95500908/159767938-28ea0783-1600-42e7-b042-3773242e6195.jpg)


##### Server .env variables needed
```
ORIGIN=http://localhost:3000
PORT=5005
DB_REMOTE
SESS_SECRET
CLOUDINARY_NAME
CLOUDINARY_KEY
CLOUDINARY_SECRET
NODEMAILER_NAME
NODEMAILER_KEY
NODEMAILER_SECRET
```

