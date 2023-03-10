# Linux para principiantes

Para iniciar los que usamos windows debemos instalar WSL para poder emular ubunutu.

Sistemas operativos

    Que es?
        Es el software principal de un sistema informatico que gestiona todo los componentes del hadware.

    Cual es el proposito del software?
        Gestionar los recursos

    Como interactuamos con el? 
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

    - grep
        Nos busca patrones de contenido en un archivo. Hace un patro de busqueda dentro de una ruta. Con grep podemos generar un filtro
    

    

    
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
                    
                Borrar un archivo

                    Con el archivo rm borramos un archivo o una carpeta. Para un archivo se hace de la siguiente manera

                        rm archivo.txt

                    Para un folder tenemos que indicarle que se haga de manera recursiva, es decir 

                        rm -r proyetos
                        
                        o

                        rm dir para eliminar el directorio

                    Para generar folders con rutas profundas por ejemplo una ruta de un proyecto básico los comandos se pueden agrupar para generar el folder
                        
                        ejemplo

                                mkdir miProyectoWeb && cd miProyectoWeb && mkdir css js && touch index.html css/style.css js/script.js
                
                Como generar un alias 

                    Un alias dentro de la terminal nos permite ahorrarnos lineas de codigos para ejecutar tareas repetitivas con un acotamiento de palabras clave en lugar de tener toda la instrucción 

                    Para generar un alias tenemos que entrar al archivo de configuracion del shell en la que estamos corriendo por ejemplo zsh, el cual tiene un archivo .zshrc.
                    En el archivo zshrc tenemos que denotar el alias nombre_del_alias="comando"

                        por ejemplo

                            alias borrar="clear"

                    si declaramos estos alias en la terminal serán alias temporales si en caso queremos que el alias perdure para simpre lo tenemos que crear directamente en el archivo de configuración 

                Para borrar un alias temporal podemos aplicar el comando
                
                    unalias nombreDelAlias

                Ver el historial del shell

                    Con el comando history vemos los comandos usados ademas podemos limitar el scope de history que necesitamos obtener
                        
                        history 10 nos mostrara el historial desde el comando guardoda en la posicion 10
                    
                    Con history | tail -n 5 
                        Nos muestra los ultimos 5 comandos usados en la shell
                    
                    Con history | head
                        Vemos los primeros 10 comandos utilizados en nuestra terminal
                    
            Como buscar un archivo

                Con el archivo find vamos ha haer la busqueda. Para ahcer una busqueda por el nombre del archivo en la carpeta donde estamos tenemos que usar lo siguiente

                    find . -name saludos.txt

                Para buscar el archivo en el equipo tenemos que indicar la ruta de todo el home 

                    find ~ -name saludos.txt
                
                Otro tipo de busqueda desde la raiz del archivo en todo el equipo tenemos que  indicar el comando con  la diagonal

                    find / -name saludos.txt
            
                Para buscar un archivo que sabemos el nombre y discriminar el hecho de que sean minusculas o mayusculas tenemos que indicar

                    find .iname HoLa.txt

                Para encontrar un archivo filtrando los archivos por la extension del archivo
                    
                    find -name "*".txt o find -name '*.txt'

            Patrones de busqueda 
                Para generar un filtro de busqueda podemos usar el comando grep 
                Por ejemplo 

                        grep Binevenido proyectoHtml/index.html
                
                Esto ira a buscar la palabra Bienvenido en la direccion proyectoHtml en el archivo index.html


                podemos indicar con una bandera los terminos stric que tenemos en el archivo

                    grep -F bienvenido proyectoHtml/index.html

                        Con -F nos forsa a encontrar el la palabra bienvenido con minusculas 
                    
                    grep -i bienvenido proyectoHtml/index.html

                            Con -i indicamos que ignore las coincidencias exactas, ignora si son mayuculas o minusculas

            Usar variables en la linea de comandos

                Con la palabra export
                    
                    ejemplo

                        export SALUDO=hola

                Imprimir en la linea de comandos

                    Para imprimir el contenido de una variable guardad usamos la palabra ecHo

                        ejemplo

                            echo "$SALUDO"

                Qué hay de guardar la variable en un archivo

                    Utilizamos echo de la siguiente manera

                            echo "Hola mi nombre es $NONBRE" >> saludoAMi.txt

                    Aca el saludo se esta guardando el archivo saludoAMi.txt incluyendo la variable que hemos guardado en export

                Como Borro una variable utilizada  

                    Con el comando unset, ejemplo

                            unset SALUDO

                    Con esto estamos borrando la variable SALUDO

            Permisos otorgados a los archivos

                Esto funciona para gestionar que tipos de permiso tienen los archivos a el usuario que los esta accesando en la sesión. Los permisos pueden ser de lectura, escritura, edición, etc.
                Con el comando ll podemos ver el listado de los archivos con los permisos que este tiene para poder  accederlo

                    chmod u+x  <archivo>

                        Aca estamos indicando que al archivo le estamos dando los permisos de ejecucion al usuario del archivo seleccionado
                    
                    chmod u-x <arcjivo>

                        Aca estamos indicando que le estamos quitando el permiso de ejecucion  al usuario en curso de ese archivo
                    
                Los grupos de permisos se dividen en 3 grupos
                    
                    '---''---''---'

                    El primer bloque pertenece a el usuario.
                    El segundo bloque pertenece a el usuario.
                    El tercer bloque pertenece a el grupo.


                Existe otro sistema donde se pueden asignar permisos desde el sistema octal, el numero 7 significa que tiene todos los permisos activos ejemplo

                Con el comando chown

                    Con este comando podemos cambiar a quien le pertenece el archivo que estamos manipulando
            
            Utilidades de red
                Son herremiantas de linea para validar el estado de una red en un sitema operativo.
                
                Comando TOP
                    Muestra informacion de los procesos actuales
                    ejemplo

                        top

                    Esto nos muestra los PID que se estan ejecutando, el procesador utilizado por el proceso, puerto donde se esta esuchando el proceso
                    Para salir de esta pantalla debemos pulsar

                        'ctrl' + 'C'
                
                    top -U manuel
                        Nos hace un filtro de los procesos por user
                
                Comando pin
                    Con el comando pin verivicamos si el puerto esta ecuchando para saber si tenemos conexion con una dirección o un puerto

                        pin google.com
                    
                    Cuando estamos trabajando con servidores muchas veces no tenemos conexion a internet entonces hacemos un pin a una dirección para ver su respuesta

                        pin 127.243.45.2

                    Con esta instruccion mandamos un request para saber si la direccion esta escuchando

                Comando ifconfig

                    Nos da informacion de la red en la que estamos conectados, información sobre el puerto al que estan conectados las antenas, etc
            
            Operadores de control

                Nosotros podemos ejecutar varias instrucciones en la terminal con los operadores de control. 
                Estos operadores nos sirven para hacer mas rapida la ejecucion de los comandos en la terminal

                    operador; 
                        ejecuta los comandos de manera consecutiva
                    
                    operador &&
                        ejecuta el segundo comando si y solo si la la instruccion anterior se ejecuto de manera satisfactoria
                        ejemplo
                            
                            mkdir koder && touch koder/elvira.txt

                        Si cumple la primera condicion se ejecuta la segunda

                    operador ||
                        ejecuta el segundo comando aunque el primero no se ejecute
                        ejemplo

                            madir koder.txt || archivo txt




                 

                


                


                
                   



