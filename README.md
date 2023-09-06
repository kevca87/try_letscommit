# Try `letscommit` with python
Este es un ejemplo de caso práctico del uso de la herramienta para generación automatica de mensajes commits `letscommit`.
Para probarlo debera clonar este repositorio con:
```
git clone https://github.com/kevca87/try_letscommit.git
```

## Instala las dependencias
Además de `letscommit` para este ejemplo se requiere tener instalado: git, Python y `pip`  para instalar las dependencias mediante los siguientes comandos:
1. Crear y activar un virtual environment
    ```
    python -m venv venv
    ```
    Windows (PowerShell o cmd)
    ```
    # In PowerShell
    venv\Scripts\Activate.ps1
    # In cmd.exe
    venv\Scripts\activate.bat
    ```
2. Instalar los requerimientos con el siguiente comando
    ```
    pip install -r requirements.txt
    ```
Esto instalará las librerias requeridas para el ejemplo.

## Crear una rama
Para mantener limpia la rama principal de este ejemplo ejecutar:
git checkout -b <nombre-de-tu-rama>

## Change, add & letscommit
Este repositorio presenta un proyecto básico de una API en Flask, que modificará simulando un proyecto real.
Si desea correr o reiniciar la aplicación use el comando:
```
python app.py
```
El proyecto muestra actualmente una aplicación web. La tarea es transformarla en una API, siguiendo los pasos:
1. Ve a `app.py` y copia el siguiente código.
    ```
    @app.route("/me")
    def me_api():
        return {
            "message":"Hello world!"
        }
    ```
2. A continuación ejecuta el comando:
    ```
    letscommit --start
    ```
    La herramienta te sugerirá 3 mensajes, elije uno ingresando un número, o 0 para escribir un mensaje propio.