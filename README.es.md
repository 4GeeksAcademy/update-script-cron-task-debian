---
title: "Creando una red NAT en VirtualBox"
subtitle: "Realizarás una red privada entre maquinas virtuales con traducción hacia la red del anfitrión, en lo que se conoce como una 'Red NAT'."
tags: ["cybersecurity"]
authors: ["arnaldoperez"]
---

# Networking on VirtualBox

<!-- hide -->
<a href="https://www.4geeksacademy.co"><img height="280" align="right" src="https://github.com/4GeeksAcademy/installing-windows-on-virtual-machine/blob/master/js-bg-badge.png"></a>

> By [@arnaldoperez](https://github.com/arnaldoperez) and [other contributors](https://github.com/4GeeksAcademy/networks-on-virtualbox/contributors) at [4Geeks Academy](https://4geeksacademy.co/)

![last commit](https://img.shields.io/github/last-commit/4geeksacademy/installing-windows-on-virtual-machine)
[![build by developers](https://img.shields.io/badge/build_by-Developers-blue)](https://4geeks.com)
[![build by developers](https://img.shields.io/twitter/follow/4geeksacademy?style=social&logo=twitter)](https://twitter.com/4geeksacademy)

*Estas instrucciones [están disponibles en 🇪🇸 español](https://github.com/4GeeksAcademy/networks-on-virtualbox/blob/master/README.es.md) :es:*
<!-- endhide -->

## Consigna

El estudiante debe crear un script en bash para actualizar la lista de repositorios y los paquetes. El script debe tener permisos de ejecución y el usuario debe estar en el grupo sudoers

## Entregable

- Archivo con el script
- Demostración de su funcionamiento

## TODO:

- Repo con instrucciones

<!-- hide -->

#### Antes de empezar...

> ¡Te necesitamos! Estos ejercicios se crean y mantienen en colaboración con personas como tú. Si encuentras algún error o falta de ortografía, contribuye y/o repórtalo.

## Instalación en un clic (recomendado)

Puedes empezar estos ejercicios en pocos segundos haciendo clic en: [Abrir en Codespaces](https://codespaces.new/?repo=4GeeksAcademy/html-forms-tutorial-exercises) (recomendado) o [Abrir en Gitpod](https://gitpod.io#https://github.com/4GeeksAcademy/html-forms-tutorial-exercises.git).

> Una vez ya tengas abierto VSCode, los ejercicios de LearnPack deberían empezar automáticamente, si esto no sucede puedes intentar empezar los ejercicios escribiendo este comando en tu terminal: `$ learnpack start`

## Instalación local:

Clona el repositorio en tu ambiente local y sigue los siguientes pasos:

1. Instala LearnPack, el package manager para tutoriales de aprendizaje y el HTML compiler plugin para LearnPack, asegúrate también de tener node.js 14+:

```bash
$ npm i learnpack -g
$ learnpack plugins:install learnpack-html
```

2. Descarga estos ejercicios en particular usando LearnPack y luego `cd` para entrar en la carpeta:

```bash
$ learnpack download html-forms-tutorial-exercises
$ cd html-forms-tutorial-exercises
```

> Nota: Una vez que termines de descargar, encontrarás una carpeta "exercises" que contiene todos los ejercicios.

3. Inicializa el tutorial/ejercicios ejecutando el siguiente comando en el mismo nivel donde se encuentra tu archivo learn.json:

```bash
$ npm i jest@24.8.0 -g
$ learnpack start
```
<!-- endhide -->

## ¿Cómo están organizados los ejercicios?

Cada ejercicio es una pequeña aplicación de React que contiene los siguientes archivos:

1. **index.js:** representa el archivo de entrada para toda la aplicación.
2. **README.md:** contiene las instrucciones de los ejercicios.
3. **test.js:** no tienes que abrir este archivo, contiene el script del test para el ejercicio.

> Nota: Los ejercicios son autograduados, pero los tests son muy rígidos y estrictos, mi recomendación es que no prestes demasiada atención a los tests y los uses solo como una sugerencia o podrías frustrarte.

## Colaboradores
 
Gracias a estas personas maravillosas ([emoji key](https://github.com/kentcdodds/all-contributors#emoji-key)):

1. [Arnaldo Perez (arnaloperez)](https://github.com/arnaloperez) cotribución: (build-tutorial) ✅, (documentación) 📖
  
2. [Alejandro Sanchez (alesanchezr)](https://github.com/alesanchezr),  contribución: (detector bugs) 🐛

3. [Lorena Gubaira (lorenagubaira)](https://github.com/lorenagubaira), contribution: (detector bugs) 🐛, contribution: (editor), (tranducción) 🌎

Este proyecto sigue la especificación [all-contributors](https://github.com/kentcdodds/all-contributors). ¡Todas las contribuciones son bienvenidas!

Este y otros ejercicios son usados para [aprender a programar](https://4geeksacademy.com/es/aprender-a-programar/aprender-a-programar-desde-cero) por parte de los alumnos de 4Geeks Academy [Coding Bootcamp](https://4geeksacademy.com/us/coding-bootcamp) realizado por [Alejandro Sánchez](https://twitter.com/alesanchezr) y muchos otros contribuyentes. Conoce más sobre nuestros [Cursos de Programación](https://4geeksacademy.com/es/curso-de-programacion-desde-cero?lang=es) para convertirte en [Full Stack Developer](https://4geeksacademy.com/es/coding-bootcamps/desarrollador-full-stack/?lang=es), o nuestro [Data Science Bootcamp](https://4geeksacademy.com/es/coding-bootcamps/curso-datascience-machine-learning).
