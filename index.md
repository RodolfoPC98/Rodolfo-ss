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

* Git **commit**.

    Aquí se añade para capturar los directorios y guardarlos en el **Repository**, una vez dada la orden se introducirá en el editor de texto, donde se digitará una pequeña descripción de los cambios hehos.

    ![Ejemplo 2](image/ejemplo02.png)

    Para salir del editor de texto, basta con presionar la tecla "Esc" y escribir ":wq" para salir del editor y guardar los cambios.

    ![Ejemplo 3](image/ejemplo03.png)

    Para verificar que los cambios se guardaron correctamente debe aparecer algo como lo siguiente:

    ![Ejemplo 4](image/ejemplo04.png)

    Una manera más sencilla de guardar las capturas en el *repository* es agregando la siguiente linea de código:

        git commit -m "Escriba aquí su mensaje"
    
    Donde "-m" indica que se va a escribir un mensaje; Se muestra en la consola de la siguiente manera:

    ![Ejemplo 5](image/ejemplo05.png)

    Para guardar la captura de manera más rápida se digita la instrucción "-am" de la siguiente manera:

    ![Ejemplo 17](image/ejemplo17.png)

* Git **log**.
    
    Muestra el historial cronológico de confimación de un repositorio. Tal como se muestra en la imagen de abajo:
    
    ![Ejemplo 6](image/ejemplo06.png)

* Git **checkout**
    
    Es utilizado para  consultar o recuperar una línea existente dentro del *repository*. En el siguiente ejemplo se revertirá los cambios de un archivo en el cual se agrego un título al archivo "index.html".
    
    ![Ejemplo 7](image/ejemplo07.png)

    Aparentemente en la consola no pasa nada, pero recupera el archivo guardado en el repositorio. Incluso si es eliminado del *Working directory*.
    
* Git **Branch**.

    Si se digita este comando nos mostrará las ramas que existen dentro del proyecto.

    ![Ejemplo 8](image/ejemplo08.png)

    Si se desea agregar alguna nueva rama se debe realizar de la siguiente manera:

    ![Ejemplo 9](image/ejemplo09.png)

    Y ahora si volvemos a mostrar las ramas existentes, deberá aparecer la nueva versión que acabamos de crear.

    ![Ejemplo 10](image/ejemplo10.png)

    Nota: para cambiar de rama, se debe escribir el comando "git checkout" y a continuación el nombre de la rama a la que se desea cambiar.

* Git **remote**.

    Conecta un repositorio local con un repositorio remoto. En este caso se creará un nuevo repositorio en *GitHub* y se copiará lo seleccionado de la siguente captura.

    ![Ejemplo 11](image/ejemplo11.png)

    Se ejecuta en la consola.

    ![Ejemplo 12](image/ejemplo12.png)

    Y con ello, tendremos conectado nuestro repositorio a *GitHub*.

* Git **push**.

    Envía *commits* locales al repositorio remoto. Requiere dos parámetros: el repositorio remoto y la rama para la que es el push.

    ![Ejemplo 13](image/ejemplo13.png)

    Una vez ejecutado el comando nos mostrará un *login* para conectar el repositorio local a *GitHub*.

    ![Ejemplo 14](image/ejemplo14.png)

    Se usará el navegador predeterminado para iniciar la sesión, y se le concederá los permisos necesarios.

    ![Ejemplo 15](image/ejemplo15.png)

    Y se mostrará en la consola de la siguiente manera para corroborar que se guardo correctamente.

    ![Ejemplo 16](image/ejemplo16.png)

* Git **clone**.

    Crea una copia de trabajo local de un repositorio remoto existente, se usa git clone para copiar y descargar el repositorio a una computadora.
    En nuestra cuenta de *GitHub* se copiará el link del proyecto que deseamos clonar.

    ![Ejemplo 18](image/ejemplo18.png)

    Se escribe el comando "git clone" seguido de la dirección copiada.

    ![Ejemplo 19](image/ejemplo19.png)
    
    Podemos ver que efectivamente se clono, y ya se encuentra de nuevo en el equipo.