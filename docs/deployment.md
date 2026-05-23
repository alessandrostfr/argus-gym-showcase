# Despliegue

## Estado actual

Argus Gym ya tiene una demo web desplegada:

**https://argusgym.vercel.app/**

El despliegue actual usa frontend en Vercel y backend en Render. Esta opción sirve como demo funcional y staging inicial.

## Estrategia futura

Más adelante se valorará migrar o replicar el despliegue en VPS para unificar portfolio, demos y proyectos bajo una infraestructura propia.

Objetivo:

- enseñar capacidad de despliegue real;
- tener control sobre infraestructura;
- alojar varios proyectos;
- preparar backups y HTTPS;
- usar una arquitectura profesional pero asumible.

---

## Infraestructura objetivo en VPS

```text
VPS Linux
Docker
Docker Compose
Reverse proxy
HTTPS
PostgreSQL
Backend FastAPI
Frontend Next.js
Proveedor externo de media
Backups automáticos
Monitorización básica
```

---

## URLs y subdominios

Demo actual:

```text
https://argusgym.vercel.app/
```

Ejemplo orientativo si se migra a dominio propio/VPS:

```text
argusgym.alessandrostfr.com
api-argusgym.alessandrostfr.com
```

También puede integrarse desde el portfolio principal con una ficha de proyecto.

---

## Componentes

### Frontend

Next.js corriendo como servicio web.

### Backend

FastAPI servido con Uvicorn/Gunicorn dentro de contenedor.

### Base de datos

PostgreSQL en el VPS o servicio gestionado si se decide más adelante.

### Media

Cloudinary o proveedor externo para evitar almacenar binarios pesados en el servidor.

### Reverse proxy

Nginx, Traefik o Nginx Proxy Manager.

### HTTPS

Let's Encrypt.

---

## Demo mode

Antes de abrir la demo:

- crear usuarios ficticios;
- poblar ejercicios;
- poblar rutinas;
- poblar publicaciones;
- poblar coach mode;
- bloquear funciones peligrosas si hace falta;
- revisar que no existan datos reales.

---

## Pendiente

- docker-compose de producción;
- variables de entorno productivas;
- backups;
- prueba de restore;
- monitorización;
- capturas definitivas;
- enlace público desde GitHub y portfolio actualizado con https://argusgym.vercel.app/.
