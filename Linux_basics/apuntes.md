# Linux para principiantes

Para iniciar los que usamos windows debemos instalar WSL para poder emular ubunutu.

Sistemas operativos
    Que es?
        Es el software principal de un sistema informatico que gestiona todo los componentes del hadware.

    Cual es el proposito del software?
        Gestionar los recursos
    Como            interactuamos con el? 
        a traves de comandos e instrucciones.
    
    Qué SO existen?
        MS-DOS
        OS
        Windows
        Lunix (diferentes distros)
            dentro de estas una de las más utiñizadas ee Ubuntu
        MAC OS
        iOS
        Androit
    
    Unix y GNU/Linux

        UNIX
        Desarrollado en los 70's, en los laboratorios bell de AT&T. Fue unos delos primeros sistemas operativos multitarea
        Desarrollado por Dennis Ritchie y Ken Thomson

        GNU/Linux
        Nace en la decada de los 80's, desarrollado por Richard Stallman crea un sistema operativo que fuera libre con dependencia del usuario.
        Linux es un kernel creado en la decada de los 90's por Linus Torvalds y se integra con la parte de GNU

    Distribuciones de Linux
        Ubuntu
        Fedora
        Linux Mint
        Red Hat
        manjaro
        debian
        Garuda linux
        endevouros
        zorin
    
    Arquitectura lInux

        Tiene diferentes capas

        Hadware:
            Los componentes de una computadora
        
        Kernel:
        Utilidades de software que se comunican directamente con el hardware

        Shell (ksh, bash, csh, zsh)
            Programa que lee e interpreta las ordenes del usuario
        Utilidades:
            Aplicaciones especializadas

Configuracion de entorno de desarrollo
    Terminal
        si se cuenta con windows instalar WSL para poder emular el ambiente de linuxsin instalar el sistema operativo.
        
Qué es un comando?
    Es una instruccion que le va a decir a la computadora que hacer.

    actualizacion de paquertes
        Se utiliza para poder actualizar los paquetes que tenemos diponibles en la distribución

