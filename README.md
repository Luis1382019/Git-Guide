# Guia de Git y Github

- [Guia de Git y Github](#guia-de-git-y-github)
  - [Git](#git)
    - [Mis comandos](#mis-comandos)
    - [Importantes basicos](#importantes-basicos)
    - [Importantes](#importantes)
    - [Remoto](#remoto)
    - [Faltante de agregar](#faltante-de-agregar)
  - [Github](#github)

## Git

Seccion con comandos e instrucciones sobre git

### Mis comandos
**Stash**
- `git showstash` = git stash --list --decorate
  
**Configuracion**
- `git conf` = git config --global -e  
  
**Log**
- `git lg` = log formateado con graph, una linea y colores agradables

**Status**
- `git st` = status --short
  
### Importantes basicos

- **Iniciales**
  - `git init` = Crea el repositorio local
  - `git log` = Registro de los commits
  - `git status` = Estado del repositorio
  - `git add example.py` = Añade el archivo example al stage
  - `git init` = Crea el repositorio local
- **Modificadores**
  - `.` = Todo
  - `*.py` = Todos los archivos .py
  - `media/` = Todos los archivos de la carpeta media
- **Configuracion**
  - `git config --global -e` = Abre el archivo de configuracion global
    
  
### Importantes

- **Ammend**
  - `git commit --ammend -m "Hola"` = Modifica el ultimo commit(Y manda los archivos del stage en la modificacion)
  
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
  - `git branch -M main` = Cambia el nombre de la rama actual, -M la forza y -m lo intenta

### Remoto
- **Fetch**  
  - `git fetch aliasRepo rama` = Descarga los cambios del repositorio pero no los aplica automaticamente
  
- **Pull**  
  - `git pull aliasRepo rama` = Descraga y aplica los cambios del repositorio

- **Push**
  - `git push -u aliasRepo main` = Primer push de la rama(-u establece la relación de seguimiento)
  - `git push aliasRepo rama` = Mandar al repositorio remoto

- **Configuraciones**
  - `git remote rename alias aliasNuevo` = Cambia el nombre del aliasRepo  
  - `git remote add aliasRepo https://github.com/usuario/repositorio.git` = Conecta el repositorio actual con uno remoto

### Faltante de agregar
- git revert

## Github
Seccion con comandos e instrucciones sobre git

- Fork: Clona el repositorio en tu cuenta
  
   ![Fork](imagenes/fork.png)

- Code: Te da el codigo para clonar el repositorio
  - Nota: Es preferible con SSH  
  
   ![Code](imagenes/code.png)