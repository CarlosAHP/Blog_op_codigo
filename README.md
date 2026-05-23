# Blog: Entornos en tiempo de ejecución / Optimizadores de código

Sitio estático (HTML + CSS) para el módulo de Compiladores. Listo para desplegar en [Vercel](https://vercel.com).

## Vista local

Abre `index.html` en el navegador o sirve la carpeta:

```bash
cd "blog optimizacion de copilador"
python3 -m http.server 8080
```

Luego visita http://localhost:8080

## Despliegue en Vercel

### Opción A: CLI

```bash
npm i -g vercel
cd "blog optimizacion de copilador"
vercel
```

Sigue el asistente. En el primer despliegue, Vercel detectará un sitio estático sin framework.

### Opción B: GitHub

1. Sube esta carpeta a un repositorio en GitHub.
2. En [vercel.com/new](https://vercel.com/new), importa el repo.
3. Deja **Framework Preset** en “Other” y **Root Directory** en la carpeta del blog (o en `/` si el repo solo contiene el blog).
4. **Build Command**: vacío · **Output Directory**: `.` (raíz del proyecto).
5. Deploy.

No hace falta `npm install`: solo `index.html`, `styles.css` y `vercel.json`.

## Archivos

| Archivo       | Descripción                          |
|---------------|--------------------------------------|
| `index.html`  | Contenido del blog                   |
| `styles.css`  | Estilos (tema oscuro, responsive)    |
| `vercel.json` | Configuración mínima para Vercel     |
| `context.md`  | Material de referencia del módulo    |
