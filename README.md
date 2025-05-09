# Practica Individual
Practica individual del curso de Git y Github de la Scesi
#
#
# Tema 1
# Introducción a Git

## ¿Qué es un control de versiones?

Es un sistema que registra los cambios hechos al código fuente.  
Permite llevar un historial detallado: qué se cambió, quién lo hizo y cuándo.

Beneficios:
- Recuperación de versiones anteriores.
- Colaboración sin sobrescribir trabajo.
- Seguimiento de errores y evolución del código.

## ¿Por qué es importante?

- **Rendimiento**: Solo guarda lo esencial.
- **Seguridad**: Cada cambio queda registrado.
- **Flexibilidad**: Permite trabajo paralelo y ramificación.

Es fundamental para cualquier equipo de desarrollo moderno.

# Breve historia de Git

## Evolución del control de versiones

- **1990**: CVS permite versionar archivos con números.
- **2005**: Linus Torvalds crea Git tras la caída de BitKeeper.
- **2008**: Nace GitHub, plataforma basada en Git.
- **2018**: Microsoft compra GitHub, generando debate.
- **2024**: Git domina el mercado. Se usa también en GitLab y Bitbucket.

Git fue diseñado para ser rápido, confiable y seguro, especialmente útil en proyectos distribuidos como el kernel de Linux.

# ¿Qué es Git?

Git es un sistema de control de versiones distribuido.  
Cada desarrollador tiene una copia completa del historial del proyecto.

Ventajas:
- Rápido y eficiente.
- Soporte para ramas y fusiones.
- Trabajo colaborativo sin conexión constante.

## ¿Qué es un repositorio?

Es donde Git guarda todo el historial de un proyecto.

Tipos:
- **Local**: en tu equipo.
- **Remoto**: en la nube, usando servicios como GitHub.

Son la base para trabajar con Git.

# Instalación y configuración básica de Git

1. Visita https://git-scm.com/downloads
2. Descarga el instalador según tu sistema.
3. Ejecuta el archivo y sigue las instrucciones.

Configuraciones clave:
- Seleccionar el editor (VSCode, Vim, etc.)
- Definir la rama principal como `main`.
- Usar Git Bash como terminal.
- Activar conexión SSH y OpenSSL.
- Habilitar caché para comandos más rápidos.
- No activar funciones experimentales.

Con esto, Git queda listo para usar en tu entorno.
#
# Tema 2
# Estados de los archivos en Git

Git maneja tres estados principales:

## 1. Modified (Modificado)
El archivo fue creado, editado o eliminado, pero los cambios no están preparados para un commit.

## 2. Staged (Preparado)
El archivo fue marcado con `git add` y está listo para ser confirmado en el repositorio local.

## 3. Committed (Confirmado)
El archivo ya fue confirmado en el repositorio local. Es como guardar el progreso del proyecto.

Estos estados ayudan a gestionar cambios de forma segura y organizada.

Permiten controlar qué archivos se agregan o no a un commit, evitando errores en el historial del proyecto.

# ¿Qué es un commit?

Un commit es un registro de cambios en el proyecto.

Piensa en él como una fotografía del estado del proyecto en un momento específico.

Cada commit contiene información: autor, fecha, mensaje descriptivo y contenido del cambio.

Son esenciales para trabajar en equipo, hacer seguimiento de la evolución del proyecto y recuperar versiones anteriores.

También pueden verse como puntos de restauración, como cuando se guarda una partida en un videojuego.

Este sistema permite experimentar sin miedo a perder avances importantes.

# Cómo hacer un commit y qué es el HEAD

## Hacer un commit:
1. Prepara archivos con `git add archivo.txt`
2. Ejecuta `git commit -m "Mensaje descriptivo"`

Un buen mensaje de commit explica claramente el cambio.

Ejemplo:
git add login.js
git commit -m "Corrige validación de campos en login"

## ¿Qué es el HEAD?
Es un puntero que indica en qué commit estás.

Actúa como un “Estás aquí” en un mapa del historial de Git.

El HEAD se actualiza con cada nuevo commit o cuando cambias de rama o commit.
#
# Tema3

# Ramas en Git

## ¿Qué es una rama?

Una rama es una versión paralela del código.  
Técnicamente, es un apuntador a un commit específico.

Permite trabajar sin afectar la rama principal, ideal para desarrollo de nuevas funciones o pruebas.

## ¿Para qué sirven?

- Fomentan el trabajo colaborativo.
- Permiten un flujo de trabajo no lineal.
- Separan funcionalidades o correcciones específicas.

Son clave para un desarrollo ordenado y seguro.

# Crear y fusionar ramas

## Crear una rama

Usa el comando:
git branch <nombre-rama>

## Fusionar ramas

Para integrar los cambios de una rama en otra, usamos:
git merge <nombre-rama>

Esto incorpora los commits de la rama seleccionada a la rama actual.

Las fusiones permiten consolidar el trabajo y mantener el historial del proyecto.

# Eliminar ramas y comandos útiles

## ¿Por qué eliminar ramas?

- Mantener limpio el repositorio.
- Las ramas deben tener un propósito puntual y corto.

Eliminar ramas que ya cumplieron su función es una buena práctica.

## Comandos útiles

- Ver ramas: `git branch` o `git branch -a`
- Eliminar rama: `git branch -d <nombre>`
- Cambiar de rama: `git switch <nombre>`
- Mezcla sin fast-forward: `git merge <rama> --no-ff`
- Cambiar con checkout: `git checkout <rama>`

# Conflictos en Git

## ¿Qué es un conflicto?

Ocurre cuando dos ramas modifican la misma línea de un archivo.

## ¿Cómo resolverlos?

Tienes tres opciones:
- Conservar cambios de `main`.
- Conservar cambios de la rama fusionada.
- Editar manualmente para combinar ambos cambios.

Al resolverlos, se guarda el archivo, se añade (`git add`) y se finaliza el merge con un commit.

Los conflictos son comunes y parte del trabajo colaborativo.
#
# Tema4

# ¿Git y GitHub son lo mismo?

**Git** es un sistema de control de versiones distribuido. Permite llevar un registro de los cambios realizados en archivos de código, facilitando la colaboración entre desarrolladores.

**GitHub**, en cambio, es una plataforma basada en la nube que permite alojar repositorios de Git.

GitHub proporciona herramientas adicionales como seguimiento de incidencias, integración continua, wikis y colaboración.

En resumen:
- Git es la herramienta de control de versiones.
- GitHub es un servicio que usa Git para facilitar la colaboración en línea.

También existen otras plataformas similares.

# ¿GitHub es único?

No, GitHub no es la única plataforma para alojar repositorios Git.

### Alternativas:
- **Bitbucket**: Plataforma de Atlassian orientada a proyectos privados.
- **GitLab**: Ofrece herramientas DevOps integradas, CI/CD y seguimiento de problemas.

Cada una tiene características distintas, pero todas permiten usar Git como sistema de control de versiones.

La elección entre ellas depende de las necesidades del equipo y del tipo de proyecto.
















