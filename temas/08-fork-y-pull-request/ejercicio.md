# Ejercicio — Fork y Pull Request

Este ejercicio lo harás sobre **este mismo repositorio** (el que estás leyendo ahora). Contribuirás con una mejora real al material del curso.

La URL del repositorio es la que tu instructor te haya indicado. Si no la tienes, búscala en la barra de direcciones de GitHub cuando estés en este repo.

---

## Paso 1: Haz fork de este repositorio

1. En GitHub, ve a la página de este repositorio
2. Haz clic en el botón **Fork** (arriba a la derecha)
3. Selecciona tu cuenta y confirma

GitHub crea una copia del repositorio en tu cuenta. A partir de ahí trabajas sobre esa copia, no sobre el original.

---

## Paso 2: Clona tu fork en local

```bash
# Sustituye TU-USUARIO por tu nombre de usuario real en GitHub
# y nombre-de-este-repo por el nombre que aparece en GitHub
git clone https://github.com/TU-USUARIO/nombre-de-este-repo.git
cd nombre-de-este-repo
```

---

## Paso 3: Crea una rama para tu contribución

```bash
git switch -c docs/mi-aportacion
```

---

## Paso 4: Elige qué mejorar

Elige una de estas opciones (o propón la tuya):

**Opción A**: Añade una pregunta al `autocheck.md` de cualquier tema que consideres útil

**Opción B**: Mejora la explicación de algún concepto que te haya costado entender

**Opción C**: Corrige algún error tipográfico o mejora de redacción que encuentres

---

## Paso 5: Haz commit de tu cambio

```bash
git add .
git commit -m "docs: [describe brevemente qué mejoraste y en qué tema]"
```

---

## Paso 6: Envía tu rama a GitHub

```bash
git push origin docs/mi-aportacion
```

---

## Paso 7: Abre el Pull Request

1. Ve a GitHub, a tu fork del repositorio
2. Verás un banner amarillo sugiriéndote abrir un PR — haz clic en **Compare & pull request**
3. Escribe un título descriptivo
4. En la descripción, explica:
   - Qué cambiaste
   - Por qué lo cambiaste
5. Haz clic en **Create pull request**

---

## Resultado esperado

- Tienes un fork del repositorio en tu cuenta de GitHub
- Has abierto un Pull Request con una mejora real
- Entiendes la diferencia entre fork, clonar y abrir un PR