Comandos básicos de la terminal.
    - sudo Aptitude 
        (administrador de paquetes)
    - sudo 
        comando de super usuario para dar la instruccion como super usuario
    - sudo apt update
        Actualizar la lista de paquetes encontrados
    - sudo apt upgrade
        actualizacion de los paquetes instalados en la computadora    
    - man
        Hace referencia a un manual, con ello tenemos las instrucciones de como usar el comando.
        Nos muestra la descripcion, en que momento lo debemos usar, como utilizarlo.
        Sirve para validar como se utilizan los comandos
        Para salir de esta ventana pulsar la tecla 'q' y salimos de el
    - pwd
        Nos muestra la ruta en la que estamos posicionados en el momento de prom
    - clear
        Limpiar la pantalla de la teminal sin borrar el historial de comandos que generamos
    - flechas de direccion
        permite navegar en los comandos que hemos mandado a ejecutar
    - cd    
        change directory, cabiar de un directorio a otro (ver apartado de sistema de archivos)
    - ls
        listar los archivos en una forma corta (list short) de la ruta donde estamos parados, con ello vemos los documentos que tenemos en la carpeta donde estamos
    - ll
        listar los archivos en una forma larga (list large) de la ruta donde estamos parados, con ello vemos los documentos que tenemos en la carpeta donde estamos
        
    - history
        historial de comandos ocupados en la sesión de la terminal
    - clear history
        borra los comandos guardos en el historial de la terminal
    - mkdir
        crea un nuevo directorio, make directory
    - touch
        crea un archivo, nombre del archivo . extencion
    - nano
        Ver los archivos en la terminal para editarlos o leerlos. Tambien podemos crear un archivo con nano al igual que con touch
            nano nombreDelArchivo.extensión
    - vi
        Es otro visualizador de archivos
    - cat 
        Tiene varias funciones, una de las mas utilizadas es para ver el contenido del archivo en la consola
    - mv
        Mover y renombrar archivos
    - cp 
        copiar un archivo 

    

    
    Como funcionan los sitemas de archivos
        Todos los archivos que estan dentro de la maquina tienen un orden que siguen para irse guardando
        Esto es com un arbol que parte de la raiz, luego tenmos los directorios, las carpetas y los archivos que generamos 

        moverse en los directorios
            / ruta raiz
            . directorio actual
            .. directorio anterior
            ~ directorio home del usuario
            
            ejemplos de como movernos

                    cd documents/kodemia

                    si quiero regrear un nivel arriba tenemos que ir un nivel hacia atrás con ..

                    por ejemplo 
                        cd ..
                        regresamos a la ruta anterior
                    con ello podemos movernos en los archivos hacia adentro y hacia afuera del directorio

                Una vez que ya estamos parados en la carpeta podemos listar los archivos que no esten ocultos con el comando 
                    ls
                podemos complementar el comando con diferentes banderas
                    ls -l 
                        Nos permite listar los archivos en forma de linea no en forma de columna
                    ls  -a
                        Nos permite ver los permisos del archivo

                Como crear un directorio
                    Con el comando mkdir espacio y el nombre del directorio a crear.
                        mkdir newFolder
                    
                    Podemos crear una carpeta nueva dentro de newFolder con la ruta
                        mkdir newFolder/docs
                    
                    Con ello estamos creando la carpera docs en la carpeta new folder, tambien podemos entrar en la carpeta de newFolder y crear la carpeta docs
                
                Como crear un archivo
                    Con el comando touch  creamos los archivos, indicando el nombre del archivo . la extensión del mismo

                        touch holakoders.txt
                    De igual manera que mkdir podemos crear archivos  indicando la ruta en la queremos posicionar el archivo

                    Tambien lo podemos crear con nano

                        nano adiosKoders.txt
                
                Leer y editar un archivo
                    Podemos utilizar diferente herramientas disponibles para abrir y editar un archivo. Una de ellas es nano, indicando nano espacio nombre del archivo con la extension del mismo
                        ejemplo
                            nano holakoders.txt
                    para guardar el archivo modificado denbemos pulsar ctrl + w o ne su defecto ctrl + x y aceptar o denegar los cambios realizados
                
                Ver el contenido del archivo en consola
                    Para visualizar el contenido del archivo en la terminal
                    cat nombre del archvio

                    Para ver cuantas lineas tiene un archivo se utiliza
                        cal -n nombre del archivo.extension
                    
                    Para concatenar dos o más archivos con el comando cat se realiza de la siguiente manera
                        cat holakoders.txt adios.txt > archivos.txt
                    
                    con ello genera un nuevo archivo que fuciona el contenido de dos archivos y lo entrega en un archivo de salida, en este caso, con el nombre archivos.txt

                Mover un archivo de una ubicación a otra
                    con el comando mv nos permite mover y renombrar archivos.
                        ejemplo

                            mv holakoders.txt hola/
                        
                        Esto nos movera el archivo holakoders.txt a la carpeta hola
                    
                    Si queremos mover un archivo a un directorio mas afuera de la ruta donde me encuentro tenemos que indicar la ruta absoluta (es decir la ruta completa) del directorio  donde queremos posicionar el archivo
                    Tambien podemos hacerlo de la siguiente manera
                        mv saludos.txt ../
                    Esto hara que el archivo salga a el folder superior 

                Renombrar un archvio
                    Con el comando mv tambien podemos renombrar el archivo por ejemplo
                        mv archivoss.txt saludos
                    
                Copiar un archivo
                    Con el comando cp pedemos copiar un archivo sin modificar el archivo actual
                        ejemplo
                            cp saludos.txt saludocopia.txt
                    Este comando nos hará una copia del archivo en la misma ruta o directorio

                    Si queremos cambiar de carpeta destino indicamos lo siguiente
                        cp saludos.txt saludo/

                        Esto nos copiara el archivo saludos.txt a la carpeta saludo

                    tambien podemos salir un directorio arriba para copiar el  archivo con el comando
                        cp adioskoder.txt ../

                    para copiar una carpeta tenemos que hacer un proceso recusivo por que es un folder y tenemos que mover todos los archivos que tiene almacenados.

                        cp -r hola ../
                    
                    con el flat -r estamos indicando que es recursivo este proceso y asi podemos copiar la carperta hola un directorio arriba
                    



