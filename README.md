![Proyecto Django](/src/djangoproject.gif)

# COMO EMPEZAR CON DJANGO

1. Instalar Python, pueden descargarlo de este enlace ![python.org](https://www.python.org/).
2. Instalar Django, para descargarlo pueden ir a este enlace ![djangoproject.com](https://www.djangoproject.com/download/).
3. Crear un directorio, en la terminal ir a ese directorio y crear el proyecto con django.
   ```
   django-admin startproject [nombre_del_proyecto]
   ```

## ¿QUÉ ES DJANGO?

Django es un framework o marco de trabajo desarrollado en Python que nos da las herramientas y librerías para crear aplicaciones web.

Cuál es el patrón de arquitectura de Django? Es el MTV o Model Template View, que es una variante del modelo MVC o Model View Controller. Expliquemos un poco:

1. Modelo (Model): Es la capa que maneja la lógica de acceso a los datos. Define la estructura de la base de datos y las relaciones entre los datos. En Django, los modelos son clases que heredan de django.db.models.Model.
   
   ```
   from django.db import models

   class Blog(models.Model):
      title = models.CharField(max_length=200)
      description = models.TextField()
      date = models.DateTimeField()
   ```

2. Vista (View): Es la capa que maneja la lógica de presentación. Recibe las solicitudes web y devuelve las respuestas. Las vistas pueden ser funciones o clases en Python.

   ```
   from django.http import HttpResponse
   from django.shortcuts import render

   def hello_world(request):
      return HttpResponse("Hello, World!")
   ```

3. Plantilla (Template): Es la capa que maneja la lógica de presentación. Define cómo se muestran los datos en la interfaz de usuario. Django utiliza un lenguaje de plantillas que permite incrustar variables y lógica de control en el HTML.

   ```
   <h1>{{ title }}</h1>
   <p>{{ content }}</p>
   ```

## Proyecto Django

Este es el proyecto Django que estoy realizando con el video de Fazt.

Django es un framework de desarrolloWeb que ahorra tiempo y hace que el desarrollo Web sea divertido. Utilizando Django puedes crear y mantener aplicacionesWeb de alta calidad con un
mínimo esfuerzo.

Primero, explicamos en profundidad lo que hace Django, y cómo crear aplicaciones Web con él. Segundo, discutiremos conceptos de alto nivel cuando se considere apropiado, contestando la pregunta “¿Cómo puedo aplicar estas herramientas de forma efectiva en mis propios proyectos?”. Aprenderás las habilidades necesarias para desarrollar sitios Web poderosos de forma rápida, con código limpio y de fácil mantenimiento.

<!-- 
https://www.youtube.com/watch?v=T1intZyhXDU 
[****](https://www.youtube.com/watch?v=o0XbHvKxw7Y)
CURSO DE DJANGO
https://www.youtube.com/watch?v=ruQIRGXfUKY&list=PLkVpKYNT_U9cl3hhVg_ROOlSY33uuBWZh&index=2
-->
