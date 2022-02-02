# Ejemplo de Docker-compose con una app python/flask

* En el archivo docker-compose.yaml, la variable ```FLASK_ENV: development``` le indica a Flask que estamos en modo desarrollo
* Junto al bind mount:
```
     volumes:
      - .:/code
```
Permite que Flask monitoree el archivo app.py por cambios, es decir, podemos
modificar la página web on the fly, sin reiniciar con docker-compose