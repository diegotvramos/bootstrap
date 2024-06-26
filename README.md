

# TALLER DE BOOTSTRAP




### Introduccion

`https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.css` Codigo fuente.

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

### Sección Layout: Gutters, Utilities y CSS Grid

**Gutters**

No es mas que el espaciado que podemos tener entre nuestras columnas, esto lo podemos trabajar a nivel de código css con el _padding_ y la propiedad _gap_ disponible en ``flexbox`` y en ``grid-css``

`https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_flexible_box_layoutTypical_use_cases_of_flexbox#card_layout_pushing_footer_down`

La propiedad CSS _grid-gap_ es una propiedad abreviada shorthand para grid-row-gap (en-US) y grid-column-gap que especifica los canales entre las filas y las columnas de la cuadrícula.

Más adelante en la seccion de clases utilitarias que hay clases que empiezan con `p` y otras que empiezan con `m` donde nos permiten aplicar tanto a los cuatro lados del modelo de caja como a los lados de forma independiente aplicar justamente ese espaciado tambien los podemos hacer con  con las clases que empiezan con `gx-5`(aplica gap en _x_ o _y_) 

```css
  .g-5,
  .gx-5 {
    --bs-gutter-x: 3rem;
  }
```

**Utilities**

si ustedes saben los fundamentos solidos de css le van a sacar muchisimo provecho a bootstrap y a cualquier framework.

Esta seccion de las `utilities` no es mas que la revición de todo los elementos de los cuales se utiliza bootstrap para crear su grid en CSS la propiedad `display` las opciones de flexbox el margin y el padding

**z-index (super-posición)**

Se usa cuando queremos darle profundidad a elementos que tengamos posicionados 

**Grid CSS**

la grid de bootstrap que ahorita está hecha con flexbox va estar diseñada y maquetada con `Grid css`


> Aviso: ¡nuestro sistema CSS Grid es experimental y está habilitado a partir de la versión 5.1.0! Lo incluimos en el CSS de nuestra documentación para mostrárselo, pero está deshabilitado de forma predeterminada. Continúe leyendo para aprender cómo habilitarlo en sus proyectos.


> CSS Grid es opcional. Deshabilite el sistema de cuadrícula predeterminado configurando $enable-grid-classes: falsey habilite CSS Grid configurando $enable-cssgrid: true. Luego, vuelve a compilar tu Sass.

```html
  <div class="grid text-center">
    <div class="g-col-3 g-start-2">.g-col-3 .g-start-2</div>
    <div class="g-col-4 g-start-6">.g-col-4 .g-start-6</div>
  </div>
```
Aún está en una version experimental

tal vez en la version 6, la grid oficial de bootstrap que actualmente está en _Flexbox_ se remplase por _grid_,  aquí todas estas nuevas opciones que flexbox, ya se implemento a la grid de bootsprap como alineacion vertical, horizontal lo de los espaciados `gutters` eso no se pierde

> por que muchas de las propiedades de alineacion, ordenamiento y espaciado en Flexbox Funcionan exactamente igual en grid

> Tienes que tener nociones, y conocimientos solidos de CSS por que sino va ser muy dificil que puedas sacar el maximo provecho a estas herramientas, es como querrerte saltar a programar en react.js y no tener conocimientos solidos de JavaScript, del DOM

Creo que entender la _Grid_ de bootstrap es lo mas importante ya de ahi en fuera va ser leer la documentacion del componente o de la opcion que queras utilizar ver los nombres de las clases, copiar y pegar código

### Sección Content

Tiene que ver con todo el reinicio de algunos elementos HTML, es la normalizacion que hace Bootstrap de las etiquetas html, tambien nos van a dar algunas variables que si tu trabajas en bootstrap con ``sass`` las vas a poder modificar como: El tamaño de la letra, la familia de fuentes color de texto el color de fondo, alineacion.

tamaño de los encabezados, las etiquetas hr(reglas horizontales) los elementos de lista, diseño predeterminado de las tablas... etc

> Esta seccion es basicamente para que te des una idea de como inicia nativamente cada etiqueta html o cada grupo de etiquetas html en bootstrap tambien tiene la seccion de tipografia.

**Typography**

podemos ver el tamaño de los encabezados, las clases por que bootstrap tiene una clase particular.
```html
  <h1>h1. Bootstrap heading</h1>
  <h2>h2. Bootstrap heading</h2>
  <h3>h3. Bootstrap heading</h3>
  <h4>h4. Bootstrap heading</h4>
  <h5>h5. Bootstrap heading</h5>
  <h6>h6. Bootstrap heading</h6>



<!-- como son h1 o h2 usan el mismo tamaño -->
  <p class="h1">h1. Bootstrap heading</p>
  <p class="h2">h2. Bootstrap heading</p>
  <p class="h3">h3. Bootstrap heading</p>
  <p class="h4">h4. Bootstrap heading</p>
  <p class="h5">h5. Bootstrap heading</p>
  <p class="h6">h6. Bootstrap heading</p>
```
tanto a la etiqueta como a la clase tiene el mismo tamaño.

```css
  h1, .h1 {
  font-size: calc(1.375rem + 1.5vw);
}
```

` <p class="h1">DIEGO villacorta</p>` pero funciona, lo utilizaria por diseño  (por semantica solo debemos tener un encabezado h1) por página pero le puedes dar a cualquier párrafo el tamaño de la h1, h2 ... por que botstrap trae esas clases

**Display**

es un tamaño de letra mas grande, se puede usar para las _Hero-image_

```css
  .display-1 {
    font-size: calc(1.625rem + 4.5vw); /*significa que si tú a un texto le aplicas la clase 
    display 1 va estar creciendo proporcionalmente no se va mantener estático este es un concepto
    del diseño FLUIDO (FLUID DESIGN) 
    */
    font-weight: 300;
    line-height: 1.2;
  }
```

desde la version 5 de bootstrap ya utilizan muchas de las funciones avanzadas de css como calc, min, max.

Lo que hace bootstrap con su tipografia  es hacer una _tipografia responsiva_ 

**Elementos de texto en linea**

![inline-text-elements](/assets/text-line-elements.JPG)

```html
  <p>You can use the mark tag to <mark>highlight</mark> text.</p>
  <p><del>This line of text is meant to be treated as deleted text.</del></p>
  <p><s>This line of text is meant to be treated as no longer accurate.</s></p>
  <p><ins>This line of text is meant to be treated as an addition to the document.</ins></p>
  <p><u>This line of text will render as underlined.</u></p>
  <p><small>This line of text is meant to be treated as fine print.</small></p>
  <p><strong>This line rendered as bold text.</strong></p>
  <p><em>This line rendered as italicized text.</em></p>
```
tamtien tiene estilos para las citas:
**blockquotes**


**nombrar a una fuente**

![naming-a-source](/assets/naming.JPG)

```html
  <figure>
  <blockquote class="blockquote">
    <p>A well-known quote, contained in a blockquote element.</p>
  </blockquote>
  <figcaption class="blockquote-footer">
    Someone famous in <cite title="Source Title">Source Title</cite>
  </figcaption>
</figure>
```

**Alignmente** 
Una crítica bastante constructiva, yo no sé por que lo cambiaron, y esto lo vamos a ver en la seccion de los padding y los margins, bootstrap desde sus inicios tiene  4 clases para alinear el texto: ``text-left, text-center, text-righ, text-justify`` y las clases que tenian que ver con `margin-rigt, margin-left, o pading-right, pading-left` abreviando era(ml, pl, pr)

pero en la vercion 5 se les ocurio la idea de para hacerlo mas orientado al modelo de alineacion  del box model ahora todo lo que era `left` fue remplazado por `Start` y todo lo que tiene que ver con `right` fue remplazado por `end`

```html
  <figure class="text-end">
  <blockquote class="blockquote">
    <p>A well-known quote, contained in a blockquote element.</p>
  </blockquote>
  <figcaption class="blockquote-footer">
    Someone famous in <cite title="Source Title">Source Title</cite>
  </figcaption>
</figure>
```

