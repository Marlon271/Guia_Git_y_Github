# Guía de Git y GitHub

Este repositorio contiene una guía ilustrada (con capturas de pantalla) para aprender los pasos básicos de Git y su integración con GitHub. Cada sección se complementa con una imagen referencial en la carpeta `imagenes`.

---

# Guía de Git y GitHub

## Tabla de Contenido
- [1. Creación de cuenta en GitHub](#1-creación-de-cuenta-en-github)
- [2. Instalación de Git](#2-instalación-de-git)
- [3. Creación de un repositorio en GitHub](#3-creación-de-un-repositorio-en-github)
- [4. Apertura de la carpeta en Visual Studio Code](#4-apertura-de-la-carpeta-en-visual-studio-code)
- [5. Configuración inicial de Git](#5-configuración-inicial-de-git)
- [6. Creación de un Repositorio Local](#6-creación-de-un-repositorio-local)
- [7. Creación y primer commit del `README.md`](#7-creación-y-primer-commit-del-readmemd)
- [8. Creación de la carpeta `imagenes` y adición de recursos](#8-creación-de-la-carpeta-imagenes-y-adición-de-recursos)
- [Contribuciones](#contribuciones)
- [Recursos Adicionales](#recursos-adicionales)
- [Licencia](#licencia)


## 1. Creación de cuenta en GitHub

Para poder usar GitHub y alojar tus repositorios en la nube, lo primero es **crear una cuenta** en [GitHub](https://github.com/):

1. Ingresa a [github.com](https://github.com/) y haz clic en **Sign up** (o **Regístrate**).  
   ![Creación de cuenta en GitHub](imagenes/1.jpg)

2. Completa el formulario con tus datos (nombre de usuario, correo electrónico y contraseña).  
   ![Formulario de registro](imagenes/2.jpg)

3. Verifica tu correo si así lo requiere GitHub.

4. Una vez creada tu cuenta, podrás iniciar sesión.  
   ![Pantalla final de registro](imagenes/3.jpg)

---

## 2. Instalación de Git

Con tu cuenta de GitHub lista, necesitas **Git** instalado en tu computadora.

- **Windows / macOS**: descarga el instalador desde [git-scm.com](https://git-scm.com/) y sigue las instrucciones.
- **Linux (Ubuntu)**:  
  ```bash
  sudo apt update
  sudo apt install git
  ```

Para verificar la instalación, en la terminal ejecuta:
```bash
git --version
```

![Instalación de Git](imagenes/4.jpg)

---

## 3. Creación de un repositorio en GitHub

1. Inicia sesión en GitHub y haz clic en el botón **New** (o “Nuevo repositorio”).  
   ![Crear repositorio desde GitHub](imagenes/5.png)

2. Asigna el nombre que desees a tu repositorio.  
   ![Configurando el repositorio](imagenes/repositorio.jpg)

3. Deja las opciones por defecto (privado o público según prefieras) y, si gustas, puedes agregar una descripción. Luego haz clic en **Create repository**.

---

## 4. Apertura de la carpeta en Visual Studio Code

Para trabajar de forma cómoda, puedes usar **Visual Studio Code** (u otro editor):

1. Ubica tu carpeta de proyecto y, en la barra de direcciones, escribe `cmd` (en Windows) para abrir la terminal.  
   ![Abrir cmd](imagenes/6.png)

2. Cuando se abra la terminal, ejecuta:
   ```bash
   code .
   ```
   Esto abrirá VS Code en la carpeta actual.  
   ![Abrir Visual Studio Code](imagenes/7.png)

3. Verifica que aparezca la interfaz de VS Code con los archivos de tu carpeta.  
   ![Interfaz de Visual Studio Code](imagenes/9.png)

---

## 5. Configuración inicial de Git

Ahora configura tus credenciales para que Git asocie los commits a tu nombre y correo:

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tuemail@example.com"
```

> Asegúrate de usar el mismo correo que registraste en GitHub.

![Configuración inicial de Git](imagenes/8.png)

---

## 6. Creación de un Repositorio Local

1. Elige o crea una carpeta para tu proyecto.
2. Abre la terminal en esa carpeta y ejecuta:
   ```bash
   git init
   ```
   Esto creará la carpeta oculta `.git`, donde Git almacenará todo el historial.

---

## 7. Creación y primer commit del `README.md`

1. Crea un archivo `README.md` (puedes hacerlo desde el explorador de VS Code).
2. Añade y confirma (commit) los cambios:
   ```bash
   git add README.md
   git commit -m "Primer commit: agrega README"
   ```

El mensaje de commit describe los cambios que acabas de realizar.

![Primer commit del README](imagenes/10.png)

---

## 8. Creación de la carpeta `imagenes` y adición de recursos

Para mantener capturas de pantalla u otros recursos gráficos:

1. Crea la carpeta:
   ```bash
   mkdir imagenes
   ```
![Carpeta de imágenes en el repositorio](imagenes/11.png)

2. Añade la carpeta y sus contenidos a Git:
   ```bash
   git add imagenes
   git commit -m "Agregar carpeta imagenes con capturas"
   ```
![añade imágenes en el repositorio](imagenes/12.png)

---
## Mirar y hacer commit y pusch para mirar que se suban las imagenes


### Próximos pasos

- **Subir el repositorio local a GitHub**: conecta tu carpeta local con el repositorio remoto en GitHub usando `git remote add origin <URL>` y luego `git push -u origin main`.  
- **Crear y gestionar ramas**: si quieres mantener un flujo de trabajo ordenado, practica crear ramas (`git checkout -b desarrollo`) y luego fusionarlas (`git merge desarrollo`).  
- **Fork y Pull Requests**: colabora en otros repositorios forkeando su proyecto y proponiendo tus cambios con un Pull Request.

---

## Contribuciones

Si alguien desea contribuir a esta guía:

1. Hacer un **Fork** de este repositorio.  
2. Clonar el fork en su máquina local.  
3. Crear una rama nueva para sus cambios.  
4. Subir esa rama a su propio fork y abrir un **Pull Request** hacia este repositorio.

---

## Recursos Adicionales

- [Documentación oficial de Git](https://git-scm.com/doc)  
- [Guía para principiantes de Git y GitHub (freeCodeCamp en español)](https://www.freecodecamp.org/espanol/news/guia-para-principiantes-de-git-y-github/)

---


