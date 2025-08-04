# Comandos de Git

## Comandos de Ramas (Branch)
- `git branch` – Muestra una lista de las ramas locales en tu repositorio Git.
- `git branch -a` – Muestra una lista de ramas locales y remotas.
- `git branch -c` – Copia una rama de Git.
- `git branch -d <nombre-rama>` – Elimina una rama local (solo si no tiene cambios sin fusionar).
- `git branch -D <nombre-rama>` – Elimina una rama local incluso si tiene cambios sin fusionar.
- `git branch -m <nombre-rama> <nuevo-nombre>` – Renombra una rama.
- `git branch -r` – Muestra una lista de ramas remotas.
- `git push <remoto> --delete <rama-remota>` – Elimina una rama remota.
- `git push --set-upstream <remoto> <rama>` – Asocia una rama local con una rama remota.

## Comandos de Checkout
- `git checkout <rama>` – Cambia a otra rama.
- `git checkout -b <rama>` – Crea una nueva rama y cambia a ella.
- `git checkout -b <rama> <remoto>/<rama>` – Crea una rama local desde una rama remota y cambia a ella.
- `git checkout <hash>` – Cambia a un commit anterior.
- `git checkout <etiqueta>` – Cambia a una etiqueta (modo HEAD separado).
- `git checkout -b <rama> <etiqueta>` – Cambia una etiqueta como rama.

## Comando Cherry Pick
- `git cherry-pick <commit>` – Aplica los cambios de un commit en otra rama.

## Comandos Clone
- `git clone <url-repositorio>` – Clona un repositorio remoto.
- `git clone <url> <directorio>` – Clona y nombra el directorio local.
- `git clone <url> --origin <nombre>` – Clona y nombra el remoto.
- `git clone <url> --branch <rama>` – Clona y cambia a la rama específica.
- `git clone <url> --depth <profundidad>` – Clona con un número limitado de commits.
- `git clone <url> --no-tags` – Clona sin las etiquetas.

## Comandos Commit
- `git status` – Muestra el estado de los archivos.
- `git add` – Añade cambios al área de preparación.
- `git commit` – Guarda los cambios en el repositorio.
- `git commit -a` – Añade todos los archivos modificados y eliminados.
- `git commit --amend` – Modifica el último commit.
- `git commit -m "mensaje"` – Añade un mensaje al commit.

## Comandos Config
- `git config --global` – Configura opciones globales.
- `git config --email` – Establece el email del usuario.
- `git config --system` – Configura a nivel del sistema.
- `git config user.name` – Establece el nombre de usuario.
- `git config --list` – Lista todas las configuraciones.
- `git config --local` – Configura a nivel de repositorio.

## Comandos Merge
- `git merge` – Une ramas de desarrollo.
- `git merge <rama>` – Une una rama a la actual.
- `git merge --abort` – Cancela el proceso de merge.
- `git merge --continue` – Continúa un merge pausado.
- `git merge --squash` – Une todos los cambios como un solo commit.
- `git merge --no-commit` – Une sin hacer commit.
- `git merge --no-ff` – Fuerza un commit de merge.

## Comandos Pull
- `git pull` – Descarga y fusiona cambios del remoto.
- `git pull --quiet` – Oculta la salida.
- `git pull --verbose` – Muestra más detalles.
- `git pull --squash` – Une como un solo commit.
- `git pull --no-commit` – Fusiona sin hacer commit.
- `git pull --no-ff` – Siempre crea un commit.
- `git pull --all` – Descarga de todos los remotos.
- `git pull --depth=<prof>` – Descarga commits limitados.
- `git pull --dry-run` – Simula la acción.
- `git pull --prune` – Limpia referencias remotas eliminadas.
- `git pull --no-tags` – No descarga etiquetas.

## Comandos Push
- `git push` – Envía la rama actual al remoto.
- `git push <remoto> <rama>` – Envía una rama específica.
- `git push <remoto> --force` – Fuerza un push.
- `git push <remoto> --all` – Envía todas las ramas.
- `git push <remoto> --tags` – Envía todas las etiquetas.

## Comandos Rebase
- `git rebase <rama>` – Aplica los commits sobre otra rama.
- `git rebase --continue` – Continúa un rebase tras conflictos.
- `git rebase --skip` – Omite el conflicto.
- `git rebase --abort` – Cancela el rebase.
- `git rebase <rama> -i` – Rebase interactivo.

## Comandos Stash
- `git stash` – Guarda los cambios actuales sin hacer commit.
- `git stash list` – Lista los stashes guardados.
- `git stash show` – Muestra los cambios del último stash.
- `git stash drop <stash>` – Elimina un stash.
- `git stash pop <stash>` – Aplica y elimina un stash.
- `git stash apply <stash>` – Aplica un stash sin eliminarlo.
- `git stash clear` – Elimina todos los stashes.
