# Comandos — Fork y Pull Request

## El fork se hace desde la interfaz de GitHub

No hay un comando de Git para crear un fork. Se hace haciendo clic en el botón **Fork** en GitHub.

---

## Clonar tu fork

```bash
# Clona tu propio fork (no el repositorio original)
git clone https://github.com/TU-USUARIO/nombre-repo.git
```

---

## Trabajar en una rama antes de abrir el PR

```bash
# Crear rama para los cambios
git switch -c feat/nombre-descriptivo

# Hacer cambios, add y commit
git add .
git commit -m "feat: descripcion de lo que aporto"

# Enviar la rama a tu fork en GitHub
git push origin feat/nombre-descriptivo
```

---

## Mantener el fork sincronizado con el original

```bash
# Añadir el repo original como segundo remoto (se hace una sola vez)
git remote add upstream https://github.com/otro/nombre-repo.git

# Traer cambios del original sin fusionar
git fetch upstream

# Incorporar los cambios a tu rama main local
git switch main
git merge upstream/main

# Enviar la actualización a tu fork en GitHub
git push origin main
```

---

## El Pull Request se gestiona desde GitHub

Una vez haces push de tu rama, GitHub muestra un botón para abrir el PR. El proceso de revisión, comentarios y merge se hace desde la interfaz web de GitHub.
