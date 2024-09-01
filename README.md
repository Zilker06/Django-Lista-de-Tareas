# Django-Lista-de-Tareas

Este proyecto es una aplicación de lista de tareas desarrollada con Django y Bootstrap 5.0.  
A continuación, encontrarás instrucciones para clonar el repositorio, instalar las dependencias y ejecutar la aplicación en tu entorno local.

**Requisitos**:
- [Visual Studio Code](https://code.visualstudio.com/Download)
- [Python](https://www.python.org/downloads/) (versión actualizada) 

**Instrucciones**
1. Clonar el Repositorio
Haz clic en el botón Code en la página del repositorio y selecciona Download ZIP.
Guarda el archivo en una ubicación accesible y descomprímelo. Deberías obtener una carpeta llamada Django-Lista-de-Tareas-main.  
2. Configurar el Entorno de Desarrollo
Abre Visual Studio Code.
Abre la carpeta del proyecto (Django-Lista-de-Tareas-main) presionando Ctrl + K, Ctrl + O y seleccionando la carpeta.
Si aparece un mensaje preguntando si confías en el autor, selecciona Sí.  
3. Crear y Activar un Entorno Virtual
Abre una terminal en Visual Studio Code presionando Ctrl + Ñ o desde el menú: Terminal -> New Terminal.

Asegúrate de que la terminal esté ubicada en la carpeta del proyecto (Django-Lista-de-Tareas-main).

Verifiquemos la version de python instalada 
```
python --version | py --version
```

Si aparece ahora crea un entorno virtual ejecutando el siguiente comando:
```
python -m venv venv | py -m venv venv
```
Ahora toca seleccionar el interpretador. Presiona F1 y escribe **Python Select Intrepreter** y selecciona la que diga recomendada o tenga una estrella.
Si Visual Studio Code no activa automáticamente el entorno virtual, actívalo manualmente con el siguiente comando:
```
./venv/Scripts/activate 
```
Si presenta errores usando esta linea, lo más comun es que ya tenga activado el entorno virtual sino deberías ver (venv) al comienzo de cada línea en la terminal, lo que indica que el entorno virtual está activo. Una vez activo, no tienes que volver a activar.

4. Instalar Dependencias
Con el entorno virtual activado, instala Django ejecutando:
```
pip install django
```
5. Migrar la Base de Datos
Crea las migraciones necesarias y aplica las migraciones a la base de datos ejecutando los siguientes comandos:
```
python manage.py makemigrations
```
```
python manage.py migrate
```
6. Ejecutar el Servidor
Inicia el servidor de desarrollo de Django con el siguiente comando:
```
python manage.py runserver
```
Abre tu navegador e ingresa la siguiente URL para acceder a la aplicación o has [click aqui](http://localhost:8000)
```
http://localhost:8000
```
¡Listo! Ahora deberías ver la página de inicio de la aplicación de lista de tareas.
