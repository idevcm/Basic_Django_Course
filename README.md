# Blog Project

This is a basic blog project developed using Django and Django REST Framework. It also includes an API that allows you to interact with the blog posts programmatically. The API documentation is generated using `drf_spectacular`. The project uses a PostgreSQL database.

## Features

- List of blog posts
- Detailed view of each blog post
- Creation of new blog posts (requires login)
- API endpoints for listing, retrieving, creating, updating, and deleting blog posts
- API documentation generated with `drf_spectacular`
- PostgreSQL database

## API Usage

The API is accessible at `localhost:8000/api`. Here are some of the endpoints you can use:

- `GET /api/posts/`: List all blog posts
- `GET /api/posts/<id>/`: Retrieve a specific blog post
- `POST /api/posts/`: Create a new blog post (requires authentication)
- `PUT /api/posts/<id>/`: Update a specific blog post (requires authentication)
- `DELETE /api/posts/<id>/`: Delete a specific blog post (requires authentication)

You can use tools like curl or Postman to interact with the API.

## API Documentation

The API documentation is available at `localhost:8000/api/schema/`. You can view the documentation in your browser to understand the structure and usage of the API.

## Database Configuration

The database configuration parameters are located in the `settings.py` file. You will find a section like this:

```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql_psycopg2',
        'NAME': '',
        'USER': '',
        'PASSWORD': '',
        'HOST': '',
        'PORT': '5432',
    }
}
```
You need to replace the empty strings with your PostgreSQL database parameters:

- `NAME`: The name of your database
- `USER`: The username of your database
- `PASSWORD`: The password of your database
- `HOST`: The host of your database (usually localhost if the database is on the same machine)
- `PORT`: The port of your database (usually 5432 for PostgreSQL)

## Setup

1. Clone the repository
2. Install the requirements using `pip install -r requirements.txt`
3. Set up your PostgreSQL database in `settings.py`
4. Create migrations using `python manage.py makemigrations`
5. Run migrations using `python manage.py migrate`
6. Start the server using `python manage.py runserver`

## Usage

Visit `localhost:8000` in your browser to view the blog posts. To create a new post, you need to log in first.

-----------------------------------------------------------------------------------------------------------------

# Proyecto Blog

Este es un proyecto básico de blog desarrollado con Django y Django REST Framework. También incluye una API que te permite interactuar con las publicaciones del blog de forma programática. La documentación de la API se genera con `drf_spectacular`. El proyecto utiliza una base de datos PostgreSQL.

## Características

- Lista de publicaciones de blog
- Vista detallada de cada publicación del blog
- Creación de nuevas publicaciones de blog (requiere inicio de sesión)
- Puntos finales de la API para listar, recuperar, crear, actualizar y eliminar publicaciones de blog
- Documentación de la API generada con `drf_spectacular`
- Base de datos PostgreSQL

## Uso de la API

La API se puede acceder en `localhost:8000/api`. Aquí hay algunos de los puntos finales que puedes usar:

- `GET /api/posts/`: Lista todas las publicaciones de blog
- `GET /api/posts/<id>/`: Recupera una publicación de blog específica
- `POST /api/posts/`: Crea una nueva publicación de blog (requiere autenticación)
- `PUT /api/posts/<id>/`: Actualiza una publicación de blog específica (requiere autenticación)
- `DELETE /api/posts/<id>/`: Elimina una publicación de blog específica (requiere autenticación)

Puedes usar herramientas como curl o Postman para interactuar con la API.

## Documentación de la API

La documentación de la API está disponible en `localhost:8000/api/schema/`. Puedes ver la documentación en tu navegador para entender la estructura y uso de la API.

## Configuración de la base de datos

Los parámetros de configuración de la base de datos se encuentran en el archivo `settings.py`. Encontrarás una sección como esta:

```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql_psycopg2',
        'NAME': '',
        'USER': '',
        'PASSWORD': '',
        'HOST': '',
        'PORT': '5432',
    }
}
```
Necesitas reemplazar las cadenas vacías con los parámetros de tu base de datos PostgreSQL:

- `NAME`: El nombre de tu base de datos
- `USER`: El nombre de usuario de tu base de datos
- `PASSWORD`: La contraseña de tu base de datos
- `HOST`: El host de tu base de datos (generalmente localhost si la base de datos está en la misma máquina)
- `PORT`: El puerto de tu base de datos (generalmente 5432 para PostgreSQL)

## Configuración

1. Clona el repositorio
2. Instala los requisitos usando `pip install -r requirements.txt`
3. Configura tu base de datos PostgreSQL en `settings.py`
4. Crea las migraciones usando `python manage.py makemigrations`
5. Ejecuta las migraciones usando `python manage.py migrate`
6. Inicia el servidor usando `python manage.py runserver`

## Uso

Visita `localhost:8000` en tu navegador para ver las publicaciones del blog. Para crear una nueva publicación, primero necesitas iniciar sesión.
