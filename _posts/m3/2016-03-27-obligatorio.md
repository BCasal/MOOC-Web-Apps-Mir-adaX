---
layout: posts
title:  "Ejercicio obligatorio"
sub-title: "Modulo 3: Javascript: Sentencia, Expresión, Variable, Función, Objeto Y DOM"
date:   2016-04-01 00:01
categories: m3
permalink: "/modulos/m3/obligatorio/"
source: "http://pruebashtml.neocities.org/2016/Miriadax/m3-obligatorio/index.html"
code: "https://drive.google.com/file/d/0B7AwER8OVKzxVTB6aTJ4NVUwS0E/view?usp=sharing"
---

Ampliar la siguiente aplicación Web (muestra la fecha y la hora):

{% highlight html %}
<!DOCTYPE html><html>
<head>
  <title>Date</title>
  <meta charset="UTF-8">
</head>
<body>
  <h1 id="h1"></h1>
  <h2 id="h2">La fecha y la hora son:</h2>
  <div id="fecha"></div>

 <script type="text/javascript">
  var fecha = new Date();
  var msj;

  if      (fecha.getHours() < 7)  { msj = "Buenas noches";}
  else if (fecha.getHours() < 12) { msj = "Buenos días";}
  else if (fecha.getHours() < 21) { msj = "Buenas tardes";}
  else                                          { msj = "Buenas noches";}

  document.getElementById("h1").innerHTML    = msj;
  document.getElementById("fecha").innerHTML = fecha;
</script>
</body>
</html>
{% endhighlight %}

Incluyendo los siguientes elementos:

<ol> 
  <li>El nombre de la persona que hace la entrega debajo del titulo &lt;h1&gt;</li>
  <li>Un bloque &lt;div&gt; debajo de la fecha y la hora y las instrucciones JavaScript necesarias para que muestre en dicho bloque el contenido de las siguientes propiedades DOM  en líneas separadas, que comiencen por el nombre de la propiedad(es) mostrada(s):</li>  
  <ol type="a">
    <li>Contenido de innerHTML de elemento identificado por id="h2"</li>
    <li>Contenido de outerHTML de elemento identificado por id="h1"</li>
    <li>Contenido de la propiedad global: location.href</li>
    <li>Contenido de la propiedad global: location</li>
    <li>Contenido de las propiedades globales: screen.width y screen.heigth</li>
  </ol>  
</ol>