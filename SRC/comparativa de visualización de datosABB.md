# Codigo para visualización de datos del sistema ABB CMS-700
En el siguiente código describe la visualización de un archivo descargado directamente de la plataforma de usuario del sistema ABB CMS-700, el cual como tiene finalidad, reordenar el formato del archivo descargado, debido a que el formato del archivo se tiene por formato predeterminado la extensión .CSV.

Por lo tanto al importar el archivo al bloque de programación "jupyter notebook" e importar la libreria "pandas", la cual ayuda a la visualización de los datos requeridos con base al periodo solicitado ..

Es decir, que si se solicita la descarga de datos correspondientes al día. El código de programación ordenará el archivo .CSV de manera que entregue los datos de consumo correspondientes de la L1, L2 y L3 en unidades de (Wh).

A continuación se muestra el código correspondiente.

importamos la libreria "pandas" misma que ayudará a la visualización de datos

importar pandas como pd

posteriormente se define el nombre del archivo correspondiente a la descarga de datos y de la misma forma se define que tipo de separaciones contiene el archivo descargado desde la plataforma de usurio ABB CMS-700

df = pd.read_csv ('ejemplo.csv', sep = ";", index_col = 0)

Con lo aterior se logra la visualización de los consumos correspondientes a las 3 líneas del sistema. A continuación se muestra lo pasos para lograr la visualización gráfica de los consumos de dichas líneas de alimentación.

importar matplotlib.pyplot como plt

importa la libreria "matplotib" la cual ofrece diferentes beneficios, entre las diferentes herramientas que contiene u ofrece, está la graficar, que en este caso graficará los consumos mencionados anteriormente.

encuestas = pd.read_csv ("datos / encuestas.csv")

Posteriormente a importar la libreria "matplotlib, se importa de la misma manera una vez mas la libreria "pandas".

finalmente se desigan los ejes "X y Y" es decir, se le asigna un valor de los visualizados para cada eje y asi observar la grafica correspondiente.

plt.show () # graficamos los datos

A continuación se muestra la grafica referente a da descarga de datos mediante un archivo .CSV.

De la misma forma se realiza la modificación de los archivos. csv para visualizar los datos historicos de medición desde la ultima conexión y puesta en servicio del sistema ABB. A continuación se muestran las grficas correspondientes a los parametros eléctricos de la instalación.

###### Potencia Reactiva.
![](https://github.com/LEANA14/SISTEMA-ABB/blob/main/Imagenes/potenciareactivagrafica.PNG?raw=true)

###### Potencia Aparente.
![](https://github.com/LEANA14/SISTEMA-ABB/blob/main/Imagenes/POTENCIAAPARENTEGRAFICA.PNG?raw=true)

###### Potencia Activa.
![](https://github.com/LEANA14/SISTEMA-ABB/blob/main/Imagenes/POTENCIAACTIVAGRAFICA.PNG?raw=true)

###### Factor de Potencia.
![](https://github.com/LEANA14/SISTEMA-ABB/blob/main/Imagenes/FACTORDEPOTENCIAGRAFICA.PNG?raw=true)

###### Voltaje
![](https://github.com/LEANA14/SISTEMA-ABB/blob/main/Imagenes/GRAFICA%20VOLTAJE%202.PNG?raw=true)

###### Corriente.
![](https://github.com/LEANA14/SISTEMA-ABB/blob/main/Imagenes/corrientegrafica.PNG?raw=true)



