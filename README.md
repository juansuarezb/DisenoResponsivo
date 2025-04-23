# DisenoResponsivo
*Aprende HTML construyendo una aplicacion de fotos de gatos*

> [!NOTE]
> ## Paso 1
> Los elementos de HTML tienen etiquetas de apertura y de cierre h1
> ```html
> <h1>Hola Mundo </h1>
> ```

> [!NOTE]
> ## Paso 2
> Los elementos de encabezado van de h1 - h6 (se utilizan para indicar la importancia del contenido por debajo de ellos.)
> ```html
> <h1>Hola Mundo </h1>
> <h2>Hola </h2>
> <h3>Mundo </h3>
> ```

> [!NOTE]
> ## Paso 3
> El elemento p es usado para crear un parrafo de texto en una pagina web
> ```html
> <p>Holaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa </p>
> ```

> [!NOTE]
> ## Paso 4
> Los comentarios en html tienen la siguiente sintaxis:
> ```html
> <!--Esto es un comentario-->
> ```

> [!NOTE]
> ## Paso 5
> HTML5 tiene diferentes elementos que ayudan a diferenciar diferentes tipos de contenido. Estos elementos hacen tu código HTML más fácil > de leer y ayudan con el Posicionamiento en buscadores (Search Engine Optimization - SEO) y accesibilidad.
> El elemento main se utiliza para representar el contenido principal del cuerpo de un documento HTML.
> ```html
> <body>
>   <main>
>     <h1>Most important content of the document</h1>
>      <p>Some more important content...</p>
>   </main>
> </body>


> [!NOTE]
> ## Paso 6
> Al colocar elementos h1, h2 dentro del main se le conoce como **nesting** <br>
> Los elementos anidados deben colocarse dos espacios más a la derecha del elemento en el que están anidados. Este espacio se llama **sangría** (indentación en programación) y se utiliza para facilitar la lectura de HTML.
> ```html
>   <main>
>      <h1>CatPhotoApp</h1>
>      <h2>Cat Photos</h2>
>      <!-- TODO: Add link to cat photos -->
>      <p>Everyone loves cute cats online!</p>
>    </main>
> ```


> [!NOTE]
> ## Paso 7
> Los *atributos* de HTML son palabras especiales usadas dentro de una etiqueta. <br>
> *El atributo src en un elemnto img especifica la URL* <br>
> ```html
>  <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg">
> ```


> [!NOTE]
> ## Paso 8
> Todos los elementos img deben tener un atributo alt
> ```html
>  <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back">
> ```


> [!NOTE]
> ## Paso 10
>   Para abrir enlances en una pestaña nueva, puedes usar el atributo target en el elemento ancla (a).
> ```html
>  <p> See more <a href="https://freecatphotoapp.com" target="_blank">cat photos</a> in our gallery. <p>
> ```

> [!NOTE]
> ## Paso 11
>   Para colocar un enlace en una imagen se anida en una etiqueta "a" a la imagen.<br>
> ```html
>  <a href="https://freecatphotoapp.com"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."></a>
> ```

> [!NOTE]
> ## Paso 12
> **El elemento section es usado para definir secciones en un documento, como capítulos, encabezados, pies de página, o cualquier otra sección del documento. Es un elemento semántico que ayuda con la SEO y la accesibilidad.**
> ```html
> <html>
>  <body>
>    <main>
>      <h1>CatPhotoApp</h1>
>      <section>
>        <h2>Cat Photos</h2>
>        <p>Everyone loves <a href="https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg">cute cats</a> online!</p>
>        <p>See more <a target="_blank" href="https://freecatphotoapp.com">cat photos</a> in our gallery.</p>
>        <a href="https://freecatphotoapp.com"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."></a>
>      </section>
>      <section>
>        <h2>Cat Lists</h2>
>        <h3>Things cats love:</h3>
>      </section>
>   </main>
>  </body>
> </html>
> ```

> [!NOTE]
> ## Paso 13
> Para crear una lista no ordenada se utiliza el elemento ul <br>
> El elemento li es usado para crear una lista en una lista <br>
> ```html
>  <ul>
>          <li>catnip</li>
>          <li>laser pointers</li>
>          <li>lasagna</li>
>  </ul>
> ```


> [!NOTE]
> ## Paso 14
> Los elementos figure representa contenido independiente y te permitirá asociar una imagen a una descripción.
>  ```html
>  <figure><img src="aasdksadka"/></figure>
>  ```
> Y para colocar una leyenda a la imagen se utiliza figcaption
> ```html
> <figcaption>Cats love lasagna.</figcaption>
> ```


> [!NOTE]
> ## Paso 15
> Los elemento de una lista ordenada aparecen enumerados.
> ```html
> <h3>Top 3 things cats hate:</h3>
>        <ol>
>          <li>flea treatment</li>
>          <li>thunder</li>
>          <li>other cats</li>
>        </ol>
> ```


> [!NOTE]
> ## Paso 16
> Ahora usaremos formularios para recolectar información del usuario.
> ```html
> <p><em>hola</em>mundo</p>
> ```


> [!NOTE]
> ## Paso 17
> Ahora usaremos formularios para recolectar información del usuario. <br>
> El elemento form se utiliza para obtener información de un usuario, como su nombre, correo electrónico y otros detalles. <br>
> El atributo action indica dónde se deben enviar los datos del formulario. <br>
> ```html
> <h2>Cat Form</h2>
>  <form action="https://freecatphotoapp.com/submit-cat-photo">
>  <input type="text"/>
> </form>
> ```
> El elemento input te permite recolectar datos desde un formulario web de diferentes formas. Al igual que los elementos img, los elementos input son un void element y no necesitan etiquetas de cierre.
> **Hay diferentes tipos de elementos input**, los cuales los puedes crear con el atributo type. Puedes crear fácilmente un campo de contraseña (password), un botón de reinicio (reset) o un control para permitir a los usuarios seleccionar un archivo desde su computadora

> [!TIP]
> Aquí tienes una lista de tipos de `<input>` en HTML:

```html
<input type="text"/>
<input type="password"/>
<input type="number"/>
<input type="checkbox"/>
<input type="color"/>
<input type="date"/>
<input type="time"/>
<input type="search"/>
<input type="file"/>
<input type="range"/>
<input type="radio"/>
<input type="submit"/>
<input type="week"/>
```

> [!NOTE]
> ## Paso18
> Para que los datos de un formulario sean accesibles en la ubicación especificada en el atributo action, debes darle al campo de texto un atributo name y asignarle un valor que represente los datos que se están enviando

> [!NOTE]
> ## Paso19
> El atributo id se utiliza para identificar elementos HTML específicos. Cada atributo id debe tener un valor único, diferente a los demás valores id de la página.
> ```html
>  <label><input type="radio" id="indoor"/>Indoor</label>
>  <label><input id="outdoor" type="radio"/>Outdoor</label>
> ```
> <p>Actualmente, ambos inputs pueden ser seleccionados a la vez. Para evitar esto podemos agregar un atributo name con un mismo valor</p>
>
> ```html
>  <label><input type="radio" id="indoor" name="indoor-outdoor"/>Indoor</label>
>  <label><input id="outdoor" type="radio" name="indoor-outdoor"/>Outdoor</label>
> ```
> <p>Agregar un atributo value con el mismo valor del id es buena practica</p>
>
> ```html
>  <label><input type="radio" id="indoor" name="indoor-outdoor" value="indoor"/>Indoor</label>
>  <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"/>Outdoor</label>
> ```