```css
  .text-end {
    text-align: right !important;
  }
```

**Images**

Yo pensaria que las imagenes fueran por defecto default responsivas pero no, si tu quieres que la imagen sea responsiva osea el `max-width:100%`tienes que usar la clase `.img-fluid`

```css
  .img-fluid {
  max-width: 100%;
  height: auto;
}
```

**La Etiqueta Picture**

nos permite tener imagenes responsivas y adaptables

Si está utilizando el ``<picture>``elemento para especificar varios ``<source>``elementos para un elemento específico ``<img>``, asegúrese de agregar las .img-*clases a la etiqueta ``<img>``y no a la ``<picture>``misma.

```html
  <picture>
  <source srcset="..." type="image/svg+xml">
  <img src="..." class="img-fluid img-thumbnail" alt="...">
</picture>
```

**Tables**
nos explica los diferentes estilos que le podemos aplicar a las tablas y a sus elementos, recuerda que como toda la parte de la documentacion es que te des cuenta  que clases tienes que activar o desactivar  en tus elementos HTML 

**Figure**

Documentación y ejemplos para mostrar imágenes y texto relacionados con el componente de figura en Bootstrap.

```html
  <figure class="figure">
  <img src="..." class="figure-img img-fluid rounded" alt="...">
  <figcaption class="figure-caption">A caption for the above image.</figcaption>
</figure>
```

### Sección Forms.

la primera sección es un  _Overview_ aca nos da los detalles de los elementos de formulario.

Asegúrese de utilizar un typeatributo apropiado en todas las entradas (por ejemplo, emailpara direcciones de correo electrónico o numberinformación numérica) para aprovechar los controles de entrada más nuevos, como verificación de correo electrónico, selección de números y más.

Imagina que tu queres colocar en una aplicación un tipico formulario de Login que pide correo y password. pues mira que ya tienes un demo funcional de bootstrap. `https://getbootstrap.com/docs/5.3/forms/overview/#overview`

```html
  <form>
  <div class="mb-3">
    <label for="exampleInputEmail1" class="form-label">Email address</label>
    <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp">
    <div id="emailHelp" class="form-text">We'll never share your email with anyone else.</div>
  </div>
  <div class="mb-3">
    <label for="exampleInputPassword1" class="form-label">Password</label>
    <input type="password" class="form-control" id="exampleInputPassword1">
  </div>
  <div class="mb-3 form-check">
    <input type="checkbox" class="form-check-input" id="exampleCheck1">
    <label class="form-check-label" for="exampleCheck1">Check me out</label>
  </div>
  <button type="submit" class="btn btn-primary">Submit</button>
</form>
```

Y es la ventaja de Un framework, que ya nos dá cosas preestablecidas.

![login](/assets/login.JPG)

> Recuerda! los elementos de los formularios, los `inputs` son elementos que trabajand en linea(ocupan el espacio que requieren) pues bootstrap los hace elementos de bloque, vé que por eso el formulario está fluyendo al 100% de la pantalla

Pues meterle validaciones por JavaScript validaciones a travez del atributo ``pattern, require`` de html

```html
<form>
  <!--desabilita todo el formulario, 'disabled' es como una propiedad de la etiqueta <fieldset> -->
  <fieldset disabled> 
    <legend>Disabled fieldset example</legend>
    <div class="mb-3">
      <label for="disabledTextInput" class="form-label">Disabled input</label>
      <input type="text" id="disabledTextInput" class="form-control" placeholder="Disabled input">
    </div>
    <div class="mb-3">
      <label for="disabledSelect" class="form-label">Disabled select menu</label>
      <select id="disabledSelect" class="form-select">
        <option>Disabled select</option>
      </select>
    </div>
    <div class="mb-3">
      <div class="form-check">
        <input class="form-check-input" type="checkbox" id="disabledFieldsetCheck" disabled>
        <label class="form-check-label" for="disabledFieldsetCheck">
          Can't check this
        </label>
      </div>
    </div>
    <button type="submit" class="btn btn-primary">Submit</button>
  </fieldset>
</form>
```
> si quieren aprender otro framework, nomas es guiarse de la documentación 

`https://getbootstrap.com/docs/5.3/forms/form-control/`

```html
  <div class="mb-3">
  <label for="exampleFormControlInput1" class="form-label">Email address</label>
  <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="name@example.com">
</div>
<div class="mb-3">
  <label for="exampleFormControlTextarea1" class="form-label">Example textarea</label>
  <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
</div>
```

la clase `class="form-control"` eso es lo que le da los estilos muy caracteristicos de los inputs de formulario de bootstrap

Hay clases para controlar el tamaño de la caja

> Solo tienes que poner atención e ir leyendo la documentación para aplicar las diferentes opciones que tiene bootstrap

* Tiene inputs-files de _CARGA DE ARCHIVOS_

* hay el input de tipo color


*`https://getbootstrap.com/docs/5.3/forms/form-control/#datalists`*
* tambien los _data lists_  autocompleta las palabras

Las listas de datos le permiten crear un grupo de ``<option>``mensajes de correo electrónico a los que se puede acceder (y completar automáticamente) desde un archivo ``<input>``. Son similares a ``<select>``los elementos, pero vienen con más limitaciones y diferencias en el estilo del menú. Si bien la mayoría de los navegadores y sistemas operativos incluyen cierto soporte para ``<datalist>``elementos, su estilo es, en el mejor de los casos, inconsistente.

```html
<label for="exampleDataList" class="form-label">Datalist example</label>
<input class="form-control" list="datalistOptions" id="exampleDataList" placeholder="Type to search...">
<datalist id="datalistOptions">
  <option value="San Francisco">
  <option value="New York">
  <option value="Seattle">
  <option value="Los Angeles">
  <option value="Chicago">
</datalist>
```

**select**


```html
<select class="form-select" aria-label="Default select example">
  <option selected>Open this select menu</option>
  <option value="1">One</option>
  <option value="2">Two</option>
  <option value="3">Three</option>
</select>
```

**Checks & radios**

```html
<div class="form-check">
  <input class="form-check-input" type="radio" name="flexRadioDefault" id="flexRadioDefault1">
  <label class="form-check-label" for="flexRadioDefault1">
    Default radio
  </label>
</div>
<div class="form-check">
  <input class="form-check-input" type="radio" name="flexRadioDefault" id="flexRadioDefault2" checked>
  <label class="form-check-label" for="flexRadioDefault2">
    Default checked radio
  </label>
</div>
```

Y al final para aquellos que vayan a utilizar _bootstrap con SASS_ mira que vienen toda las variables y esas variables tu desde SASS las puedes modificar pero recuerda que:

> tu desde Bootstrap trae varias variables css en su hoja de estilos nativa que tambien nosotros podemos modificar.

Lo primero que tiene bootstrap es la definicion de toda las variables css con las que trabaja, entonces todas estas las vamos a poder modificar.

**Range**

Los inputs de tipo rango

**Input group**
la etiqueta y el input se vuelve un elemento agrugado.

![input-group](/assets/input-group.JPG)

**layout**

Disposición, aca algunos acomodos, se está ayudando del sistema de grid

![layout](/assets/layout-form.JPG)

```html
  <div class="row">
  <div class="col">
    <input type="text" class="form-control" placeholder="First name" aria-label="First name">
  </div>
  <div class="col">
    <input type="text" class="form-control" placeholder="Last name" aria-label="Last name">
  </div>
</div>
```

**Validation**


Cómo funciona
Así es como funciona la validación de formularios con Bootstrap:

La validación de formularios HTML se aplica a través de dos pseudoclases de CSS ``:invalidy :valid``. Se aplica a ``<input>``, ``<select>``y ``<textarea>``elementos.

¿que es una pseudoclases de CSS?

Pseudo-classes
Una pseudoclase CSS es una palabra clave que se añade a los selectores y que especifica un estado especial del elemento seleccionado. Por ejemplo, :hover aplicará un estilo cuando el usuario haga hover sobre el elemento especificado por el selector.


```css
  div:hover {
  background-color: #F89B4D;
}
```

