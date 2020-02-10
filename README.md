# Curso De Datos Con Python

## Temario

Clase 1: Pandas I
objetos DataFrame, Series, Index, acceso por loc, iloc, query, between

Clase 2: Pandas II y estadística descriptiva
Groupby, agg, pivot_table, melt. Media, mediana, moda. Desvio estandar, varianza, deviacion absoluta media/mediana. Distribuciones: simetrica, asimetrica, uniforme, normal. Quantiles. Valores anomalos/outiers

Clase 3: Pandas III
fillna, lambda, apply, regex (esta es mezcla de la clase que dabamos de 'Limpieza de Datos' y de Data Wrangling), .str

Clase 4: Pandas IV
Joins y manejo de indices temporales y .dt, set_index

Clase 5: Visualización I
intro matplotlib y Plotly

Clase 6: Proyecto integrador
buscar alguna base interesante para analizar y graficar en clase.

Clase 7: Datos geograficos
Teoria de informacion geograficas y procesamiento de datos vectoriales con Geopandas

Clase 8: Visualización II
continuacion de Plotly, visualizacion de mapas con plotly, ejemplo con Dash?? 

Clase 9: Otras herramientas
Git para versionado de codigo y reporteria usando Jupyter. Tambien Docker? En esta clase tambien podrian ir definiendo el tp final

Clase 10: Introducción a la regresión lineal
Introducción a la regresión lineal. Definir programa

Clase 11: Proyecto final
Clase para trabajar en los proyectos.

Clase 12: Entrega de proyectos
Entrega de proyectos

## Antes de empezar:
Querés hacer este curso con Conda o instalando un entorno virtual desde pip?
Acá tenés los pasos fundamenteales para tomar una u otra decisión. Al respecto, debés saber que si bien conda es la opción más popular para crear entornos aislados en los que las librerías no entren en conflicto manteniendo o respetando versiones, muchos usuarios también optan por la creación de un entorno via pip para tener un trackeo más efectivo y claro de los paquetes que instalan.

Dentro del terminal de tu sistema operativo podemos seguir cualquiera de los caminos que más te guste.

1. Te recomendamos que dentro de tu directorio principal...

$ pwd 
  /users/alumno 

2. Crees una carpeta de cursos que nos sirva para alojar el nuestro, pongámosle...

$ mkdir cursos_python

3. Y desde ahí, clonemos el repositorio de nuestro curso haciendo

git clone https://github.com/CoDeArgentina/curso-python-data.git
* los usuarios de windows deben instalar git bash para windows (desde acá, https://gitforwindows.org/) previamente. Acá un instructivo de cómo hacerlo: https://www.techoism.com/how-to-install-git-bash-on-windows/

4. Ahora nos vamos a mover dentro de la carpeta de nuestro curso (o proyecto).
$ cd curso-python-data

Y desde allí podemos a) empezar a usar CONDA (la creación de un ambiente en conda puede tranquilamente preceder la creación de nuestro proyecto. Se puede, primero crear el ambiente y luego desde allí realizar los pasos anteriores) ó b) Crear un entorno virtual. 

Si optaste por la primera. Un entorno virtual en conda se crea de la siguiente manera:

CONDA
-----

01) conda create -n myenv python=3.6
02) conda activate myenv
03) conda install nb_conda
04) conda install jupyter
05) conda activate jupyter notebook
06) jupyter notebook
07) en el local host dirigirse a la carpeta del proyecto curso-python-data y abrir clase o notebook nuevo elegiendo el kernel con el nombre que le dimos a nuestro entorno y cliqueando en 'new'.

Si optaste por un entorno virtual, podés seguir por acá:

VIRTUAL ENVIRONMENT
-------------------

WARNING: Para simplificar, el siguiente grupo de instrucciones están escritas en bash (el interprete de comandos por defecto en GNU/LINUX). Si sos usuario de otro sistema operativo como windows, te recomendamos que simplemente busques los comandos equivalentes (googleando salen fácil!).

01) sudo apt-get install python-virtualenv ó
    (python -m pip install --user virtualenv)
...Dentro de la carpeta de nuestro proyecto curso-python-data
02) virtualenv --python=python3.6 myvenv ó 
    (python -m venv myenv - Acá no se especifica la versión de python!) 
03) source myenv/bin/activate
04) cd myenv
05) pip install ipykernel
06) ipython kernel install --user --name=python-data
07) jupyter notebook
08) en el local host dirigirse a la carpeta del proyecto curso-python-data y abrir clase o notebook nuevo elegiendo el kernel con el nombre 
    que le dimos a nuestro entorno y cliqueando en 'new'.


También podés seguir este tutorial: https://anbasile.github.io/programming/2017/06/25/jupyter-venv/.

