

# TALLER DE BOOTSTRAP

### Introduccion

Es un _framework_ hecha por gente que trabajaba en twiter, en el año 2011.

No solo te pormite crear interfaces, sino tambien te brinda clases **utilitarias** si tu sabes css le vas a poder sacar muchisimo provecho.

Hace unos año salió _Tailwindcss_ de parte de toda la comunidad que le da soporte a las herramientas de vue.js. 

Te reto a que despues de terminar el curso, repliques el proyecto pero usando otras librerias como _Tailwindcss_.

Si no quieres seguirme paso a paso en el codigo que copio de esta version,  simplemente te vas a la documentacion de la version que esté en ese momento y lo reemplazas por mi código

Este taller te va servir independientemente de la version de _bootstrap_ que salga

> "Mientras tu sepas diminar CSS realmente los frameworks lo que te ayudan es a agilizar el tiempo de desarrolo de una interfaz web"

pero si tu vez a estas herramientas como que te van a salvar la vida y que tu no te preucupes por aprender y dominar css que es el lenguague en el que están basados pues es ahi justamente el framework mas que hacerte un bien te va hacer un mal. Y por eso mucho tiempo yo fui opositor hasta bootstrap 4 pero es perspectiva cambió por que el ``grid` de _bootstrap 5_ ya no lo hacian con los viejos `Floats` y ya lo hacian con flexbox "NO, la herramienta no es mala, lo que relamente es malo es utilizarla sin tener conocimientos de css" 

"utiliza Bootstrap pero ten buenos fundamentos de CSS" 

### Tipos de instalaciones de Bootstrap

Con el pasar del tiempo se han vuelto muy populares los frameworks para desarrollo basados en javaScript como _Angular_ , _Vue.js_  librerias como _React_ 

Entonces hoy en dia pracicamente todo se descarga por dependencias pero no es la unica manera

>  A travez de _NPM_ que es el gestor de paquetes de `Node`

>> ``npm i bootstrap@5.3.3``

que es la version acutual hoy 9 de abril 2024 si tu quieres usar _Bootstrap_ como un _Package-manager_

pero no es la unica manera de hacerlo.

> puedes descargarlo manualmente el codigo CSS y el código javaScript. con los 

>> CDN `<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">`

Para aquellos que sean más desarrolladores  pueden integrar perfectamente a su flujo de trabajo en _Webpack_ en _Parcel_ y _Vite_ 

Si ustedes trabajan _bootstrap_ de forma un poco mas orientada hacia la programación  es que el código fuente de _Bootstrap_ está escrito en _SASS_ eso les va permitir cambiar todos los valores de variables que trae por defecto _Bootstrap_ y activar toda la gama de colores con sus respectivos matices.

Entonces si estan desarrollando una aplicacion con react con _Angular_, _Vue.js_,  y están trabajando orientado a componentes y con una filosofia de trabajo _Beem_, _SMCSS_ 

> Recuerda, este curso es para aprender _Bootstrap_ y no tanto como para incorporarlo en algun stack de desarrollo en particular, para que la gente que todavia no está tan metida en código y está como mas de la parte de diseño y la maquetación  pueda llevar este curso, nosotros vamos a utilizar la parte de la instalación  atraves de los _CDNs_ 

la documentación de _Bootstrap_ 

### Estructura de la documentación 

en la parte lateral izquierdo, se encuentra todo los temas de la documentación. Quiero que te des cuenta que si tu vas a alguna documentación de algun otro proyecto, otro tipo de frameworks que no sean de maquetación  sino mas de programacióm como: Angular, vue.js, React, te vas a dar cuenta eque en estricto sentido los sitios de documentación  mas populares tienen casi la misma estructura.

En la parte central vamos a encontrar el contenido de esa seccion. Hay algunas documentaciones que lo que hacen es poner un menú de las secciones de ese contenido.

![estructura-bootstrap](/assets/estructura-documentacion.JPG)

> `On this page ` (en esta página que vamos a ver)

Quiero que te des cuenta como están construidas toda las documentaciones.