Las pseudoclases, junto con los pseudoelementos, permiten aplicar un estilo a un elemento no sólo en relación con el contenido del árbol de documento, sino también en relación a factores externos como el historial del navegador (:visited, por ejemplo), el estado de su contenido (como :checked en algunos elementos de formulario), o la posición del ratón (como :hover que permite saber si el ratón está encima de un elemento o no).

Nota: En lugar de usar pseudoclases, pseudo-elements puede usarse para dar estilo a una parte específica de un elemento.

Sintaxis
``selector:pseudoclase { propiedad: valor; }``

Al igual que las clases, se pueden concatenar la cantidad de pseudoclases que se deseen en un selector.

Indice de las pseudo-clases estándar
:active
:checked
:default
:dir()
:disabled
:empty
:enabled
:first
:first-child
:first-of-type
:fullscreen
:focus
:hover
:indeterminate
:in-range
:invalid
:lang()
:last-child
:last-of-type
:left
:link
:not()
:nth-child()
:nth-last-child()
:nth-last-of-type()
:nth-of-type()
:only-child
:only-of-type
:optional
:out-of-range
:read-only
:read-write
:required
:right
:root
:scope (en-US)
:target
:valid
:visited


al momento de darle submit from, con colores nos dijo: esto está bien, esto está mal

![alt text](/assets/validation-form.JPG)

```html
  <form class="row g-3 needs-validation" novalidate>
  <div class="col-md-4">
    <label for="validationCustom01" class="form-label">First name</label>
    <input type="text" class="form-control" id="validationCustom01" value="Mark" required>
    <div class="valid-feedback">
      Looks good!
    </div>
  </div>
  <div class="col-md-4">
    <label for="validationCustom02" class="form-label">Last name</label>
    <input type="text" class="form-control" id="validationCustom02" value="Otto" required>
    <div class="valid-feedback">
      Looks good!
    </div>
  </div>
  <div class="col-md-4">
    <label for="validationCustomUsername" class="form-label">Username</label>
    <div class="input-group has-validation">
      <span class="input-group-text" id="inputGroupPrepend">@</span>
      <input type="text" class="form-control" id="validationCustomUsername" aria-describedby="inputGroupPrepend" required>
      <div class="invalid-feedback">
        Please choose a username.
      </div>
    </div>
  </div>
  <div class="col-md-6">
    <label for="validationCustom03" class="form-label">City</label>
    <input type="text" class="form-control" id="validationCustom03" required>
    <div class="invalid-feedback">
      Please provide a valid city.
    </div>
  </div>
  <div class="col-md-3">
    <label for="validationCustom04" class="form-label">State</label>
    <select class="form-select" id="validationCustom04" required>
      <option selected disabled value="">Choose...</option>
      <option>...</option>
    </select>
    <div class="invalid-feedback">
      Please select a valid state.
    </div>
  </div>
  <div class="col-md-3">
    <label for="validationCustom05" class="form-label">Zip</label>
    <input type="text" class="form-control" id="validationCustom05" required>
    <div class="invalid-feedback">
      Please provide a valid zip.
    </div>
  </div>
  <div class="col-12">
    <div class="form-check">
      <input class="form-check-input" type="checkbox" value="" id="invalidCheck" required>
      <label class="form-check-label" for="invalidCheck">
        Agree to terms and conditions
      </label>
      <div class="invalid-feedback">
        You must agree before submitting.
      </div>
    </div>
  </div>
  <div class="col-12">
    <button class="btn btn-primary" type="submit">Submit form</button>
  </div>
</form>
```

Acá pueden ver los elementos que se están agregando una `div` con el texto _Looks good!_  con la clase `class="valid-feedback"` ahora muy importante.

> tenemos que respetar los IDs y los atributos name, por que es justamente de esa manera como va reaccionar justamente esas validaciones.

Adicionalmente hay que agregar un par de codigo JavaScript 

```javaScript
  // Example starter JavaScript for disabling form submissions if there are invalid fields
(() => {
  'use strict'

  // Fetch all the forms we want to apply custom Bootstrap validation styles to
  const forms = document.querySelectorAll('.needs-validation')

  // Loop over them and prevent submission
  Array.from(forms).forEach(form => {
    form.addEventListener('submit', event => {
      if (!form.checkValidity()) {
        event.preventDefault()
        event.stopPropagation()
      }

      form.classList.add('was-validated')
    }, false)
  })
})()
```
ejecutas esto en tu programación javaScript,  si lo analizamos, se está autoejecutando por que está en una función anonima autoejecutable está usando el modo estricto  y guarda en una constante `forms` todo los elementos que coincidan con la clase `.needs-validation` por eso es muy importante respetar las clases y los atributos que bootstrap nos ofrecen en su marcado html como esto genera un list node del dom que como tal no es un arreglo aquí gracias al metodo `Array.from(forms).forEach` le permite a esta variable `forms` poder utilizar todo los métodos que tienen los arreglos y entonces poder ejecutar el forEach y lo que está haciendo hasta cierto punto es una mala práctica está generando un  `.addEventListener('submit',` de tipo _submit_ por cada elemento de formulario que exista 

y agrega está clase: `'was-validated'` buscalá en la hoja de css de Bootstrap

Si ustedes quisieran modificar los estilos que ya trae predeterminanamente las clases  de bootstrap. OJO 👁 No lo hagan en hoja de estilos de Bootstrap sinó en una independiente ustedes van haciendo esas modificaciones para que por cascada primero tome los de bootstrap y luego al cargar su hoja de estilos que seria la última que tendria que cargar entonces detecte las modificaciones.

Asi es como lo vamos a hacer 😉

A manera de mejora, yo en lugar de hacer por cada formulario activar un manejador de eventos yo haria la tecnica de la delegación de eventos de al documento asignarle el _Submit_ y simplemente detectar el _target_ si es un formulario desencadenar la programación 

**Validation - tooltips**

![tooltips](/assets/tooltips-form.JPG)

en lugar de que salga los mensajes de navegacion en el documento html,  salen como Tooltips, 

> recuercuerda el codigo fuente de bootrap trane integrada  la libreria _Pooper_ recuerda que en el guetting started nos ofrecian tener separada  la libreria _Pooper_ es la que utiliza bootrap para generar estos `tooltips`

si ustedes eligieron solo el codigo javaScript de bootstrap sin el `Pooper` esto no les va funcionar, por eso para mi por unos cuantos kilobites de lo que pesa la libreria _Pooper_ prefiero integrar el archivo JS que ya trae a pooper y el código fuente de bootstrap.

Tambien puedes modificar los estilos que trae por defecto con SASS.

> ¡TODO RADICA EN ESTAR LEYENDO Y PONIENDOLE ATENCIÓN A LA DOCUMENTACION!

### Components

La seccion de componenetes es una lista de todo los elementos visuales de IU.

Vienen en orden alfabético, tienes que estar leyendo la ducumentación, poner atención, respetar los nombres de clase, los _Data-attributs_ que trae.

los _``Data-attributs``_ son los que permiten cambiar cierto comportamiento en la interactividad.

> Te invito a que leeas a detalle la documentación  de cada uno de los componentes que pretendas utilizar y al igual que en las otas secciones acá abajo viene todo el control de las variables para SASS. Y LAS VARIABLES DISPONIBLES EN CSS. En la hoja de estilos nativa purita.

> Acuerdate que al inicio tiene una sección con toda las variables globales que utiliza pero cada componente internamente trae sus propias variables y eso hace muy comodo la modificacíon directamente  con CSS si no utilizas SASS {ME GUSTA TRABAJAR CON EL CSS ARTESANAL, EL CSS PURO} ami no me gusta usar este tipo de metalenguajes y preprocesadores como SASS 

