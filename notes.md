# CSS 

## __GENERALIDADES__

<p>Documento que aplica todos los estilos en forma de cascada, es como podemos mstrar todos los elementos de html, pero no solo como cajas sino como circulos, otras figuras y demas. le da estilo visual </p>

<p>En el head "link rel="stylesheet" href="style.css"" hay que poner el documento Css</p>

<P>Los estilos se podrian poner en las mismas etiquetas, o dentro de una caja de etique Style, pero esto a la hora de correr el proyecto lo haria lento, la mejor manera es dentro del docuemnto css llamando las eqtiquetas a las que les vamos a pones estilo</P>

# _Tips en CSS_

<ul>
    <li> para dejar un comentario /* comentario */</li>
    <li>para mandar a llamar las etiquetas para aplicar estilos, clase (punto (.) al principio), y para id (# al principio)</li>
    <li>se necesita nombre de clases, para evitar que nos modifique todas las etiquetas, usando BEM (para nombrar las clases)</li>
    <li>BEM = es una metodologia que permite crear la arquitectura del proyecto</li>
    <li>BEM (bloque - elemento - modificador) <a href="https://9elements.com/bem-cheat-sheet">BEM</a></li>
    <li></li>



    
</ul>

### _Pseudoclass & Pseudoelement_

<ul>
    <p>La pseudo clases (:class), define el estilo de un ESTADO especila de un elemento.</P>

<p>El pseudo elemento (::element), define ell estilo de UNA PARTE especifica de un elemento</p>
</ul>


### _Anatomia CSS_

<ol>
    <ul> P { color: red;}
        <li>
            P = es el selector (pseudoelemento, pseudoclase)
            y es decirle a que elemento quiero agregarle estilo
        </li>
        <li> 
            {} = declaracion de estilo, el estilo que se le va aaplicar (color) y la propiedad (red)
        </li>
    </ul>


### _Modelo de cajas_

<p>Los elemento se renderizan como cajas, lo que permite agregarle ciertos estilos</p>
<ol>
    <li> MARGIN
        <p>
           Espacio externo de la caja hacia afuer
        </p>
    </li>
    <li> BORDER
        <p>
            linea que define cada uno de los elelmentos, viene predeterminado como transparente
        </p>
    </li>
    <li> PADDING
        <p>
            Espacio interno de la caja hacia adentro, ayuda a posicionar el contenido
        </p>
    </li>
    <li> CONTENIDO
        <p>
            Texto, imagenes, videos
        </p>
        <ul>Width
            <p>largo, tamañao del contenido o de la caja contenedora
            </p>
        </ul>
        <ul>Height
            <p>Alto, que se quiere que tenga el contenido
            </p>
        </ul>
    </li>
</ol>

### __ES MUY IMPORTANTE PONER AL COMIENZO DE LA HOJA DE ESTILO (*) EL SELECTOR UNIVERSAL PARA RETIRAR LOS ELEMENTOS padding, margin, QUE YA VIENEN PREDETERMINADOS POR__

### _Herencia_

<p>Es el codigo CSS que se le va a pasar de un padre a un hijo</p>

### __COMO SE CONTROLA EL ORDEN AL DECLARAR CSS__
<p>3 puntps importanes para definir que estilos implementar</P>

<ol>
    <li> IMPORTANCIA     
         <ul>Va a implementar los estilos que tiene el navegador</ul>
         <ul>Los estilos que hemos declarado</ul>  
         <ul>Declaraciones importantes (!important) EVITARLO</ul>
    </li>
    <li> ESPECIFICIDAD
         <ul> !important, punto mas importante NO ES BUENA PRACTICA HAY QUE EVITARLO</ul>
         <ul>inline Styles, son estilos que se deben en la etiqueta html, punto 4 de importancia EVITARLO</ul>  
         <ul> Todos los estilos que se le apliquen a los (#id)</ul>
         <ul> Todos los estilos que se le apliquen a las (.class)</ul>
         <ul> Todos los estilos que se le apliquen a selectores como etiquetas de html (tag)</ul> 
    </li>
    
</ol>

## _Combinadores_
<p> Ayudar a tener una especificidad mas certera</P>

<ol>
    <li> div + p {...}   
         <p> Hermano adyacente cercano (Adjacent sibling) </p>
    </li>
    <li> div ~ p {...}  
         <p>Hermano general (General sibling)</p>
    </li>
    <li> div > p {...}
         <p>Hijo (Child)</p>
    </li>
    <li> div p {...}
         <p>Desendiente (Decentdant)</p>
    </li>   
</ol>

## _Medidas_

   ### __Minimo y Maximo__ ###

<ol>
    <li> Min-width   
         <p>Delimita hasta lo minimo que puede llegar un contenido ejemplo section </p>
    </li>
    <li> Max-width 
         <p>Limitar el crecimiento de un contenedor</p>
    </li>

<p>Nos ayuda a hacer ciertos contenedores de forma flexible</p>
</ol>

  ## _Posicion_ ##

<ol>
    <li> Statick   
         <p> Por defecto</p>
    </li>
    <li> Absolute </li>
    <li> Relative </li>
    <li> Fixed </li>
    <li> Sticky </li>
     <p> Se puede usar el botton, left o right, en todos menos Static</p>
</ol>

## _Display_ ##

<p></p>

## _Display flex_ ##

<p>por defecto los acomoda en linea</p>
<<li> Flex-direction</li>    
         <p> Te permite elegir la alineación de los elementos hijos sea en vertical (column) u horizontal (row), esta alineación viene por defecto.</p>
<li> Flex-wrap</li>   
         <p> Permite que un elemento cuyo tamaño sea mayor al de la página haga un salto de línea sin salirse del contenedor, pues este se agranda.</p>
<li> Order</li>   
         <p> Especifica el orden utilizado para disponer los elementos en su contenedor flexible. Los elementos estarán dispuestos en orden ascendente según el valor de order.</p>
<li> Flex-grow</li>   
         <p> Especifica qué cantidad del espacio restante dentro del contenedor flexible, debería ocupar el ítem en cuestión según su dirección principal, esta última determinada por flex-direction.</p>
<li> Flex-basis</li>   
         <p> Especifica el tamaño inicial de un elemento flexible.</p>

<ul> justify-content
    <li>Flex-start</li>
        <p>Alinear items del flex desde el comienzo.</p>
     <li>Flex-end</li>
        <p>Alinear items desde el final.</p>
    <li>Center</li>
        <p>Alinear items en el centro del contenedor.</p>
    <li>Space-between:</li>
        <p>Distribuir items uniformemente, el primer items al inicio, el último al final.</p>
    <li>Space-around</li>
        <p>Distribuir items uniformemente, estos tienen el mismo espacio a su alrededor.</p
    <li>Space-evenly</li>
        <p>Distribuye uniformemente el espacio entre los items y su alrededor..</p>
        
</ul>

<ul> Align-items
    <p>irve para alinear los elementos hijos de forma vertical.</p> 
    <li>Flex-start</li>
        <p>Se alinean desde arriba</p>
     <li>Flex-end</li>
        <p>Se alinean desde abajo.</p>
    <li>Center</li>
        <p>Alinea los item al centro del eje y del contenedor.</li>
    <li>Stretch</li>
        <p>Estira el alto de los elementos hijos al 100% del alto del elemento padre</p>
    <li>Baseline</li>
        <p>Escala el alto del elemento al tamaño de su contenido.</p>
        
</ul>

## _Variables_ ##
  
 <p> Nos servirán para guardar valores que reiteradamente ocuparemos en el desarrollo de nuestro proyecto. Realmente se le ve mas utilidad en proyectos grandes. Pero claro, es importante conocerlo desde ahora. Se declara dentro de :root ta que serán variables globales.</p>

  ## _Font (fuente)-Web fonts_ ##

<p>para descargar fuentes una pag (google fonts)</p>
<ol>
    <li> Serif </li>  
         <p> Por defecto</p>
    <li> Sans-serif </li>
    <li> Cursive </li>
    <li> Monospace </li>

</ol>
    
