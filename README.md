## ClimApp: Tu aplicación para revisar el clima

ClimApp es una sencilla aplicación web para consultar el clima. Utiliza Flask en el backend y se conecta a una base de datos para almacenar y recuperar información.

## Características

* Consulta del clima por ciudad.
* Diseño simple y limpio usando plantillas Jinja2.
* Servidor de desarrollo y producción usando Waitress.

## Instalación

1. Clona el repositorio:

```bash
git clone https://github.com/tu_usuario/climApp.git
```

2. Crea un entorno virtual (recomendado):

```bash
python3 -m venv venv
source venv/bin/activate  # En Linux/macOS
venv\Scripts\activate  # En Windows
```

3. Instala las dependencias:

```bash
pip install -r requirements.txt
```

4. Configura las variables de entorno (si es necesario).  Crea un archivo `.env` en la raíz del proyecto y define las variables que necesite la aplicación, como la clave de la API del clima o la configuración de la base de datos.  Por ejemplo:

```
API_KEY=tu_clave_api
DATABASE_URL=sqlite:///db/climApp.db
```

5. Ejecuta la aplicación:

```bash
python server.py
```

## Uso

Abre tu navegador web y ve a `http://127.0.0.1:5000/` (o el puerto que esté configurado en `server.py`).


## Capturas de Pantalla


![Pantalla principal](1.png)
![Página de resultados](2.png)
![Página sin resultados](3.png)


## Estructura del proyecto

* `climApp/`: Directorio principal de la aplicación ().
* `db/`: Contiene la base de datos.
* `static/`: Archivo estático CSS.
* `templates/`: Plantillas HTML para la interfaz de usuario.
* `.gitignore`: venv __pycache__.
* `requirements.txt`
* `server.py`: Archivo principal del servidor Flask.
* `weather.py`: La lógica para obtener y procesar datos del clima.

## Contribuciones

Las contribuciones son bienvenidas. Por favor, abre un *issue* o envía un *pull request*.

## Dependencias

blinker==1.6.2
certifi==2023.5.7
charset-normalizer==3.2.0
click==8.1.5
colorama==0.4.6
Flask==2.3.2
idna==3.4
itsdangerous==2.1.2
Jinja2==3.1.2
MarkupSafe==2.1.3
python-dotenv==1.0.0
requests==2.31.0
urllib3==2.0.3
waitress==2.1.2
Werkzeug==2.3.6