```css
  --#{$prefix}accordion-color: #{$accordion-color};
--#{$prefix}accordion-bg: #{$accordion-bg};
--#{$prefix}accordion-transition: #{$accordion-transition};
--#{$prefix}accordion-border-color: #{$accordion-border-color};
--#{$prefix}accordion-border-width: #{$accordion-border-width};
--#{$prefix}accordion-border-radius: #{$accordion-border-radius};
--#{$prefix}accordion-inner-border-radius: #{$accordion-inner-border-radius};
--#{$prefix}accordion-btn-padding-x: #{$accordion-button-padding-x};
--#{$prefix}accordion-btn-padding-y: #{$accordion-button-padding-y};
--#{$prefix}accordion-btn-color: #{$accordion-button-color};
--#{$prefix}accordion-btn-bg: #{$accordion-button-bg};
--#{$prefix}accordion-btn-icon: #{escape-svg($accordion-button-icon)};
--#{$prefix}accordion-btn-icon-width: #{$accordion-icon-width};
--#{$prefix}accordion-btn-icon-transform: #{$accordion-icon-transform};
--#{$prefix}accordion-btn-icon-transition: #{$accordion-icon-transition};
--#{$prefix}accordion-btn-active-icon: #{escape-svg($accordion-button-active-icon)};
--#{$prefix}accordion-btn-focus-box-shadow: #{$accordion-button-focus-box-shadow};
--#{$prefix}accordion-body-padding-x: #{$accordion-body-padding-x};
--#{$prefix}accordion-body-padding-y: #{$accordion-body-padding-y};
--#{$prefix}accordion-active-color: #{$accordion-button-active-color};
--#{$prefix}accordion-active-bg: #{$accordion-button-active-bg};
```
Al buscar la clase _.accordion_ en la hoja de estilos css. ve que están todas esas variables que me está listando bootstrap en la documentación y acá el valor por defecto,  si yo quisiera modificar el color del acordion de un `--bs-body-color: #212529;` lo puedo hacer en mi hoja.

> no es que vayas a modificar la hoja de estilos de bootstrap, lo ideal cuando empiezas a hacer un proyecto es cargar la hoja de estilos y debajo cargar tu hoja propia donde ahi vas hacer modificaciones

```css
.accordion {
  --bs-accordion-color: var(--bs-body-color);
  --bs-accordion-bg: var(--bs-body-bg);
  --bs-accordion-transition: color 0.15s ease-in-out, background-color 0.15s ease-in-out, border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out, border-radius 0.15s ease;
  --bs-accordion-border-color: var(--bs-border-color);
  --bs-accordion-border-width: var(--bs-border-width);
  --bs-accordion-border-radius: var(--bs-border-radius);
  --bs-accordion-inner-border-radius: calc(var(--bs-border-radius) - (var(--bs-border-width)));
  --bs-accordion-btn-padding-x: 1.25rem;
  --bs-accordion-btn-padding-y: 1rem;
  --bs-accordion-btn-color: var(--bs-body-color);
  --bs-accordion-btn-bg: var(--bs-accordion-bg);
  --bs-accordion-btn-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='none' stroke='%23212529' stroke-linecap='round' stroke-linejoin='round'%3e%3cpath d='M2 5L8 11L14 5'/%3e%3c/svg%3e");
  --bs-accordion-btn-icon-width: 1.25rem;
  --bs-accordion-btn-icon-transform: rotate(-180deg);
  --bs-accordion-btn-icon-transition: transform 0.2s ease-in-out;
  --bs-accordion-btn-active-icon: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='none' stroke='%23052c65' stroke-linecap='round' stroke-linejoin='round'%3e%3cpath d='M2 5L8 11L14 5'/%3e%3c/svg%3e");
  --bs-accordion-btn-focus-box-shadow: 0 0 0 0.25rem rgba(13, 110, 253, 0.25);
  --bs-accordion-body-padding-x: 1.25rem;
  --bs-accordion-body-padding-y: 1rem;
  --bs-accordion-active-color: var(--bs-primary-text-emphasis);
  --bs-accordion-active-bg: var(--bs-primary-bg-subtle);
}
```

**Alerts**
Si quieres poner algunos mensajes les puedes poner los colores que ya trae bootstrap

**Badge**
Que son como las notificaciones que vemos en redes sociales

**Breadcrumb**

![migaja](/assets/migaja.JPG)

menus que vemos como de navegación  que se llaman 'migajas de pan' que suelen ser  muy frecuentes en comercios electrónicos donde estamos en una categoria pasamos a una subcategoria, pasamos al producto

**Buttons** 

tenemos grupo de botones

**Card**

Las típicas targetas

**Collapse**
Son como los toogles que nos permiten mostrar y ocultar contenido, de hecho el collapse se usa en el `navbar`

**Dropdowns**

Que nos permiten generar submenús  de una opcion 

**Modal**

ventana modal

**NavBar**

Es de los primeros que vamos a utilizar y que nos va permitir formar nuestro menú de navegación 

**Navs & tabs** 

navegacion por secciones

**Offcanvas**
![offcanvas](/assets/offcamvas.JPG)

cuando nosotros tenemos un elemento que sale, un panel de navegación esto puede ser como el típico boton de hamburguesa

o la interfaz de YOUTUBE todo el menú de navegación que tiene youtube mas o menos funciona de esta forma

**Pagination**
En caso de que estés aciendo una aplicación que traiga resultados de una base de datos y los quieras paginar

**Placeholders**

![placeholders](/assets/placeholders.JPG)

Cuando está como cargando (cuando está tardando la interfaz) y ya luego se reemplaza por el contenido

**Scrollspy**

![scrollspy](/assets/scrollspy.JPG) 

conforme vas avanzando te va mostrando la seccion en la que te encuentras. {tendriamos que programarlo para que se active solo en tamaño de escritorio}


en las versiones 4 de bootstrap no tenia tantas variables css para el control de los elementos. 
En estas ultimas versiones de bootstrap restructuraron en el código fuente de Bootstrap, si tu comparas la hoja de estilos de bootstrap 4 con cualquiera de la 5, cada uno de los componentes no tenia su lista personalizada de las variables que utilizaba,

Ahora al tener cada componente su propio conjunto de variables eso permite hacer mas amigable  la personalizacion 😊😊 por que tu ya no tendrias que meterte con sobreescribir el codigo css de bootstrap simplemente irte a las variables de cada componente que te interesa modificar y hacer la modificacion pertinente

**tooltips**

la mayoria de los componentes de bootstrap tu vas a tener que meter codigo javaScript para hacerlos funcionar.

¿Como funciona?

en base a las clases css que tienen activadas y a los diferentes `Data-attributs` ej: `data-bs-placement` que bootstrap a creado con los diferentes valores.

al tu ya tener bien codificado tu código html entonces la programación js lee ese código html y ya hace funcionar al componente de esa manera

```html
  <button type="button" class="btn btn-secondary" data-bs-toggle="tooltip" data-bs-placement="top" data-bs-title="Tooltip on top">
  Tooltip on top
</button>
<button type="button" class="btn btn-secondary" data-bs-toggle="tooltip" data-bs-placement="right" data-bs-title="Tooltip on right">
  Tooltip on right
</button>
<button type="button" class="btn btn-secondary" data-bs-toggle="tooltip" data-bs-placement="bottom" data-bs-title="Tooltip on bottom">
  Tooltip on bottom
</button>
<button type="button" class="btn btn-secondary" data-bs-toggle="tooltip" data-bs-placement="left" data-bs-title="Tooltip on left">
  Tooltip on left
</button>
```

### Sección Helpers

traducido al español seria como los Auxiliares

Mientras que los componentes son un elemento que tiene parte interactiva pero con parte visual, 

Un Auxiliar es algo, es como un componenete que tiene la parte de código, nos ayuda a modificar algunas cosas

#### Clearfix

Esto ya es bastante viejo, yo les sugiero no utilizar,

Hace 10 años cuando no existia _FLEXBOX ni GRIDCSS_ la unica manera era con _Floats_ 

```css
  @mixin clearfix() {
  &::after {
    display: block;
    clear: both;
    content: "";
  }
}
```

era un hack muy utilizado en el diseño web

#### Color & Background 

los colores base que trae bootstrap son 8 colores 
![colores](/assets/colores.JPG)

