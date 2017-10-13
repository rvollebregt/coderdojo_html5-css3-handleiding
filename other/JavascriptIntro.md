# JavaScript introductie

JavaScript (ook wel JS genoemd) is een scripttaal die wordt gebruikt om webpagina's van meer interactiviteit te voorzien en zelfs om gehele webapplicaties te maken.
Wij gaan hier JS gebruiken om wat elementen op je site te voorzien van leuke extra's.

## Hello World!
We beginnen met het gebruikelijke `Hello World` voorbeeld. Open een nieuw HTML bestand in je favoriete teksteditor en voeg de HTML structuur toe. Vervolgens maken we een nieuw JavaScript bestand aan. Noem deze file `helloworld.js`.

In dit bestand gaan we onze JavaScript code toevoegen. We maken een simpele popup met een `Hello World!` tekst er in:

```
  alert('Hello World!');
```

We roepen hiermee de `alert` functie mee aan en geven de tekst `'Hello World!'` als input.
Om de JS te kunnen gebruiken op onze pagina, moeten we het script inladen. Dit kan door de `<script>` tag te gebruiken.
Je kan deze óf in de `<head>` óf in de `<body>` tag zetten:

```
  <script src="helloworld.js"></script>
```

Zorg ervoor dat de HTML en JS bestanden beiden zijn opgeslagen en open dan de pagina in je browser. Als je het goed hebt gedaan krijg je nu een popup te zien met je tekst!

__Korte opdracht:__
Probeer je popup aan te roepen als je op een plaatje klikt, en niet meteen als de pagina opent. Je kan hiervoor het `onclick` attribuut gebruiken op je `<img>` tag.

## Tekst aanpassen met JavaScript
We gaan nu proberen een eerder toegevoegde tekst in je HTML bestand te veranderen met JS. Zorg ervoor dat je een `<h1>` tag hebt toegevoegd met daarin een korte tekst en ook een `id` attribuut met daarin `header`.
Daarna gaan we in een nieuw `.js` bestand onze code toevoegen.

We gaan voor deze opdracht gebruik maken van `variables`. Een variable heeft als doel om een 'waarde' op te kunnen slaan, om deze later nog een keer op te kunnen vragen.
We maken als volgt een variable aan in JavaScript:

```
  var mijnHeaderTekst;
```

We hebben nu `mijnHeaderTekst` beschikbaar om een waarde aan toe te kennen. Dit kunnen we doen met het `=` teken.

```
  mijnHeaderTekst = 'Dit is de nieuwe tekst voor mijn header!'
```

We hebben met de regel hierboven de tekst toegevoegd aan de variable `mijnHeader`. Nu moeten we er voor zorgen dat je header in de HTML wordt aangepast naar je nieuwe tekst. In je `.js` bestand kunnen we nu een regel code toevoegen om je `<h1>` tag op te zoeken:

```
  mijnHeader = document.querySelector('#header');
```

Zoals je ziet zorgen we er ook voor dat je header meteen in een variable wordt opgeslagen, zodat we hem later kunnen opvragen of aanpassen. Met `document.querySelector` kunnen we bijvoorbeeld het `id` attribuut van een element gebruiken om het element op te zoeken.

Als we nu de tekst willen aanpassen naar de tekst van `mijnHeaderTekst` hoeven we nog maar één ding te doen:
```
  mijnHeader.textContent = mijnHeaderTekst;
```
We veranderen met deze regel de `textContent` van het element naar jouw eerder ingestelde tekst.
Als je nu weer je HTML en JS opgeslagen hebt, en de pagina opent in je browser, krijg je de nieuwe tekst te zien!
