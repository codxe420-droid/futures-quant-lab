# Futures Quant Lab — Phase 0

Private research-only starter. No exchange credentials, order placement, or real trading.

## Requirements
- Docker and Docker Compose
- Git

## Start
1. Copy `.env.example` to `.env`.
2. Change `POSTGRES_PASSWORD` to a strong local development password.
3. Run `docker compose up --build`.
4. Open the forwarded frontend port `5173`.
5. Backend API docs: `/docs` on forwarded port `8000`.
6. Backend health: `/api/v1/health`.

## Stop
`docker compose down`

To remove the local database volume too (destructive):
`docker compose down -v`

## Services
- Frontend: React + Vite
- Backend: FastAPI
- Database: PostgreSQL 16 + TimescaleDB

Phase 0 only verifies that the application, API, and database communicate.