```html
  <div class="text-bg-primary p-3">Primary with contrasting color</div>
<div class="text-bg-secondary p-3">Secondary with contrasting color</div>
<div class="text-bg-success p-3">Success with contrasting color</div>
<div class="text-bg-danger p-3">Danger with contrasting color</div>
<div class="text-bg-warning p-3">Warning with contrasting color</div>
<div class="text-bg-info p-3">Info with contrasting color</div>
<div class="text-bg-light p-3">Light with contrasting color</div>
<div class="text-bg-dark p-3">Dark with contrasting color</div>
```

> lo puedes aplicar tanto en el fondo `class="bg-dark"`, como en el color de texto `class="text-primary"` 


```html
  <p class="text-white bg-danger">
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sit beatae nisi nulla quaerat amet vitae sequi asperiores quae possimus praesentium fugit corrupti nihil delectus mollitia reiciendis, esse voluptates corporis. Assumenda.
    </p>
```

Simplemente es que te adaptes a la nomenclatura de las clases que nos ofrece CSS 

#### Colored links 

Desde html5 el color de los enlaces ya tiene un color predeterminado Azul y cuando lo usamos se pone morado, 

```html
  <a href="#" class="display-1">Enlace color por defecto</a>
  <!--  -->
    <a href="#" class="display-1 text-primary">Enlace</a> 
    <a href="#" class="display-1 link-warning">Enlace</a>
```
Lo que hace es modificar el color pro boootstrap nos está ofreciendo los estilos particulares

¿Entonces Cúal es la diferencia?

el enlace que utilizó la clase `class="text-primary"` no hace ningun efecto (hover) al pasar el cursor por encima como los demas enlaces si lo hacen


#### Anillo de enfoque
Clases de utilidad que le permiten agregar y modificar estilos de anillos de enfoque personalizados a elementos y componentes.


#### enlace de icono (Icon link)

```html
   <h2>enlace de icono (Icon link)</h2>
    <a class="icon-link icon-link-hover" style="--bs-icon-link-transform: translate3d(0, -.125rem, 0);" href="#">
      <svg class="bi" aria-hidden="true"><use xlink:href="#clipboard"></use></svg>
      Icon link
    </a>
```

#### Position 

Para posicionar un elemento

**Fixed top**

* `<div class="fixed-top">...</div>`

* `<div class="sticky-top">...</div>`


Una de las cosas por la que bootstrap se ha vuelto muy popular es que todas estas utilidades  y clases auxiliares  que nos ofrece en todo los espectros de las mediaquerys

**Responsive sticky top**

```html
  <div class="sticky-sm-top">Stick to the top on viewports sized SM (small) or wider</div>
<div class="sticky-md-top">Stick to the top on viewports sized MD (medium) or wider</div>
<div class="sticky-lg-top">Stick to the top on viewports sized LG (large) or wider</div>
<div class="sticky-xl-top">Stick to the top on viewports sized XL (extra-large) or wider</div>
<div class="sticky-xxl-top">Stick to the top on viewports sized XXL (extra-extra-large) or wider</div>
```

ejemplo, en la version pequeña la quiero abajo, y en la version large (lg) lo quiero arriba, si yo voy invocando estas clases, esrtas clases se van modificando a lo largo del espectro de las media queris


```html
   <h2>Positions</h2>
    <!-- eso quiere decir que desde el mobil va empesar pegada abajo, y con 'sticky-lg-top' entonces se va ir arriba -->
    <nav class="sticky-bottom sticky-lg-top display-2 text-danger">Stiky Responsive Nav</nav>
```

Como es un comportamiento `sticky`

> recuerda que en el `sticky` debe de haver contenido y se va quedar pegada cuando llegue a top, entonces para poder hacer eso ¿que puedo hacer yo en mi código? pues crear 50 _<br>_ 

> mientras cualquier tamaño menor a large _LG_ ve que el posicionamiento es abajo

ve como todas estas clases que nos va ofrecer utilitarias y auxiliares bootstrap menejan el espectro de toda las mediaQueris disponibles en el framework, es increible, por que en lugar de que tu te vayas a tu hoja de estilos y vayas haciendo tus mediaQueris y creando tus estilos aca simplemente vas activando las clases que necesites a lo largo del espectro de las media querys.

Los puristas de CSS van a decir: "tu codigo html va quedar muy verboso" pero hagamos conciencia de algo:

imagina que estas trabajando en un proyecto, donde quizá la parte mas importante es la programación, la lógica la coneccion a la base de datos y la IU. la puedes hacer con Bootstrap, por que no es tan detallada como el trabájo en la parte de la programación , entonces _Y o no perderia el tiempo haciendo artesanalmente cuando Bootstrap me ofrece esto_ 

Mi sitio web es como mi jardin personal, por eso es que lo tengo con código css purito, como es un proyecto personal y yo me tomo el tiempo, y tambien me sirve para practicar codigo css artesanal pues ahi no voy a utilizar bootstrap.

> Hay que saber en que proyectos combiene o no utilizar esto, cuando yo necesite agilidad en el desarrollo y la construccion de mis interfaces por supuesto que voy a utilizar un framework frontend, cuando la prioridad sea la parte des servidor, la logica de la programacion, la interactividad con javaScript por su puesto que voy a preferir la ayuda de un framework como bootstrap.


#### Ratio

Hay una nueva propiedad en css que se llama `aspect-ratio`. 

Antes para poner en La pantalla ancha o pantalla panorámica (en inglés: widescreen) un video de Youtube y para que no se hiciera cuadrado extraño, habia una tecnica de aplicar un `padding-booton` de 56.25% 

si pegamos un _Iframe de youtube_ aparentemente está bien, pero cuando tenemos la pantalla mas pequeña  al frame de youtube, ve que ya no es resposivo.

Pero lo puedo hacer responsivo y que se vea correctamente dependiendo del `aspect-ratio` 


```html
  <div class="ratio ratio-1x1">
  <div>1x1</div>
</div>
<div class="ratio ratio-4x3">
  <div>4x3</div>
</div>
<div class="ratio ratio-16x9">
  <div>16x9</div>
</div>
<div class="ratio ratio-21x9">
  <div>21x9</div>
</div>
```

la que nos comviene es la `16x9` es como la version  en formato _widescreen_  si usamos `<div class="ratio ratio-16x9">` ya se hace responsivo  y en forma horizontal.

> Ve que con esas clases tenemos un video de youtube totalmente responsivo y adaptable

```html
  <h2>ratios</h2>
    <div  class="ratio ratio-16x9">
      <iframe width="560" height="315" src="https://www.youtube.com/embed/JuBBIJ7adjM?si=gXcmqLlKg8lGDwwF" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>
```

#### Stacks 

Estos son pequeños helpers para ayudarnos a la alineación de los _layout_ en formato vertical u horizontal

**Vertical**

Úselo .`vstack` para crear diseños verticales. Los elementos apilados tienen el ancho completo de forma predeterminada. Utilice `.gap-*` utilidades para agregar espacio entre elementos.

```html
  <div class="vstack gap-3">
  <div class="p-2">First item</div>
  <div class="p-2">Second item</div>
  <div class="p-2">Third item</div>
</div>
```

**Horizontal**
Úselo `.hstack` para diseños horizontales. Los elementos apilados están centrados verticalmente de forma predeterminada y solo ocupan el ancho necesario. Utilice ``.gap-*`` utilidades para agregar espacio entre elementos.

```html
  <div class="hstack gap-3">
  <div class="p-2">First item</div>
  <div class="p-2">Second item</div>
  <div class="p-2">Third item</div>
</div>
```



```css
  .ms-auto {
  margin-left: auto !important;
}
```

Usando utilidades de margen horizontal .ms-autocomo espaciadores:

![stacks](/assets/stacks.JPG)

<div class="hstack gap-3">
  <div class="p-2">First item</div>
  <div class="p-2 ms-auto">Second item</div>
  <div class="p-2">Third item</div>
</div>

> Esto nos podria servir cuando yo quisiera hacer una pequeña navegación responsiva, digamos como sin tanto diseño 


#### Stretched link

Es el diseño para nuestros enlaces, esto sobre todo cuando nuestros elementos van a estar posicionados de forma relativa a un elemento padre

