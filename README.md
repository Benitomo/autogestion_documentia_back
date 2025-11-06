# Proyecto: Autogestión Documentia (Backend)

## Descripción

Este es el servicio backend para la gestión de documentos de Documentia.

## Requisitos del Sistema

* **Versión de Python Requerida:** 3.10.13
* **Gestor de Entornos:** Se recomienda el uso de `pyenv` y `venv`.

## Configuración del Entorno de Desarrollo

1.  **Instalar la versión de Python requerida:**
    ```bash
    pyenv install 3.10.13
    pyenv local 3.10.13
    ```

2.  **Crear y activar el entorno virtual:**
    ```bash
    python -m venv venv
    source venv/bin/activate
    ```

3.  **Instalar las dependencias:**
    ```bash
    pip install -r requirements.txt
    ```


## Despliegue 

1. docker build -t autogestion-back:latest .
2. docker tag autogestion-back:latest us-docker.pkg.dev/co-impocali-cld-01/impocali-backend/autogestion-back:latest
3. docker push us-docker.pkg.dev/co-impocali-cld-01/impocali-backend/autogestion-back:latest
4. kubectl apply -f deployment.yaml
