# info de la materia: st0263-242
#
# Estudiante(s): Andrés Felipe Téllez Rodríguez, aftellezr@eafit.edu.co
#
# Profesor: EDWIN NELSON MONTOYA MUNERA, emontoya@eafit.edu.co

# Aplicación Monolítica con Balanceo y Datos Distribuidos (BD y archivos) Kubernetes
#
# 1. breve descripción de la actividad
#
En el reto 2 – parte 1, se desplegó una versión dockerizada de un CMS o LMS, con un
balanceador simple de cargas, sin autoescalamiento y con integración de la base de datos y
el sistema de archivos distribuido.
En este reto 2 parte 2, uds desplegarán la misma aplicación del reto 2 parte 1, pero en un
clúster Kubernetes en nube. Se utilizará un servicio administrado en nube como EKS de AWS
o Kubernets de GCP
## 1.1. Que aspectos cumplió o desarrolló de la actividad propuesta por el profesor (requerimientos funcionales y no funcionales)
Lo que se cumplio fue tanto el desplegado de moodle con el sistema NFS, conexion al cluster EKS, y uso de una instancia de bases de datos.
## 1.2. Que aspectos NO cumplió o desarrolló de la actividad propuesta por el profesor (requerimientos funcionales y no funcionales)
Lo que desafortunadamente no se desarrollo fue tanto el balanceador de cargas, como el nombre de dominio, y Certificado SSL

# 3. Descripción del ambiente de desarrollo y técnico

Para desarrollarlo se baso en el primer reto lo que implica las instancias de EC2 donde se abre los puertos de aurora/Mysql, Ademas de el puerto 80, 443, los 700 y 7001 de TCP para el balanceador
Ademas de que se necesita para el cluster el CLI de aws y configurarlo ademas de kubectl (este lo puedes manejar si es necesario en docker) y si es necesario para mayor facilidad se usa Helm


 
![image](https://github.com/user-attachments/assets/11fc4f59-8c22-4c18-85dc-671111a43589)
![image](https://github.com/user-attachments/assets/c5cdd129-b1bf-469d-8cbb-d48d848f9ad8)
![image](https://github.com/user-attachments/assets/88bdce85-8c31-40f1-81ad-0fc64b0c5ae1)


# 4. Descripción del ambiente de EJECUCIÓN 
Idealmente cuando funciona simplemente se entra al dominio donde envia a uno de las dos instancias.
Lo que sucede es que necesito ingresar a la ip de cada instancia para poder ingresar a la pagina, seguido de un /moodle para que ingrese a la pagina.
Por detras es que se entran y salen los datos a la base de datos, y la instancia Nfs ayuda a centralizar los datos. Por su parte a pesar de que debido a los parametros no se usa al 100% el cluster este esta enfocado a ayudar a la escalabilidad y la disponibilidad ademas de otros lo que permite que sea mas estable el archivo


## opcionalmente - si quiere mostrar resultados o pantallazos 
![image](https://github.com/user-attachments/assets/a0680575-6431-4f9b-ad9d-dffc6dbe7ee9)
![image](https://github.com/user-attachments/assets/3124eb1e-b391-4394-a805-044f3379e6b9)


# 5. otra información que considere relevante para esta actividad.

# referencias:
## [sitio1-url ](https://www.youtube.com/watch?v=z3uzxUez8rw&list=PLkqaOL-oB94HAIRkA_5qdqk-x-1Hgo4i2&index=1)
## [sitio2-url](https://www.youtube.com/watch?v=DCoBcpOA7W4)
## [sitio1-url ](https://www.youtube.com/watch?v=_2otJP0xmfs)
## [sitio1-url](https://www.youtube.com/watch?v=lNm61mN67DQ)
## [sitio1-url](https://www.youtube.com/watch?v=xJ7BKnZbwCU)
## [sitio1-url](https://www.youtube.com/watch?v=AOmw6pl7iWk)
## sitio1-url
## sitio1-url
## sitio1-url
## sitio1-url
## sitio1-url
## sitio1-url
