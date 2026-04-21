# Autocheck — El ciclo básico

## Preguntas

1. **Describe los tres estados de un archivo en Git.**
   ¿Qué diferencia hay entre working directory y staging area?

2. **¿Por qué existe la staging area?**
   ¿Qué ventaja tiene que no exista en sistemas más simples de "guardar"?

3. **¿Qué pasa si ejecutas `git commit` sin haber hecho `git add`?**
   Pruébalo en tu repositorio de práctica para ver el resultado.

4. **¿Qué muestra `git log --oneline`?**
   ¿Qué es ese identificador corto que aparece al principio de cada línea?

5. **¿Cuál es la diferencia entre `git diff` y `git diff --staged`?**

---

## Comprobación práctica

Ejecuta en tu repositorio de práctica:

```bash
git log --oneline
```

¿Tienes al menos 2 commits? ¿Los mensajes tienen sentido sin necesidad de abrir los archivos?

---

## Señales de que lo tienes controlado

- Puedes hacer el ciclo completo (editar → add → commit) sin consultar nada
- Entiendes para qué sirve la staging area
- Sabes leer la salida de `git status` e interpretar los colores
- Puedes ver el historial con `git log --oneline`
