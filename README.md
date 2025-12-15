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

---

### pom.xml
Este trabajo está hecho en un proyecto de Maven para que se pueda trabajar con datos JSON, por lo tanto, hay que configurar el archivo pom.xml.

Lo únio que hay que hacer es añadir la dependencia del JSON para que el programa funcione correctamente.

<img width="941" height="504" alt="Captura de pantalla 2025-12-15 205414" src="https://github.com/user-attachments/assets/1ed08890-353c-453d-9364-af5d82a3dfcc" />

---

Resultados:

Lo primero que se mostrará al iniciar el programa es el mensaje que indica que tenemos que introducir el símbolo o el nombre de la moneda:

<img width="591" height="261" alt="Captura de pantalla 2025-12-15 212316" src="https://github.com/user-attachments/assets/21ab0829-a489-4356-aac2-944e084e26af" />

Si introducimos el símbolo o el nombre de una moneda existente este será el resultado:

<img width="487" height="340" alt="Captura de pantalla 2025-12-15 212330" src="https://github.com/user-attachments/assets/231aa12b-9b9c-4ccc-8e0a-a414c8109863" />
<img width="487" height="340" alt="Captura de pantalla 2025-12-15 212345" src="https://github.com/user-attachments/assets/fbc1d869-3555-4517-87f9-a86b5f132f30" />

Pero, si de lo contrario introducimos una moneda que no existe aparecerá este mensaje:

<img width="502" height="257" alt="Captura de pantalla 2025-12-15 212441" src="https://github.com/user-attachments/assets/c0ce2a48-a2a2-43dc-a6af-008e0499b11b" />
