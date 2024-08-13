# Recomendador de Libros

Este proyecto es un recomendador de libros que utiliza un archivo CSV con datos de libros y sus géneros. Para poder utilizar el recomendador, es necesario seguir los siguientes pasos.

## Requisitos

- Python 3.x
- Bibliotecas necesarias (puedes instalar las dependencias ejecutando `pip install -r requirements.txt`)

## Configuración

1. **Descargar el archivo CSV**

   Debes descargar el archivo `Goodreads_books_with_genres.csv`, que se encuentra adjunto en este repositorio.

2. **Cambiar la dirección de lectura del archivo CSV**

   En el código del recomendador, localiza la línea donde se carga el archivo CSV y modifica la ruta de acceso para que apunte al archivo descargado. Asegúrate de que el nombre del archivo y la extensión sean correctos. Ejemplo:

   ```python
   # Antes
   df = pd.read_csv("ruta/anterior/Goodreads_books_with_genres.csv")

   # Después
   df = pd.read_csv("ruta/nueva/Goodreads_books_with_genres.csv")
