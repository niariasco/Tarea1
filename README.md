<!DOCTYPE html> 
<html lang="en">
<head> 
    <meta charset="UTF-8"> <!--//set de caracteres -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> <!--//despliegue de la pagina en distintos devices.-->
    <title>title : Tarea 1</title> 
      <link rel="icon" type="image/x-icon" href="images/Amapola.jpeg"> 
</head>

    <!--<!DOCTYPE html> Define el elemento raíz de un documento HTML. --> 
 <!-- The link element. : icono-->
<!--título  de  un  documento  HTML,  que  se  muestra  en  la  barra  de  título  del  navegador o en la pestaña de la página.-->
 <!--head : Define  la  cabeza  de  un  documento  HTML,  que  contiene  información  sobre  el 
documento, como el título, los enlaces, los estilos y los scripts.-->
   <!--<meta>:  Define  los  metadatos  de  un  documento  HTML,  como  el  autor,  la  descripción,  las 
palabras clave, el juego de caracteres o la vista de compatibilidad. -->

<body>  <!-- cuerpo  de un documento HTML,  que  contiene el  contenido  visible  de  la página.-->

    <!--The base element : URL base para todos los enlaces relativos de un documento HTML.-->
    <a href="https://www.w3schools.com/" target="_blank"></a>
    
     <!--Image default element.-->
    <h2>This is img element : </h2>
    <img
    src="images/Amapola.jpeg" width="300" height="300"
    alt="Imagen no encontrada"
   />
   
           <h1 style="text-align: center;">Etiquetas de estructura de sección</h1>
   <!--<h1>  -  <h6> Definen  los  encabezados  de  un  documento  HTML. -->
<h1>The h1-h6 element. </h1>
<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<h3>This is heading 3</h3>
<h4>This is heading 4</h4>
<h5>This is heading 5</h5>
<h6>This is heading 6</h6>

  <!--Define  un  grupo  de  encabezados  de  un  documento  HTML,  que  pueden  ser  un 
  título y un subtítulo, o varios niveles de encabezados relacionados.-->
    <hgroup>
        <h1>The hgroup element. Form1</h1>
        <h1>Hgroup1 </h1>
        <h2>Hgroup2</h2>
    </hgroup>
  
 <!--impresion : This is heading 1 This is heading 2 This is heading 6-->
    <hgroup>
        <h1>The hgroup element. Form2</h1>
    This is heading 1
    This is heading 2
    This is heading 6
    </hgroup>
   
 
 <!-- address : información de contacto del autor o el propietario de un documento o un  artículo  HTML-->
    <h1>The address element</h1>
    <address>
    Hecho por <a href="https://niariasco.github.io/Tarea1/">Nicole Arias</a>.<br> 
    Visita el sitio web : <br>
    https://niariasco.github.io/Tarea1/<br>
    Sarchi, Alajuela<br>
    CR
    </address>

<!--div : división o una sección genérica de un documento HTML-->
    <h1>The div element</h1>
    <style>
        .myDiv {
          border: 5px outset red;
          background-color: lightblue;    
          text-align: center;
        }
        </style>
        <div class="myDiv">
          <h2>Encabezado</h2>
          <p>Tarea1.</p>
        </div>
        <p>Fuera del div.</p>    
        

<!--iframe : división : mostrar una página web dentro de una página web-->
        <h1>The iframe element</h1>
        <iframe src="https://niariasco.github.io/Tarea1/" title="Tarea1 iframe">
        </iframe>
       
<!--iframe : división : mostrar una página web dentro de una página web-->
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>: Mapa de Sarchí, Alajuela</title>
        <h1>iframe Form2 : Mapa de Sarchí, Alajuela</h1>
        <iframe 
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3151.835434508616!2d144.9537363153187!3d-37.81627974202154!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x8fa0596559c82661%3A0x6fb47b55d280c3be!2sProvincia%20de%20Alajuela%2C%20Sarch%C3%AD!5e0!3m2!1ses!2scr!4v1690375098131!5m2!1ses!2scr" 
            width="600" 
            height="450" 
            style="border:0;" 
            allowfullscreen="" 
            loading="lazy">
        </iframe>


    <h1 style="text-align: center;">Etiquetas de estructura de grupo</h1>

<!-- <ul>:  lista desordenada de un documento HTML, que contiene elementos que no
tienen un orden específico. -->
<h2>The ul element</21>

<ul style="list-style-type:circle">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>

<ul style="list-style-type:disc">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>

<ul style="list-style-type:square">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>

