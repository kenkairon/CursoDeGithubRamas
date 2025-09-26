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

# 📝 Ejercicios de ramas en Git

Este documento contiene diferentes ejercicios prácticos para aprender y reforzar el trabajo con **ramas en Git**.  

---

## 📌 1. Crear ramas (E-Commerce)

1. Ve al siguiente link (**cuidado, si recargas se borra el gráfico**):  
   👉 https://git-graph-creator.netlify.app/
2. Crea las ramas de acuerdo a las siguientes tareas asignadas:

### 📄 Tareas asignadas
| Nº | Tarea                                    | Persona | Página     |
|----|------------------------------------------|---------|------------|
| 1  | Base de la página (header, body y footer) | Pedro   | Home       |
| 2  | Crear el menú                             | Karla   | Home       |
| 3  | Crear el banner                           | Jose    | Home       |
| 4  | Lista de productos                        | Karla   | Productos  |
| 5  | Ubicación de la empresa con Google Maps   | Pedro   | Contacto   |
| 6  | Redes sociales de la empresa              | Jose    | Contacto   |
| 7  | Formulario de contacto                    | Karla   | Contacto   |

### 🔀 Flujo de trabajo
4. Crea una rama `Home`  
5. Crea una rama `Productos`  
6. Crea una rama `Contacto`  
7. Realiza las tareas 1, 2 y 3  
8. Integra las tareas de **Home** a `master`  
9. Karla se atrasó en la tarea 4 → integra los cambios de `Home` en `Productos`  
10. Karla termina la tarea 4 e integra `Productos` a `master`  
11. La rama `Contacto` debe integrar todo lo de **Home** y **Productos**  
12. Realiza las tareas 5, 6 y 7  
13. Integra las tareas de `Contacto` a `master`  

---

## 📌 2. Ejercicio ramas (Agencia de viajes)

1. Ve al siguiente link (**cuidado, si recargas se borra el gráfico**):  
   👉 https://git-graph-creator.netlify.app/
2. Crea las ramas de acuerdo a las siguientes tareas asignadas:

### 📄 Tareas asignadas
| Nº | Tarea                                    | Persona | Página     |
|----|------------------------------------------|---------|------------|
| 1  | Base de la página (header, body y footer) | Pedro   | Home       |
| 2  | Buscador de viajes                        | Laura   | Home       |
| 3  | Paquetes del mes                          | Karla   | Home       |
| 4  | Reseñas de clientes                       | Jose    | Home       |
| 5  | Equipo de la empresa                      | Laura   | Nosotros   |
| 6  | Misión                                    | Jose    | Nosotros   |
| 7  | Visión                                    | Pedro   | Nosotros   |
| 8  | Tabla para cotizar viajes                 | Pedro   | Cotizar    |
| 9  | Redes sociales de la empresa              | Jose    | Contacto   |
| 10 | Formulario de contacto                    | Karla   | Contacto   |

### 🔀 Flujo de trabajo
4. Crea una rama `home`  
5. Crea una rama `nosotros`  
6. Crea una rama `cotizar`  
7. Realiza las tareas 5, 6 y 7  
8. Integra **nosotros** a `master`  
9. El feature `home` se atrasó → integra cambios de `nosotros` en `home`  
10. Realiza tareas 1, 2, 3 y 4  
11. Integra **home** a `master`  
12. Crea la rama `contacto` desde `master`  
13. Realiza tareas 9 y 10  
14. Integra **contacto** a `master`  
15. El feature `cotizar` se atrasó → integra cambios de `master` en `cotizar`  
16. Realiza la tarea 8  
17. Integra **cotizar** a `master`  

📷 Sube tu captura aquí:  
👉 https://drive.google.com/drive/folders/1NKK1xt-zE9pnviI5UEkrPpGP6sISefnA?usp=sharing  

---

## 📌 3. Trabajar ramas en código (E-Commerce)

1. Crea un repositorio `e-commerce` en GitHub  
2. Crea una carpeta `e-commerce` en tu escritorio y ábrela en VS Code  
3. Crea un archivo `index.html`  
4. Agrega el siguiente código:

```html
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>E-Commerce</title>
  </head>
  <body>
  </body>
</html>
```
5. Inicia Git y mueve los cambios al área de preparación

6. Realiza la confirmación

7. Conecta el repositorio local con el remoto (origin)

8. Realiza push para subir los cambios

9. Visualiza cambios en 👉 https://html-preview.github.io/

10. Checa las ramas que tienes

11. Crea la rama Home

12.Verifica las nuevas ramas

13. En Home, agrega el menú:
```html
<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.1/jquery.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
<link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet"/>
<nav class="navbar navbar-inverse">
  <div class="container-fluid">
    <div class="navbar-header">
      <a class="navbar-brand" href="#">Home</a>
      <a class="navbar-brand nv1" href="#">Productos</a>
      <a class="navbar-brand nv1" href="#">Contacto</a>
    </div>
  </div>
</nav>
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