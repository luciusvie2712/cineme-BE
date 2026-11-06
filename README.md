# Cinema Backend — Express/MongoDB Scaffold

> **Status:** Early-stage backend exercise. This repository should **not** be treated as a production-ready cinema API.

## Technology

- Node.js / Express 5
- MongoDB via Mongoose
- dotenv and nodemon

## Repository state

The repository includes `app.js`, `src/config/`, `src/models/`, and a `package.json`. The committed entry point references `./config/db`, whereas the database configuration resides under `src/config/`. This import path requires correction before a clean local startup can be assumed.

The repository also contains a tracked `node_modules/` directory. It should be removed from Git tracking and ignored in a future code-cleanup commit.

## Development setup

```bash
git clone https://github.com/luciusvie2712/cineme-BE.git
cd cineme-BE
npm install
```

The `dev` script is `nodemon app.js`. **Do not expect a successful startup before checking the configuration import, connection settings and required environment variables.**

The package currently contains no runnable automated test suite (`npm test` is a placeholder).

## Engineering follow-up

- Fix database imports, environment validation and startup errors.
- Add endpoint definitions, request validation and centralized error handling.
- Add authentication/authorization where required.
- Add integration tests, GitHub Actions and a reproducible local setup.
- Remove tracked dependencies and document the data model before using this project in a portfolio.