<!--<ol>: Define una lista ordenada de un documento HTML, que contiene elementos que tienen
un orden numérico o alfabético. -->
<h1>The ol and li element</h1>

<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

<ol start="50">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

<ol style="list-style-type:upper-roman" >
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

<ol style="list-style-type:lower-alpha">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

<ol id="alphabet-list" style="list-style-type:none;"></ol>

<script>
  const items = ["Coffee", "Tea", "Milk", "aba", "hoy"];
  const startCharCode = "Z".charCodeAt(0); // Código ASCII de 'Z'
  
  const list = document.getElementById("alphabet-list");
  items.forEach((item, index) => {
    const letter = String.fromCharCode(startCharCode - index); // Genera Z, Y, X...
    const listItem = document.createElement("li");
    listItem.textContent = `${letter}. ${item}`;
    list.appendChild(listItem);
  });
</script>

<!--<dl>: Define una lista de descripción de un documento HTML, que contiene elementos que
tienen un término y una descripción.
• <dt>: Define un término de una lista de descripción de un documento HTML, que puede ser
una palabra, un nombre o una frase.
• <dd>: Define una descripción de una lista de descripción de un documento HTML, que puede
contener texto, imágenes, enlaces u otros elementos.-->
<p> dl , dt , dd element :</p>

<dl>
  <dt>CocaCola (dt)</dt>
  <dd>Cafe Negro(dd)</dd>
  <dt>Cafe con Leche(dt)</dt>
  <dd>Pepsi(dd)</dd>
</dl>



<!--• <figure>: Define una figura de un documento HTML, que puede contener una imagen, un
diagrama, un gráfico, un código u otro contenido ilustrativo.-->
<!--• <figcaption>: Define una leyenda de una figura de un documento HTML, que puede contener
texto, enlaces u otros elementos.-->
<h1>The figure and figcaption element</h1>

<figure>
  <img src="images/Amapola.jpeg" alt="Trulli" style="width:20%">
  <figcaption>figcaption : Fig.1 - Amapolla,Flor Rosa, De clima caliente.</figcaption>
</figure>

<!--• <details>: Define un elemento que puede expandirse o contraerse para mostrar u ocultar
información adicional de un documento HTML.-->
<!--• <summary>: Define un elemento que muestra un resumen o un título de un elemento
<details> de un documento HTML.-->

<h1>The details and summary element </h1>

<details>
  <summary>UTN matricula 2025</summary>
  <p>La Universidad Técnica Nacional (UTN) realiza anualmente el Proceso de Admisión para Nuevo Ingreso a carreras en todas sus sedes universitarias.
La solicitud de admisión para ingresar en el 2025, se realiza del 5 de agosto al 24 de setiembre de 2024, puede acceder en el siguiente enlace al sistema SIGU para completar la solicitud de admisión.
La UTN no realiza examen de admisión. </p>
</details>


<!--• <dialog>: Define un elemento que muestra un diálogo, una ventana emergente o una alerta
de un documento HTML--->
<h1>The dialog element</h1>
<dialog open>Este es el elemento dialog </dialog>
<br><br><br>


 <h1 style="text-align: center;">Etiquetas de texto </h1>

<!--  <p>: Define un párrafo de un documento HTML, que puede contener texto, imágenes, enlaces
u otros elementos.-->
    <p>
        <h3>elemento p </h3>
        <a href="https://www.utn.ac.cr/">Accesar UTN website</a> 
    </p>

<!--• <br>: Define un salto de línea de un documento HTML, que se utiliza para separar el texto
sin crear un nuevo párrafo.
-->
<h1>The br element</h1>
<p>Para Forzar<br>el corte de lineas<br> en el texto,<br> use el elemento <br> br.
</p>

<!--• <pre>: Define un texto preformateado de un documento HTML, que conserva los espacios y
los saltos de línea tal como se escriben en el código fuente.-->
<h1>The pre element</h1>

<pre>
El texto de un elemento pre
se muestra en una fuente de ancho fijo
y conserva
tanto los espacios        como los
saltos de línea
</pre>

<!--• <blockquote>: Define una cita en bloque de un documento HTML, que puede contener un
texto citado de otra fuente, con una sangría respecto al texto normal.-->
<h1>The blockquote element</h1>
<p>He aquí una cita del sitio web de WWF:</p>
<blockquote cite="http://www.worldwildlife.org/who/index.html">
Desde hace 50 años, WWF protege el futuro de la naturaleza. WWF, la principal organización conservacionista del mundo, trabaja en 100 países y cuenta con el apoyo de 1,2 millones de miembros en Estados Unidos y cerca de 5 millones en todo el mundo.
</blockquote>


