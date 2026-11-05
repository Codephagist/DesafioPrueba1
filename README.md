# DesafioPrueba1

## Cómo trabajar en el repo

Nadie puede subir cambios directo a `main`. Cada persona trabaja en su propia rama y envía sus cambios con un Pull Request (PR). El owner (@OsvaDev-HUB) revisa y aprueba cada PR antes de unirlo a `main`.

### Ramas de cada integrante

| Integrante | Rama |
|---|---|
| DeveloperGerard | `dev/DeveloperGerard` |
| otrolemao | `dev/otrolemao` |
| Xunork | `dev/Xunork` |

### 1. Aceptar la invitación (solo la primera vez)

Entra a https://github.com/OsvaDev-HUB/DesafioPrueba1/invitations y acepta.

### 2. Clonar el repo y entrar a tu rama (solo la primera vez)

```bash
git clone https://github.com/OsvaDev-HUB/DesafioPrueba1.git
cd DesafioPrueba1
git checkout dev/TU_USUARIO
```

### 3. Antes de empezar a trabajar, traer lo último de main

```bash
git checkout dev/TU_USUARIO
git pull origin main
```

### 4. Guardar tus cambios

```bash
git add .
git commit -m "feat: Se agrega el formulario de login"
```

Usa un prefijo en el mensaje: `feat:`, `fix:`, `docs:`, `style:`, `refactor:`.

### 5. Subir tu rama a GitHub

```bash
git push origin dev/TU_USUARIO
```

### 6. Abrir el Pull Request

- **Opción web:** entra al repo en GitHub y haz clic en el botón verde **"Compare & pull request"**. Revisa que diga `base: main` y `compare: dev/TU_USUARIO`, escribe qué hiciste y envíalo.
- **Opción terminal** (si tienes `gh` instalado):

```bash
gh pr create --base main --fill
```

### 7. Esperar la revisión

Si te piden cambios, hazlos en tu misma rama y vuelve a subir:

```bash
git add .
git commit -m "fix: Se corrige lo que pidio la revision"
git push origin dev/TU_USUARIO
```

El PR se actualiza solo.

### 8. Cuando aprueben y unan tu PR

Vuelve al paso 3 para traer lo último de `main` antes de seguir trabajando.

### Importante

- Nunca trabajes directo en `main`.
- Trabaja siempre en tu rama `dev/TU_USUARIO`.
- Si `git push` a `main` te da error, es normal: está protegido.
