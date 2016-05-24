Basis HTML5 & CSS3 (voor CoderDojo)
=====

*Auteur(s): Richard Vollebregt*

Inhoudsopgave
=====

* [Voorwoord](#voorwoord)

HTML5
-----
<!-- TODO Toevoegen van links naar de juiste headings -->
1. [Basis structuur](#basis-structuur)
* [Teksten](#teksten)
* Lijsten
* Links & knoppen
* Plaatjes
* Tabellen
* Formulieren
* Meta informatie
* Structuur & Semantiek
* HTML5 elementen
* Referentie

CSS3
-----
<!-- TODO Toevoegen van links naar de juiste headings -->
1. Basis
* Classes & ID's
* Kleuren & Achtergronden
* Teksten & fonts
* Margin & padding
* Positionering
* Basis selectors
* Basis effecten & animaties


Opdrachten
-----
<!-- TODO Toevoegen van links naar de juiste headings -->
* [Opdracht 1](#opdracht1): Maak een lijst met links naar je favoriete pagina's   
  * <sub>Hoofdstukken 1 t/m 3 van HTML</sub>


* [Opdracht 2](#opdracht2): Maak een tabel die de Eredivisie statistieken toont
  * <sub>Hoofdstuk 4 t/m 6 van HTML</sub>


* Opdracht ?: Maak een menu die openklapt


Links met extra informatie
-----
* Wat zijn pixels? https://nl.wikipedia.org/wiki/Pixel
* Hoe werken kleuren? https://nl.wikipedia.org/wiki/RGB-kleursysteem
* Referentie voor HTML elementen: https://nl.wikipedia.org/wiki/Lijst_van_HTML-elementen
* Referentie voor CSS eigenschappen: http://83.96.174.175/referentie/css/


Voorwoord <a name="voorwoord"></a>
======

Welkom bij deze basis tutorial voor het leren van HTML & CSS. Deze tutorial is speciaal geschreven voor gebruik bij CoderDojo's.
Voel je vrij om stukken over te nemen, uit te breiden en/of te verbeteren.

Veel plezier met het leren van HTML & CSS!


Basis structuur <a name="basis-structuur"></a>
======

### Wat is HTML?
HTML is een afkorting voor __Hypertext Markup Language__. Met deze taal vertel je aan je browser (bijvoorbeeld Chrome, Safari of Internet Explorer) hoe hij een webpagina moet tonen. We gaan in dit hoofdstuk de basis structuur bekijken.

### Een simpele HTML pagina
Een HTML pagina bestaat uit een aantal __tags__. Deze tags zijn de basis voor het bouwen van je pagina. Een tag kan je herkennen aan deze tekens: __<__ en __>__. Sommige HTML elementen hebben maar 1 tag, zoals `<img>`. Andere HTML elementen hebben een openende en een sluitende tag, zoals `<html></html>`, hier plaats je weer andere tags of tekst tussen. De sluitende tag kan je herkennen aan de __/__.

Om een HTML pagina te maken zijn er een aantal tags die noodzakelijk zijn.
Allereerst moeten we aangeven dat het om een HTML pagina gaat. Dit doe je met de `<html></html>` tag. Alle andere tags komen hiertussen te staan. We voegen eerst een `<head></head>` tag toe. Dit element voorziet je pagina van extra informatie, zoals een titel. Onder deze tag zetten we een `<body></body>` tag neer. Dit is het gedeelte waar je je webpagina in bouwt. Hier kun je de meeste andere tags of tekst in plaatsen. Hieronder staat de uitgewerkte HTML:

~~~
<html>
  <head>
    <title>Dit is de titel van je webpagina</title>
  </head>
  <body>
    Dit is de body van je webpagina.
  </body>
</html>
~~~

*Dit is de basis structuur van een webpagina.*

__Korte opdracht:__
Neem deze HTML structuur over in je tekst editor en verander daarna de titel en de tekst van de webpagina. Sla daarna het bestand op als een .html bestand en open deze in je browser. Als je extra uitleg nodig hebt, kun je een van de coaches aanspreken.

Teksten <a name="teksten"></a>
======

TODO
