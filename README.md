Generación de Resúmenes Automáticos con GPT-2: Un Proyecto de NLP Paso a Paso

Paso 1: Extracción de texto desde un archivo PDF 📄
El primer paso fue extraer el texto de un archivo PDF utilizando la librería pdfplumber

Paso 2: Limpieza del texto 🧹
Una vez que obtuve el texto del PDF, lo limpié utilizando expresiones regulares (re) para eliminar URLs, referencias a notas y caracteres especiales. Esto asegura que el modelo trabaje solo con contenido relevante y libre de ruido.

Paso 3: Tokenización del texto 🔑
Para que el modelo pueda entender y trabajar con el texto, utilicé la librería nltk para dividir el texto en oraciones. Esto facilita la manipulación del texto y la posterior generación de resúmenes.

Paso 4: Cargar y usar el modelo GPT-2 🧠
Después de limpiar y preparar el texto, utilicé GPT-2, un modelo de lenguaje preentrenado de OpenAI, para generar resúmenes. Utilicé la librería transformers de Hugging Face para cargar y trabajar con el modelo. GPT-2 es muy potente para tareas de generación de texto.

Paso 5: Generación de Resúmenes Automáticos ⚡
Finalmente, utilicé GPT-2 para generar un resumen del texto de entrada. Al usar el método generate(), definí parámetros como max_length para controlar la longitud del resumen generado.


Librerías Utilizadas 📚
pdfplumber: Permite la extracción de texto de PDFs, incluso con estructuras complejas.

re (expresiones regulares): Utilizado para limpiar el texto, eliminar URLs, y realizar ajustes.

nltk: Librería popular para trabajar con el procesamiento de lenguaje natural, especialmente útil para tokenización.

transformers: Una de las librerías más potentes para trabajar con modelos preentrenados como GPT-2, BART y T5, proporcionada por Hugging Face.

torch: Framework de aprendizaje profundo que permite ejecutar el modelo en GPU para acelerar el procesamiento.