> **Es el primer paso que debes identificar** la **Forma** la  *Estructura y donde vas a encontrar cada cosa de la documentación de Bootstrap* si te pones a investigar la documentación de algun otro proyecto. te vas a dar cuenta que siguen la misma estructura, ya es una cuestion  de Usabilidad.


### Sección Getting started

!Empieza rapido

en la version 4 ya dejaron la dependencia de ``Jquery``. la mayoria de estos _frameworks frontend_ cuando salieron 2010 -2011 no era muy bueno despues de 2015 jquery perdió su sentido de ser util, hoy en dia se sigue utilizando pero para darle mentenimiento a sitios web que en años nunca les han dado mantenimiento o por que ya tengan una plantilla de código muy vieja o por que utilizen _WordPress_ en la gran cantidad de plugins y plantillas que ha generado la comunidad pues sigue utilizando jquery 2024 

desde 2016 javaScript de forma pura lo que se conoce como(VanillaJS) ya nos entrega todo eso que antes hacia por nosotros _Jquery_

materialcss es el primer framework que se desintoxicó de `Jquery` solo tiene 2 versiones. 😔😔

lo unico que mandamos a llamar son: 

> las hojas de estilo de bootstrap

> el javaScript

>> java script utiliza otra libreria interna llamada `Popper.js` es una libreria que se utiliza para la parte de los tool-tips si no los vas a usar, podrian utilizar la version de bootstrap que no incluye `Popper.js` 

**Inicio rápido**

copiamos y pegamos el código html con los enlaces incluidos del CDN DE BOOTSTRAP Y JAVASCRIPT.

```html
    <!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Bootstrap demo</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
  </head>
  <body>
    <h1>Hello, world!</h1>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
  </body>
</html>
```
si ejecutamos, ve que no tiene la tipografia Time NewsRoman predeterminada de los navegadores es la tipografia de Bootstrap.

> **Recomendación**. cada vez que ustedes vayan a comenzar un proyecto con bootstrap lo primero que deben hacer es irse a copiar este template ☝☝ salvo que si ustedes esten haciendo un proyecto en react, angular y entonces ahi lo vayan bajando como dependencias, ya ahi se adaptan a la estructura de la herramienta con la que estén trabajando.

> Para aquellos que estén desarrollando aplicaciones con frameworks reactivos y quieran implementar bootstrap a su flujo de trabajo les invito a que se leean la guia de documentación para implementar Bootstrap en un proyecto que esté gestionado con `Webpack` o en un proyecto que esté gestionado con `Parcel` o `Vite`(nuevo) {es para la gente que esté desarrollando aplicaciones} 

Para los que desarrollamos sitios vean como simplemente mandando a llamar los CDNS ya tenemos listo el Template Start de bootstrap.

### Seccion Customize.

Es para poder configurar personalizar, a nuestro antojo la parte de variables, colores, tipografias.

El código fuente de bootstrap está escrito en SASS. y en la documentacion les va dando una guia de como ir importando cada cosa, y vean que cad una de las secciones de bootstrap tiene su propio archivo SASS .

De forma básica Bootstrap siempre ha tenido estos colores: color primario, color secundario de éxito... desde la version 4 de Bootstrap hay una gama de colores, solamente que para utilizar estas variantes tienes que trabajar con SASS.

> la seccion _Customize_ de la documentación  es para explicarte la integracion de si tu queres sacarle mayor provecho mayor personalizacion a Bootstrap, **te recomiento en la medida de lo posible no modifiques los valores drasticamente** por que cuando tu ese proyecto lo queras descargar otra vez una nueva version de bootstrap pues esa nueva version va planchar los valores que hayas modificado, por eso es muy importante la estructura de archivo que te dice.

your-project/
├── scss/
│   └── custom.scss
└── node_modules/
│   └── bootstrap/
│       ├── js/
│       └── scss/
└── index.html

no debes tocar el codigo que te da bootstrap eso tiene que estár en la carpeta _node_modules_(no tocar) de tu proyecto u aplicación, y ya lo que tu quiereas configurar, lo pones en `custom.scss` entonces no vayas a modificar los valores en código fuente de Bootstrap por que a la siguiente vez que actualizes bootstrap esos valores se van a planchar.

> Recuerda hacerlo en una hoja super css `.SCSS` independiente.