#### Text truncation

Cuando tienes un texto muy largo con estas clases de `.text-truncate` lo que hace es acortarlo

```html
  <h2>Text Truncate</h2>
    <p class="text-white bg-danger text-truncate">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Autem soluta ipsam eligendi at blanditiis doloremque dolor, laboriosam, tenetur quia repudiandae, quam veritatis ratione minima! Ab amet nemo sapiente qui aliquam.
    </p>
```

lo que detecta es el ancho de la pantalla.

Bootstrap tiene unas clases para controlar la altura y la anchura ej: `.w-50` eso significa que el parrafo va tener el 50% de la pantalla


#### Visually hidden

nos ayuda cuando tenemos elementos con accesibilidad

### Seccion UTILITIES parte 1.

**API**

Es muy similar a los helpers, a los auxiliares, estan mas organizadas en cuestion de las propiedades CSS de las que nos ayuda a nivel de SASS tiene una explicacion de la API basadas en la herramienta de sass que generan estas clases 

> Para aquellos amantes de SASS

#### Background

Como poder generar las clases de color empienzan con `bg` y el color que les quieras aplicar, una de las ventajas de usar bootstrap cundo lo generas con SASS es que te genera toda esta variante de los colores dependiendo del color de opacidad que hayas trabajado

![background-opacity](/assets/background-opacity.JPG)

```html
  <div class="bg-success p-2 text-white">This is default success background</div>
<div class="bg-success p-2 text-white bg-opacity-75">This is 75% opacity success background</div>
<div class="bg-success p-2 text-dark bg-opacity-50">This is 50% opacity success background</div>
<div class="bg-success p-2 text-dark bg-opacity-25">This is 25% opacity success background</div>
<div class="bg-success p-2 text-dark bg-opacity-10">This is 10% opacity success background</div>
```

#### Borders

Ideal para imágenes, botones o cualquier otro elemento. 

```html
  <span class="border"></span>
  <span class="border-top"></span>
  <span class="border-end"></span>
  <span class="border-bottom"></span>
  <span class="border-start"></span>
```
si tu estás actualizando un proyecto que hayas hecho en bootstrap 4 a 5 ten en consideracion que lo que se llamaba `left` ahora sellama `start` y lo que se llamaba `right` ahora se llama `end` 

* tambien podemos eliminar bordes específicos con la clase: `border border-top-0`.
* tambien podemos aplicar bordes de colores con la clase: `class="border border-primary"`.


#### Colors 

> Consejo de accesibilidad: el uso de colores para agregar significado solo proporciona una indicación visual, que no se transmitirá a los usuarios de tecnologías de asistencia como lectores de pantalla. Asegúrese de que el significado sea obvio a partir del contenido mismo (por ejemplo, el texto visible con un contraste de color suficiente ) o que se incluya a través de medios alternativos, como texto adicional oculto con la .visually-hiddenclase.

> el color blanco y negro manejas ciertas opacidades: `class="text-white-50 bg-dark"` y `class="text-black-50 bg-white"`.

```css
  .text-white-50 {
  --bs-text-opacity: 1;
  color: rgba(255, 255, 255, 0.5) !important;
}
```

De hecho sol las unicas 2 que tienen la variante de opacidad al 50%

si tu quisieras manejar algun nivel de opacidad para alguno de estos colores, lo único que puedes hacer es replicar este código y te lo pegas en tu hoja particular de estilos en el proyecto que estés haciendo.


#### Display

 Admitimos deliberadamente solo un subconjunto de todos los valores posibles para la propiedad ``display``. Las clases se pueden combinar para obtener varios efectos según sea necesario.

Todo los valores de Display están mapeados en clases:

* none
* inline
* inline-block
* block
* grid
* inline-grid
* table
* table-cell
* table-row
* flex
* inline-flex

```html
  <div class="d-inline p-2 text-bg-primary">d-inline</div>
  <div class="d-inline p-2 text-bg-dark">d-inline</div>
```

> `d == display`

ejemplo:

```html
  <h3>Display</h3>
    <p class="text-danger bg-dark d-none">
      Lorem ipsum, dolor sit amet consectetur adipisicing elit. Similique mollitia inventore, modi facere eveniet repudiandae voluptatem rerum ex ducimus dolor, perspiciatis, enim animi! Aliquid nam nulla est magnam alias aperiam!
    </p>
```
```css
  .d-none {
  display: none !important;
  }
```


> **none**	`d-none`Desaparece la visualización de un elemento para que no tenga ningún efecto en el diseño (el documento se representa como si el elemento no existiera). Todos los elementos descendentes también tienen su pantalla apagada.Para que un elemento ocupe el espacio que normalmente tendría, pero sin producir nada, utilice la propiedad ``visibility``.

![display-block](/assets/display-block.JPG)

> `.d-md-block` En el tamaño mediano la disposicion de este elemento va ser en bloque

![display-inline](/assets/display-inline.JPG)

> `.d-lg-inline` Para que en _large_ sea en linea 


El siguiente tema es `Flex` te vas a dar cuenta como bootstrap tiene mapeada toda las propiedades de flexbox

### Flex


> tienes que tomar cuso de flexbox si no lo has hecho.

Esta fue una de las caracteristicas en la v4 de bootstrap que me enamoró  para que le diera una oportunidad.

Tiene mapeada toda las propiedades de flexbox y lo tiene mapedado en toda las _media querys_

>- **Enable flex behaviors**

* .d-flex
* .d-inline-flex
* .d-sm-flex
* .d-sm-inline-flex
* .d-md-flex
* .d-md-inline-flex
* .d-lg-flex
* .d-lg-inline-flex
* .d-xl-flex
* .d-xl-inline-flex
* .d-xxl-flex
* .d-xxl-inline-flex


>- **Direction**

* .flex-row
* .flex-row-reverse
* .flex-column
* .flex-column-reverse
* .flex-sm-row
* .flex-sm-row-reverse
* .flex-sm-column
* .flex-sm-column-reverse
* .flex-md-row
* .flex-md-row-reverse
* .flex-md-column
* .flex-md-column-reverse
* .flex-lg-row
* .flex-lg-row-reverse
* .flex-lg-column
* .flex-lg-column-reverse
* .flex-xl-row
* .flex-xl-row-reverse
* .flex-xl-column
* .flex-xl-column-reverse
* .flex-xxl-row
* .flex-xxl-row-reverse
* .flex-xxl-column
* .flex-xxl-column-reverse

```html
<h3>FlexBox</h3>
<!-- en el tamaño medium el flex box se vuelva en fila -->
<!-- <section class="d-md-flex"> 
'd-flex flex-column'  hasta acá va ser para la version movil.
-->
<section class="d-flex flex-column flex-sm-column-reverse flex-md-row flex-lg-row-reverse ">
  <article>flex 1</article>
  <article>flex 2</article>
  <article>flex 3</article>
  <article>flex 4</article>
  <article>flex 5</article>
</section>
```
Hacer esto de manera artesanal hubiera implicado hacer mis 4 media querys y estar cambiando el valor de la propiedad ``flex-direction`` en esas media querys.

Bootstrap no solo va ser copiar y pegar código como el acordion, eso es a nivel de IU, pero tu tambien puedes utilizar y sacar el máximo provecho a tus conocimientos de css y utilizar estas clases utilitarias y auxiliares que nos ofrece bootstrap.


>- **Justify content**
>- **Align items**
>- **Align self**
>- **Fill**
>- **Grow and shrink**
>- **Auto margins**
>>- With align-items
>- **Wrap**
>- **Order**
>- **Align content**
>- **Media object**
>- **CSS**
>>- Sass utilities API


### Seccion Utilities parte 2

#### Float 
Los viejos Floats para poder flotar algo a la izquierda o a la derecha

#### Interactions

para seleccionar texto o inavilitarla

**Selección de texto**

**Eventos del puntero**

#### Link
Las utilidades de enlace se utilizan para estilizar los anclajes y ajustar su color, opacidad, desplazamiento de subrayado, color de subrayado y más.

