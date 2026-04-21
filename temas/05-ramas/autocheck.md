# Autocheck — Ramas

## Preguntas

1. **¿Qué es una rama en Git?**
   ¿Es una copia del proyecto? ¿Qué es exactamente?

2. **¿Por qué es útil trabajar en ramas en lugar de hacerlo todo en `main`?**
   Da al menos dos situaciones donde las ramas sean beneficiosas.

3. **¿Qué diferencia hay entre `git switch` y `git checkout`?**
   ¿Cuál usarías preferentemente y por qué?

4. **Si estás en la rama `main` y creas cambios, ¿están visibles desde otra rama?**
   ¿Y al revés?

5. **¿Cuándo usarías `git branch -D` en lugar de `git branch -d`?**
   ¿Qué riesgo tiene?

6. **En un flujo con `main` y `dev`, qué papel cumple cada rama?**
   Explica por qué normalmente no se trabaja directo en `main`.

7. **¿Desde dónde conviene crear una rama de tarea en ese flujo?**
   ¿Qué problema aparece si la creas desde una base vieja?

8. **¿Por qué no conviene crear 10 ramas "por adelantado" al arrancar un proyecto?**
   Da al menos dos motivos prácticos.

---

## Comprobación práctica

```bash
git log --oneline --graph --all
```

¿Puedes interpretar la salida? ¿Ves dónde divergen las ramas?

---

## Señales de que lo tienes controlado

- Puedes crear, listar y cambiar de rama sin ayuda
- Entiendes que los cambios son locales a cada rama hasta que se fusionen
- Usas nombres de rama descriptivos
- Sabes visualizar el estado de las ramas con `--graph`
- Sabes cuándo crear una rama y cuándo no, según la necesidad real
