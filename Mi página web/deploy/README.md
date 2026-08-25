# Door Windows Center — sitio

Sitio estático de una página.

## Archivos

- `index.html` — la página
- `assets/` — fotos, logo y video
- `ds/` — estilos
- `support.js` — runtime de la página
- `server.js` + `package.json` — servidor mínimo para Railway (sin dependencias)

## Subir a GitHub

Importante: los archivos van en la **raíz** del repositorio. `index.html` y `package.json`
deben verse al abrir el repositorio, no dentro de una carpeta.

1. En el repositorio: Add file → Upload files.
2. Arrastra **el contenido** de esta carpeta (todos los archivos y las carpetas
   `assets/` y `ds/`), no la carpeta `deploy` completa.
3. Commit changes.

## Railway

1. New Project → Deploy from GitHub repo → este repositorio.
2. Railway detecta Node y arranca con `npm start`.
3. Settings → Networking → Custom Domain → `www.doorwindowscenter.com`.
4. Copia el CNAME que da Railway en el DNS de GoDaddy.

## Hosting normal (cPanel, FTP)

Copiar `index.html`, `assets/`, `ds/` y `support.js` a `public_html`.
`server.js` y `package.json` no hacen falta ahí.
