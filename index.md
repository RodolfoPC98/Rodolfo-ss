# <img src="image/logo-git.png" alt="Logo Git" width="40px"> Comandos útiles de Git y GitHub

Se debe de tener como requisito previo una cuenta en *[GitHub](https://github.com/)* y tener instalado *[Git](https://git-scm.com/download/win)*, así como un editor de texto que le resulte más cómodo. Una vez cumplidos los requerimientos se configurará el nombre y el correo del usuario con los siguientes comandos:

    git config --global user.name "Juan Perez"
    git config --global user.email tuemail@ejemplo.com

Una vez configurado los datos del usuario a continuación se mostrarán los comandos básicos para utilizar en cualquier proyecto: 

* Git **init**.

    Con este comando se inicia la sesión de git, se debe de iniciar por primera y única vez cuando no haz creado un directorio de **GIT**, una vez ejecutado se habrá cargado el **Working Directory** (directorio de trabajo), donde se creará una carpeta oculta llamada "*.git*" la cual llevará el control de los cambios del proyecto.

* Git **add**.

    Este comando tiene la función de subir los ficheros del **Working Directory** al **Staging Area** (área de ensayo).

* Git **status**.
    
    Con esta instrucción podremos ver el *estado* de los directorios guardados en el *Staging Area*, y los que aún se encuentran dentro del *Working Directory* sin guardar. A continuación, se mostrará un ejemplo, donde indicará en color verde los cambios que fueron guardados previamente con "git add", y con color rojo los cambios que aún no han sido guardados. 
    ![Ejemplo 1](image/ejemplo01.png)

* Git **commit**

    Aquí se añade para capturar los directorios y guardarlos en el **Repository**, una vez dada la orden se introducirá en el editor de texto, donde se digitará una pequeña descripción de los cambios hehos.
    ![Ejemplo 2](image/ejemplo02.png)
    Para salir del editor de texto, basta con presionar la tecla "Esc" y escribir ":wq" para salir del editor y guardar los cambios.
    ![Ejemplo 3](image/ejemplo03.png)
    Para verificar que los cambios se guardaron correctamente debe aparecer algo como lo siguiente:
    ![Ejemplo 4](image/ejemplo04.png)
    Una manera más sencilla de guardar las capturas en el *repository* es agregando la siguiente linea de código:

        git commit -m "Escriba aquí su mensaje"
    
    Donde "-m" indica que se va a escribir un mensaje; Se muestra en la consola de la siguiente manera:
    ![Ejemplo05](image/ejemplo05.png)

* Git **checkout**
    
    Es utilizado para  consultar o recuperar una línea existente dentro del *repository*.