<!--• <q>: Define una cita en línea de un documento HTML, que puede contener un texto citado
de otra fuente, entre comillas.-->
<h1>The q element</h1>
<p>El texto en el elemento q es :
    <q>Este es el texto en el elemento q :</q>
    fuera del elemento q.</p>.


<!--<cite>: Define el título de una obra citada de un documento HTML, que puede ser un libro,
un artículo, un sitio web o cualquier otra fuente.-->
<h1>The cite element</h1>
<img src= "images/scream_vert-a59c4997eed62f01e7ce9f7471890ea40f1f4636.jpg" width="220" height="227" alt="The Scream">
<p><cite>The Scream</cite> by Edward Munch. Painted in 1893.</p>


<!--• <abbr>: Define una abreviatura o un acrónimo de un documento HTML, que puede mostrar
el significado completo al pasar el cursor sobre el texto.-->
<h1>The abbr element</h1>
<p>El <abbr title="Structured Query Language">SQL</abbr> is a standard language for database creation and manipulation.</p>

<!--• <dfn>: Define una definición de un término de un documento HTML, que puede mostrar una
descripción más detallada al pasar el cursor sobre el texto.-->
<h1>The dfn element</h1>
<p>
    El término <dfn title="Lenguaje de Marcado de Hipertexto">HTML</dfn> se refiere al estándar para crear páginas web.
    </p>

<!--<code>: Define un fragmento de código de un documento HTML, que se muestra con una
fuente monoespaciada y sin ningún formato especial.-->
<h1>The code element</h1>
<p>The HTML <code>button</code> tag defines a clickable button.</p>

<!--• <kbd>: Define una entrada de teclado de un documento HTML, que se muestra con una fuente monoespaciada y se 
utiliza para representar combinaciones de teclas o comandos. -->
<h1>The kbd element</h1>
<p>Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy text (Windows).</p>
<p>Press <kbd>Cmd</kbd> + <kbd>C</kbd> to copy text (Mac OS).</p>

<!--• <b>: Define un texto en negrita de un documento HTML, que se utiliza para resaltar o enfatizaruna parte del texto.-->
<h1>The b element</h1>
<p>This is normal text - <b>and this is bold text</b>.</p>

<!--• <strong>: Define un texto fuerte de un documento HTML, que se utiliza para indicar la
importancia o la urgencia de una parte del texto.-->
<h1>The strong element</h1>
<p><strong>This text is important!</strong></p>

<!--• <i>: Define un texto en cursiva de un documento HTML, que se utiliza para marcar 
una parte del texto como diferente o especial, como un término técnico, un idioma extranjero o un pensamiento.-->
<h1>The i element</h1>
<p><i>Lorem Ipsum</i> is the most popular filler text in history.</p>


<!--• <em>: Define un texto enfático de un documento HTML, que se utiliza para expresar el
énfasis o el tono de una parte del texto.-->
<h1>The em element</h1>
<p>You <em>have</em> to hueey up!.</p>


<!--• <mark>: Define un texto marcado de un documento HTML, que se utiliza para 
resaltar o señalar una parte del texto, como una coincidencia de búsqueda o una referencia.-->
<h1>The mark element</h1>
<p>Do not forget to buy <mark>milk</mark> today.</p>


<!--• <small>: Define un texto pequeño de un documento HTML, que se utiliza para mostrar
información secundaria, como una nota al pie, una fecha o una hora.-->
<h1>The small element</h1>
<p><small>10:30am</small></p>


<!--• <del>: Define un texto eliminado de un documento HTML, que se utiliza para mostrar texto
que ha sido borrado o modificado, con una línea que lo atraviesa.-->
<!--• <ins>: Define un texto insertado de un documento HTML, que se utiliza para mostrar texto
que ha sido añadido o modificado, con una línea que lo subraya.-->
<h1>The ins element</h1>
<h1>The del element</h1>
<p>Mi color favorito es <del>naranja</del><ins>celeste</ins>!</p>




<!--• <sub>: Define un texto subíndice de un documento HTML, que se utiliza para mostrar texto 
que aparece ligeramente por debajo de la línea base, como una fórmula química o una nota al pie.-->
<!--• <sup>: Define un texto superíndice de un documento HTML, que se utiliza para mostrar texto 
que aparece ligeramente por encima de la línea base, como un exponente o una referencia. -->
<h1>The sup element</h1>
<h1>The sub element</h1>

