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
    - nano
        Ver los archivos en la terminal para editarlos o leerlos
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
        listar los archivos de la ruta donde estamos parados, con ello vemos los dicumentos que tenemosen la carpeta donde estamos
    - history
        historial de comandos ocupados en la sesión de la terminal
    - clear history
        borra los comandos guardos en el historial de la terminal

    
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




