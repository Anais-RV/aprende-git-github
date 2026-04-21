# Ejercicio — Conectar con GitHub

## Requisito previo

Necesitas tener una cuenta en [github.com](https://github.com). Si no la tienes, créala antes de empezar.

---

## Paso 1: Crea el repositorio en GitHub

1. Accede a tu cuenta de GitHub
2. Haz clic en **New repository**
3. Nombre: `practica-git`
4. Visibilidad: pública o privada, como prefieras
5. **Importante**: no marques "Add a README file" ni ".gitignore" — ya los tienes en local
6. Haz clic en **Create repository**

---

## Paso 2: Conecta tu repositorio local

GitHub te mostrará instrucciones. Ejecuta en tu terminal, dentro de `practica-git`:

```bash
git remote add origin https://github.com/TU-USUARIO/practica-git.git
```

Cambia `TU-USUARIO` por tu nombre de usuario real en GitHub.

Verifica que se añadió:

```bash
git remote -v
```

---

## Paso 3: Envía tu historial

```bash
git push -u origin main
```

> **Si es la primera vez que haces push desde esta máquina**, Git puede pedirte que te autentiques. En Windows, normalmente se abre el navegador para que inicies sesión con tu cuenta de GitHub. Si no ocurre así o tienes algún error, consulta la sección "Autenticación" en la explicación de este tema antes de continuar.

---

## Paso 4: Verifica en GitHub

Abre tu navegador y ve a `https://github.com/TU-USUARIO/practica-git`. Deberías ver todos tus archivos y, si haces clic en "Commits", tu historial completo.

---

## Paso 5: Edita desde GitHub y trae los cambios

1. En GitHub, abre `notas.md` y haz clic en el icono del lápiz para editarlo
2. Añade una línea al final: `- GitHub es el remoto donde vive el historial compartido`
3. Escribe un mensaje de commit y guarda desde la web

Ahora en tu terminal local:

```bash
git pull
```

Abre `notas.md` y verifica que el cambio que hiciste en la web está ahora en tu máquina.

---

## Paso 6: Practica el flujo completo

Haz un cambio local → commit → push, y verifica que aparece en GitHub.

---

## Resultado esperado

- Tu repositorio está en GitHub y sincronizado con tu máquina
- Sabes hacer `push` para enviar y `pull` para recibir cambios
- Entiendes que hay un repositorio local y uno remoto, y cómo se sincronizan
