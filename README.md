# Panel de trabajos

Panel con una fila por trabajo: **Yo debo**, **Esperando de ellos** y **Bitácora**, más un radar arriba con lo vencido, lo que hay que insistir y los trabajos sin movimiento.

## Actualizar el panel en tu repo (una vez)

1. En el repo, reemplaza `index.html` por el nuevo (Add file → Upload files, o abre `index.html` → lápiz → pega el contenido).
2. Borra `pendientes.md`: ya no se usa.
3. Abre la página (`https://TU-USUARIO.github.io/Panel-Pendientes/`). La primera vez te pide **crear una contraseña**. Anótala: si se pierde, los datos no se pueden recuperar.

## Que guarde solo (recomendado)

Sin esto, "Guardar" copia el contenido cifrado y te abre GitHub para que lo pegues. Con esto, guarda directo a los 2–3 segundos de cada cambio.

1. En GitHub: Settings (de tu cuenta) → Developer settings → Personal access tokens → **Fine-grained tokens** → Generate new token.
2. Repository access: **Only select repositories** → `Panel-Pendientes`.
3. Permissions → Repository permissions → **Contents: Read and write**.
4. Copia el token y pégalo en el panel: **Ajustes → Token**. Queda guardado solo en ese navegador.

## Privacidad

El repo es público, pero `datos.enc.json` está cifrado (AES-256-GCM, clave derivada de tu contraseña con PBKDF2 en tu navegador). En GitHub solo se ve texto ilegible. La contraseña y el token nunca salen de tu navegador, salvo el token hacia la API de GitHub para guardar.

Mientras no hayas guardado la primera vez, el archivo no existe. Las demás cosas del repo (`index.html`, este README) no contienen datos tuyos.

## Uso diario

- **Agregar rápido** (barra de arriba): elige trabajo, tipo y escribe. Sirve para anotar sin buscar la fila.
- En cada fila puedes agregar directo en cada lista (texto, persona y fecha opcionales).
- Check = hecho / recibido. Doble clic edita un texto. ⚑ marca lo importante. ✕ borra.
- Lo que pediste y lleva 5+ días sin llegar aparece en **Hay que insistir**.
- Estado de cada trabajo: verde (al día), amarillo (atención), rojo (urgente).