> Toda esta sección de _Customize_  es todo los cambios toda la organización del código fuente en este metaleguaje llamado SASS que al final compila y nos entrega esa hoja css que yo estoy mandando a llamar desde la _CDN_

### Sección Layout(disposición): Brakpoints y Containers

#### Breakpoints

Son los puntos de interrupción que utilizamos en el diseño css para poder cambiar la distribución de la maquetación  es lo que nos permite cambiar de una columna a dos columnas conforme vayamos teniendo mas ancho de pantalla, o tambien aplicar ciertas mediaqueris especiales para cuando el usuario no prefiera animaciones o prefiera temas oscuros

![breakpoints](/assets/breakpoints.JPG)

trata de aprenderte de memoria este cuadro, por que son las media queris  que utiliza bootstrap .

las media queris de Bootstrap son: donde (Prefijo- md, sm, lg)

**Extra small (none)** siendo la primera (no tiene prefijo de clase) su dimenciones van a ser  menosde 576px, osea si tu tienes una interfaz de hasta 575px de anchura ahi va aplicar el primer _breakpoint_ que es _extra small_(por defecto)

**Small (sm)** y va ser mayor o igual a 576px hasta 767px 

**Medium (md)** mayor o igual  a 768px hasta 991px


Si tú trabajas _bootstrap_ con SASS hay un archivo que se llama: `_variables.scss` si tu decides modificar esas mediaQueris lo puedes hacer modificando el código fuente con un archivo SASS que tu vayas configurando.

Bootstrap es un framework _Movile First_ eso significa que las media queris van a estar con la propiedad ``min-width`` 

Cada vez que inicien un proyecto, tengan a la mano las media querys ya listas para cuando ya esten desarrollando su sitio puedan tener esto a la mano 

```css
  /* // Small devices (landscape phones, 576px and up) */
@media (min-width: 576px) {  }

/* // Medium devices (tablets, 768px and up) */
@media (min-width: 768px) {  }

/* // Large devices (desktops, 992px and up) */
@media (min-width: 992px) {  }

/* // X-Large devices (large desktops, 1200px and up) */
@media (min-width: 1200px) {  }

/* // XX-Large devices (larger desktops, 1400px and up) */
@media (min-width: 1400px) {  }
```
#### Containers

En la cabezera de la docuemntacion de bootstrap, el color morado fluye al 100% 

Los conenedores en bootstrap nos permiten definir cierto margen a la izquierda y a la derecha para nuestro contenido, 

si inspeccionamos el conenido de la cabezera tambien está dentro de un contenedor `.container-xxl`

![containers](/assets/containers.JPG)

en la version 4 teniamos el contenedor normalito ya tenemos mas tamaños

¿en que radica la diferencia de estos? 
pues el tamaño de anchura que tienen en cada una de las _Mediaqueris_ y por ende el espaciado de margen de izquierda y derecha 

en el primer tamaño que `Extra small` todos ocupan el 100% de la pantalla

**small** en esta mediaquery mira que el contenedor `.container .container-sm` van a medir 540px de ancho eso significa que van a tener al rededor de 36 px de espacio dividido a dos sale a 18px  

Con esta gran variedad de contenedores _bootstrap_ nos da opcion  a ir eligiendo el contenedor que mas nos convenga dependiendo de cuanto espaciado queramos darle  a nuestros elementos Si tu no quieres que tu contenido tenga un contenedor si no que fluya al 100% pues tambien tenemos la clase: `.container-fluid` con esto siempre va estar al 100%

Abajo en la documentación viene la forma para modificar los valores de espaciado via SASS

la otra seccion muy inportante es la GRID.

### Sección Layout: Grid de Bootstrap(Rows & Columns) 

**No vayan a confundirlo con el sistema de maquetacion de un css Grid** 

El diseño web se basó del diseño editorial y en el diseño editorial(revistas periodicos) su sistema de maquetación para desarrollar un proyecto editorial consta de 12 columnas se va distribuyendo el contenido de la revista, periodico. 

Entonces el diseño web al tomar como referencia los conceptos bases del diseño editorial pues tambien trajo esto del _Grid-sistem_ por eso es que la mayoria de los _Frameworks_ como _Bootstrap_ _Fundation_ y es un **Sistema de 12 columnas** 

