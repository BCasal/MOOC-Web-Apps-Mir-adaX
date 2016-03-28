---
layout: posts
title:  "Ejercicio obligatorio"
sub-title: "Modulo 1: Introducción a los elementos básicos de HTML, CSS"
date:   2016-03-23 00:04
categories: m1
permalink: "/modulos/m1/obligatorio/"
source: "http://pruebashtml.neocities.org/2016/Miriadax/m1-p2p-obligatorio-01/index.html"
code: "https://drive.google.com/file/d/0B7AwER8OVKzxMDZWZThoX1M2Y1k/view?usp=sharing"
---

**Construir una página HTML titulada:
Secciones y líneas generales de un documento HTML5.**
<br>
Utilizar el texto a continuación.
**Deben emplearse las marcas básicas de HTML y estilos según
los contenidos del módulo 1** de este curso.

<h3>Texto para el ejercicio</h3>

<h4>Secciones y líneas generales de un documento HTML<sub>5</sub></h4>

La especificación HTML<sub>5</sub> trae muchos nuevos elementos a los
desarrolladores web, permitiéndoles describir la estructura de un documento
web con semántica estandarizada. Este documento describe estos elementos y
cómo usarlos para definir el perfil de cualquier documento.

<h5>Problemas resueltos por HTML<sub>5</sub></h5>

La definición de la estructura de un documento en HTML4 y su algoritmo
de perfilado es muy tosco y genera numerosos problemas:


1. HTML<sub>5</sub> quita la necesidad de elementos &lt;div&gt; para definir
   secciones semánticas sin definir valores específicos para los atributos
   class, introduciendo un nuevo elemento, &lt;section&gt;,
   el elemento de sección HTML.
   
2. Mezclar varios documentos es difícil: la inclusión de un sub-documento en
   un documento principal. Esto se resuelve en HTML<sub>5</sub> con los
   elementos de seccionado (&lt;article&gt;, &lt;section&gt;,
   &lt;nav&gt; y &lt;aside&gt;) son siempre subsecciones de su sección
   ancestra más cercana.
   
3. HTML<sub>5</sub> introduce el elemento &lt;hgroup&gt; que oculta
   todos los elementos de cabecera excepto el primero de más alto rango
   (por ejemplo, &lt;hgroup&gt;&lt;h1&gt;Justine&lt;/h1&gt;&lt;h2&gt;Les
   Malheurs de la Vertu&lt;/h2&gt;&lt;/hgroup&gt; crea el perfil 1. Justine).
   
4. Un documento puede tener secciones especiales conteniendo información
   relacionado que no es parte del flujo principal. HTML<sub>5</sub>
   introduce el elemento &lt;aside&gt; permitiendo a dichas secciones no
   ser parte del perfil principal.
   
5. Hay información relacionada no al documento pero si al sitio entero,
   como logos, menús, tablas de contenidos, o información de derechos
   de autor y notas legales. Para ese propósito, HTML<sub>5</sub> introduce
   tres elementos de sección específicos: &lt;nav&gt; para colecciones de
   enlaces, como una tabla de contenidos, &lt;footer&gt; y &lt;header&gt;
   información relacionada con el sitio.

De manera más general, HTML<sub>5</sub> trae precisión a las características
de seccionado y cabecera, permitiendo a los perfiles de documento ser
predecibles y usados por el navegador para mejorar la experiencia de usuario.

<h5>El algoritmo de perfilado de HTML<sub>5</sub></h5>

<h6>Definiendo secciones en HTML<sub>5</sub></h6>

Todo el contenido incluido dentro del elemento &lt;body&gt; es parte de
una sección. Las secciones en HTML<sub>5</sub> pueden ser anidadas.
Además de la sección principal, definida por el elemento &lt;body&gt;,
los límites de la sección son definidos explícita o implícitamente.
La secciones definidas explícitamente son el contenido definido en
las etiquetas &lt;body&gt;, &lt;section&gt;, &lt;article&gt;, &lt;aside&gt;,
&lt;footer&gt;, &lt;header&gt;, y &lt;nav&gt;.

> Nota: Cada sección puede tener su propia jerarquía de cabeceras.
  Por lo tanto, incluso una sección anidada puede tener un elemento &lt;h1&gt;.
  Consulte también Definiendo cabeceras en HTML<sub>5</sub>.

Ejemplo:

    <section>
      <h1>Forest elephants</h1>
      <section>
        <h1>Introduction</h1>
        <p>In this section, we discuss the lesser known forest elephants.</p>
      </section>
      <section>
        <h1>Habitat</h1>
        <p>Forest elephants do not live in trees but among them.</p>
      </section>
      <aside>
        <p>advertising block</p>
      </aside>
    </section>
    <footer>
      <p>(c) 2010 The Example company</p>
    </footer>
