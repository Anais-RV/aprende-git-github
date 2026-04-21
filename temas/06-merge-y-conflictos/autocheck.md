# Autocheck — Merge y conflictos

## Preguntas

1. **¿Qué es un merge?**
   ¿Qué sucede exactamente en el historial cuando haces uno?

2. **¿En qué rama debes estar para hacer `git merge`?**
   ¿En la que quieres incorporar los cambios, o en la que tiene los cambios nuevos?

3. **¿Qué es un conflicto de merge y cuándo ocurre?**
   ¿Es un error de Git, o una situación normal?

4. **¿Qué son los marcadores `<<<<<<<`, `=======` y `>>>>>>>`?**
   ¿Qué debes hacer con ellos?

5. **¿Qué pasa si ejecutas `git merge --abort`?**
   ¿Cuándo tiene sentido usarlo?

---

## Comprobación práctica

```bash
git log --oneline --graph --all
```

¿Tu historial refleja los merges que hiciste? ¿Entiendes el gráfico?

---

## Señales de que lo tienes controlado

- Puedes hacer un merge y saber en qué rama ejecutar el comando
- Sabes leer los marcadores de conflicto sin entrar en pánico
- Puedes resolver un conflicto manualmente y completar el merge
- Limpias las ramas fusionadas con `git branch -d`
