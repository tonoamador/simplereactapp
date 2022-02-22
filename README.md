# Despliege de una aplicación de React en AWS

## Prerrequisitos

[Tener una cuenta de GitHub](https://github.com/). Para descargar el código y hacer "fork" de la aplicación.

## Hacer Fork de la aplicación 

En este tutorial se ha omitido los pasos de descarga del código y creación de la aplicación en local, con fines prácticos y didacticos. Además, de aprovechar los beneficios de este servicio "AWS Amplify" que hara estos pasos por nosotros. 

1) Ir al repositorio de la aplicación: https://github.com/java-in-action/simplereactapp

2) Dentro de la página de GitHub, dar click en el botón Fork. De esta manera ustedes crearan una copia del proyecto dentro de su repositorio, que vamos a usar más adelante. 

![Hacer Fork de la aplicación](/img/fork_app.png)


### Desplegar la aplicación React en AWS Amplify

1) Iniciar sesión en [AWS Console](https://aws.amazon.com/es/)  
2) Buscar el servicio **AWS Amplify**  
![AWS Amplify>Todas las aplicaciones](/img/aws_amplify.jpg)  
3) Expandir el menú y dar clic en **Todas las aplicaciones**  
![AWS Amplify>Todas las aplicaciones](/img/todas_las_aplicaciones.jpg)  
4) clic en **Nueva aplicación>>Alojar aplicación web**  
![AWS Amplify>Todas las aplicaciones](/img/alojar_aplicacion.jpg)
5) Seleccionar la opción de **GitHub** y clic en **Continuar**  
![AWS Amplify>Todas las aplicaciones](/img/opcion_git_hub.jpg)  
6) Establecer y autorizar la conexión con el repositorio de GitHub  
    6.1) Clic en **Authorize aws-amplify-console**  
![Autorizar la conexión con GitHub](/img/git_autorizacion.png)  
    6.2) Introducir el **password** de su cuenta de GitHub  
7) Seleccionar el repositorio respectivo a su fork, ejemplo: mi-repositorio/**simplereactapp** 
![Seleccionar Repositorio](/img/seleccionar_repo.jpg)
8) Aceptar los valores por defecto y clic en **Siguiente**
9) Dar clic en **Guardar e implementar**
![Guardar e Implementar](/img/guardar_implementar.jpg)
Nota: El proceso tardara unos minutos. Esperar a que los siguientes pasos cambien verde: Aprovisionar, Compilar, Implementar y Verificar.  
Estado inicial:
![Paso inicial, aprovisionar](/img/paso_aprovisionar.jpg)  
Estafo final:
![Paso finar, verificar](/img/paso_fina_verificar.jpg)

10) Identificar la url donde se desplego la aplicación (caudro rojo) y abrirla, ejemplo: https://main.d2de214va3s2xg.amplifyapp.com/

### Lanzar el proceso de integración continua
1) Hacer la siguiente modificación en el archivo **src/App.js**, directamente en GitHub: Remplacen con su nombre el texto "Mi Nombre".

3) Ir a la consola de Amplify y observar el "Pipeline" la línea de producción.
4) Esperar que cada paso se complete (en verde) e refrescar la url de despliege Ej. https://main.d2de214va3s2xg.amplifyapp.com/, para comprobar que el cambio se ha desplegado correctamente.


## Conclusión
Este tutorial enseña como desplegar una aplicación de front-end hecha en react en un servicio de AWS Amplify. El reto esta en configurar el repositorio de gitHub con AWS Amplify. 

Lo interesante de este simple ejercicio, es entender como AWS nos ofrece un servicio que automatiza todo el proceso de despliege e integra un proveedor de repositorio de código (GitHub). 

### Referencias

[Download Node.Js](https://nodejs.org/en/download/)  
[Downloading and installing Node.js and npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
[Install Git](https://github.com/git-guides/install-git)  
[How to install Git Bash in Windows](https://www.educative.io/edpresso/how-to-install-git-bash-in-windows)  
[AWS Amplify](https://aws.amazon.com/es/amplify/)  
[What are the differences between npm and npx ?](https://www.geeksforgeeks.org/what-are-the-differences-between-npm-and-npx/#:~:text=NPX%3A%20The%20npx%20stands%20for,without%20even%20installing%20that%20package.)  
[Pushing changes to GitHub](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/making-changes-in-a-branch/pushing-changes-to-github)





