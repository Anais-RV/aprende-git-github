# Ejercicio — Configuración e inicio

## Paso 1: Configura Git con tu nombre y email

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"
```

Verifica que se guardó correctamente:

```bash
git config user.name
git config user.email
```

---

## Paso 2: Crea una carpeta para practicar

Crea una carpeta nueva llamada `practica-git` en cualquier lugar de tu sistema. Puedes hacerlo desde el explorador de archivos o desde la terminal:

```bash
mkdir practica-git
cd practica-git
```

---

## Paso 3: Inicializa el repositorio

Dentro de la carpeta `practica-git`, ejecuta:

```bash
git init
```

Deberías ver un mensaje similar a:
```
Initialized empty Git repository in .../practica-git/.git/
```

Comprueba que la carpeta `.git/` existe (puede estar oculta):

```bash
# En Git Bash, macOS o Linux:
ls -a

# En PowerShell (Windows):
Get-ChildItem -Force
```

---

## Paso 4: Crea un .gitignore básico

Crea un archivo llamado `.gitignore` en la raíz de `practica-git` con este contenido:

```
.DS_Store
Thumbs.db
*.log
```

---

## Paso 5: Comprueba el estado

```bash
git status
```

Deberías ver que Git detecta el archivo `.gitignore` como un archivo nuevo no rastreado. En el siguiente tema aprenderás qué hacer con él.

---

## Resultado esperado

- Git está configurado con tu nombre y email
- Tienes una carpeta `practica-git` inicializada como repositorio Git
- Existe un archivo `.gitignore` básico
- `git status` muestra el archivo como no rastreado (untracked)
