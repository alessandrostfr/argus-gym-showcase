# Decisiones técnicas

## Backend con FastAPI

FastAPI permite trabajar con APIs claras, tipado, validación con Pydantic y una estructura cómoda para separar rutas, servicios y repositorios.

## SQLAlchemy + Alembic

El proyecto tiene muchos dominios y relaciones. SQLAlchemy permite modelar el dominio con control, y Alembic mantiene la evolución de la base mediante migraciones.

## PostgreSQL como objetivo de producción

SQLite fue útil en fases tempranas, pero PostgreSQL es la base adecuada para despliegue real, datos relacionales y evolución del producto.

## Next.js + TypeScript como frontend principal

La app empezó con una capa visual más rápida para prototipar, pero el objetivo actual es un frontend web más profesional con Next.js, TypeScript y componentes reutilizables.

## Mobile-first

El uso natural de una app fitness sucede muchas veces desde el móvil. Por eso las decisiones de UX priorizan navegación rápida, pantallas legibles y acciones claras.

## Studio con wizards

Los formularios largos son incómodos. En Studio se usan flujos por pasos para posts, workouts y exercises.

## Cropper de media por tipo de contenido

Cada contenido necesita una proporción distinta:

- posts: 4:5;
- exercises: 1:1;
- workouts: 1.91:1.

La imagen se normaliza antes de subirse para que feed, preview y tarjetas sean consistentes.

## Coach mode como diferencial

No se trata solo de tener usuarios y rutinas. El coach mode permite enseñar diseño de producto más avanzado: relaciones, asignaciones, seguimiento y check-ins.

## Admin como producto interno

El panel admin no es una pantalla decorativa. Sirve para moderación, reportes, auditoría y operación interna.

## Showcase sin código

Publicar un showcase permite enseñar el producto sin exponer el repositorio real, credenciales, configuraciones ni datos sensibles.
