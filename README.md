# Guía Básica sobre Git

## Introducción a Git
Git es un sistema de control de versiones distribuido utilizado para gestionar el historial de cambios de un proyecto, especialmente en el desarrollo de software. Permite a múltiples personas colaborar en el mismo proyecto al mismo tiempo sin conflictos.

## Instalación de Git
### En Windows
1. Descarga Git desde [git-scm.com](https://git-scm.com/).
2. Ejecuta el instalador y sigue las instrucciones del asistente de instalación.
3. Verifica la instalación abriendo la terminal (Git Bash) y escribiendo `git --version`.

### En Mac
1. Abre la terminal.
2. Instala Homebrew (si no está instalado): `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
3. Instala Git con Homebrew: `brew install git`
4. Verifica la instalación: `git --version`.

### En Linux
1. Abre la terminal.
2. Utiliza el gestor de paquetes de tu distribución (ejemplo para Ubuntu/Debian): `sudo apt-get install git`.
3. Verifica la instalación: `git --version`.

## Configuración Inicial
1. Configurar el nombre de usuario:
   ```sh
   git config --global user.name "Tu Nombre"
   ```
2. Configurar el correo electrónico:
   ```sh
   git config --global user.email "tuemail@ejemplo.com"
   ```

## Comandos Básicos de Git
### Clonar un Repositorio
   ```sh
   git clone <url-del-repositorio>
   ```
   Esto descarga una copia del repositorio en tu sistema local.

### Ver el Estado del Repositorio
   ```sh
   git status
   ```
   Muestra los cambios que han sido hechos pero no confirmados.

### Añadir Archivos a la Zona de Staging
   ```sh
   git add <archivo>
   ```
   Puedes añadir todos los cambios con `git add .`.

### Confirmar Cambios
   ```sh
   git commit -m "Mensaje de confirmación"
   ```

### Ver el Historial
   ```sh
   git log
   ```

### Sincronizar Cambios
#### Recuperar Cambios del Repositorio Remoto
   ```sh
   git pull
   ```
#### Enviar Cambios al Repositorio Remoto
   ```sh
   git push
   ```

## Ramas en Git
### Crear una Nueva Rama
   ```sh
   git branch <nombre-de-la-rama>
   ```

### Cambiar de Rama
   ```sh
   git checkout <nombre-de-la-rama>
   ```

### Fusionar Ramas
   ```sh
   git merge <nombre-de-la-rama>
   ```
   Esto fusiona la rama especificada en la rama actual.

### Lista de Ramas
   ```sh
   git branch
   ```

## Solución de Conflictos
1. Git marcará el archivo conflictivo.
2. Edita el archivo para resolver el conflicto.
3. Añade el archivo resuelto a la zona de staging: `git add <archivo>`.
4. Confirma el cambio: `git commit -m "Resuelve conflicto en <archivo>"`.

## Buenas Prácticas
- Realiza commits frecuentemente con mensajes claros.
- Utiliza ramas para desarrollar nuevas funcionalidades.
- Sincroniza tus cambios regularmente con `git pull` y `git push`.
- Revise las diferencias antes de confirmar con `git diff`.

## Recursos Adicionales
- [Documentación oficial de Git](https://git-scm.com/doc)
- [Pro Git Book](https://git-scm.com/book/en/v2)
- [GitHub Learning Lab](https://lab.github.com/)

Esta guía proporciona una introducción básica a Git, pero hay muchas más funcionalidades que puedes explorar y aprender según tus necesidades y experiencia.