#### Object fit (ajustes del objeto)

Utilice las utilidades de ajuste de objetos para modificar cómo se debe cambiar el tamaño del contenido de un elemento reemplazado , como ``<img>`` o ``<video>``, para que se ajuste a su contenedor.

#### Opacity

La _opacity_ propiedad establece el nivel de opacidad de un elemento. El nivel de opacidad describe el nivel de transparencia, donde ``1`` no es transparente en absoluto, ``.5`` es visible en un 50% y ``0`` es completamente transparente.

Establezca el valor ``opacity ``de un elemento mediante ``.opacity-{value}``utilidades

bootstrap maneja las opacidades en fraciones de 25%

¿Qué pasaria si tu necesitaras una opacidad de 805? 
Te creas una clase utilitaria.
ojo no en el archivo de bootstrap sino en una hoja personal donde vayas trabajando las modificaciones y te creas una clase llamada opacity: 80% 

#### Overflow Desbordamiento

Nos dice que es lo que va pasar con el contenido que desborde su caja contenedora.

```html
  <div class="overflow-auto">...</div>
  <div class="overflow-hidden">...</div>
  <div class="overflow-visible">...</div>
  <div class="overflow-scroll">...</div>
```
#### Position

Utilice estas utilidades abreviadas para configurar rápidamente la posición de un elemento.

Los 5 tipos de posicionamientos que tenemos en bootstrap.

```html
<div class="position-static">...</div>
<div class="position-relative">...</div>
<div class="position-absolute">...</div>
<div class="position-fixed">...</div>
<div class="position-sticky">...</div>
```

Organice elementos fácilmente con las utilidades de posicionamiento de bordes. El formato es ``{property}-{position}``.

Cuando la propiedad es una de:

* ``top`` - para la _top posición_ vertical
* ``start`` - para la _left posición_ horizontal (en LTR)
* ``bottom`` - para la _bottom posición_ vertical
* ``end`` - para la _right posición_ horizontal (en LTR)

Donde la posición es una de:

* 0- para 0 posición de borde
* 50- para 50% posición de borde (al centro)
* 100- para 100% posición de borde (al final)

![position](/assets/position.JPG)

> ¿Cumple la misma funcion que un grid🤔🤔? creo que no por que una grid ordena.

Si tú necesitas valores diferentes ya sea que tu te crees tu clase y vayas modificando o siquieres seguir el patron de las clases de bootstrap, pues te creas una clase top-40 y aplicas  `top-40` 

*incluso centrar elementos*

![position-examples](/assets/position-examples.JPG)

*Es hora de que heches a volar tu imaginación y dependiendo de las necesidades que tengas en la IU que estes construyendo*


#### Shadows

para aplicar sombras {En modo oscuro no se nota}

Tiene varios tamaños

#### Sizing

![sizing](/assets/sizing.JPG)

```html
  <div style="height: 100px;">
  <div class="h-25 d-inline-block" style="width: 120px;">Height 25%</div>
  <div class="h-50 d-inline-block" style="width: 120px;">Height 50%</div>
  <div class="h-75 d-inline-block" style="width: 120px;">Height 75%</div>
  <div class="h-100 d-inline-block" style="width: 120px;">Height 100%</div>
  <div class="h-auto d-inline-block" style="width: 120px;">Height auto</div>
</div>
```

donde 

```css
  .h-25 {
  height: 25% !important;
}
```

> Cuando estes trabajando la altura tu elemento contenedor padre debe tener una altura definida en un valor absoluto como los `px` 

![sizing-height](/assets/sizing-height.JPG)

```html
  <div style="height: 100px;">
    <div class="h-25 d-inline-block" style="width: 120px;">Height 25%</div>
    <div class="h-50 d-inline-block" style="width: 120px;">Height 50%</div>
    <div class="h-75 d-inline-block" style="width: 120px;">Height 75%</div>
    <div class="h-100 d-inline-block" style="width: 120px;">Height 100%</div>
    <div class="h-auto d-inline-block" style="width: 120px;">Height auto</div>
  </div>
```



***Relativo a la ventana gráfica*** Esto nos puede servir para construir una ``hero-image``
También puede utilizar utilidades para establecer el ancho y el alto en relación con la ventana gráfica.

```html
  <div class="min-vw-100">Min-width 100vw</div>
  <div class="min-vh-100">Min-height 100vh</div>
  <div class="vw-100">Width 100vw</div>
  <div class="vh-100">Height 100vh</div>
```

```css
  .vw-100 {
  width: 100vw !important;
}

.min-vw-100 {
  min-width: 100vw !important;
}
```

**Ejemplo:**

```html
  <div class="bg-dark w-100 min-vh-100 d-flex justify-content-center align-items-center">
  <!-- '.align-items-center' para alinear en el eje transversal -->
  <h2 class="display-1 text-white ">Relative to the viewport</h2>
</div>
```

alinea y centra lo que entra en el tamaño movil si pasa de su tamaño ya no alinea. hay que poner una letra responsiva? 🤔🤔


> lo solucione con estó `.text-center` 😊😊


![hero](/assets/hero-image.JPG)


A mayor conocimiento de CSS y a mayor conocimiento que tengas de las utilidades de bootstrap.

Bootstrap ya se ha vuelto _Utilities-first_ tiene demaciadas utilidades aca simplemente vas a estar invocando diferentes clases que oviamente van activando ciertas propiedades css.

Tawild se clasifica como un _framework utility-first_

> Los _framework utility-first_ no solo te van a dar los componentes (el código para que tu ahi lo copies y nada mas modifiques el contenido) como los componenetes de Bootstrap, sino que acá trae muchas utilidades que si tu tienes buenos conocimientos de css entonces le puedes sacar el maximo provecho

la siguiente seccion de utilidades mapea lo que es el modelo de caja las propiedades _margin y padding_ del modelo de caja de css

### Sección Utilities Spacing (Margin & Padding)

> Margin: Es el espacio externo entre los elementos y podemos aplicarlos a un lado o a los 4

> Padding: es la distancia que hay del borde de la caja al contenido 

![padding](/assets/padding.JPG)

**Spacing**

(margin, padding, and gap) margen, relleno y espacio 


Las clases se nombran usando el formato ``{(property(Propiedad))}{sides(lado)}-{size(tamaño)}`` para ``xs`` y ``{property(propiedad)}{sides(lado)}-{breakpoint(punto de interrupción)}-{(size(tamaño))}`` para `sm, md, lg, xl`y `xxl`.

 > ¡Importante! tambien son responsivas sea en `sm, md, lg, xl`y `xxl`.

Cuando la _propiedad_ es una de:

* ``m`` - para clases que establezcan ``margin``
* ``p`` - para clases que establezcan ``padding``

> Recuerda que el _margin_ y el _padding_ se pueden aplicar de 1 a 4 valores, recuerda que cuando aplicamos el _margin_ a dos valores el primer valor es para _(top y booton)_ horizontales y el segundo valor para _(left y right)_ eje horizontal

Donde los lados _(sides)_ es uno de:

* ``t`` - para clases que establecen ``margin-top`` o ``padding-top``
* ``b`` - para clases que establecen ``margin-bottom`` o ``padding-bottom``
* ``s`` - (start) para clases que se establecen ``margin-left`` o ``padding-left`` in LTR ``margin-right`` o ``padding-right`` en RTL
* ``e`` - (end) para clases que se establecen ``margin-right`` o ``padding-right`` en LTR, ``margin-left`` o ``padding-left`` en RTL
* ``x`` - para clases que establecen tanto ``*-left`` y ``*-right``
* ``y`` - para clases que establecen tanto ``*-top`` y ``*-bottom``
* en blank: para clases que establecen a ``margin`` o ``padding`` en los 4 lados del elemento


Donde el tamaño _(size)_ es uno de:

