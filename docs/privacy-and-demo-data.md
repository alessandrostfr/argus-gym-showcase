# Privacidad y demo data

## Por qué el repositorio real es privado

Argus Gym incluye:

- autenticación real;
- sesiones;
- configuración de proveedores externos;
- credenciales en variables de entorno;
- integración de media;
- flujos internos;
- datos de usuarios de prueba;
- lógica de producto en evolución.

Por eso el código fuente principal no se publica.

---

## Qué se puede mostrar públicamente

Sí se puede mostrar:

- arquitectura;
- capturas;
- demo con datos ficticios;
- roadmap;
- decisiones técnicas;
- flujo de producto;
- stack;
- problemas resueltos;
- limitaciones conocidas.

---

## Qué no se debe mostrar

No se debe publicar:

- `.env`;
- tokens;
- secretos OAuth;
- URLs privadas de servicios;
- bases de datos reales;
- capturas con emails reales;
- logs;
- datos personales;
- código interno si se decide mantener privado.

---

## Demo pública

Demo actual: **https://argusgym.vercel.app/**

La demo pública debe usar datos ficticios o datos sanitizados:

- usuarios demo;
- rutinas demo;
- posts demo;
- conversaciones simuladas;
- coach/alumno ficticios;
- métricas generadas;
- admin con datos controlados.

---

## Checklist antes de publicar capturas

- No aparecen emails reales.
- No aparecen tokens.
- No aparecen URLs internas privadas.
- No aparecen datos personales.
- No aparecen errores con stack traces.
- No aparecen paneles con credenciales.
- La demo está separada del entorno privado o no contiene datos personales reales.


## Capturas públicas

Las capturas incluidas en este showcase deben mantenerse con datos ficticios o sanitizados. Antes de actualizar imágenes, revisar que no aparezcan emails reales, nombres personales sensibles, tokens, errores internos, paneles con información privada o datos que no deban ser públicos.
