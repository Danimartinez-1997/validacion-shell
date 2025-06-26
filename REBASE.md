# Reescritura del historial con git rebase -i

## Objetivo

Limpiar el historial de commits y dejar mensajes claros y significativos.

## Commits originales

- "Cambios"
- "Arreglos"
- "Actualización de cosas"

## Pasos realizados

1. Ejecuté `git rebase -i HEAD~3` para reescribir los últimos 3 commits.
2. Cambié el primer commit a `reword` y los otros dos a `squash`.
3. Unifiqué los tres commits en uno solo con el mensaje:
   > "Mejorar limpieza.txt con varias líneas nuevas"
4. Guardé y cerré el editor.
5. Finalmente, actualicé el repositorio remoto con:
   ```bash
   git push --force
