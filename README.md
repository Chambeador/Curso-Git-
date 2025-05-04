# Curso Git

✨ El principio de mi proyecto Git

<p align="center">
  <img src="https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png" alt="Logo de Git" width="250"/>
</p>

<br>

 *¡Vamos con todo!*

### Comandos:
- `git add nombre.extension`: Lleva un archivo al área de *staged* (preparación).
- `git status`: Muestra todos los archivos y su estado actual en el repositorio.

##  Clase 2: Comandos y Ramas
En la clase 2 aprendimos los comandos mas basicos para trabajar con git y a crear, movernos entre ramas y a eliminar ramas.
### Comandos de Git
- `git add archivo.algo`: Lleva un archivo al área de *staged* (preparación).
- `git status`: Muestra el estado actual del repositorio y los archivos.
- `git commit`: Realiza un commit con los cambios agregados.
- `git commit -m "mensaje"`: Hace un commit con un mensaje descriptivo.
- `git restore --staged archivo.algo`: Quita un archivo del área *staged* (lo desprepara).
- `git add .`: Agrega todos los archivos modificados al área de *staged*.
- `git log --oneline`: Muestra el historial de commits en una sola línea por commit.
- `git help`: Muestra ayuda general o de un comando específico.
- `git commit --amend -m "nuevo mensaje"`: Reemplaza el mensaje del último commit.

### ¿Qué es el HEAD?
`HEAD` es un puntero que indica en qué commit estás actualmente.  
Siempre apunta al **último commit de la rama activa**.

### ¿Que son las Ramas?
Es un instantaneo del codigo.
A nivel tecnico es un nuevo apuntador hacia una de las confirmaciones.

### Comandos de Git para trabajar con Ramas:
- `git branch nombre`: Crea una nueva rama.
- `git switch nombre`: Cambia a una rama existente.
- `git switch -c nueva-rama`: Crea y cambia a una nueva rama.
- `git checkout nombre`: Cambia de rama (forma clásica).
- `git branch -d nombre`: Elimina una rama local (solo si ya fue fusionada).
- `git branch -D nombre`: Fuerza la eliminación de una rama local (aunque no haya sido fusionada).




## Clase 3: Merge de Ramas y Conflictos

En la clase 3 aprendimos como fusionar ramas, como solucionar conflictos y las mejores practicas para eliminar ramas.

### Merge de Ramas

- `git merge rama`: Fusiona la rama indicada con la rama activa.
- `git merge --no-ff rama`: Fusiona la rama indicada, pero siempre crea un commit de merge, incluso si la fusión podría hacerse de manera "fast-forward".
- `git merge --abort`: Cancela la fusión en curso y vuelve al estado anterior.

### ¿Qué es Fast Forward?
El **fast-forward** ocurre cuando la rama en la que estás no tiene cambios que se aparten de la rama que estás fusionando. En este caso, Git solo mueve el puntero de la rama actual al ultimo commit de la rama fusionada, sin crear un commit adicional.

### Eliminar Ramas: ¿Por qué es importante?
Eliminar ramas es una buena práctica. Las ramas deben crearse con un propósito específico y de corto plazo. Después de fusionarlas, eliminar las ramas innecesarias mantiene el repositorio limpio y organizado.

### Comandos para Eliminar Ramas
- `git branch -d <nombre>`: Elimina una rama **solo si ha sido fusionada** con la rama actual. Es una forma segura de borrar ramas.
- `git branch -D <nombre>`: Elimina una rama **forzadamente**, incluso si **no ha sido fusionada**.

### Conflictos en Git

Cuando Git no puede fusionar automáticamente dos ramas debido a cambios contradictorios, se produce un **conflicto**. Para resolverlo, puedes usar:

- `git diff`: Muestra las diferencias entre las ramas, lo que te ayudará a identificar el conflicto y solucionarlo manualmente si no estas usando Visual Studio Code.




## Clase 3:

Estamos creando ramas clase 3
estamos trabajando con conflictos
vamos a crear un conflicto ahora vamos