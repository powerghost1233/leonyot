# León TV Admin
Panel de clientes y suscripciones en Node.js y PostgreSQL.

## Render
1. Sube el contenido de esta carpeta a un repositorio privado de GitHub.
2. Crea una base de datos PostgreSQL persistente (en Render u otro proveedor) y copia su URL de conexión.
3. En Render, crea un Blueprint desde el repositorio (`render.yaml`). Configura `DATABASE_URL` y `ADMIN_PASSWORD` en el panel de Render. Nunca subas `.env` real a GitHub.
4. Despliega y entra con usuario `admin` y la contraseña configurada.

## Desarrollo local
`npm install`, copia `.env.example` a `.env`, rellena las variables y ejecuta `npm start`.

## Notas
Versión inicial: clientes, suscripciones, renovación con historial, indicadores y autenticación. Antes de uso comercial, añadir CSRF, auditoría, copias de seguridad, recuperación de contraseña y políticas de protección de datos. La eliminación de un cliente borra su historial. No incluye todavía importación CSV ni notificaciones automáticas.