![grid-system](/assets/grid-system.JPG)

```html
  <div class="container text-center">
  <div class="row">
    <div class="col">
      Column
    </div>
    <div class="col">
      Column
    </div>
    <div class="col">
      Column
    </div>
  </div>
</div>
```
En este pequeño ejemplo si el _grid_ de _bootstrap_ es de 12 elementos eso significa que 12 / 3columnas que voy a tener significa que cada columna puede ocupar  hasta 4 espacios de la grid de bootstrap, actualmente la grid de bootstrap está creada con flexbox 

El ejemplo anterior crea tres columnas de igual ancho en todos los dispositivos y ventanas gráficas utilizando nuestras clases de cuadrícula predefinidas. Esas columnas están centradas en la página con el padre .container.

![layout-grid](/assets/layout-grid.JPG)

esta tablita la tienen que tener muy presente cada vez que vayan a trabajar con bootstrap, por que te explica que tiene 12 columnas

para utilizar el sistema de columnas de bootstrap tu **puedes o no** meter a un contenedor tu estructura de maquetación pero lo que si es forzoso es un elemento de fila _`row`_

> OJO aqui bootstrap para su documentación siempre va estár utilizando las _divs_ en la medida de lo que puedan traten  de trabajar sementicamente no esten utilizando todo el tiempo `DIV` 

ve que las columnas se encerro en una clase llamada `.row` entonces para usar la grid de bootstrap las columnas se tienen que envolver en un contenedor ``row``. 

> Cuando ustedes vayan a maquetar en bootstrap lo ideal es que pienzen en que en cada fila de contenido debe ocupar 12 espacios de la grid entonces todos los elementos que ustedes quieren que compartan el mismo espacio deben de sumar 12 

eje: si van a tener un mapa y un formulario pero quizá el formulario es un poco mas grande que el mapa pues al mapa le dan 4 y al formulario 8 de tal menera que 4col mas 8col es igual a 12col 

> todo los elementos que ustedes quieran  que comparta la misma fila de contenido al final la sumatoria del numero de columnas tiene que dar 12

¿Por que en el ejemplo de bootstrap no viene ningun numerito? 
por que la grid de bootstrap acual está trabajando con flexbox  entonces gracias a la propiedad que tiene flexbox sobre sus hijos de ignorar al ancho y repartir el espacio proporcionalmente por eso es que acá yo no tuve que ponerle un prefijo de número a la columna y entonces como tiene 3 elementos la grid se adapta

si ejecuto el código demo, ve que el espacio lo divide proporcionalmente

¿Que pasa si es que agrego una columna más?

Gracias a que la grid de bootstrap está maquetada en flexbox se reparten el espacio proporcionalmente, mira que tengo 4 columnas del mismo tamaño

puedes omitir el `.container`

Entonces cuando tu queras que los elementos de las filas que te va formando bootstrap vayan a ser del mismo tamaño puedes omitir el especificar el número, pero cuando ya necesites que ciertos elementos ocupen cierto espaciado.

cuando tu necesites que los elementos que vayan a compartir en la fila de contenido que vayan a tener diferente número entonces para so sirven esta tablita: 

![layout-grid](/assets/layout-grid.JPG) 

esta tablita nos dice:

> en el tamaño extra-small  no hay ningun prefijo `.col` o `.col-`(si no vas a especificar numero de columna) como la `row` es flexbox

lo puesed buscar en la hoja de estilos indentada: `https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.css` 

```css
  .row {
  --bs-gutter-x: 1.5rem;
  --bs-gutter-y: 0;
  display: flex;
  flex-wrap: wrap; /*envuelve a los hijos y cuando los hijos empiezan a tener un 
  ancho específico si no alcanzan a caber en la primera fila de contenido, lo que va
  haciendo flexbox es generar una segunda fila, una tercera y una cuarta, etc
  
  Eso nos va dar el efecto de tener filas y columnas, no trabaja como GRID CSS donde ahi si
  podemos definir columnas y filas trabaja con el sistema de fexbox  y gracias a las propiedades
  de flexbox es que nos permiten tener este sistema de filas y columnas

  */
  margin-top: calc(-1 * var(--bs-gutter-y));
  margin-right: calc(-0.5 * var(--bs-gutter-x));
  margin-left: calc(-0.5 * var(--bs-gutter-x));
}
.row > * {
  flex-shrink: 0;
  width: 100%;
  max-width: 100%;
  padding-right: calc(var(--bs-gutter-x) * 0.5);
  padding-left: calc(var(--bs-gutter-x) * 0.5);
  margin-top: var(--bs-gutter-y);
}
```
Si tu sabes CSS vas a poderle sacar muchisimo provecho a Bootstrap si tu no sabes css tal ves ya te está saliendo humo de la cabeza

