# FastApi Ejemplo

Ejemplo de aplicación FastApi con uso de ORM (SQLlchemy) que accede a BD sqlite.
La aplicación por defecto espera conexiones em el puerto 8000

## Prueba aplicación en local

1. Desplegar
    ```console
    $ python3 -m venv venv
    $ source venv/bin/activate
    (venv) $ pip install -r requirements.txt 
    (venv) $ cd src 
    (venv) src $ rm students.db  
    (venv) src $ python crea_db.py 
    ...
    (venv) src $ uvicorn app:app --host 0.0.0.0
    ``` 
2. Acceder a `http://localhost:8000/docs` para ver la documentación de la API y probar las distintas rutas definidas. Por ejemplo:
   * http://localhost:8000/docs
   * http://localhost:8000/students
   * http://localhost:8000/students/2
   


