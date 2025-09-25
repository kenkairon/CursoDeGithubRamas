# Creación de Ramas

## Primero 
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
