---
marp: true
theme: catppuccin.css
paginate: true
---

# Instalación

## Outer games Studios 🛰️

---

## Introducción

Antes de ver a fondo las capacidades de Git y GitHub, conviene instalar todo lo necesario. Esta guía ayuda con la instalación.

---

## ¿Qué?

Se mencionó en la guía pasada, pero Git es un programa. Esto quiere decir que se debe instalar en tu máquina. GitHub, por el contrario, es una página web, por lo que no se debe de instalar localmente. Esta guía se enfoca en instalar Git. 

Antes de nada, cabe recalcar que mucha de la funcionalidad de Git es a través de la terminal. ¡No le tengas miedo! Va a ser tu mejor amiga durante toda tu carrera. 

---

## Plataforma 

La instalación es diferente para cada plataforma. A continuación mostramos cómo se instala en cada plataforma.

---

### Windows

Visita la página de [Git](https://git-scm.com/downloads/win), y elige la versión correcta. Durante la instalación sigue los pasos, y ¡listo!

Para comprobar la instalación, abre tu terminal (cmd, no necesariamente la de git que acabas de instalar), y ejecuta el comando:

```
git --version
```

---

### MacOS

Si tu Mac es relativamente nueva, seguramente ya tienes instalado Git. Para comprobar puedes ejecutar en tu terminal el siguiente comando:

```zsh
git --version
```

Si aparece un error es porque no tienes Git instalado. La siguiente slide muestra como instalarlo.

---

### MacOS

Primero debemos de instalar Homebrew. Homebrew es un _Package Manager_, lo que te permite instalar varias cosas mediante la terminal. Para esto solo visita su [página oficial](https://brew.sh/). 

La forma tradicional es utilizando el comando que aparece en la página, lo copias y lo ejecutas en tu terminal. Después debes seguir ciertas instrucciones para configurar todo. 

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Pero **no** es necesario hacer esto. Puedes ir al link que aparece, descargar el `pkg` desde GitHub.

![Image](./../img/homebrew.png)

Nota: srry por la calidad xd. Tmb sorry por no poner el link, se actualiza constantemente. 

---

### MacOS

Si todo se instaló correctamente puedes ejecutar el siguiente comando:

```zsh
brew install git
```

¡Y listo! Confirma tu instalación con:

```zsh
git --version
```

---

### Linux

me reúso a creer que alguien que usa Linux no sabe instalar Git.

--- 

## Setup

¡Fuiste engañado! Esta no solo es una guía para la instalación, también es una guía para configurar todo. 

Primero configuraremos Git, y después conectaremos Git con GitHub. 

---

## Setup

La configuración esencial para Git son tus credenciales, cada que hagas un _screenshot_ va a aparecer esta información acerca de ti. Simplemente ejecuta estos comandos:

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

Ingresa tu nombre y tu correo en los parámetros, y ¡listo!

---

## Setup

Acabamos de instalar Git, pero hay que recordar que vamos a usar GitHub, por lo que necesitamos linkear ambos. Existen dos métodos, SSH y HTTP. SSH es generalmente mejor, pero es un poco más complicado de configurar en windows, por lo que usaremos HTTP para windows y SSH para mac y linux.

---

### Windows

Para esto ya debes de tener una cuenta en GitHub. Dentro de la página ve a tu `perfil > settings > developer settings > personal access tokens > tokens (classic)` y genera un nuevo token. Cuando generes tu nuevo token, **copialo** inmediatamente y **guardalo** en un lugar seguro. Cada vez que intentes hacer una acción que involucre a GitHub se te pedirá. 

Nuevamente, SSH es mejor que HTTP, por lo que si te interesa puedes investigar acerca de cómo configurar SSH en Windows (o pregúntale a chat). Debido al alcance de esta guía, no se puede explicar el proceso para windows.

---

### MacOS y Linux

El proceso para mac y linux es virtualmente el mismo. Para esto ya debes de tener una cuenta en GitHub. Primero debes generar tu clave SSH. Para esto, dentro de tu terminal, ejecuta el comando:

```bash
ssh-keygen -t ed25519 -C "your.email@example.com"
```
 
Esto genera dos claves, tu clave pública y tu clave privada. Recuerda, solo comparte tu clave **pública**. 

Ahora ejecuta el siguiente comando:

```bash
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
```

Esto añade tu clave al sistema.

---

### MacOS y Linux

Finalmente sólo queda compartirle tu clave pública a GitHub. Para esto ejecuta:

```bash
cat ~/.ssh/id_ed25519.pub
```

Y copia todo el texto que aparece. Esta es tu clave pública. Abre tu sesión en GitHub, navega a `perfil > settings > ssh and gpg keys > new ssh key` y pega tu clave pública. ¡Y listo! Ya estas listo para usar Git. 

---

## Recap

En esta guía aprendimos a instalar y configurar Git. No te preocupes si no entendiste todos los comandos o instrucciones, es algo que se aprende con la práctica. Si algo no funcionó o te atoraste en algún paso, no dudes en contactarnos, estamos dispuestos a ayudarte. 

---

# ¡Gracias!

## siguiente parte: Git Básico
