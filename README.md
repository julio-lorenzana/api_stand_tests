# API Stand Tests - Urban Grocers

## Este proyecto contiene pruebas automatizadas para la API de Urban Grocers, específicamente para el endpoint de creación de usuarios. Las pruebas verifican diferentes escenarios de validación del campo `firstName`.

## Tecnologías Utilizadas
- **Python 3.13.3**
- **Pytest** - Framework de pruebas
- **Requests** - Para realizar peticiones HTTP a la API

## Estructura del Proyecto

api_stand_tests/
- **.gitignore**                 # Archivos a ignorar por Git.
- **configuration.py**           # Archivo de configuraciones de las rutas
- **create_user_test_py**        # Archivo principal con las pruebas
- **data.py**                    # Datos de prueba
- **README.md**                  # Este archivo
- **sender_stand_request.py**    # Funciones para enviar peticiones HTPP

## Casos de Prueba Incluidos
### Pruebas Positivas
- **Prueba 1:** firstname con 2 caracteres ("Aa")
- **Prueba 2:** firstname con 15 caracteres ("Aaaaaaaaaaaaaaa")

### Pruebas Negativas
- **Prueba 3:** firstname con 1 caracter ("A")
- **Prueba 4:** firstname con 16 caracteres ("Aaaaaaaaaaaaaaaa")
- **Prueba 5:** firstname con espacio ("A Aaa")
- **Prueba 6:** firstname con simbolos especiales ("\"N°%@\",")
- **Prueba 7:** firstname con string de números ("123")
- **Prueba 8:** Sin el firstname ()
- **Prueba 9:** firstname vacío ("")
- **Prueba 10:** firstname con números (12)

## Cómo Ejecutar las Pruebas
### Prerrequisitos
- Necesitas tener instalados los paquetes pytest y request para ejecutar las pruebas.
- Ejecuta todas las pruebas con el comando pytest.

2. Instalar las dependencias:
bash
pip install pytest requests

### Ejecutar todas las pruebas
bash
pytest create_user_test.py

### Ejecutar con salida detallada
bash
pytest create_user_test.py -v

### Ejecutar mostrando prints
bash
pytest create_user_test.py -s

## Configuración
Asegúrate de que la URL de la API esté correctamente configurada en el archivo sender_stand_request.py.

## Autor
[Tu nombre]

## Notas
Este proyecto fue desarrollado como parte del Sprint 6 del curso de QA Engineer.
```

Qué incluir específicamente
Para tu proyecto, te recomiendo agregar:

Tu información personal en la sección "Autor"
URL de la API si es pública
Resultados esperados de cada prueba
Capturas de pantalla de las pruebas ejecutándose (opcional)