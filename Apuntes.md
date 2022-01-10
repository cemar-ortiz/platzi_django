# Clase 1: Qué aprenderas sobre Django

Conoceremos Django, porqué existe, y qué problema resuelve. Haremos un clon de Instagram llamado "Platzigram"

# Clase 2: Historia de web development

Al inicio de la web, todos los sitios eran basados en texto. Eventualmente era necesario conectar a una bdd o implementar lógica, ahí nacieron los CGI Scripts (perl, python, bash).

Eran díficiles de mantener y escalar. PHP es popular porque agrega la capacidad de poder incluir la lógica dentro del template. Aún así no resolvía el problema de la escalabilidad y cosas de no repetir código.

Ahí nacieron los Frameworks para manejar con una sola herramienta peticiones HTTP, conexiones a base de datos, interacción con templates HTML y otras cosas más.

Django nace como solución para un sitio de noticias. Tenía como objetivo hacer más fácil el mantenimiento, construir objectos request y response, hacer más rápido el desarrollo e incluir un ORM (para conectarte a una base de datos a través de python).

Viene listo para todo, precargado con muchas herramientas y resuelve cosas como administración de contenido, seguridad y autenticación de usuarios. Django es un framework muy escalable, es cuestión de configuración de servidores y te permite moldear proyectos tal como tu lo necesites.

Está escrito en Python y es una gran ventaja porque significa que la curva de desarrollo es corta. Django considera muy bien el DRY. Tiene una buena comunidad de desarrollo. Es open source y está bien documentada.

# Clase 3: Creación del proyecto Platzigram / Tu primer Hola, mundo! en Django

```
django-admin startproject platzigram
```

en settings.py están las configuraciones del proyecto
en urls.py está el administrador de rutas
en wsgi.py está la interfaz que se usa para desplegar el servidor
manage.py construye una interfaz sobre django-admin

Dentro de cada file vienen notas útiles sobre qué variables hay en ellas y cómo se usan

Para exponer el proyecto en localhost:8080

```
python manage.py runserver
```

# Clase 4: El objeto Request