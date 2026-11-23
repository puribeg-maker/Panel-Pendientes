# Panel de pendientes

Panel visual de pendientes y próximos pasos por trabajo. Es un sitio estático: `index.html` lee `pendientes.md` y lo dibuja.

## Publicar (una sola vez)

1. Crea un repositorio nuevo en GitHub (por ejemplo `panel`) y sube estos tres archivos: `index.html`, `pendientes.md` y `README.md`.
2. En el repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: `main` / `(root)` → Save**.
3. A los 1–2 minutos queda en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`.

## Actualizar

Abre `pendientes.md` en GitHub, toca el lápiz (Edit), cambia lo que necesites y presiona **Commit changes**. El sitio se actualiza solo en un minuto aprox. El botón "Editar en GitHub" del panel te lleva directo al archivo.

Formato:

```
## Nombre del trabajo
estado: verde | amarillo | rojo
proximo: el siguiente paso concreto
nota: comentario opcional
- [ ] Pendiente | 2026-12-01 | alta
- [x] Cosa ya hecha
```

La fecha y la prioridad (alta, media, baja) son opcionales. Para agregar un trabajo nuevo, copia un bloque `## ...` completo.

## Ojo con la privacidad

GitHub Pages publica el sitio en una URL abierta a cualquiera que la tenga, aunque el repo sea privado. Por eso conviene escribir los pendientes sin datos sensibles de clientes (montos, nombres completos de pacientes, etc.), o usar el panel solo con lo que no te importaría que alguien viera.
