  # Instrucciones
  
Hacer click en el enlace de Drive "https://short.gy/bK9spn" donde se encuentra compartido el archivo en formato .zip,   descomprimirlo en una carpeta y seguir las instrucciones correspondientes al sistema operativo que se este empelando.


## Para usuarios Ubuntu 18.04 o 20.04:

Abrir una consola, y ejecutar los siguientes comandos:

sudo apt update
sudo apt -y upgrade

Comprobar la instalación de Python3, escribir en la consola:  

python3 -V

Deberá obtener algo parecido a "Python 3.8.2" como respuesta.

Luego ejecutar:

sudo apt install -y python3-pip  
pip3 install numpy  
pip3 install  pandas  

Lo cual instalará Python 3 y las librerias necesarias para ejecutar el código.

Después descomprimir el archivo "CUN.zip"

Finalmente, abrir una consola en la ubicacion del archivo (o abrir un terminal desde la ubicacion del archivo empleando el boton derecho del raton), y ejecutar:

python3 GeneradordeMuestras.py


## Para usuarios Windows:

Descomprimir el archivo "CUN.zip". 

Ejecutar "Generador de Muestras.exe" simplemente hacer doble click sobre el mismo. 

Aviso: La interfaz puede tardar unos segundos en cargarse.


# Notas de la version

-La libreria de Numpy se ha actualizado, ahora se genera asi:

    rng = default_rng(z)
    number = rng.choice(len(ids), size=a.articles, replace=False)
Siendo z la semilla, la principal mejora es que ahora se puede elegir si se quiere con o sin repeticion la muestra generada.    
