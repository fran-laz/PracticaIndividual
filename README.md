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

# Navegando por GitHub

GitHub permite gestionar múltiples aspectos de los repositorios:

- **Repository > Code**: Archivos del repositorio.
- **Pull Requests**: Solicitudes de cambio.
- **Actions**: Automatización de flujos de trabajo.
- **Projects**: Gestión tipo kanban.
- **Wiki**: Documentación interna.
- **Security**: Vulnerabilidades.
- **Insights**: Estadísticas.
- **Settings**: Configuraciones del repo.

Además, GitHub permite buscar perfiles, proyectos y organizaciones fácilmente desde su interfaz.

# Repositorios remotos y SSH en GitHub

Los repositorios remotos permiten sincronizar cambios entre computadoras.

### Para conectar un repositorio local a uno remoto:
git remote add origin <url>
git push origin main


### Para usar SSH:
1. Generar key: `ssh-keygen -t rsa -b 4096 -C "tu.email@gmail.com"`
2. Activar el agente: `eval "$(ssh-agent -s)"`
3. Añadir key: `ssh-add ~/.ssh/id_rsa`
4. Copiar la clave pública y pegarla en GitHub.

También puedes clonar repositorios, crear ramas remotas y sincronizar cambios fácilmente con comandos Git.
#
# Tema5
# ¿Cuál es la diferencia entre git push y git pull?

## git push
Este comando se usa para enviar (empujar) los cambios desde el repositorio local al repositorio remoto.

Ejemplos:
- `git push origin main`: Empuja los cambios a la rama `main` remota.
- `git push -u origin rama`: Establece upstream.
- `git push -f`: Forzado (con precaución).
- `git push -d origin rama`: Elimina una rama remota.

## git pull
Este comando se usa para traer (jalar) cambios del repositorio remoto al local.

Ejemplos:
- `git pull`: Trae cambios de la rama remota relacionada.
- `git pull origin rama`: Desde rama específica.
- `git pull --all`: Trae de todas las ramas.

Ambos comandos mantienen sincronizados los repositorios locales y remotos.

# Experimentos con git push y git pull

## git push
- Puedes hacer push desde una rama secundaria a `main`.
- `git push -u` establece upstream: vincula la rama local a la remota.
- `git push -f` debe usarse con cuidado, puede sobrescribir cambios.
- `git push -d` permite eliminar ramas remotas que ya no se usan.

## git pull
- Puedes traer cambios desde otras ramas sin cambiar de rama local.
- También puedes traer múltiples ramas con un solo comando.
- `git pull` puede generar conflictos si hay cambios locales no sincronizados.
- Es buena práctica hacer `pull` antes de trabajar para evitar conflictos.

Estos experimentos ayudan a comprender mejor cómo fluye el trabajo entre local y remoto.

# ¿Qué es una Pull Request?

Una Pull Request (PR) es una solicitud para integrar cambios de una rama a otra dentro de un repositorio.

## ¿Cómo se hace una PR?
1. Subes tu rama con `git push`.
2. Luego:
   - GitHub puede sugerirte crear una PR automáticamente.
   - O puedes ir a la pestaña Pull Request y crearla manualmente.

## Buenas prácticas al hacer una PR
- Que el código esté enfocado en una sola funcionalidad.
- Explicar claramente los cambios realizados.
- Incluir imágenes, GIFs o videos puede ser muy útil.

## Revisar una PR
- Da feedback constructivo y claro.
- Considera el contexto del cambio, incluso si no es el código más elegante.
#
# Tema6
# ¿Qué es GitFlow?

GitFlow es una metodología para trabajar con Git de forma colaborativa y organizada.  
Fue propuesto por Vincent Driessen y establece un flujo de trabajo estándar que facilita  
el desarrollo en equipos, especialmente cuando hay múltiples versiones del producto en diferentes etapas.

En esencia, GitFlow define cómo y cuándo crear ramas para ciertas tareas como desarrollo de funciones,  
preparación para lanzamientos, corrección de errores y mantenimiento en producción.  
Promueve una estructura ordenada de ramas para minimizar conflictos y mejorar la trazabilidad.

Este flujo de trabajo establece ciertas ramas principales y su propósito en el ciclo de vida del proyecto,  
asegurando que cada cambio pase por un proceso lógico y predecible antes de llegar a producción.

