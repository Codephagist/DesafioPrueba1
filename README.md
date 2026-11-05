# DesafioPrueba1

## Cómo trabajar en el repo

El repo está en la organización **Codephagist**:
https://github.com/Codephagist/DesafioPrueba1

Cada integrante tiene su propia rama y **solo puede subir cambios a la suya**. Nadie puede subir directo a `main`: todo se envía con un Pull Request (PR) y el owner (@OsvaDev-HUB) lo revisa antes de unirlo.

### Ramas de cada integrante

| Integrante | Rama |
|---|---|
| DeveloperGerard | `dev/DeveloperGerard` |
| otrolemao | `dev/otrolemao` |
| Xunork | `dev/Xunork` |

### 1. Clonar el repo

Si ya lo habías clonado antes de que se moviera a la organización, actualiza la URL:

```bash
git remote set-url origin https://github.com/Codephagist/DesafioPrueba1.git
git fetch origin
```

Si todavía no lo clonas:

```bash
git clone https://github.com/Codephagist/DesafioPrueba1.git
cd DesafioPrueba1
```

### 2. Entrar a tu rama

Cambia `TU_USUARIO` por tu usuario de GitHub:

```bash
git checkout dev/TU_USUARIO
```

### 3. Antes de empezar a trabajar, traer lo último de main

```bash
git pull origin main
```

### 4. Guardar tus cambios

```bash
git add .
git commit -m "feat: Se agrega el formulario de login"
```

Usa un prefijo en el mensaje: `feat:`, `fix:`, `docs:`, `style:`, `refactor:`.

### 5. Subir tu rama

```bash
git push origin dev/TU_USUARIO
```

### 6. Abrir el Pull Request

- **Web:** entra al repo y haz clic en **"Compare & pull request"**. Revisa que diga `base: main` y `compare: dev/TU_USUARIO`, escribe qué hiciste y envíalo.
- **Terminal** (si tienes `gh` instalado):

```bash
gh pr create --base main --fill
```

### 7. Si te piden cambios

Hazlos en tu misma rama y vuelve a subir:

```bash
git add .
git commit -m "fix: Se corrige lo que pidio la revision"
git push origin dev/TU_USUARIO
```

El PR se actualiza solo.

### 8. Cuando aprueben y unan tu PR

Vuelve al paso 3 antes de seguir trabajando.

### Importante

- Nunca trabajes en `main`.
- Si `git push` te da error al subir a `main` o a la rama de otro, es normal: están protegidas.
