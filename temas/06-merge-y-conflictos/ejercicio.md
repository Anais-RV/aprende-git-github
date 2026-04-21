# Ejercicio — Merge y conflictos

## Parte 1: Un merge sin conflictos

### Paso 1: Prepara el escenario

Desde `practica-git`, asegúrate de estar en `main` y de que la rama `experimento/nueva-seccion` existe y tiene commits:

```bash
git switch main
git log --oneline --graph --all
```

### Paso 2: Haz el merge

```bash
git merge experimento/nueva-seccion
```

Si el merge va bien, Git crea un commit de fusión automáticamente (o hace un "fast-forward" si no hay divergencia — ambos son correctos).

### Paso 3: Comprueba el resultado

```bash
git log --oneline --graph
```

Observa cómo el historial muestra la fusión. Abre `notas.md` y verifica que la sección de ramas aparece ahora en `main`.

### Paso 4: Elimina la rama fusionada

```bash
git branch -d experimento/nueva-seccion
```

---

## Parte 2: Crear y resolver un conflicto

Este ejercicio te hace crear un conflicto intencionalmente para aprender a resolverlo sin miedo.

### Paso 1: Crea una nueva rama

```bash
git switch -c experimento/conflicto
```

### Paso 2: Edita la primera línea de `notas.md` en esta rama

Cambia el título por:
```markdown
# Mis notas de Git y GitHub
```

Haz commit:

```bash
git add notas.md
git commit -m "docs: expandir titulo en rama de experimento"
```

### Paso 3: Vuelve a main y edita la misma línea

```bash
git switch main
```

Edita también la primera línea de `notas.md`, pero de otra forma:
```markdown
# Notas de aprendizaje - Git
```

Haz commit:

```bash
git add notas.md
git commit -m "docs: reformular titulo en main"
```

### Paso 4: Intenta el merge

```bash
git merge experimento/conflicto
```

Git avisará de un conflicto. Abre `notas.md` y verás los marcadores:

```
<<<<<<< HEAD
# Notas de aprendizaje - Git
=======
# Mis notas de Git y GitHub
>>>>>>> experimento/conflicto
```

### Paso 5: Resuelve el conflicto

Elige el título que prefieras (o combina los dos), elimina los marcadores y guarda el archivo.

### Paso 6: Completa el merge

```bash
git add notas.md
git commit -m "merge: resolver conflicto de titulo en notas"
```

---

## Resultado esperado

- Has completado un merge sin conflictos
- Has creado, entendido y resuelto un conflicto manualmente
- Tu historial refleja los merges realizados