GitFlow no es una herramienta, sino una convención de uso de Git.  
Sin embargo, existen herramientas que ayudan a implementarlo fácilmente en distintos entornos.

> Requiere disciplina y se recomienda para equipos con ciclos de desarrollo definidos.

# Ramas en GitFlow

GitFlow establece un conjunto de ramas bien definidas para organizar el desarrollo:

- `main` o `master`: contiene el código en producción, siempre estable.
- `develop`: incluye el código que está en integración y pruebas antes de liberarse.
- `feature`: ramas que nacen de `develop` para trabajar en nuevas funcionalidades.
- `release`: ramas temporales para preparar una versión estable desde `develop`.
- `hotfix`: ramas críticas que nacen desde `main` para corregir errores urgentes.

Cada rama tiene una función específica en el ciclo de vida del software,  
lo que facilita el mantenimiento, la colaboración y el control de calidad.

El flujo habitual consiste en trabajar en ramas `feature`, integrarlas en `develop`,  
crear una `release` para probar, y finalmente fusionar a `main` cuando esté listo.

Este sistema minimiza conflictos y mejora la estabilidad del producto en cada etapa.

# Flujos alternativos a GitFlow

Existen otros flujos de trabajo que se adaptan a diferentes necesidades de los equipos:

## GitHub Flow
Un flujo más simple y ágil. Solo utiliza `main` y ramas auxiliares que se integran mediante Pull Requests.  
Ideal para proyectos con despliegue continuo y necesidades de cambio frecuente.

## Trunk Based Development
Promueve una única rama (`main`) y ramas efímeras de vida muy corta.  
Depende fuertemente de un sistema CI/CD eficiente y de buenas prácticas de desarrollo.

## Ship / Show / Ask
Modelo basado en confianza y responsabilidad del equipo:
- **Ship**: se fusiona directamente a `main` sin revisión.
- **Show**: se revisa de manera automática y se fusiona.
- **Ask**: se abre una PR para discutir y revisar los cambios antes de integrar.

Este último modelo solo funciona en equipos maduros con buena comunicación,  
automatización de pruebas y responsabilidad individual clara.
#
# Tema7

# ¿Para qué sirven las buenas prácticas en Git?

Las buenas prácticas permiten que todo el equipo tenga un estándar de trabajo uniforme.  
Facilitan la colaboración, el entendimiento del historial de cambios y la resolución de problemas.  
Cuando se trabaja con muchas personas o se mantiene un proyecto a largo plazo,  
tener un historial limpio y coherente en los commits hace la diferencia.

Además, ayudan a prevenir errores comunes y fomentan una cultura de desarrollo más profesional.  
Un proyecto bien gestionado con buenas prácticas en Git se vuelve más fácil de escalar, mantener y revisar.

También permiten detectar errores más rápido y evitan que se generen conflictos innecesarios al momento de hacer merges.

# ¿Cada cuánto debería hacer un commit?

Lo ideal es hacer commits con frecuencia, pero con sentido.  
Cada commit debe representar una unidad lógica del trabajo realizado,  
como una función implementada o una corrección puntual.

Hacer commits frecuentes permite:
- Revertir cambios con facilidad.
- Detectar errores más rápido.
- Tener trazabilidad sobre el desarrollo.

Evita hacer un solo commit gigante que abarque demasiadas acciones distintas.  
En su lugar, divide los cambios en partes comprensibles y coherentes.

No significa que debas hacer un commit por cada línea,  
sino encontrar un punto medio con sentido técnico y práctico.

# Escribir buenos commits y nombres de ramas

Un buen commit tiene un mensaje claro, corto y en imperativo, por ejemplo:  
"Add login validation" o "Fix user profile bug".  
Evita usar más de 50 caracteres y no pongas punto final.

Usar prefijos semánticos ayuda a clasificar rápidamente los cambios:
- `feat:` nueva funcionalidad.
- `fix:` corrección de errores.
- `docs:` cambios en documentación.
- `refactor:` limpieza o mejora del código sin cambiar su funcionalidad.
- `style:`, `test:`, `perf:`, `ci:`, `build:` según el tipo de cambio.

En cuanto al nombre de la rama, debe ser:
- Claro, corto y descriptivo.
- Relacionado con lo que se va a hacer.
- Consistente con otras ramas del proyecto.
- Puede incluir un ID del sistema de tickets si se usa uno.

Ejemplo: `feat/login-form-validation` o `fix/issue-42-navbar`.
#
# Tema8