**Estableciendo un ancho de columna** 

cuando tu necesites que el ancho de las celdas de tus grids de bootstrap tengan mas espacios unas que otras entonces vas a empezar a utilizar el prefijo.

asi: 

```html
  <div class="container text-center">
      <div class="row">
        <div class="border col">
          Column
        </div>
        <div class="border col-6">
          Column
        </div>
        <div class="border col">
          Column
        </div>
        <div class="border col">
          Column
        </div>
      </div>
    </div>
```
![ancho](/assets/ancho-col.JPG)

La segunda columna ocupa la proporcion de 6 columnas 

![reticula](/assets/reticula.JPG)

```css
  .col-6 {
    flex: 0 0 auto;/*esta propiedad es la que a las columnas de bootstrap cuando no 
    las especificamos un ancho se adapta al tamaño (reparte el espacio entre los números de elementos que haya)
    pero cuando ya le agregamos un numerito estos se comvierte en un porcentaje que equivale a una 12va fraccion
    de la reticula que aco de diseñar en figma
    */
    width: 50%; /*tiene el ancho del 50%*/
  }
```

¿Que pasa cuando el numero de columnas especificados pasa de 12?

pues crea otra fila se desplaza a la fila siguiente

```html
<div class="container text-center">
      <div class="row">
        <div class="border col-3">
          Column
        </div>
        <div class="border col-6">
          Column
        </div>
        <div class="border col-3">
          Column
        </div>
        <div class="border col">
          Column
        </div>
      </div>
    </div>
```


![desplazamiento](/assets/desplazamiento.JPG)

¿y por que está ocupando todo el espacio? recuerda que esa cuarta columna no tiene un valor especificado, recuerda que gracias a la propiedad de `flex` lo que hace es ocupar el espacio disponible y como ya no hay mas columnas hermanas  ocupa todo el espacio disponible

en la version 3 la grid de bootstrap estaba maquetada con los viejos floats desde que bootstrap implementó  en su version 4 la grid con flexbox podemos tener la combinacion de ir definiendo el ancho especifico tomando en cuenta el sitema de referencia de 12 columnas o tambien ir aprovechando esto de si no especificamos el valor se va adaptar al espacio proporcional que sobre.

tienes que probar como es que van funcionando la mezcla de estas combinaciones tanto el 'tamaño de las mediaqueris(_breakpoints sm -lg, -xl_)' como por los números

> lo primero que vamos a hacer en este sitio que vamos a maquetar es ir definiendo esos tamaños

> Gracias a esto, bootstrap nos va permitir hacer interfaces responsivas muy cencillas 

> {TODO ES POR PORCENTAJES 100% / 12}


### Sección Layout: Grid Responsiva 

```html
  <h2>Grid Responsiva</h2>
    <!-- section.row>article.border.col-12.col-sm-6.col-md-4.col-lg-3.col-xl-2.col-xxl-1*19{Elemento $} -->
    <!-- 
      
      en el tamaño (extra-small)  quiero 1 columna entonces 12 / 1 = 12 [ojo, no tiene prefijo como los demas]
      en el tamaño SM  quiero 2 columnas entonces 12 / 2 = 6
      En el tamaño MD quiero 3 columnas entonces 12 / 3 = 4
      En el tamaño LG quiero 4 columnas entonces 12 / 4 = 3
      En el tamaño XL quiero 6 columnas entonces 12 / 6 = 2
      En el tamaño XXL quiero 12 columnas entonces 12 / 12 = 1
     -->

    <section class="row">
      <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 1</article>
      <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 2</article>
      <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 3</article>
      <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 4</article>
      <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 5</article>
      <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 6</article>
      <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 7</article>
      <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 8</article>
      <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 9</article>
      <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 10</article>
      <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 11</article>
      <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 12</article>
      <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 13</article>
      <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 14</article>
      <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 15</article>
      <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 16</article>
      <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 17</article>
      <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 18</article>
      <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 19</article>
    </section>
```

