# Setup local

Este repositorio showcase no contiene el código fuente, así que no existe instalación local aquí.

El repositorio real es privado.

Esta página se mantiene para explicar la estructura técnica general del proyecto real y el tipo de entorno usado durante desarrollo.

## Backend

- Python;
- FastAPI;
- SQLAlchemy;
- Alembic;
- PostgreSQL;
- Pydantic;
- Uvicorn;
- variables de entorno.

## Frontend

- Next.js;
- React;
- TypeScript;
- Tailwind;
- componentes reutilizables.

## Servicios

- Cloudinary / media provider;
- Google OAuth;
- Sentry opcional.

## Validación en el repositorio real

El proyecto real se valida con:

```bash
# Backend
python -m compileall app
pytest
alembic upgrade head

# Frontend
npm run build
```

Estos comandos son orientativos y no aplican a este showcase.
