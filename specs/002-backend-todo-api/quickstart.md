# Quickstart: Todo Backend API

## Prerequisites

- Python 3.11+
- Neon PostgreSQL connection string
- `BETTER_AUTH_SECRET`

## Environment Setup

Create a `.env` file in the `backend/` directory:

```env
BETTER_AUTH_SECRET=<your-secret-key-here>
BETTER_AUTH_URL=http://localhost:3000
DATABASE_URL=<your-neon-database-url>
```

## Local Development

1. Navigate to `backend/`
2. Install dependencies:
   ```bash
   pip install fastapi uvicorn sqlmodel pyjwt asyncpg pydantic-settings
   ```
3. Run the server:
   ```bash
   uvicorn app.main:app --reload
   ```

## Testing

Run tests using pytest:

```bash
pytest
```
