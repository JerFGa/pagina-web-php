# Laravel Course API

Proyecto de práctica en Laravel 12 con vistas web y una API REST para productos. El repositorio incluye controladores web, controladores API, recursos JSON y persistencia con migraciones y factories.

## Requisitos

- PHP 8.2 o superior
- Composer
- Node.js y npm
- Una base de datos compatible con Laravel

## Instalación

1. Instala dependencias de PHP con `composer install`.
2. Instala dependencias frontend con `npm install`.
3. Copia el archivo de entorno con `cp .env.example .env`.
4. Genera la clave de la aplicación con `php artisan key:generate`.
5. Ejecuta las migraciones con `php artisan migrate`.

## Ejecución

- Servidor Laravel: `php artisan serve`
- Compilación de assets: `npm run dev`
- Pruebas: `php artisan test`

## API REST

Las rutas principales están definidas en `routes/api.php`.

- `GET /api/products` lista productos en formato JSON.
- `GET /api/products/{id}` obtiene un producto por id.
- `GET /api/v2/products` lista productos usando recursos JSON.
- `GET /api/v2/products/{id}` obtiene un producto usando recursos JSON.
- `GET /api/v3/products` retorna una colección personalizada.
- `GET /api/v3/products/paginate` retorna productos paginados.

## Estructura general

- `app/Http/Controllers/Api` contiene los controladores de la API.
- `app/Http/Resources` contiene los recursos para serialización JSON.
- `app/Models` contiene los modelos Eloquent.
- `database/migrations` contiene las tablas del proyecto.

## Licencia

Este proyecto conserva la licencia MIT del esqueleto de Laravel.
