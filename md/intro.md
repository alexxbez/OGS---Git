---
marp: true
theme: catppuccin.css
paginate: true
---

# Git y Github 

## Outer games Studios 🛰️

---

## Git y Github

Dentro de esta guía vamos a aprender que es _Git_ y _GitHub_, qué cosas nos permiten hacer y sus diferencias. Esta es simplemente una guía introductoria. 

---

## ¿Por qué?

Para entender mejor que son estas herramientas es conveniente primero entender que problema resuelven. 

---

## ¿Por qué?

Dentro de grandes bases de código (como los videojuegos) existe un gran problema para **colaborar** con otras personas. 

Imagina esto: **tu** editas un archivo para calcular la velocidad de un personaje. Este archivo se llama `personaje.gd`. Luego se lo pasas a tu **compañero** que también agrega algunas funcionalidades y lo llama `personaje_v1.md`. Sería horrible tener que guardar tantas versiones del mismo archivo. 

---

## ¿Por qué?

Ahora imagina esto: le pasas tu `personaje.gd` a **dos** compañeros. Uno de ellos crea su propio `personaje_v1.gd` y otro crea también su propia version de `personaje_v1.gd`. Ahora tienes dos archivos con el mismo nombre, pero diferente contenido. Cuando decidas integrarlo al proyecto, ¿cuál vas a integrar? ¡Eso es lo que resuelve Git!

---

## Git

Git es un programa que te ayuda a tener un control de versiones en tu proyecto. Permite tomar capturas _capturas_ de tu proyecto (como si fuera un screenshot del estado actual de tu proyecto), lo que te permite volver atrás y visitar _capturas_ pasadas.

---

## Git

Git también facilita la colaboración en proyectos, debido a que Git guarda la información de _quien_ realiza la captura. Esto nos ayuda a corregir el código cuando dos personas modifican lo mismo. 

---

## Git

Para lograr esto git usa un archivo (técnicamente directorio/folder) **mágico**: `.git/`. Más adelante veremos qué es lo que podemos hacer con este archivo y por qué es tan útil. Por ahora solo ten en mente que **toda** la funcionalidad de Git se basa en este sólo archivo mágico.

---

## GitHub

Ahora pasamos a **GitHub**. Quizá leyendo esto te diste cuenta de un problema: el archivo de Git sigue siendo **local**. Aunque Git me ayuda a tomar esos _screenshots_, para compartirlo a otras personas terminaría enviándolo por correo o mensaje, y terminaría con varios `proyecto_v1`, `proyecto_v4`, etc. ¡Esto es lo que GitHub resuelve!

Algo que se debe entender es que Git y GitHub **no** son la misma cosa. Esto es algo que muchos principiantes confunden, y es importante entender esta distinción. 

---

## GitHub

GitHub es una plataforma web que permite hostear y compartir proyectos de Git. Tiene muchas, MUCHAS más funcionalidades, pero esta es la función fundamental que tiene. GitHub es, en esencia, una plataforma dónde puedes subir archivos en la nube. Cualquier tipo de archivo se puede subir, y de esta forma se puede compartir. Cada _repositorio_ (vamos a entender qué es esto más adelante), es como si fuera un directorio/carpeta, y dentro de este folder puedes tener varios archivos.

Esto es similar a un Google Drive. Puedes tener varias carpetas, y dentro de esas carpetas guardar varios tipos de archivos. 

---

## GitHub

Pero GitHub se especializa en un tipo de carpeta: aquellas que tengan el directorio mágico: `.git/`. Todo proyecto de programación en GitHub tiene este archivo mágico. De ahí viene el nombre, GitHub es un _Hub_ dónde se pueden hostear proyectos con `.git/`.

--- 

## Recap

Para recapitular:

- Git te ayuda a tomar _screenshots_ de tu proyecto
- Git utiliza un directorio mágico `.git/`

- GitHub es un lugar para hostear proyectos que usan Git.
- GitHub es un google drive con muchos proyectos con `.git/`

--- 

# ¡Gracias!

## Siguiente parte: Instalación
