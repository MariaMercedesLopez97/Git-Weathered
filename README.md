Proyecto de Consulta de Clima CLI

Este es un script en Python para consultar el clima de una ubicación específica utilizando la API de OpenWeatherMap. El script acepta la ciudad como argumento y te permite seleccionar el formato de salida (JSON, texto o CSV). Además, puedes optar por guardar los resultados en un archivo.

Requisitos
 
- Python 3.x
- Una cuenta de [OpenWeatherMap](https://openweathermap.org/) para obtener la clave de API.
- Un archivo `.env` con la clave de API configurada:

```bash
API_KEY=tu_clave_aqui

Instalacion

1- Clonar el repositorio
git clone https://github.com/tu_usuario/tu_proyecto.git
cd tu_proyecto

2- Crear un Entorno Virtual
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate

3- Instalar las Dependencias
pip install -r requirements.txt

4- Crear un archivo .env en la raíz del proyecto e introducir tu clave de API:
API_KEY=tu_clave_aqui

Uso

EL script acepta dos argumentos obligatorios: la ciudad y el formato de salida, además de una opción para guardar los resultados en un archivo.

python clima.py <ciudad> <formato> [--guardar]

Ejemplos

1- Obtener el clima de Madrid en formato JSON:
python clima.py Madrid json

2-Obtener el clima de Nueva York en formato de texto:
python clima.py "New York" texto

3- Guardar el clima de Tokio en un archivo CSV:
python clima.py Tokio csv --guardar

Formatos de salida 

JSON: muestra los resultados en formato JSON.
Texto: muestra los resultados como texto.
CSV: muestra los resultados como una tabla en formato CSV.

Posibles Errores

Error HTTP: Ocurre si hay un problema con la solicitud HTTP (p. ej., la ciudad no es encontrada).
Error de conexión: Indica que hay problemas de red.
Error inesperado: Cualquier otro tipo de error será mostrado con este mensaje.