# ¿Cuándo deshacer cambios en Git?

Deshacer cambios en Git es útil cuando:
- El proyecto dejó de funcionar por un cambio reciente.
- Queremos recuperar una parte del código eliminado.
- Se borró un archivo importante por error.

No siempre se trata de errores graves; a veces solo queremos regresar a un punto anterior,  
ver cómo estaba un archivo o corregir una acción equivocada.

Existen comandos para estos casos, algunos afectan el historial y otros no.  
Elegir el correcto depende de lo que queremos lograr y si trabajamos solos o en equipo.

Siempre es buena práctica entender si el cambio será visible en el historial (no destructivo)  
o si va a modificarlo (destructivo), ya que esto puede afectar la colaboración con otras personas.

# Comandos para deshacer cambios en Git

Git ofrece distintos comandos para deshacer cambios, cada uno con un propósito específico:

## Comandos destructivos
Modifican el historial de commits.
- `git reset --soft HEAD~1`: Regresa al commit anterior pero conserva los cambios en el área de staging.
- `git reset --hard HEAD~1`: Elimina los cambios completamente.
- También se puede usar con un hash SHA específico.

## Comandos no destructivos
Conservan el historial.
- `git revert <SHA>`: Crea un nuevo commit que revierte los cambios del commit indicado.
- `git checkout <SHA> -- <archivo>`: Recupera un archivo o versión específica de un commit anterior.

**Consejo:**  
Usa `revert` si ya compartiste tus cambios con otros,  
y `reset` solo si estás trabajando en una rama local que nadie más usa.
#
# Tema9

# Hooks en Git

## ¿Qué es un Hook?
Los hooks en Git son scripts que permiten ejecutar acciones automáticas en respuesta a ciertos eventos. Son útiles para automatizar tareas, validar contenido, o integrar herramientas externas. Existen dos tipos: del lado del cliente y del servidor.

## Hooks del lado del cliente
Funcionan en tu repositorio local. Algunos ejemplos son:

- **pre-commit**: Ejecuta validaciones antes del commit. Útil para linters o evitar agregar demasiados archivos.
- **commit-msg**: Valida el contenido del mensaje del commit.
- **prepare-commit-msg**: Modifica automáticamente el mensaje del commit.
- **post-commit**: Ideal para notificaciones (como Slack) tras un commit exitoso.
- **pre-push**: Ejecuta pruebas antes de subir los cambios.
- **post-checkout/post-merge**: Limpian el entorno tras cambios de rama o fusiones.

## Hooks del lado del servidor
Operan en servidores remotos, como GitHub. Permiten mayor control sobre los pushes:

- **pre-receive**: Valida los commits antes de aceptarlos.
- **update**: Controla cambios en ramas o referencias específicas.
- **post-receive**: Notifica por correo o actualiza interfaces con nueva información del repositorio.

## Crear un Hook personalizado
1. Ubica la carpeta `.git/hooks`.
2. Crea un archivo con el nombre del hook deseado (ej. `pre-commit`).
3. Escribe el script deseado en bash, python u otro lenguaje.
4. Asegúrate de que tenga permisos de ejecución.

# Alias en Git

Un alias en Git permite acortar comandos repetitivos o complejos. Se configura de forma global o local, y ayuda a trabajar de forma más ágil.

### Ejemplos de configuración:
git config --global alias.co checkout
git config --global alias.cm "commit -m"


Esto te permite usar:

- `git co` → `git checkout`
- `git cm "mensaje"` → `git commit -m "mensaje"`

# Trucos en Git

## Guardar cambios temporalmente con git stash
- `git stash`: Guarda archivos modificados.
- `git stash -u`: Incluye archivos sin seguimiento.
- `git stash pop`: Restaura los cambios guardados.

## Aplicar un commit específico con cherry-pick
- `git cherry-pick <SHA>`: Aplica un commit de otra rama a la actual.

## Encontrar errores con git bisect
- `git bisect start` → Inicia la búsqueda.
- `git bisect bad` → Marca el commit actual como defectuoso.
- `git bisect good` → Marca un commit anterior como correcto.
- `git bisect reset` → Termina la búsqueda.

## Otros trucos útiles
- Modificar el último commit:
  `git commit --amend -m "nuevo mensaje"`

- Recuperar archivo de otra rama:
  `git checkout <SHA> <archivo>`






















