# Les 2.3 Concept en Frontend (Lijstjes)

## 0. Concept & Q&A

- Team samenstellen door docenten
- Rubric bespreken
- Concept bedenken in teams
- Inloggegevens per team voor API
- Q&A over lesstof week 1 en 2
- bouwen individuele feature en teamleden ondersteunen

## 1. Concept

Denk na over de matching site die je wilt gaan bouwen en uit welke afzonderlijke onderdelen deze kan bestaan.

1. Denk na over een concept voor de matching site. Wie ga je matchen met wie of wat? Kun je een creatieve manier bedenken, om matches tot stand te brengen? Brainstorm over een aantal mogelijkheden. Door welke bestaande concepten kun je je laten inspireren? Documenteer je onderzoek op je wiki en kies vervolgens een concept uit om verder uit te werken.
2. Denk na over je doelgroep. Wat zijn dit voor mensen, wat vinden ze leuk en wat voor functionaliteit verwachten ze? Wat zijn hun wensen en uitdagingen? Misschien kun je een aantal mensen interviewen of online informatie vinden over deze groep. Documenteer je onderzoek wederom op de wiki.
3. Beschrijf op je wiki een aantal (ongeveer 5) [Job Stories](https://jtbd.info/replacing-the-user-story-with-the-job-story-af7cdee10c27) op om ideeën te genereren over de functionaliteit die nodig is op je matching site. Maak uit de gevonden job stories een keuze voor een functionaliteit die jij verder uit gaat werken.
4. Werk de gekozen job story op je wiki verder uit door hier een [requirements list](https://cmdmethods.nl/cards/stepping-stones/requirements-list) voor op te stellen.
5. Schets ten slotte één of meer lo-fi [wireframes](https://cmdmethods.nl/cards/stepping-stones/design-specification) om een idee te krijgen van het gebruikers interface.

Leg al het bovenstaande vast op je wiki, zodat we je hier ook feedback op kunnen geven. Voor nu is het vooral belangrijk om meer duidelijkheid te krijgen over wat je de komende weken gaat maken.

## 2. ListJS: lijsten filteren, sorteren en doorzoeken

List.js is een JavaScript-bibliotheek die programmeurs kunnen gebruiken bij het maken van interactieve lijsten. Het stelt de bezoeker in staat om in de front-end een lijst met gegevens te filteren, sorteren en doorzoeken zonder dat daarvoor gebruik wordt gemaakt van backend-code of een database.

### Filteren

Met ListJS kun je de _list items_ in een lijst filteren.

HTML

```
<head>
<script src="//cdnjs.cloudflare.com/ajax/libs/list.js/2.3.1/list.min.js"></script>
</head>

<body>
    <div id="nameList">
        <input type="search" class="search" placeholder="Filter by name..." />

        <ul class="list">
          <li><span class="name">Emma</span></li>
          <li><span class="name">Noah</span></li>
          <li><span class="name">Olivia</span></li>
          <li><span class="name">Liam</span></li>
          <li><span class="name">Ava</span></li>
        </ul>
    </div>
</body>
```

- De script-tag voor het importeren van List.js is in de _head_ van de pagina geplaatst om ervoor te zorgen dat de bibliotheek geladen is voordat je eigen scripts worden uitgevoerd.
- De content die je 'zoekbaar' wil maken moet een class krijgen. Vandaar dat er een _span_-element voor wordt gebruikt zodat je die class eraan kan koppelen. Die class aan de _li_ koppelen zal niet werken.

JavaScript

```
let options = {
  valueNames: [ 'name' ],
};

let userList = new List('nameList', options);

```

- In de variabele _options_ geef je aan welke _class_ de content heeft die je wil doorzoeken. Je kan meerdere _classes_ toevoegen aan de array _valueNames_ als dat nodig is. Alle content in al die _classes_ wordt dan meegenomen in je zoekopdracht.
- `new List()` initialiseert List.js. Het definieert de (standaard) configuratie en initialiseert de bibliotheek met je specifieke instellingen.
- Het eerste argument van `new List()` is de _div_ waar de zoekbalk en de te doorzoeken content in staat. In dit geval is dat de ID _nameList_

### Bronnen en tools

- [Bekijk deze slides](/bronnen/Frontend/fe-1-lijstjes.pdf) (Drag 'n drop en carousel optioneel, die worden ook behandeld in week 4)

- library: **[list.js - voor zoeken en sorteren](https://listjs.com/)** (www)
- library: **[Hammer.js - swipen en andere touch events](https://hammerjs.github.io/)** (www)

### Oefeningen

- code: **[Oefening lijstjes en libs - views](https://codepen.io/shooft/pen/wvErdwQ)** (Codepen)
- code: [**Oefening lijstjes en libs - filteren**](https://codepen.io/shooft/pen/BaOwRyq) (Codepen)
- code: [**Oefening lijstjes en libs - zoeken**](https://codepen.io/shooft/pen/PodJmzy) (Codepen)
- code: [**Oefening lijstjes en libs - sorteren**](https://codepen.io/shooft/pen/XWPeRjK) (Codepen)

### Uitwerkingen

- uitwerking: **[Oefening lijstjes en libs - views](https://codepen.io/shooft/pen/BaOwRBq)** (Codepen)
- uitwerking: [**Oefening lijstjes en libs - filteren**](https://codepen.io/shooft/pen/bGxoWNO) (Codepen)
- uitwerking: **[Oefening lijstjes en libs - zoeken](https://codepen.io/shooft/pen/BaOwRzv)** (Codepen)
- uitwerking: **[Oefening lijstjes en libs - sorteren](https://codepen.io/shooft/pen/ExewmgN)** (Codepen)
