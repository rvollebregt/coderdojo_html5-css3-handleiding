Basis HTML5 & CSS3 (voor CoderDojo)
=====

*Auteur(s): Richard Vollebregt*

Inhoudsopgave
=====

* [Voorwoord](#voorwoord)

## [HTML5](#html5)

<!-- TODO Toevoegen van links naar de juiste headings -->
1. [Basis structuur](#basis-structuur)
* [Teksten](#teksten)
* [Lijsten](#lijsten)
* [Links](#links)
* [Plaatjes](#plaatjes)
* [Tabellen](#tabellen)
* Formulieren
* Meta informatie
* Structuur & Semantiek
* HTML5 elementen
* Referentie

## [CSS3](#css3)

<!-- TODO Toevoegen van links naar de juiste headings -->
1. [Basis](#css-basis)
* [Classes & ID's](#classes)
* [Kleuren & Achtergronden](#kleuren)
* Teksten & fonts
* Margin & padding
* Positionering
* Basis selectors
* Basis effecten & animaties


## [Opdrachten](#opdrachten)
<!-- TODO Toevoegen van links naar de juiste headings -->
* [Opdracht 1](#opdracht1): Maak een lijst met links naar je favoriete pagina's   
  * <small>Hoofdstukken 1 t/m 4 van HTML</small>
* [Opdracht 2](#opdracht2): Maak een tabel die de Eredivisie statistieken toont
  * <small>Hoofdstuk 5 & 6 van HTML</small>
* [Opdracht 3](#opdracht3): Voeg kleur toe aan je lijst met links van Opdracht 1
  * <small>Hoofdstuk 1 t/m 3 van CSS</small>
<!-- * Opdracht ?: Maak een menu die openklapt -->


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

<a name="html5"></a> HTML5
======


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

Tabellen zijn een goede oplossing als je veel informatie op je website wil zetten.
Een tabel maak je met het HTML element `<table>`. Hieronder zie je een voorbeeld:

~~~
  <table>
  <tr>
    <td><b>Datum</b></td>
    <td><b>Tijd</b></td>
    <td><b>Locatie</b></td>
    <td><b>Wat</b></td>
  </tr>
  <tr>
    <td>28-05-2016</td>
    <td>11:00</td>
    <td>Bibliotheek Tiel</td>
    <td>HTML/CSS</td>
  </tr>
  <tr>
    <td>25-06-2016</td>
    <td>11:00</td>
    <td>Bibliotheek Tiel</td>
    <td>HTML/CSS</td>
  </tr>
  </table>
~~~

<table>
<tr>
  <td><b>Datum</b></td>
  <td><b>Tijd</b></td>
  <td><b>Locatie</b></td>
  <td><b>Wat</b></td>
</tr>
<tr>
  <td>28-05-2016</td>
  <td>11:00</td>
  <td>Bibliotheek Tiel</td>
  <td>HTML/CSS</td>
</tr>
<tr>
  <td style="border: 2px solid red" colspan="2">25-06-2016 om 11:00</td>
  <td>Bibliotheek Tiel</td>
  <td>HTML/CSS</td>
</tr>
</table>

Een tabel bestaat uit rijen en kolommen. In HTML maak je eerst een rij met een `<tr>` element, daarna voeg je daartussen je tabel cellen toe met de `<td>` elementen. Dit worden je kolommen. Zorg ervoor dat je evenveel tabel cellen hebt per rij.

__Korte opdracht:__
Maak een kleine tabel in je HTML bestand. Als je dit hebt gedaan kan je opzoeken hoe je een tabel cel over 2 cellen kan laten lopen zoals het voorbeeld hierboven.

<a name="css3"></a> CSS
=====

<a name="css-basis"></a> Basis
=====

CSS (Cascading Style Sheets) wordt gebruikt om de weergave van je HTML en webpagina aan te passen. Je kunt bijvoorbeeld de grootte van je tekst aanpassen, achtergrondkleuren instellen en HTML elementen verplaatsen. In de volgende hoofdstukken gaan we zoveel mogelijk in op de basis van het toevoegen van CSS aan je webpagina en aantal verschillende CSS eigenschappen.

Eerst gaan we een nieuw CSS bestand aanmaken in dezelfde map als je HTML bestand. Deze kunnen we bijvoorbeeld __style.css__ noemen. We gaan deze daarna in je HTML bestand invoegen. Dit gebeurt met een `<link>` tag die je in de `<header>` zet. Het CSS bestand wordt dan op de pagina ingeladen. Het voordeel van deze manier van toevoegen van CSS is dat je niet voor elke pagina weer dezelfde CSS hoeft toe te voegen.

`<link rel="stylesheet" href="style.css" >`

We voegen hier twee verschillende attributen toe, namelijk het `rel` attribuut en `href`. De `rel` eigenschap moet aanwezig zijn op de tag, hier geef je mee aan dat het om een Style Sheet gaat. Met `href` geef je aan waar het bestand staat.

__Korte opdracht:__
Zorg ervoor dat je een nieuw CSS bestand aanmaakt in de map met je HTML bestand. Zet daarna correct de `<link>` tag tussen je `<head>` tags.

<a name="classes"></a> Classes & ID's
=====

Om goed gebruik te kunnen maken van CSS moeten we weten wat classes & ID's zijn.
Classes en ID's kunnen we aan HTML elementen koppelen met een attribuut. Dit gebeurt met de eigenschappen `class` en `id`. Het verschil tussen deze twee attributen is dat een class meerdere keren mag voorkomen op een pagina en een ID maar één keer voorkomt op een pagina.

We kunnen in ons CSS bestand een class toevoegen als volgt:

`.rood`

We gebruiken een punt voor de classnaam om aan te geven dat het om een class gaat. Een classnaam kan je altijd zelf bepalen. Vervolgens kunnen we aan deze class eigenschappen toekennen. Om dat te doen moeten we deze CSS eigenschappen tussen __{__ en __}__ tekens plaatsen, dat ziet er zo uit:

~~~
/* Dit is een class */
.rood {
  color: red;
}

/* Dit is een ID */
#geel {
  color: yellow;
}
~~~

Eerst kies je de eigenschap die je wil gebruiken. Na de naam van de eigenschap dat je wil gebruiken zet je een __:__ en volgt daarna de waarde die je wil gebruiken. Uiteindelijk sluit je de regel af met een __;__. In dit voorbeeld hierboven veranderen we de kleur van tekst naar rood van elk HTML element dat de class __rood__ heeft. Die voegen we met een attribuut toe aan een HTML tag net zoals hieronder.

`<strong class="rood">Dit is rode vetgedrukte tekst</strong>`

Voor ID's kunnen we hetzelfde doen als voor een class. Alleen gebruiken we in plaats van een __.__ een __#__.

`<strong id="geel">Dit is een gele vetgedrukte tekst</strong>`

__Korte opdracht:__
Zoek op internet wat de verschillen zijn tussen classes en ID's en welke je beter kan gebruiken.

<a name="kleuren"></a> Kleuren & Achtergronden
=====

Nu we hebben geleerd hoe je classes en ID's kan gebruiken, kunnen we de echte eigenschappen van CSS bekijken en toevoegen.
We maken eerst een nieuwe class aan in het CSS bestand.

~~~
.blauw {}
~~~

Om de kleur van tekst te kunnen aanpassen, gebruiken we de eigenschap `color`. Ook kunnen we de kleur van de achtergrond aanpassen. Hier gebruiken we `background-color` voor.

~~~
.blauw {
  color: white;
  background-color: blue;
}
/* Let op: we sluiten een CSS regel altijd af met een ; */
~~~

Met deze CSS class kunnen we nu de achtergrond blauw maken en de kleur van de tekst wit. Deze class kan je aan een element van je HTML pagina toevoegen.

`<h1 class="blauw">Dit is een Header met een blauwe achtergrond</h1>`

__Korte opdracht:__
Voeg een class toe aan je CSS bestand. Gebruik je gemaakte class op een HTML element naar keuze. Als je het goed hebt gedaan krijg je nu een blauw blok met witte tekst te zien.

Let op: Als je CSS niet werkt, controleer dan of je CSS bestand in je `<head>` is ingevoegd en of je CSS regels met een __;__ zijn afgesloten.

Zoek op internet op welke andere kleuren je kan gebruiken in je CSS. Er zijn meerdere kleuren beschikbaar die je met hun naam kan toevoegen, zoals `red, black, grey` etc. Maar we kunnen ook zelf een kleur maken met het RGB-kleursysteem. Je kan [hier](https://nl.wikipedia.org/wiki/RGB-kleursysteem) meer info vinden er over.


<a name="opdrachten"></a> Opdrachten
=====

<a name="opdracht1"></a> Opdracht 1:
=====
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


<a name="opdracht2"></a> Opdracht 2:
=====
Maak een tabel die de Eredivisie statistieken toont
-----

Voor deze opdracht gaan we gebruik maken van tabellen en plaatjes (Hoofdstuk 5 & 6 van HTML). Je kan een nieuw HTML bestand aanmaken of doorgaan op het bestand dat je in [Opdracht 1](#opdracht1) hebt gemaakt.

Ga naar de site http://www.eredivisie.nl en bekijk de huidige stand. Deze kan je (voor een deel) overnemen voor je eigen tabel (of je verzint zelf wat voor in je eigen tabel). Hieronder staat een stappenplan die kan gebruiken voor het maken van je tabel:

- Bedenk hoe de structuur wordt van je tabel. Hoeveel rijen en kolommen heb je nodig?
- Voeg de structuur toe in je HTML, je kan gebruik maken van kopieëren en plakken om het wat te versnellen.
- Vul daarna je tabel cellen met alle informatie (je kan ook de plaatjes van de clubs downloaden en toevoegen bijvoorbeeld).
- Zet om de plaatjes een link heen naar de site van de voetbalclub.

<a name="opdracht3"></a> Opdracht 3
=====

Gebruik voor deze opdracht het resultaat van Opdracht 1. Deze kunnen we nu verder uitbreiden met kleuren.

- Maak een class aan voor de achtergrondkleur en tekstkleur van je body. Voeg deze daarna toe in je HTML.
- De kleur van je links veranderen niet, deze hebben al een andere kleur door je browser gekregen. Maak een aparte class aan die je op je links kan gebruiken en verander de tekst- en achtergrondkleur.
- Geef ook je __unordered list__ een ander kleurtje, je zult zien dat de bolletjes voor de links van kleur veranderen.
- Extra: kan je ook alle links in één keer veranderen van kleur zonder elke link een class te geven? Hoe kan je dit voor elkaar krijgen?

!["Opdracht 3 afbeelding"](examples/images/example3.png)
