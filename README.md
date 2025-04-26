> <h1>Aprende CSS Básico construyendo un Menú de una cafetería.</h1>
> <p>CSS le dice al navegador <strong>como</strong> mostrar la página web, se puede establecer el color, fuente y mucho más.</p>

<section> 
<h4><em>Paso 1:</em></h4>
<p>Agregar la estructura básica para construir la página web</p>
<ol>
    <li><strong>Declaración DOCTYPE</strong></li>
    <p>DOCTYPE le indica al navegador la versión del código HTML .</p>
    <li><strong>Elemento HTML</strong></li>
    <p>Representa el elemnto raiz que contiene a todos los otros elementos</p>
</ol>
</section>

```html
<DOCTYPE html> <html lang="en"></html> </DOCTYPE>
```

<section>
    <h4><em>Paso 2:</em></h4>
    <p>Añadir un elemento head para poder añadir un elemento title</p>
</section>

```html
<DOCTYPE html>
  <html lang="en">
    <head>
      <title>Cafe Menu</title>
    </head>
  </html>
</DOCTYPE>
```

<section>
    <h4><em>Paso 3:</em></h4>
    <p>Existen elementos que proporcionan información adicional no visible como <em>title</em> pero que son útiles para los motores de búsqueda. <p>
    <p>Añade un elemento meta (dentro del head) con un atributo charset con valor utf-8 </p>
</section>

```html
<DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="utf-8" />
      <title>Cafe Menu</title>
    </head>
  </html>
</DOCTYPE>
```

<section>
    <h4><em>Paso 4:</em></h4>
    <p>Es hora de darle contenido al menú, agrega un elemento para el body y anida un elemento main.<p>
    
</section>

```html
<DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="utf-8" />
      <title>Cafe Menu</title>
    </head>
    <body>
      <main>
        <h1>CAMPER CAFE</h1>
      </main>
      <section>
        <h2>COFFEE</h2>
      </section>
    </body>
  </html>
</DOCTYPE>
```

<section>
    <h4><em>Paso 5:</em></h4>
    <p>Es hora de darle estilo al contenido, para modificar esto añade un elemento style dentro del elemento head<p>    
</section>

```html
<DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="utf-8" />
      <title>Cafe Menu</title>
      <style></style>
    </head></html
></DOCTYPE>
```

<section>
    <h4><em>Paso 6:</em></h4>
    <p>Centra el contenido del elemento h1 estableciendo su propiedad text-align: center<p>   
</section>

```html
<DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="utf-8" />
      <title>Cafe Menu</title>
      <style>
        h1 {
          text-align: center;
        }
      </style>
    </head>
  </html></DOCTYPE
>
```

<section>
    <h4><em>Paso 7:</em></h4>
    <p>Añade otr selector de tipo para centrar al elemento h2 y otro para el elemento p.<p>   
</section>

```html
<style>
  h1 {
    text-align: center;
  }
  h2 {
    text-align: center;
  }
  p {
    text-align: center;
  }
</style>
```

<section>
    <h4><em>Paso 8:</em></h4>
    <p>Puede añadir el mismo grupo de estilos a varios elementos creando una lista de selectores: <p>   
</section>

```html
<style>
  h1,
  h2,
  p {
    text-align: center;
  }
</style>
```

<section>
    <h4><em>Paso 9:</em></h4>
    <p>Ahora tienes que vincular el archivo styles.css para que los estilos se apliquen de nuevo. Dentro del elemento head, añade un elemento link. Asigna un atributo rel con el valor "stylesheet" y un atributo href con el valor "styles.css" <p>   
</section>

```html
<DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="utf-8" />
      <title>Cafe Menu</title>
      <link rel="stylesheet" href="styles.css" />
    </head></html
></DOCTYPE>
```

<section>
    <h4><em>Paso10:</em></h4>
    <p>Para que el estilo de la página se vea similar tanto en móvil como en pc de escritorio se tiene que agregar el elemento meta con un atributo especial <strong>content</strong>
</section>

```html
<DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="utf-8" />
      <title>Cafe Menu</title>
      <link rel="stylesheet" href="styles.css" />
      <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    </head></html
></DOCTYPE>
```

<section>
    <h4><em>Paso11:</em></h4>
    <p>Cambiar el color del background del body en el archivo styles.css</p>
</section>

```css
h2, p {
  text-align: center;
  color: #ffebe3;
}

body {
  background-color: #3e2c22;
}
```

<section>
    <h4><em>Paso12:</em></h4>
    <p>El elemento div se utiliza principalmente para el diseño.</p>
</section>

```html
<body>
  <div id="menu">
    <main>
      <h1>CAMPER CAFE</h1>
      <p>Est. 2020</p>
      <section>
        <h2>Coffee</h2>
      </section>
    </main>
  </div>
</body>
```

<section>
    <h4><em>Paso13:</em></h4>
    <p>El objetivo ahora, es hacer que él div no ocupe todo el ancho de la página. La propiedad CSS width, es perfecta para esto.</p>
</section>

```css
#menu {
    width: 300px;
    /* Los comentarios en CSS se ven así */
}
```

<section>
    <h4><em>Paso14:</em></h4>
    <p>Ahora, para centrar horizontalmente al elemento #menu se puede dar el valor "auto" a las propiedades margin-left y margin-right.</p>
</section>

```css
#menu {
  width: 80%;
  background-color: burlywood;
  margin-left: auto;
  margin-right: auto;
}
```