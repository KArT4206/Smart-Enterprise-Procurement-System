# Security

- Passwords are hashed with BCrypt. Sessions use signed JWTs (`jwt.expiration` = 24 h), and the frontend signs users out after inactivity.
- Every API route except login, registration and the public department list requires a valid token. Role checks run on the server and are mirrored by route guards in the UI.
- New sign-ups stay pending until an administrator approves them and assigns a role.
- `DB_PASSWORD` and `JWT_SECRET` come from environment variables only; `application.properties` has no default values for them. Use a random secret of at least 256 bits.
- Seed data contains demo users with hashed passwords. Change or remove them before any shared deployment.

To report a vulnerability, open a private security advisory on this repository.
