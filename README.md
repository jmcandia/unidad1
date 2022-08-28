# Programación Back-End, Unidad 1: Tecnologías del lado del Servidor

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

## Prerequisitos

Antes de clonar el repositorio y poder ejecutar el proyecto, se debe instalar [Python](https://python.org) en el sistema operativo.

## Instalación

1. Clonar el proyecto:

   ```bash
   git clone https://github.com/jmcandia/unidad1.git
   ```

2. Ir al directorio del proyecto:

   ```bash
   cd unidad1
   ```

3. Luego, debemos instalar `virtualenv` para crear un entorno virtual.

   ```bash
   # Se actualiza pip a la última versión
   python3 -m pip install --upgrade pip
   # Se instala virtualenv
   pip install virtualenv
   ```

   Una vez instalado, se crea un entorno virtual, dentro del directorio del proyecto:

   ```bash
   virtualenv env
   ```

   Si recibe el siguiente mensaje de error al ejecutar el comando anterior:

   ```cmd
   "virtualenv" no se reconoce como un comando interno o externo,
   programa o archivo por lotes ejecutable.
   ```

   O bien, si recibe el siguiente mensaje de error:

   ```ps1
   virtualenv: The term 'virtualenv' is not recognized as a name of a cmdlet, function, script file, or executable program.
   Check the spelling of the name, or if a path was included, verify that the path is correct and try again.
   ```

   Entonces debe ejecutar el comando:

   ```cmd
   python3 -m virtualenv env
   ```

   Para activar el entorno virtual, se debe ir al directorio del proyecto y ejecutar el comando:

   En linux:

   ```bash
   source env/bin/activate
   ```

   En windows:

   ```cmd
   env\Scripts\activate.bat
   ```

   Una vez activado, el nombre del actual ambiente aparece a la izquierda de la consola:

   En linux:

   ```bash
   (env) usuario@equipo:~/unidad1$
   ```

   En windows:

   ```cmd
   (env) C:\unidad1>
   ```

   Para salir del entorno virtual, se debe ejecutar el comando:

   ```bash
   deactivate
   ```

   > **Nota:** Este paso es opcional, pero sirve para no tener que instalar los paquetes en la instancia del usuario.

4. Ahora es momento de instalar los paquetes necesarios para el proceso:

   ```bash
   pip install -r requirements.txt
   ```

   > **Nota:** Si está usando el entorno virtual, debe asegurarse de activarlo previamente.

## Ejecución

Para ejecutar el proceso, debemos ejecutar el siguiente comando:

```bash
python3 manage.py runserver
```

## Authors

José Miguel Candia

- [GitHub](https://github.com/jmcandia)
- [Twitter](https://twitter.com/jmcandia)
- [LinkedIn](https://linkedin.com/in/jmcandia/)
