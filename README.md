# Simple Todo Application Backend (Express)

This workspace contains the Express backend for the Simple Todo Application.

For a full repository overview (including the React frontend workspace), see:

- `../simple-todo-application-245386-245400/README.md`

## What this backend currently provides

This backend currently exposes:

- `GET /`: Health endpoint returning status, timestamp, and environment.
- `GET /docs`: Swagger UI (OpenAPI server URL is set dynamically based on request host/protocol).

Todo CRUD endpoints are not implemented in the current backend source.

## Local development

```bash
cd backend
npm install
npm run dev
```

The backend uses:

- `HOST` (default `0.0.0.0`)
- `PORT` (default `3000`)
- `NODE_ENV` (used in the health response; default `development`)

## Scripts

From `backend/package.json`:

- `npm start`: run production server (`node src/server.js`)
- `npm run dev`: run with nodemon (`nodemon src/server.js`)
- `npm test`: run Jest
- `npm run lint`: run ESLint
