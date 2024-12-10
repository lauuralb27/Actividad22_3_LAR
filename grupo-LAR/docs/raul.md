# Tutorial de PaperMod

## Paso 1 Configuracion del Hugo
Para empezar tendremos que ir a Visual Studio, donde podremos conectarnos a la maquina virtual en remoto por SSH, para poder trabajar mejor.

Luego tendremos que ir a un Terminal y crear uno nuevo ahi lo que haremos un

`wget https://github.com/gohugoio/hugo/releases/download/v0.135.0/hugo_0.135.0_linux-amd64.deb`

Con el podremos hacer que luego se instale el hugo con 

`apt install ./hugo_0.135.0_linux-amd64.deb`

Eso si haciendolo siempre dentro de root.

Luego de eso saldremos de root y crearemos un sitio con

`hugo new site Actividad22_2_LAR --format yaml `

Y aqui deberemos de hacer algo diferente ya que usaremos un estilo nuevo.

## Paso 2 Instalacion del estilo

Para ello deberemos de entrar con *cd* a sitio que acabamos de hacer y en su config.yml o como se llame ya que a veces se llama Hugo.yml, pero antes de hacer eso deberemos de hacer el siguiente comando:

`git init`

Para inicializarlo y luego haremos:

`git submodule add --depth=1 https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod`

Esto instalara el estilo, y con:

`git submodule update --init --recursive`

Esto se necesitara para reclonar los repositorios, ya que sin esto no se pueden clonar.

Y para terminar haremos un: 

`git submodule update --remote --merge`

## Paso 3 Configuracion del Sitio

Para configurar el sitio tendremos que ir al config.yml y dentro de este agregar una linea que seria:

`theme: ["PaperMod"]`

Asi se crearia el sitio con el estilo que queramos, en mi caso PaperMod.

Cada estilo tiene su propia Wiki para poder instalarlo correctamente, se recomienda que se vea.

## Paso 4 Crear un Post

Para crear un post tendremos que estar dentro del sitio (del directorio donde este) y hacer un:

`hugo new posts\NombrePost\index.md`

Haremos un markdown sencillito
(Para las imagenes es indicandolo con ./NombreImagen.png o .jpg, vamos el formato que tenga)

Una vez realizado, guardaremos con Ctrl+S y en el terminal haremos un:

`hugo server --bind "Ip_Maquina"`

Asi activamos el sitio, solo tendremos que ir a un navegador y ponere la ip y automaticamente deberia de enviar a la pagina.

# Paso 6 Pasarlo a Github

Para ello deberemos de ir a Github y crear un repositorio con el mismo nombre del sitio.

(Para no liarnos)

Cuando lo hagamos tendremos que copiar el link que nos sale e ir al Visual y hacer un 

`git remote origin https://nombreusuario:token@ruta_del_git`

Asi lo conectamos al repositorio y para ponerlo simplemente haremos un *git add*, *git commit -m "Comentario"* y un *git push -u origin master*.

Cuando lo hagamos vamos a GitHub y dentro del repositorio, vamos a Setting, Work and Pages y activamos el sitio de manera normal.

Si queremos podemos usar CloadFlare o Netify para que se visualice mejor.

---