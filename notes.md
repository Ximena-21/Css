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
    <li> 
        <p>
        </p>
    </li>
</ol>