# Despliege de una aplicación de REACT en AWS

aaa

## Prerrequisitos

[Descargar e instalar Node.J](https://nodejs.org/en/download/)  
Tener instaldo NPM arriba de su versión 5.2.0

[Instalar Git en la máquina local](https://github.com/git-guides/install-git). Se tiene que tener instalado Git. Se recomienda instalar una consola de comandos como [Git Bash](https://www.educative.io/edpresso/how-to-install-git-bash-in-windows)

[Tener una cuenta de GitHub](https://github.com/). Para descargar el código del ejemplo se necesita tener una cuenta en GitHub.


## Crear una aplicación REACT - Hello World

En la consola de comandos, ejecutar el siguiente comando. El proceso tardará unos minutos en descargar e instalar todo lo necesario.

`npx create-react-app simplereactapp`

## Ejecutar la aplicación 

Ir al directorio simplereactapp:

`cd simplereactapp`

Correr la aplicación con el siguiente comando:

`npm start`

Enseguida se abrirá tú navegador en el siguiente link (host):  
[http://localhost:3000/](http://localhost:3000/)

![Aplicación React Desplegada Correctamente](/img/reac_app_desplegada.png)

## Subir la aplicación a GitHub

Se recomienda subir el código creado en el paso anterior a su GitHub para poder integrarlo con el servicio de AWS, en el paso siguiente. El alcance de este tutorial no cubré la explicación de como subir el código al repositorio.

En caso de que se queira omitir este paso, se puede utilizar el siguiente url: 
https://github.com/java-in-action/simplereactapp.git en el siguiente paso.

Nota: Git dejó de usar password recientemente para subir cambios, es muy probable que tengas que crear un Personal AccessToken para subir tus cambios. Esta opción se encuentra en Configuración o Settings > Developer settings > Personal Access Token.


### Desplegar la aplicación React en AWS Amplify

1) Iniciar sesión en [AWS Console](https://aws.amazon.com/es/)
2) Buscar el servicio **AWS Amplify**
3) En la sección de Amplify Hosting, clic en **Introducción**
4) Seleccionamos la opción de **GitHub**
   Nota: La consola de Amplify requiere acceso de solo lectura al repositorio.
5) Clic en el botón **Continuar**
6) Clic en **Implementar aplicación**
7) Clic en **Conectarse a GitHub**
8) Clic en **Authorize aws-amplify-console**
    Nota: Se solicitarán las credenciales (el usuario y/o password) para continuar.
9) Crear **rol de servicio**, clic en **Crear un nuevo rol**
    9.1) Dejar seleccionado **Servicio de AWS**
    9.2) En el catálogo Casos de uso para otros servicios de AWS buscar y seleccionar  **Amplify**
    9.3) Seleccionar la opción **Amplify - Backend Deployment** y click en **Siguiente**
    9.4) Aceptar los valores por default y dar un nombre al rol, como: **AmplifyConsoleServiceRole-AmplifyRole**
10) Regresar a la pantalla de Implementación de la aplicación y dar clic en **Actualizar Roles Existente**
11) Seleccionar el rol creado y dar clic en **Guardar e Implementar**




   

 Dejar los valores por defecto y dar clic en **Guardar e implementar**




