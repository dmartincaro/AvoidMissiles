EXPLICACIÓN SOBRE LA ESTRUCTURA Y FUNCIONAMIENTO DEL CÓDIGO.

Avoid Missiles se compone de 2 partes fundamentales: 
- Página web: dentro de la carpeta ProyectoWeb, en ella se generan los entrenamientos y se ven los resultados.
- Juego y Red neuronal: en la carpeta global, los archivos.Py "AvoidMissiles" y "Red".

Para ver la página web, solo hay que ejecutar cualquiera de los html (inicio o estadísticas). 
Para generar un entrenamiento, hay que poner los valores que se consideren, pulsar el botón de descarga justo bajo ellos. Se genera un archivo .json que hay que guardar en esta carpeta para utilziar esos ajustes.

Juego:
AvoidMissiles se desarrolla utilziando Pygame. 
En AvoidMissiles.py se define el juego.

En Red.Py se define la red. Necesita un entorno en el que esté instalado TensorFlow y tflearn.

Se incluyen unos ajustes de prueba.

Pasos para ejecutarlo:

1. Asegurarse que el archivo json del que cogen los datos tanto AvoidMissiles como Red tiene el mismo nombre del que aparece en el código (en este caso, 'prueba').

2. Si se quiere generar un entrenamiento con esos parámetros, dejar al final del texto activa la sentencia Red.start(). (Necesario para generar la primera base de datos)

3. Si se quiere correr un test sobre un entrenamiento ya realizado, dejar al final del texto activa la sentencia Red.test()

4. Para visualizar las partidas de juego cambiar los gui=False por gui=True en las líneas 95 (partidas de test) o 27 (partidas de entrenamiento).

5. Activar el entorno en el que se han instalado los paquetes de TensorFlow Tflearn y Pygame en el prompt de Anaconda.

6. Ejecutar la orden python Red.py.

Los gráficos se generan automáticamente, se deben guardar en la carpeta img, dentro de ProyectoWeb, para poder visualizarlas dentro de la página web al refrescar dicha ventana.
