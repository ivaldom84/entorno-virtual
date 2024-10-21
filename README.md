# ENTORNO VIRTUAL 
# Instalación de un Entorno Virtual con pyenv

# Instalación de un Entorno Virtual con pyenv

Este documento describe cómo instalar `pyenv` y crear un entorno virtual en Windows, macOS y Linux.

## Requisitos Previos

Asegúrate de tener `git` instalado en tu sistema. Puedes descargarlo desde [git-scm.com](https://git-scm.com/).

## Instalación en Windows

1. **Instalar Git**:
   - Descarga e instala [Git para Windows](https://git-scm.com/download/win).

2. **Instalar pyenv-win**:
   - Abre PowerShell y ejecuta:
     ```bash
     git clone https://github.com/pyenv-win/pyenv-win.git $HOME/.pyenv
     ```

3. **Agregar pyenv a tu PATH**:
   - Abre tu perfil de PowerShell:
     ```bash
     notepad $PROFILE
     ```
   - Agrega las siguientes líneas:
     ```bash
     $env:PYENV = "$HOME\.pyenv"
     $env:Path += "$env:PYENV\bin;$env:PYENV\shims"
     ```

4. **Recargar tu perfil**:
   ```bash
   . $PROFILE
