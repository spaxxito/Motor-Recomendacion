# Recomendador de Libros

Este proyecto es un recomendador de libros que utiliza un archivo CSV con datos de libros y sus géneros. Para poder utilizar el recomendador, es necesario seguir los siguientes pasos.

## Requisitos

- Python 3.x
- Bibliotecas necesarias ( son bibliotecas muy comunes, pero de ser necesario, puedes instalar las dependencias ejecutando `pip install -r requirementsreco.txt`)

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

3. **Uso**
   Al final del notebook, aparecerán 3 pestañas entre las cuales elegir para decidir a partir de que valor quieres recibir la recomendación. Estas opciones serán :

   -Autor: Simplemente tienes que poner el nombre del Autor de un libro y aparecerán en pantalla sus libros y otros libros que tengan una temática similar. Como ejemplo puedes usar "george r.r. martin" o "charles dickens". El buscador funciona
   también con nombres incompletos, como puede ser "edgar all" en lugar de Edgar Allan Poe.

   -Género: Puesto que el propio recomendador está basado en el género de las obras ya que el csv con el que cuento no dispone de sinopsis, al buscar por género se realizará mas bien una función de filtro. Algunos ejemplos de uso serían:
   "fantasy". Tambien se pueden buscar mas géneros de una sola vez mediante "Horror;Fantasy;Fiction". Al utilizar el recomendador por "Género" la lista estará ordenada por la métrica calculada "Score", si se desea ordenar por popularidad,
   aparece un boton debajo.

   -Libro similar: Al igual que en el caso de Autor, solo es necesario escribir el nombre de un libro y el recomendador dara libros de temática similar. Puede probar con libros como "1984" y "Coralin" siendo realmente el libro de "Coraline" pero
   mal escrito.

4. **Final**

   La decisiones técnicas tomadas vienen explicadas en el notebook asi como la preparación de los datos.
