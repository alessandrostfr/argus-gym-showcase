# Caso de estudio: Argus Gym

## Contexto

Argus Gym nació como una aplicación fitness, pero con el tiempo se convirtió en un proyecto de producto completo: entrenamiento, comunidad, contenido, progreso, comunicación, roles internos y experiencia mobile-first.

La idea no era hacer una app de gimnasio básica, sino trabajar con un producto lo bastante amplio como para tomar decisiones reales de arquitectura, UX y dominio.

---

## Objetivo

Construir una plataforma donde un usuario pueda:

1. crear o descubrir rutinas;
2. planificar entrenamientos;
3. ejecutar una sesión en vivo;
4. registrar sets, pesos y notas;
5. ver progreso;
6. compartir contenido;
7. interactuar con otros usuarios;
8. recibir asignaciones de un coach;
9. operar con panel admin cuando sea necesario.

---

## Qué lo hace interesante

El valor técnico del proyecto no está en una única pantalla, sino en la conexión entre módulos:

- un workout creado en Studio puede aparecer como contenido;
- una rutina puede planificarse;
- una planificación puede convertirse en una sesión;
- una sesión genera progreso;
- el progreso alimenta dashboard y perfil;
- el contenido puede compartirse;
- un coach puede asignar rutinas;
- un admin puede moderar recursos;
- las métricas permiten observar uso del producto.

---

## Principales módulos

### Backend

El backend se apoya en FastAPI, SQLAlchemy y Alembic. Está organizado por capas: rutas, schemas, modelos, servicios y repositorios.

Áreas destacadas:

- auth;
- usuarios y perfiles;
- workouts;
- ejercicios;
- planificación;
- sesiones;
- social;
- media;
- chat;
- notificaciones;
- coach;
- admin;
- analytics.

### Frontend

El frontend moderno usa Next.js, TypeScript y componentes reutilizables. La dirección actual es web-first y mobile-first, dejando la capa antigua como mantenimiento transicional.

Rutas destacadas:

- `/dashboard`;
- `/calendar`;
- `/studio`;
- `/discover`;
- `/chat`;
- `/coach`;
- `/admin`;
- `/profile`;
- `/u/{nickname}`.

### Producto

El proyecto fue evolucionando por bloques, priorizando primero funcionalidad base y después experiencia de uso, autenticación, media, comunidad, coach mode, analytics y despliegue.

---

## Decisiones relevantes

### 1. Separar backend y frontend

El backend mantiene la lógica de negocio y la API. El frontend se centra en experiencia de usuario, rutas, componentes y flujos.

### 2. Migrar hacia Next.js

La primera capa visual fue útil para avanzar rápido, pero la dirección profesional actual es Next.js + TypeScript para una UX más pulida y escalable.

### 3. Tratar el calendario y el entrenamiento como núcleo

La parte social existe, pero el producto no debe olvidar el caso principal: planificar, entrenar y progresar.

### 4. Mantener código privado y showcase público

El proyecto contiene lógica sensible, configuración y flujos internos. El showcase público permite enseñar arquitectura y producto sin exponer el repositorio real.

---

## Estado actual

El proyecto ya tiene una base amplia y funcional. La siguiente fase relevante para portfolio será:

- revisar y preparar la demo actual con datos ficticios: https://argusgym.vercel.app/;
- añadir capturas limpias;
- documentar el flujo completo;
- conectar el showcase con el portfolio público.

---

## Qué aprendí construyéndolo

- organizar un backend grande por dominios;
- trabajar con migraciones y modelos relacionales;
- diseñar APIs para frontend;
- pensar en UX mobile-first;
- construir flujos largos sin quedarme en pantallas sueltas;
- manejar autenticación, sesiones y proveedores externos;
- documentar decisiones técnicas;
- trabajar por versiones y roadmap.
