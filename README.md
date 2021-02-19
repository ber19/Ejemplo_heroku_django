# Heroku_django
La plataforma hecha con Django con configuración para despliegue en Heroku con integracion a AWS S3. Sin haber hecho makemigrations

## Pasos:
1. Crear la migración inicial, en local. Instalar el entorno python y ejecutar:<br/>
&nbsp;&nbsp;python manage.py makemigrations
2. Una vez subido a Heroku. Ejecutar la migracion inicial:<br/>
&nbsp;&nbsp;heroku run python manage.py migrate
3. Crear un usuario administrador para entrar a la plataforma:<br/>
&nbsp;&nbsp;heroku run python manage.py createadmin

## Varables de entorno necesarias:<br/>
- AWS_ACCESS_KEY_ID
- AWS_SECRET_ACCESS_KEY
- S3_BUCKET&nbsp;&nbsp;(el nombre del bucket)
- DJANGO_DEBUG = False
- DJANGO_PRODUCTION = True
- SECRET_KEY&nbsp;&nbsp;(es opcional)