* ``0`` - para clases que eliminan el ``margin`` o el ``padding`` configurándolo en ``0``
* ``1`` - (por defecto) para clases que establecen el ``margin`` o el ``padding`` en ``$spacer`` ``* .25``
* ``2`` - (por defecto) para clases que configuran ``margin`` o ``padding`` para ``$spacer`` ``* .5``
* ``3`` - (por defecto) para clases que configuran ``margin`` o ``padding`` para ``$spacer``
* ``4`` - (por defecto) para clases que configuran ``margin`` o ``padding`` para ``$spacer`` ``* 1.5``
* ``5`` - (por defecto) para clases que configuran ``margin`` o ``padding`` para ``$spacer`` ``* 3``
* ``auto``- para clases que configuran el ``margin`` modo automático

> no puedes tener _paddings_ automáticos pero el valor de `auto` si sirve para las clases de `margin`

Ejemplos
A continuación se muestran algunos ejemplos representativos de estas clases:

```css
  .mt-0 {
  margin-top: 0 !important;
}

.ms-1 {
  margin-left: ($spacer * .25) !important;
}

.px-2 {
  padding-left: ($spacer * .5) !important;
  padding-right: ($spacer * .5) !important;
}

.p-3 {
  padding: $spacer !important;
}
```
**Negative margin**

```css
  .mt-n1 {
  margin-top: -0.25rem !important;
}
```

##### GAP (brecha)

Cuando estamos trabajando con el modelo GRID o con el modelo FLEXBOX 

> Propiedad GAP: es la **separacion** entre los elementos del GRID o del flexbox 

 Esto puede ahorrarle la necesidad de agregar utilidades de margen a elementos secundarios individuales de una cuadrícula o contenedor flexible. Las utilidades de Gap responden de forma predeterminada y se generan a través de nuestra API de utilidades, basada en el ``$spacers`` mapa de Sass.

![gap](/assets/gap.JPG)

 ```html
  <div class="grid gap-3">
    <div class="p-2 g-col-6">Grid item 1</div>
    <div class="p-2 g-col-6">Grid item 2</div>
    <div class="p-2 g-col-6">Grid item 3</div>
    <div class="p-2 g-col-6">Grid item 4</div>
  </div>
 ```

EJERCICIO

> ¡CUIDADO! recuerda poner toda las clases en **minuscula** por que si es sensible a mayusculas y minusculas.

> ¿Como puedo lograr que en el tamaño `lg` el parrafo se centrara? Con la tecnica de **margenes automáticos** a _left_ y _right_ con la clase `.mx-lg-auto`

```css
  .mx-lg-auto {
    margin-right: auto !important;
    margin-left: auto !important;
  }
```

```html
  <h2>Spacing</h2>
  <p class="bg-danger text-white m-3 p-5 m-sm-0 p-sm-3 mt-md-5 pb-md-4 w-50 mx-lg-auto py-lg-5 ps-xl-5 pe-xxl-5">
    <!-- 'X' representa: left y right, 'Y' representa: top y booton -->
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis sunt distinctio, ipsa hic corporis fugiat quod, rerum quasi exercitationem, ut et ad voluptatibus similique laboriosam! Eveniet similique ipsam at tempore?
  </p>
```


```css
.m-3 {
  margin: 1rem !important;
}
```

### Sección Utilites parte 3

##### TEXT 

para controlar los mas comun: alignment, wrapping, weight, and more

![text-align](/assets/text-align.JPG)

```html
  <p class="text-start">Start aligned text on all viewport sizes.</p>
  <p class="text-center">Center aligned text on all viewport sizes.</p>
  <p class="text-end">End aligned text on all viewport sizes.</p>

<!-- estas secciones tambien las tenemos disponibles a lo largo de el espectro de las 'media-querys' -->

  <p class="text-sm-end">End aligned text on viewports sized SM (small) or wider.</p>
  <p class="text-md-end">End aligned text on viewports sized MD (medium) or wider.</p>
  <p class="text-lg-end">End aligned text on viewports sized LG (large) or wider.</p>
  <p class="text-xl-end">End aligned text on viewports sized XL (extra large) or wider.</p>
  <p class="text-xxl-end">End aligned text on viewports sized XXL (extra extra large) or wider.</p>
```

##### Font size

> Acuerdate que ya teniamos estas clases de `display` que son muy grandes pero tambien tenemos otras clases que son responsivas

![text-size](/assets/text-size.JPG)

```html
  <p class="fs-1">.fs-1 text</p>
  <p class="fs-2">.fs-2 text</p>
  <p class="fs-3">.fs-3 text</p>
  <p class="fs-4">.fs-4 text</p>
  <p class="fs-5">.fs-5 text</p>
  <p class="fs-6">.fs-6 text</p>
```
```css
  .fs-1 {
  font-size: calc(1.375rem + 1.5vw) !important;
}
```


##### Font weight and italics

y en sass todolo lo que puedes modificar `mixes o mixeds`
##### Line height

##### Text decoration

#### Vertical align (alineación vertical)


```html
  <table style="height: 100px;">
  <tbody>
    <tr>
      <td class="align-baseline">baseline</td>
      <td class="align-top">top</td>
      <td class="align-middle">middle</td>
      <td class="align-bottom">bottom</td>
      <td class="align-text-top">text-top</td>
      <td class="align-text-bottom">text-bottom</td>
    </tr>
  </tbody>
</table>
```
#### Visibility

un ejemplo:

```html

```

![text-justify](/assets/text-justify.avif)
 
**Yo no suelo justificar el texto por que se vuelve cansada la lectura**


#### z-index
Utilice nuestras utilidades de bajo nivel z-indexpara cambiar rápidamente el nivel de pila de un elemento o componente.

![z-index](/assets/z-index.JPG)

```html
  <div class="z-3 position-absolute p-5 rounded-3"><span>z-3</span></div>
  <div class="z-2 position-absolute p-5 rounded-3"><span>z-2</span></div>
  <div class="z-1 position-absolute p-5 rounded-3"><span>z-1</span></div>
  <div class="z-0 position-absolute p-5 rounded-3"><span>z-0</span></div>
  <div class="z-n1 position-absolute p-5 rounded-3"><span>z-n1</span></div>
```

### Extend

es la capacidad que tenemos de poder extender las caracteristicas de Bootstrap, son recomendaciones

**Resumen**

Profundizaremos más en cada uno de estos, pero en un nivel alto, esto es lo que guía nuestro enfoque.

* Los componentes deben ser responsivos y estar orientados a dispositivos móviles
* Los componentes deben construirse con una clase base y extenderse mediante clases modificadoras.
* Los estados de los componentes deben obedecer a una escala de índice z común
* Siempre que sea posible, prefiera una implementación HTML y CSS en lugar de JavaScript.
* Siempre que sea posible, utilice utilidades en lugar de estilos personalizados.
* Siempre que sea posible, evite imponer requisitos estrictos de HTML (selectores secundarios)


#### Iconos

bootstrap tiene sus propios iconos

los iconos los puedes descargar en `npm` e incluso los puedes abrir en un documento de figma por si estas haciendo un diseño IU  antes de pasarlo a codigo.

Hay formas de utilizarlos 

1. enbebido: copiamos el codígo svg.

2. como imagen externa: lo descargas en formato vectorial lo pones en una etiqueta img

3. como fuente: agregamos la clase: `<i class="bi-alarm"></i>`

> el código SVG es código vectorial en formato html

Cuando mandas a llamar el icono por el ``Icon font`` fuente web, debes mandar a llamar el **CDN de los iconos de bootstrap** por que no se va visualizar, no se va ver.

`<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">`

### ABOUT acerca.

es el historial de todo lo que le han ido implementando, como se mantiene el codigo en GitHub, historia,

Todos estos tipos de proyectos generalmente son construidos por un equipo de dessarrolladores que colaboran en plataformas como github, 

Las licencias son OpenSourse la que tiene boostrap y la parte de las traducciones (pero no están al 100% con la documentación oficial), 

Estamos en el mundo de la programación, el ingles no tiene que ser una limitante todo los lenguajes de programación se escriben en ingles

**Migración** 
En esta sección tu te puedes enterar de todo los cambios y tambien algunas recomendaciones de si tienes un proyecto de una version anterior como poder migrarlo


---

## Comenzando a crear un sitio web con Bootstrap










