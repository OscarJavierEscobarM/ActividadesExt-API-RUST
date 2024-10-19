# ActividadesExt-API-RUST

El objetivo principal de este repositorio es crear una API utilizando Rust para posteriormente con Docker crear una imagen y ejecutarla

la principal funcion de esta API es permitir al usurio registrar una actividad extraescolar la cual debera llevar la siguiente estructura:

![image](https://github.com/user-attachments/assets/ee31afc2-0db6-4904-8d19-1482287bcc0a)

el usuario podra realizar las siguientes acciones

GET actividad
http://localhost:8080/actividad

POST insertar-actividad
http://localhost:8080/insertar-actividad

GET actividad-id/{id}
http://localhost:8080/actividad-id/{id}

DELETE borrar-actividad/{id}
http://localhost:8080/borrar-actividad/{id}

se crea un Dockerfile para la aplicación

![image](https://github.com/user-attachments/assets/3313ef8e-8a00-4fac-9f77-b7a0d8a04d9e)

ahora utilizando Docker constuiremos una imagen de nuestra aplicación : docker build . -t actividades-api-rust

posteriormente la ejecutaremos con el siguiente comando : docker run -it -p 8080:8080 actividades-api-rust

con esto ya tendremos la aplicación ejecutandose en Docker

![image](https://github.com/user-attachments/assets/e0b94d5a-caf0-4ebb-8bc9-2a7425347819)

ahora realizaremos pruebas utilizando Postman
POST insertar-actividad
http://localhost:8080/insertar-actividad

![image](https://github.com/user-attachments/assets/3090b6ec-d5ca-4207-9378-814c175a0619)

![image](https://github.com/user-attachments/assets/83725a76-3171-4e93-9a5c-5bdbcc1a48d3)


GET actividad
http://localhost:8080/actividad

![image](https://github.com/user-attachments/assets/d6cfd413-4f9e-43d2-867c-eaea8d95590b)

GET actividad-id/{id}
http://localhost:8080/actividad-id/{id}

![image](https://github.com/user-attachments/assets/75a2f96b-b9a0-4cd0-8cd5-3955b3f403d2)


DELETE borrar-actividad/{id}
http://localhost:8080/borrar-actividad/{id}

![image](https://github.com/user-attachments/assets/a9d34ec1-4456-4824-959d-203ae7a06c66)

![image](https://github.com/user-attachments/assets/8299484f-7641-4d04-b959-d2f614909a97)

![image](https://github.com/user-attachments/assets/9e0375d3-15a8-448f-929d-68e649284f36)




