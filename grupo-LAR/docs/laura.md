# Instalación de MkDocs

MkDocs es una herramienta poderosa y simple para crear documentación estática a partir de archivos Markdown. Esta guía detalla cómo instalar MkDocs en **Debian** utilizando un entorno virtual de Python.
##  Actualización del sistema  
Actualiza los repositorios y paquetes del sistema para garantizar que trabajes con las versiones más recientes. 

![Update-Install](/imagenes/apt-get-install.PNG "Actualizar")

##  Instalación de Git  
Instala Git, que será necesario para gestionar proyectos de MkDocs y trabajar con repositorios.  
![Instalacion](/imagenes/apt-install-git.PNG "Instalacion")

##  Instalación de Python y pip  
Instala Python 3 y su administrador de paquetes pip, herramientas necesarias para manejar dependencias.  
![Instalacion](/imagenes/apt-install-python3.PNG "Instalacion")

![Instalacion](/imagenes/apt-install-python3-dev-python3-pip.PNG "Instalacion")

##  Instalación del módulo de entornos virtuales  
Configura el módulo que permite crear y gestionar entornos virtuales de Python.  

![Instalacion](/imagenes/apt-install-python3.11-venv.PNG "Instalacion")

## Creación de un entorno virtual  

### 5.1 Ubica tu carpeta personal  
Accede a tu directorio personal o a la ubicación deseada donde crearás el entorno virtual.  

### 5.2 Crea un entorno virtual  
Configura un entorno virtual de Python donde se instalarán las dependencias de MkDocs.  

![Crear](/imagenes/python3_-m_venv_my-env.PNG "Crear")


### 5.3 Activa el entorno virtual  
Activa el entorno para comenzar a instalar dependencias y trabajar en el entorno aislado.  

![Activar](/imagenes/source_my-env-bin-activate.PNG "Activar")



## Instalación de MkDocs  
Instala MkDocs dentro del entorno virtual para gestionar la documentación de tus proyectos.  

![Instalacion](/imagenes/pip3-install-mkdocs.PNG "Instalacion") 

## Verificaciones y comprobaciones  

### 7.1 Verifica las versiones de Python y pip  
Asegúrate de que Python y pip están correctamente configurados en tu entorno virtual.  

![Verificacion](/imagenes/python3--version.PNG "Verificacion") 

![Verificacion](/imagenes/pip3--version.PNG "Verificacion") 


### 7.2 Instala y verifica dependencias adicionales  
Prueba la instalación de bibliotecas complementarias y lista las dependencias instaladas.  

![Verificacion](/imagenes/pip3-install-requests.PNG "Verificacion") 

![Verificacion](/imagenes/pip3-list.PNG "Verificacion") 

![Verificacion](/imagenes/pip3-freeze.PNG "Verificacion") 

### 7.3 Verifica la instalación de MkDocs  
Comprueba que MkDocs está correctamente instalado verificando su versión.  

![Verificacion](/imagenes/mkdocs--version.PNG "Verificacion") 

## ¡Instalación completada!  
Ahora tienes MkDocs instalado y listo para usar. Puedes comenzar a crear tu proyecto y servir la documentación en un navegador.  




## Mkdocs 

## Creamos repositorio en Github
Entramos en gitHub y creamos un repositorio llamado Actividad22_3_LAR

![Repositorio](/imagenes/crear-repositorio.PNG "Repositorio") 

## Creamos grupo LAR

![LAR](/imagenes/mkdocs-grupo-lar.PNG "LAR")

## Configuramos el mkdocs.yml

![LAR](/imagenes/mkdocs-yml.PNG "LAR")

## Visualizar la pagina 
Visualizamos la pagina de mkdocs con el comando mkdocs serve -a y la ip del debian

![LAR](/imagenes/mkdocs-serve.PNG "LAR")