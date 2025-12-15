# Trabajo 35: Uso de APIs
En este trabajo, además de usar las funciones que vimos en la tarea anterior, tenemos que usar GET y REST (Representational State Transfer) para poder conectarnos con la API y obtener los datos que contenga.

---

### Código:
Dentro de el mismo código podemos crear todo el programa ya que no resulta ser uno muy extenso.

De primeras, después de declarar los imports y el main, tenemos que crear nuesto Scanner para poder introducir por teclado la moneda que queramos.

Después, dentro del try-catch para manejar excepciones, introducimos HttpClient, HttpRequest y HttpResponse, el primero nos permite realiza las solicitudes del GET, el segundo es necesario para poder enviar las solicitudes, aquí es donde montamos nuestro GET, poniendo la url, indicando que tipo de solicitud es con el GET y, por último, el build() para terminar el constructor y la funcion del tercero es esperar por la respuesta.

Abajo de las funciones Http se encuentran las funciones JSON, la primera, JSONObject, transforma el texto a unos datos que pueden ser consultados por claves y la segunda función, JSONArray, se encarga de manejar estos datos para devolverlos en una lista.

Una vez declarado todo lo demás, hay que iniciar un bucle que se ocupará de leer lo que introduzcamos y mostrar los resultados de la moneda que hayamos escrito; si la moneda existe, mostrará sus datos, de lo contrario, mandará un mensaje de error diciendo que la moneda no existe.


<img width="811" height="1217" alt="Captura de pantalla 2025-12-15 205334" src="https://github.com/user-attachments/assets/275e2d0c-e38a-4c8e-893b-531646c80006" />
