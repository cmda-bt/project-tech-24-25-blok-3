# Les 3.1 Formulieren en animeren

## 1. Formulieren met JSON
### Theorie

Leer meer over formulieren, soorten inputs en hun attributen door het volgende materiaal te bestuderen:
* 🎦 [Bekijk een video over formulieren](https://dlo.mijnhva.nl/d2l/le/content/536505/viewContent/1996729/View)
* De belangrijkste info uit bovenstaande video is ook terug te vinden in onze [kennisbank](https://bnieskens.notion.site/Formulieren-9265d336e2954c71be6be4ab847f8fcc)
* Learn [Web Forms](https://developer.mozilla.org/en-US/docs/Learn/Forms) op MDN. Lees de hoofdstukken:
  * Introductory guides
  * The different form controls
  * Form styling guides en Validating
  * Submitting form data.

### Oefening: Login op basis van JSON

1. Bestudeer het [codevoorbeeld voor een inlogfomulier](https://scrimba.com/scrim/co3f042a6a22d4846e9104959) op Scrimba
2. Bespreek met je mede-studenten hoe dit precies werkt:
    * in welke variabelen staan de inloggevens die de gebruiker heeft ingevuld?
    * in welke variabelen staan de geldige inloggevens?
    * hoe worden de ingevulde gegevens vergeleken met de geldige gegevens?
3. Start je Data API en maak een paar gebruikers aan
    * gebruik tabbed postman in je browser om handmatig gebruikers toe te voegen
    * geef je users een naam en wachtwoord
4. Verander het codevoorbeeld zodat het de lijst met bestaande gebruikers ophaalt uit jouw Data API in plaats van het JSON bestand
    * welke URL moet je nu meegeven aan de Fetch API?
    * hoe is de structuur van de JSON-data uit de API anders dan de structuur van het eerdere JSON bestand?

### Oefening: Formulier voor het aanmaken van een nieuw account
* Maak een formulier waarmee nieuwe gebruikers zich kunnen registreren
* Een gebruiker heeft in elk geval een naam en een wachtwoord
* Voeg velden toe die voor jouw feature nuttig zijn: e-mail, leeftijd, woonplaats, favoriete muziek, huisdier???
* Maak alleen de HTML / CSS, dus nog geen JS code om het formulier te verwerken

Maak deze opdracht af voor de volgende les.


## 2. Formulieren met de Data API
### Opdracht: Opslaan van nieuwe accounts

Bij deze opdracht gaan we verder met het formulier wat je hebt gemaakt voor het aanmaken van nieuwe accounts. We gaan er nu voor zorgen dat die nieuwe accounts ook echt bewaard gaan worden. Je kunt dan een nieuw account aanmaken en vervolgens, met het inlogformulier uit de vorige opdracht, ook echt inloggen op dat nieuwe account.

We gaan nu een stuk JavaScript toevoegen aan je nieuwe formulier om te zorgen dat de ingevulde gegevens voor het nieuwe account ook worden opgeslagen door de Data API. 

1. Schrijf een JavaScript functie die wordt geactiveerd zodra de gebruiker het registratieformulier verstuurd. Doe dit door een onClick event toe te voegen aan de submit button.
2. Gebruik in je JavaScript functie de Fetch API om je nieuwe gebruiker op te laten slaan door de Data API. Hier komen een aantal nieuwe aspecten bij kijken. Bekijk de [documentatie over Fetch](https://developer.mozilla.org/en-US/docs/Web/API/fetch) om te zien hoe je deze nieuwe opties kunt toevoegen.
     * tot nu toe heb je met Fetch HTTP GET requests gedaan. Nu willen we een HTTP POST request doen. We zullen dus de request method moeten aangeven bij de aanroep van Fetch.
     * Het opslaan van gegevens via een API is 'gevaarlijker' dan alleen het uitlezen van gegevens. Je krijgt daarom nu te maken met een extra beveiling, de zogenaamde Cross-Origin Resource Sharing, oftewel CORS. Je zult nu bij de aanroep van Fetch de mode CORS moeten aangeven.
     * Tenslotte wil je nu ook een body meegeven aan je HTTP request met daarin de gegevens over de nieuwe gebruiker in JSON formaat. Hierbij moet je de indeling volgen zoals gespecificeerd in de README van de Data API.
3. Het is een goed idee om nu te controleren of je nieuwe gebruiker goed is opgeslagen. Dit kun je doen door in de browser met tabbed postman een actuele lijst op te vragen van alle gebruikers uit de Data API. Staat de nieuwe gebruiker er tussen en kloppen alle gegevens?
4. Kijk tenslotte of je nu het inlogformulier uit de vorige les kunt gebruiken om in te loggen als je nieuwe gebruiker


## Huiswerk: Voorbereiding voor volgende les

Maak voor de volgende verdiepingsles een eigen Atlas MongoDB account en database aan volgens de instructies in de officiele [MongoDB start with guide](https://www.mongodb.com/docs/guides/atlas/account/). Volg in elk geval de stappen:
1. Create MongoDB account
2. Create a cluster
3. Add a database user
4. Configure a network connection
