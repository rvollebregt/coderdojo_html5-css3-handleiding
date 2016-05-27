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
* [Lijsten](#lijsten)
* [Links](#links)
* [Plaatjes](#plaatjes)
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
  * <sub>Hoofdstukken 1 t/m 4 van HTML</sub>


* [Opdracht 2](#opdracht2): Maak een tabel die de Eredivisie statistieken toont
  * <sub>Hoofdstuk 5 & 6 van HTML</sub>


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

<a name="lijsten"></a> Lijsten
======

Bij het maken van webpagina's zijn lijsten vaak erg handig. Ze geven je overzicht en structuur. Hieronder vind je een voorbeeld van een lijst in HTML:

~~~
<ul>
  <li>Melk</li>
  <li>Brood</li>
  <li>Kaas</li>
</ul>
~~~

<ul>
  <li>Melk</li>
  <li>Brood</li>
  <li>Kaas</li>
</ul>

Er zijn een aantal verschillende typen lijsten. In dit hoofdstuk bespreken we er twee van. Dit zijn de __unordered list__ `<ul></ul>` en de __ordered list__ `<ol><\ol>`. Zoals je misschien al door hebt, heeft de unordered list geen nummering en de ordered list wel.
Tussen deze lijst elementen worden altijd de __list items__ `<li></li>` geplaatst zoals in het voorbeeld hierboven.

__Korte opdracht:__
Maak een eigen lijst op je webpagina. Je kunt bijvoorbeeld een opsomming maken van al je verschillende spellen of films die je thuis hebt. Zorg dat je favoriete lijst items goed te zien zijn door de tekst bijvoorbeeld vetgedrukt of cursief te maken.

<a name="links"></a> Links
======

Op je pagina is het natuurlijk leuk als je naar mensen naar andere websites of één van je andere pagina's kan sturen. Dit kunnen we doen met links.
Een link kunnen we maken door het `<a></a>` element te gebruiken (`<a>` is een afkorting voor anchor).

Om een link te maken kunnen we een stuk tekst omringen met deze tags. Alleen moeten we ook aan deze tag kunnen vertellen waar de link naar toe moet verwijzen. Om dat voor elkaar te krijgen kunnen we een eigenschap toevoegen aan de openende tag. Dit heet een __attribute__. Voor deze tag gaan we het __href__ attribuut gebruiken. Dat ziet er zo uit:

`<a href="http://www.google.com">Dit is een link naar Google</a>`

We gebruiken de volgende manier om een attribuut toe te voegen:

`href="http://jouwwebsitehier.nl"`

Deze manier geldt voor het toevoegen van alle beschikbare attributen. Vaak hebben HTML elementen meerdere attributen die je kan gebruiken. Welke eigenschappen je kan gebruiken is afhankelijk van het HTML element. De attributen staan altijd in de openings-tag. Het is ook mogelijk om meerdere attributen toe te voegen per tag.

__Korte opdracht:__
Voeg in je tekst een link toe naar een website die je vaak bezoekt. Zoek ook op internet op waar de __target__ attribuut voor is bij de `<a>` tag en voeg deze op de juiste manier toe aan je link.

<a name="plaatjes"></a> Plaatjes
======
Een website is natuurlijk niet interessant zonder plaatjes. Met HTML kunnen we heel gemakkelijk onze eigen afbeeldingen toevoegen met de `<img>` tag.
Dit is een HTML element die maar één tag gebruikt. Om een plaatje toe te voegen moeten we het `src` attribuut gebruiken ('source', vertaald naar het Nederlands is dat 'bron'). Hieronder zie je een voorbeeld:

`<img src="afbeelding1.jpg">`

!["Dit is een afbeelding"](images/afbeelding1.jpg)

Het pad van de afbeelding wordt altijd gezien vanuit de map waar je HTML bestand staat. Dat betekent dat als je plaatje in de map __images__ staat, dat je als pad `images/afbeelding1.jpg` gebruikt om deze te laden.

!["Screenshot mappenstructuur"](images/afbeelding2.png)

Browsers ondersteunen een aantal verschillende soorten bestandsformaten. De meest voorkomende bestandsformaten zijn __.png__, __.jpg__ en __.gif__.

__Korte opdracht:__
Zoek een leuk plaatje van het internet en download deze naar je eigen computer. Vervolgens plaats je het plaatje bij je HTML bestand in een nieuwe folder (gebruikelijk is om de folder __images__ te noemen). Voeg nu een nieuwe `<img>` tag toe in je HTML bestand. Probeer ook uit te vinden welk attribuut je kan gebruiken om je plaatje een titel te geven.

<a name="tabellen"></a> Tabellen
======

<a name="opdracht1"></a> Opdracht 1:
======
Maak een lijst met links naar je favoriete pagina's
------

Voor de eerste opdracht maken we een nieuw HTML bestand aan. Maak hiervoor een nieuwe map aan.

Zorg ervoor dat je de hoofdstukken 1 t/m 4 hebt gelezen van het HTML onderdeel. Deze hoofdstukken geven uitleg over hoe je de elementen moet gebruiken.
Hieronder staat een stappenplan die je kan volgen om de opdracht te maken.

- Bouw eerst je basis HTML structuur op.
- Voeg dan een titel toe aan je pagina. Kies een goede omschrijving voor wat er op de pagina komt te staan.
- Voeg een kopregel toe en een korte paragraaf die omschrijft waar je lijstje over gaat.
- Maak een nieuw lijstje aan onder de paragraaf. Kies bijvoorbeeld een aantal leuke websites uit.
- De leukste items in je lijst geef je een vetgedrukte tekst.
- Maak nu alle lijst items klikbaar in je pagina en geef er een aantal een target.
- Als je klaar bent kijk je of je links werken. Wat valt je op als je een link heb bezocht en je opent opnieuw je webpagina?

!["Opdracht 1 eindresultaat"](examples/images/example1.png)


<a name="opdracht2"></a> Opdracht 2
======

<a name="opdracht3"></a> Opdracht 3
======
