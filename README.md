# Guía para Configurar Kubernetes con MySQL y WordPress:
 
### Estudiante(s): 

nombres: - Andres Guerra MOntoya, - Juan Esteban Cardona, - Carlos Andres Mosquera.

### Profesor: Edwin Nelson Montoya.

# 1. breve descripción de la actividad:
En esta actividad, se ha proporcionado una guía detallada para configurar un entorno de Kubernetes con dos aplicaciones esenciales: MySQL y WordPress. Los pasos abordados fueron:

- Instalación y configuración de microk8s y kubectl.
- Creación de un secreto en Kubernetes para la contraseña de root de MySQL.
- Configuración de almacenamiento persistente para MySQL y WordPress.
- Despliegue de MySQL en Kubernetes.
- Creación de un servicio para MySQL.
- Despliegue de WordPress en Kubernetes.
- Creación de un servicio de WordPress con un balanceador de carga.
  
## 1.1. Que aspectos cumplió o desarrolló de la actividad propuesta por el profesor (requerimientos funcionales y no funcionales)

- Instalación de Software: Configuramos microk8s y kubectl en el sistema para gestionar el clúster de Kubernetes.
- Creación de Secretos: Creamos el secreto y la copntrasena hasheada.
- Almacenamiento Persistente: Debe ser posible configurar y aplicar el almacenamiento persistente en Kubernetes para las aplicaciones MySQL y WordPress.
- Despliegue de MySQL: pudimos desplegar una instancia de MySQL en el clúster de Kubernetes.
- Balanceador de cargas: Pudimos aplicar el balanceador de cargas para el kluster de kubernetes.

 ![WhatsApp Image 2023-10-24 at 10 02 22 PM](https://github.com/Guerrita/Reto-4-st0263-232/assets/105470955/ea585a0b-bbd7-4e78-9da4-47a58d900dc7)

 
 ![WhatsApp Image 2023-10-24 at 10 03 49 PM](https://github.com/Guerrita/Reto-4-st0263-232/assets/105470955/163a6533-52b0-4075-bf4c-d515ff03b2c1)



## 1.2. Que aspectos NO cumplió o desarrolló de la actividad propuesta por el profesor (requerimientos funcionales y no funcionales)

- Despliegue en Wordpress: Tuvimos problemas con la coexion de la base de datos al despliegue de wordpress.
- No se tiene nombre de dominio ni certificado SSL.

![WhatsApp Image 2023-10-24 at 10 04 14 PM](https://github.com/Guerrita/Reto-4-st0263-232/assets/105470955/2d132175-b8d0-43f8-9bca-8ad0bade1599)


![WhatsApp Image 2023-10-24 at 10 04 41 PM](https://github.com/Guerrita/Reto-4-st0263-232/assets/105470955/237ac935-6b87-404e-9117-2bf84300c52d)


# 2. información general de diseño de alto nivel, arquitectura, patrones, mejores prácticas utilizadas.

- La arquitectura se basa en microservicios y sigue el modelo cliente-servidor:

- MySQL: Se despliega como un contenedor que ejecuta un servidor MySQL.

- WordPress: Se despliega como otro contenedor que contiene la aplicación WordPress. Este contenedor se comunica con el servidor MySQL para almacenar y recuperar datos.

- Balanceador de Carga: El servicio de WordPress se expone externamente utilizando un balanceador de carga. Para el uso de la IP Externa.

# 3. Descripción del ambiente de desarrollo y técnico: lenguaje de programación, librerias, paquetes, etc, con sus numeros de versiones.

- Kubernetes.
- Docker.
- KubeCtl.
- MicroK8s.

# 4. Descripción del ambiente de EJECUCIÓN (en producción) lenguaje de programación, librerias, paquetes, etc, con sus numeros de versiones.

Comandos usados de a cuerdo a la guia que dearrollamos:

[https://docs.google.com/document/d/1IzgpjLHFNoqKKWUEz5LVZOwIaq70W4_FY4l8Tedyu4E/edit](https://docs.google.com/document/d/1IzgpjLHFNoqKKWUEz5LVZOwIaq70W4_FY4l8Tedyu4E/edit?usp=sharing)

# referencias:

- MicroK8s: [https://microk8s.io/#get-started](https://microk8s.io/docs/high-availability)https://microk8s.io/docs/high-availability
- Guia Alterna: https://engr-syedusmanahmad.medium.com/wordpress-on-kubernetes-cluster-step-by-step-guide-749cb53e27c7
- Guia Alterna: https://www.cloudsigma.com/how-to-deploy-wordpress-with-persistent-volume-on-kubernetes-cluster/
- Video de apoyo: https://www.youtube.com/watch?v=e_MAZGeosSw
