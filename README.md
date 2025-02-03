# Mis comandos de git

- [Mis comandos de git](#mis-comandos-de-git)
  - [Creados por mi](#creados-por-mi)
  - [Pendientes](#pendientes)
  - [Remoto](#remoto)
  - [Investigar](#investigar)

## Creados por mi
**Stash**
- `git showstash` = git stash --list --decorate
  
**Configuracion**
- `git conf` = git config --global -e  
  
**Log**
- `git lg` = log formateado con graph, una linea y colores agradables

**Status**
- `git st` = status --short
  
## Pendientes
Comandos que aun no memorizo bien

- **Ammend**
  - `git commit --ammend -m "Hola"` = Modifica el ultimo commit(Y manda archivos del stage en la modificacion)
  
- **Stash**
  - `git stash` = stash  
    `git stash apply` = aplica el stash  
    `git stash pop` = aplica el stash y lo borra  
    `git stash drop` = borra el stash  

- **Reflog**
  - `git reflog` = Registro de los HEAD 

- **Reset:**
  - `--soft` = No cambia el stage ni el directorio
  - `--mixed` = Vacia el stage
  - `--hard` = Vacia el stage y el directorio

- **Tag**
  - `git tag etiqueta hashCommit`

- **Branch**
  - `gti branch -d mirama` = Eliminar ramas

## Remoto
- **Fetch**  
  - `git fetch *aliasRepo* *rama*` = Descarga los cambios del repositorio pero no los aplica automaticamente
  
- **Pull**  
  - `git pull *aliasRepo* *rama*` = Descraga y aplica los cambios del repositorio

- **Push**
  - `git push *aliasRepo* *rama*` = Mandar al repositorio remoto

- **Configuraciones**
  - `git remote rename alias aliasNuevo` = Cambia el nombre del aliasRepo

## Investigar
- git revert