<p>mostrar texto que aparece <sub> por debajo de la linea base</sub> text.</p>
<p>mostrar texto que aparece <sup> por encima de la linea base</sup> text.</p>


<!--• <time>: Define una fecha o una hora de un documento HTML, que se utiliza para mostrar-->
<h1>The time element</h1>
<p>Open from <time>10:00</time> to <time>21:00</time>, every weekday.</p>
<p>Note: The <time> element works in all of the major browsers.</p>

<!--• <data>: Define un dato con un valor asociado de un documento HTML, que se utiliza para
mostrar información que puede ser leída por máquinas o humanos.-->
<h1>The data element</h1>
<ul>
  <li><data value="21053">Cherry Tomato</data></li>
  <li><data value="21054">Beef Tomato</data></li>
  <li><data value="21055">Plum Tomato</data></li>
</ul>

<!--• <span>: Define una sección de texto de un documento HTML, que se utiliza para aplicar un
estilo o una manipulación con JavaScript a una parte del texto.-->
<h1>The span element</h1>
<p>My mother has <span style="color:blue;font-weight:bold">blue</span> eyes and my father has 
<span style="color:darkgreen;font-weight:bold">dark green</span> eyes.</p>


  <h1 style="text-align: center;">Etiquetas de enlace</h1>
<!--• <a>: Define un enlace de un documento HTML, que puede contener texto, imágenes u otros
elementos-->
<h1>The a element</h1>
<a href="https://www.w3schools.com">Visit W3Schools.com!</a>

<!--• <area>: Define un área de enlace de un elemento <map> de un documento HTML, que puede
tener una forma de rectángulo, círculo o polígono.-->
<!--<map>: Define un mapa de imagen de un documento HTML, que puede contener áreas de
enlace que se activan al hacer clic sobre una imagen.-->
<h1>The area and map element</h1>
<p>Haz Click en la computadora</p>
<img src="images/pc_ver_1.png" alt="Workplace" usemap="#workmap" width="400" height="379">
<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="cuadrado" href="images/cuadrado.png">
</map>

  <h1 style="text-align: center;">Etiquetas de imagen</h1>

<!--• <img>: Define una imagen de un documento HTML, 
que puede tener un atributo src para indicar la URL de la imagen, un atributo alt para indicar el texto alternativo de la imagen, 
y otros atributos para indicar el tamaño, el título o el estilo de la imagen.-->
<h1>The img and map element</h1>
<img src="images/images.png" alt="Escudo de Heredia" width="300" height="300">

<!--• <picture>: Define una imagen con varias fuentes de un documento HTML, 
que puede contener elementos <source> para indicar diferentes versiones de la 
imagen según el tamaño de la pantalla, el tipo de dispositivo o el formato de la imagen.-->
<!--<source>: Define una fuente de imagen o de audio de un elemento <picture> o <audio> de un documento HTML, 
que puede tener un atributo srcset para indicar la URL de la fuente, y un atributo media para indicar la condición de la fuente.-->
<!--No pude agregar un audio por el error : 
The file type .mp3 is only supported on our paid plans. Upgrade your plan, if you want to unlock more file types for your space.
Pero este seria el ejemplo :
<audio controls>
  <source src="horse.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
</audio>
-->

<h1>The picture and source element</h1>
<p>Resize the browser window to load different images.</p>
<picture>
  <source media="(min-width:650px)" srcset="images/cattleDog.jpg">
  <source media="(min-width:465px)" srcset="images/cattleDogs.jpg">
  <img src="images/cattledoMountaing.jpg" alt="Flowers" style="width:auto;">
</picture>


<!--<canvas>: Define un lienzo de un documento HTML, que puede contener gráficos dibujados
con JavaScript o con la API de WebGL.-->
<h1>The canvas element</h1>
<canvas id="myCanvas" width="400" height="200" style="border:1px solid #000000;">
  Your browser does not support the canvas element.
</canvas>

<script>
  // Obtener el lienzo por su ID y el contexto 2D
  var canvas = document.getElementById("myCanvas");
  var ctx = canvas.getContext("2d");

  // Dibujar un rectángulo
  ctx.fillStyle = "#FF0000"; // Color rojo
  ctx.fillRect(50, 50, 150, 100); // Coordenadas (x, y) y tamaño (ancho, alto)
</script>


