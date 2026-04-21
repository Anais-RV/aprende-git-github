# Configuración e inicio

## Antes de empezar: decirle a Git quién eres

La primera vez que usas Git en tu máquina, necesitas configurar tu nombre y tu email. Git va a guardar esta información en cada commit que hagas, para saber quién lo realizó.

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"
```

El flag `--global` significa que esta configuración se aplica a **todos tus proyectos** en esta máquina. Solo tienes que hacerlo una vez.

---

## Inicializar un repositorio: `git init`

Un **repositorio** (o "repo") es simplemente una carpeta que Git está vigilando. Para convertir cualquier carpeta en un repositorio Git:

```bash
git init
```

Esto crea una carpeta oculta llamada `.git/` dentro de tu carpeta. Ahí es donde Git guarda todo el historial. No toques ni borres esa carpeta.

---

## El archivo .gitignore

No todos los archivos de tu proyecto necesitan estar en el historial. Los archivos del sistema operativo, las dependencias descargadas o los archivos con contraseñas no deberían subirse a Git.

El archivo `.gitignore` le dice a Git qué archivos o carpetas debe ignorar:

```
# Ejemplo de .gitignore

# Archivos del sistema operativo
.DS_Store
Thumbs.db

# Carpeta de dependencias de Node
node_modules/

# Archivos de entorno con datos sensibles
.env
```

Cada línea es un patrón. Puedes usar `*` como comodín. Los comentarios se escriben con `#`.

---

## Verificar la configuración

Puedes ver tu configuración actual en cualquier momento:

```bash
git config --list
```

---

## Resumen del flujo inicial

1. Crea o navega hasta la carpeta de tu proyecto
2. Ejecuta `git init`
3. Crea un archivo `.gitignore` si lo necesitas
4. ¡Listo para empezar a hacer commits!
