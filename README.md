# JWKS Server (Python/Flask)

Implements:
- RSA key gen with `kid` and expiry
- `GET /jwks` and `GET /.well-known/jwks.json` (only non-expired keys)
- `POST /auth` (valid JWT) and `POST /auth?expired=true` (expired JWT)
- JWT header includes `kid`

## Setup
```bash
python -m venv .venv
# Windows
.venv\Scripts\activate.bat
pip install -r requirements.txt
