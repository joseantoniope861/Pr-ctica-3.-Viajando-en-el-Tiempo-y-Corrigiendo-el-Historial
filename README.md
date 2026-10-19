# 3. Ejercicios de Autoevaluación
   
# 1. Identificación de Versiones: ¿Cuál es el hash abreviado del commit donde solo existía la función sumar (C1)?
	El hash abreviado del commit C1 (donde solo existía la función sumar) es c94c784 (tal como apareció en tu historial con git log --oneline

# 2. Referencia a un Ancestro: Escriba el comando exacto para hacer un viaje en el tiempo (switch o checkout) en modo desacoplado al commit inmediatamente anterior a la etiqueta v1.0-estable, usando la notación de ancestro (~ o ^).

	El comando para viajar en el tiempo   es: git switch --detach v1.0-estable~1

## 3. Seguridad y Borrado: Si usted hubiera usado git reset --hard <HASH_C2> en lugar de git revert HEAD en el punto 3.4, ¿cuál habría sido la principal implicación si este repositorio estuviera compartido en GitHub con otros compañeros?

git reset --hard es muy peligroso porque borra los cambios y cambia lo que ya pasó.

git revert es seguro para trabajar en grupo: crea un paso nuevo que arregla el fallo sin borrar nada.
       
## 4. Propósito de HEAD: Tras finalizar el punto 3.5, ¿a qué está apuntando HEAD en su repositorio? ¿A un commit específico (Detached HEAD) o a la rama principal (main)?
	Head está apuntando a la rama principal. El --amend actualiza y reemplaza el último commit de la rama sin sacarte de ella.
