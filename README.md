

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

> Recuerda hacerlo en una hoja super css `.SCSS` independiente


