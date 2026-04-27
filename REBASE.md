# Limpieza de commits con rebase

## Situación inicial

Se han creado varios commits con mensajes poco descriptivos como "cambios", "arreglos" y "actualizacion", simulando un historial desordenado.

## Proceso realizado

Se ha utilizado el comando:

git rebase -i HEAD~3

Esto permite modificar los últimos tres commits.

En el editor, se han cambiado las opciones de:

pick cambios
pick arreglos
pick actualizacion

a:

pick cambios
squash arreglos
squash actualizacion

De este modo, los commits se han fusionado en uno solo.

## Resultado

Se ha obtenido un único commit con un historial más limpio y fácil de entender.

## Conclusión

El uso de rebase interactivo permite mejorar la calidad del historial de commits, haciendo que sea más claro y profesional.