Cuando tu ya tienes la referencia quizá en un figma en una imagen la UI (iterface user) o como yo que ya tengo construido el sitio, va ser muy sencillo poder generarlo

Ve que las columnas fluyen al 100% de la pantalla

¿Que pasa si aplico la clase contenedor? 

pues lo que hace es dar un espaciado a los lados tanto de margen izuierdo como Derecho, 

![cabezera](/assets/cabezera.JPG)

mientras que el colorcito morado de la cabezera fluye al 100%  el contenido de la cabezera que va del logo al boton de modo oscuro, está  dentro de un contenedor

¿De que va depender?

![container](/assets/containers.JPG)

si pones por ejemplo `.container-lg` apartir de el punto de interrupcion de tamaño `lg` es que se aplica el contenedor para adelante:

```css
  .container,
.container-fluid,
.container-xxl,
.container-xl,
.container-lg,
.container-md,
.container-sm {
  --bs-gutter-x: 1.5rem;
  --bs-gutter-y: 0;
  width: 100%;
  padding-right: calc(var(--bs-gutter-x) * 0.5);
  padding-left: calc(var(--bs-gutter-x) * 0.5);
  margin-right: auto;
  margin-left: auto;
}
```

> Aquí el `.container-sm` en tamaño _Extra small_ va estár al 100% pero que en _small_ ya no va estar al 100% sino el maximo tamaño va tener 540px(**Es el tamaño que va tener el contenedor**) 

> Aquí la cuestion es que vayan viendo que contenedor les funciona, **Personalmente yo utilizo el container normalito** por que pues ya estoy acostumbrado a utilizarlo  muy pocas veces utilizé : `.container-sm,.container-md,.container-lg,.container-xl,.container-xxl,` pero no dudes en utilizarlo si lo necesitas

Si yo le pongo `.container-flid` a mi grid del contenedor se va conportar como la que no tiene contenedor y fluid al 100%, el contenedor fluido fluye al 100%

```html
   <h2>Grid Responsiva en un contenedor</h2>
    <div class="container-fluid">

      <section class="row">
        <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 1</article>
        <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 2</article>
        <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 3</article>
        <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 4</article>
        <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 5</article>
        <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 6</article>
        <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 7</article>
        <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 8</article>
        <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 9</article>
        <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 10</article>
        <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 11</article>
        <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 12</article>
        <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 13</article>
        <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 14</article>
        <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 15</article>
        <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 16</article>
        <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 17</article>
        <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 18</article>
        <article class="border col-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 col-xxl-1">Elemento 19</article>
      </section>
```

Tambien Podemos manejar alineacion horizontal, vertical, cambiar el orden de los elementos(order classes) pero tienes que tener conocimientos solidos de FlexBox.

¿Que pasa si yo quiero tener un espacio vacio entre 2 columnas?

_https://getbootstrap.com/docs/5.3/layout/columns/#offsetting-columns_

Muchos lo que hacen es establecer una div que tenga el número de columnas que va representar ese espacio vacio y lo dejan sin contenido pero eso a nivel de html no está bien dejar un elemento vacio, entonces para eso cuando nosotros necesitemos dejar espacios vacios  dentro de la grid de 12 columnas. para eso tenemos: 

**OFFSETTING-COLUMNS**

lo que hay que hacer es agregar la clase ``.offset`` , la media queri donde lo vayamos a querer aplicar y el numero de columnas que vamos a dejar hacia la izquierda: 

![offsetting-columns](/assets/offsetting-columns.JPG)



> Esto siempre va ser hacia la Izquierda. 

> a la derecha realmente si ya no tienes elementos ese espacio va quedar por defecto vacio por como estamos acostumbrados a trabajar el acomodo de los elementos en html y css.

### 


