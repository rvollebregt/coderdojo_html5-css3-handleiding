Basis HTML5 & CSS3 (voor CoderDojo)
=====

*Auteur(s): Richard Vollebregt*

Inhoudsopgave
=====

* [Voorwoord](#voorwoord)

## HTML5

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

## CSS3

<!-- TODO Toevoegen van links naar de juiste headings -->
1. Basis
* Classes & ID's
* Kleuren & Achtergronden
* Teksten & fonts
* Margin & padding
* Positionering
* Basis selectors
* Basis effecten & animaties


## Opdrachten
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


<a name="voorwoord"></a> Voorwoord
======

Welkom bij deze basis tutorial voor het leren van HTML & CSS. Deze tutorial is speciaal geschreven voor gebruik bij CoderDojo's.
Voel je vrij om stukken over te nemen, uit te breiden en/of te verbeteren.

Veel plezier met het leren van HTML & CSS!


<a name="basis-structuur"></a> Basis structuur
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

<a name="teksten"></a> Teksten
======

In dit hoofdstuk bespreken we kort de verschillende elementen die zijn te gebruiken voor het plaatsen van teksten. Hieronder volgt een korte opsomming van de verschillende tags met een voorbeeld en wat je met het element kan doen.

#### Paragraaf
`<p>Dit is een paragraaf</p>`

Met het paragraaf element kan je netjes een stuk tekst invoegen. Binnen deze paragraaf kan je ook andere elementen toevoegen om bijvoorbeeld een stukje van de tekst vetgedrukt of cursief te maken.

#### Kopregels
`<h1>Dit is een kopregel</h1>`

Met __heading__ elementen kan je een kopregel toevoegen. Deze worden gebruikt voor het toevoegen van een titel aan je tekst. Deze komen bijvoorbeeld boven een paragraaf te staan. Er zijn 6 verschillende heading elementen, namelijk van `<h1></h1>` t/m `<h6></h6>`. Deze verschillen (standaard) in grootte, waar `<h1>` het grootst is en `<h6>` het kleinst.

#### Vet gedrukt
`<b>Dit is een vetgedrukte zin</b>`  
`<strong>Dit is een belangrijke vetgedrukte zin</strong>`

#### Cursief
`<i>Dit is een cursief gedrukte zin</i>`  
`<em>Dit is een belangrijke cursief gedrukte zin</em>`

Om stukken tekst vetgedrukt of cursief te maken, kun je hier de bovenstaande tags omheen zetten. Er is een verschil tussen de twee soorten. Hier kan je meer over vinden in het hoofdstuk over Semantiek.

__Korte opdracht:__
Zoek op internet een 'Lorem Ipsum' generator (en als je wilt de oorsprong van deze tekst). Voeg 2 paragrafen van deze tekst toe aan je eigen webpagina en maak een aantal stukken <em>cursief</em> en <strong>vetgedrukt</strong>. Zorg er daarna voor dat elke paragraaf erboven een kopregel krijgt in verschillende groottes.
