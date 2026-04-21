# Comandos — Configuración e inicio

## Configuración global

```bash
# Establecer nombre de usuario
git config --global user.name "Tu Nombre"

# Establecer email
git config --global user.email "tu@email.com"

# Ver toda la configuración actual
git config --list

# Ver un valor concreto
git config user.name
```

---

## Inicializar un repositorio

```bash
# Convertir la carpeta actual en un repositorio Git
git init

# Inicializar una carpeta nueva con nombre específico
git init nombre-del-proyecto
```

---

## Comprobar el estado del repositorio

```bash
# Ver en qué estado están los archivos del repositorio
git status
```

Este comando lo usarás constantemente. Nunca está de más ejecutarlo antes de cualquier otra acción.
