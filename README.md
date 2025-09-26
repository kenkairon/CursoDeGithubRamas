# Creación de Ramas
![imagen](image/nombreimagen.png)
## Primero creamos  
1. En GitHub, haz clic en **New**`
2. Nombre: `CursoDeGithubRamas`
3. Descripción: *Educacion y Aprendizaje*
4. Clic en ***Create repository***

## Segundo
1. En repositorio local creamos la carpeta 03CursoGitRamas
```sh
mkdir 03CURSOGITRAMAS
code .
git init
git add .
git commit -m "Agregar archivo README.md"
git remote add origin git@github.com:kenkairon/CursoDeGithubRamas.git
git remote -v
git branch -m main
git push -u origin main
```

## Crear y Listar ramas

```bash 
# Listar todas las ramas locales
git branch
# Listar ramas locales y remotas
git branch -a
# Crear una nueva rama
git branch nombre-rama
# Crear y moverse a una nueva rama
git checkout -b nombre-rama
```

## Cambiar de Rama
```bash
# Cambiar a una rama existente
git checkout nombre-rama

# Desde Git 2.23 también se puede usar:
git switch nombre-rama

```

## Fusionar ramas con Merge

```bash
# Cambiar a la rama principal
git checkout main

# Fusionar una rama con main
git merge nombre-rama

```

## Eliminar Ramas
```bash
# Eliminar rama local
git branch -d nombre-rama

# Forzar eliminación local
git branch -D nombre-rama

# Eliminar rama remota
git push origin --delete nombre-rama

```
## Rebase(Alternativa de merge)

```bash
# Mover commits de una rama sobre otra
git checkout nombre-rama
git rebase main

```
## Actualizar tu rama con cambios de main
```bash
# Estando en tu rama
git checkout nombre-rama

# Traer cambios de main a tu rama
git pull origin main

```
## Flujo de Trabajo Recomendado

### 1- Crear rama desde main

```bash
git checkout -b feature/nueva-funcionalidad

```
### 2- Trabajar y hacer commits
```bash
git add .
git commit -m "feat: nueva funcionalidad"

```
### 3- Subir la rama al repositorio
```bash
git push -u origin feature/nueva-funcionalidad

```
### Crear Pull Request (PR) en GitHub/GitLab

### Revisar y aprobar cambios

## Fusionar con main y eliminar la rama