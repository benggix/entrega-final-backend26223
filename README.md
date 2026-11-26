# Articulo API (Spring Boot + PostgreSQL + Docker)

## 1. Cómo levantarlo
Requisito: Docker Desktop instalado y abierto.

```bash
docker compose up --build
```
- Primera vez tarda unos minutos (descarga imágenes y dependencias Gradle).
- Cuando veas `Started ArticuloApiApplication` la API está en `http://localhost:8080`.
- Parar: `Ctrl+C` y luego `docker compose down` (los datos se conservan).
- Parar y BORRAR datos: `docker compose down -v`.

Qué crea el compose:
| Servicio | Qué es | Puerto |
|---|---|---|
| `db` | PostgreSQL 16 (base `articulos_db`, user `postgres`, pass `postgres`) | 5432 |
| `api` | Tu app Spring Boot compilada dentro de Docker (no necesitás Java ni Gradle instalados) | 8080 |

## 2. Link video:
En construccion