<!--<svg>: Define un gráfico vectorial escalable de un documento HTML, que puede contener
elementos que definen formas, textos, filtros, animaciones o transformaciones.-->
<h1>The svg element</h1>
<svg width="400" height="400" xmlns="http://www.w3.org/2000/svg">
  <!-- Dibujar un círculo -->
  <circle cx="200" cy="200" r="100" stroke="black" stroke-width="3" fill="red" />
  
  <!-- Dibujar un rectángulo -->
  <rect x="50" y="50" width="300" height="100" stroke="black" stroke-width="3" fill="green" />
  
  <!-- Dibujar una línea -->
  <line x1="50" y1="200" x2="350" y2="200" stroke="blue" stroke-width="3" />
  
  <!-- Dibujar texto -->
  <text x="150" y="250" font-family="Verdana" font-size="35" fill="black">SVG Example</text>
</svg>




<h1 style="text-align: center;">Etiquetas de miltimedia</h1>



<!--• <audio>: Se utiliza para insertar archivos de audio en una página web.-->
<!--• <source>: Utilizada dentro de las etiquetas <audio> y <video> para especificar las fuentes
del archivo multimedia en diferentes formatos.-->
<h1>The audio element</h1>
<p>Click on the play button to play a sound:</p>

<audio controls>
  <source src="horse.mp3" type="audio/mp3">
    El buscador no soporta el audio.

</audio>


<!--• <video>: Se utiliza para insertar archivos de video en una página web.-->
<!--• <source>: Utilizada dentro de las etiquetas <audio> y <video> para especificar las fuentes
del archivo multimedia en diferentes formatos.-->
<h1>The video and source element</h1>
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  El buscador no soporta el video.
</video>
 <audio controls>
        <!-- Fuentes de audio en diferentes formatos -->
        <source src="music.mp3" type="movie/mp3">
        <source src="music.ogg" type="movie/ogg">
        <source src="music.wav" type="movie/wav">
        
        <!-- Mensaje si el navegador no soporta el audio -->
        Your browser does not support the audio element.
</audio>



<!--• <track>: Se utiliza dentro de la etiqueta <video> para incluir subtítulos o descripciones de
audio.-->
<h1>The track element</h1>

<p>
Video proveniente de : 
<a href="https://en.wikipedia.org/wiki/Bruno_Mars" target="_blank">Bruno Mars</a>.
</p>
<video width="320" height="240" controls>
  <source src="Bruno Mars - When I Was Your Man (Official Music Video).mp4" type="video/mp4">
  <track src="fgsubtitles_en.vtt" kind="subtitles" srclang="en" label="English">
</video>

<!--• <canvas>: Aunque no está directamente relacionada con multimedia, la etiqueta <canvas> 
puede usarse para renderizar gráficos, incluidos los generados dinámicamente, como juegos y visualizaciones.-->
<h1>The canvas element</h1>
       <canvas id="myCanvas" width="500" height="300" style="border:1px solid #000000;"></canvas>

  <canvas id="myCanvas">
Your browser does not support the canvas tag.
</canvas>

<script>
const c = document.getElementById("myCanvas");
const ctx = c.getContext("2d");
ctx.fillStyle = "red";
ctx.fillRect(20, 20, 75, 50);

//Turn transparency on
ctx.globalAlpha = 0.2;
ctx.fillStyle = "blue"; 
ctx.fillRect(50, 50, 75, 50); 
ctx.fillStyle = "green"; 
ctx.fillRect(80, 80, 75, 50);
</script>



<!--<svg>: es un contenedor para gráficos SVG que tienen varios métodos para dibujar trazados,
cuadros, círculos, texto e imágenes gráficas.-->

<h1>The svg element</h1>
    <!-- SVG con un área de 500x500 píxeles -->
    <svg width="500" height="500" xmlns="http://www.w3.org/2000/svg">
        <!-- Dibuja un rectángulo -->
        <rect x="50" y="50" width="150" height="100" fill="blue" />

        <!-- Dibuja un círculo -->
        <circle cx="300" cy="100" r="50" fill="brown" />

        <!-- Dibuja una línea -->
        <line x1="50" y1="200" x2="450" y2="200" stroke="pink" stroke-width="2" />

        <!-- Dibuja texto -->
        <text x="100" y="400" font-family="Arial" font-size="24" fill="orange">Hola SVG!</text>
    </svg>

<!--• <iframe>: realice las configuraciones para mostrar videos de YouTube utilizando esta
etiqueta.-->
<h1>The iframe element</h1>
<iframe 
    width="560" 
    height="315" 
    src="https://www.youtube.com/embed/rac_f5keP98?si=jCSo_cWZWudLzS2f" 
    title="YouTube video player" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
    allowfullscreen>
</iframe>


</body>
</html>


