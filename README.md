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

---






