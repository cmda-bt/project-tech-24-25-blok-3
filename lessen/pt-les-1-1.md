# Les 1.1 Introductie project en Github basics
## 1. Toelichting project, eindopdracht en planning
## 2. Introductie van lesmaterialen 
[Lesmaterialen](/lesmaterialen.md)

## 3. Facultatieve huiswerkopdrachten
Maak onderstaande opdrachten wanneer je herhaling van deze concepten kan gebruiken. Je mag hier zelf een keuze uit maken. Er is geen deadline voor deze opdrachten. 
- [PT 001 - Variabelen, datatypen en logica](https://scrimba.com/scrim/co965427c94fe66f3b4fedb37)
- [PT 002 - Variabelen, scope en hoisting](https://scrimba.com/scrim/c6rnM3cp)
- [PT 003 - Arrays definiëren](https://scrimba.com/scrim/co7ff4cdebcd149396dc9cf73) 
- [PT 004 - Array methoden](https://scrimba.com/scrim/cofb64e2990eb6578f16d922a)
- [PT 005 - Geavanceerde Array methoden](https://scrimba.com/scrim/co3804c55a622720647c1b62a)
- [PT 006 - Functies](https://scrimba.com/scrim/co2be4b47843a41d9ecf98332)
- [PT 007 - Objecten](https://scrimba.com/scrim/co3c54779a3d30a1dbe92c4b6)
- [PT 008 - Herhalingen (loops)](https://scrimba.com/scrim/cwmgz7Cm)

Onderstaand vind je de uitwerkingen voor de huiswerkopdrachten. Uiteraard mag je daar in de les vragen over stellen. 
- [Scrimba playlist met oplossingen](https://scrimba.com/playlist/prvKnPefp)


## 4. Git & GitHub basics

De basis van Git en het social coding platform GitHub.

## 1. Aanmaken GitHub Account

Als je dit nog niet eerder had gedaan, maak dan [een account aan op GitHub](https://help.github.com/articles/signing-up-for-a-new-github-account/). Neem een moment om je [GitHub profiel](https://github.com/settings/profile) te vullen met je naam, een leuke foto en andere relevante info over jezelf. Het is fijn als de docenten je aan je naam of foto enigszins kunnen herkennen, maar verder is creativiteit hier toegestaan.

> Je mag er zeker voor kiezen online anoniem te blijven door geen persoonlijke gegevens op GitHub te delen, maar een professioneel gevuld GitHub profiel kan je helpen bij het zoeken van een stage of baan later.

## 2. Git installeren

_Windows:_  
Download en installeer [Git for Windows](https://gitforwindows.org/). De meeste opties bij het installeren zijn standaard goed ingevuld, maar een paar instellingen verdienen je aandacht:

- Je kunt je eigen favoriete editor kiezen (Visual Studio Code of een andere).
- Het handigste is om als default branch name voor nieuwe repositories te kiezen voor 'main'. Vroeger was de default meestal 'master', maar dat heeft nogal ongelukkige associaties met het slavernijverleden. Als je kiest voor 'main' werkt het straks goed samen met GitHub, waar dat ook de standaard naam is.
- Kies tenslotte voor 'Git from the command line and also from 3rd party software', zodat je zowel vanuit PowerShell als uit bv Visual Studio Code met Git kunt werken.

_MacOS:_  
**Git installeren**\
Open een terminal en geef het commando `git --version` om te controleren of en welke versie van Git is geïnstalleerd. Apple levert in MacOS namelijk een eigen versie van het Git-protocol. Dit is niet de meest recente versie maar je gaat er alles mee kunnen doen wat vereist is voor dit project.

Is er geen versie van "Apple git" geinstalleerd, dan kun je dat alsnog doen door de Developer Tools te installeren. De instructies daarvoor vind je in de [Handleiding Git & VSCode op MacOS](https://bnieskens.notion.site/Apple-Git-VS-code-ac5ff7c895df4a2dbe29eb3600f8fb7c?pvs=4).

Wil je toch de (meest recente versie van de) 'officiële' Git installeren, dan vind je op de website van [Atlassian](https://www.atlassian.com/git/tutorials/install-git) een uitgebreide tutorial.

## 3. Van start met GIT

Verdiep je verder in de basics van Git door onderstaand artikel te lezen en de oefening te maken:

- Lees hoofdstuk [**1.1, 1.2 & 1.3**](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control) van het _Pro Git Online Book_.
- Volg de oefening: [Introduction to GitHub](https://github.com/skills/introduction-to-github) op GitHub Skills.

## 4. Git gebruiken met VS Code

Je kunt Git op verschillende manieren gebruiken, bijvoorbeeld met instructies vanuit de Command Line (Terminal op de Mac, of PowerShell voor Windows), of via een aparte GUI zoals Git Desktop. Veel studenten werken met Visual Studio Code voor het bewerken van hun code en daar is ondersteuning voor Git al ingebouwd.

- Bekijk de video [Using Git with Visual Studio Code](https://www.youtube.com/watch?v=i_23KUAEtUM)

## 5. Repository & commit

Opdracht: maak op GitHub een nieuwe repository aan. Hierin komt straks de code van je feature en de bijbehorende documentatie. Maak in je nieuwe repository alvast een readme.md aan, die je later nog kunt invullen. Ook kun je een license toevoegen. Maak in je repo ook alvast een wiki aan, met daarin een eerste pagina. In je wiki ga je je eigen onderzoek tijdens Project Tech vastleggen. Verken de interface van je repository en kijk eens naar de verschillende mogelijkheden en instellingen. Wat zie je terug van de dingen die je hierboven hebt geleerd?

Leer jezelf aan om, zodra je een klein stukje code of documentatie hebt geschreven, zo veel mogelijk **kleine commits** te maken. Het is heel normaal om 5 of 6x per dag een commit te maken in plaats van één grote commit aan het einde van de dag. Het is daarbij ook een goede gewoonte om je commit te beschrijven met een duidelijke commit message.

- Lees het artikel: [How to write a commit message](https://cbea.ms/git-commit/)
- Denk na over je eigen git strategie: hoe ga je je commit messages opstellen? Ga je gebruik maken van branches en zo ja, op welke manier? Ga je gebruik maken van issues of de project-tools binnen GitHub? Doe zelf onderzoek naar de verschillende mogelijkheden en maak een nieuwe pagina aan op je wiki, waarin je je gekozen Git strategie beschrijft.

## 6. Gitignore

Niet alle bestanden die op je computer staan, horen ook in je repo thuis. Denk aan systeembestanden (zoals de .DS_Store files die een Mac automatisch overal aanmaakt), logfiles, tijdelijke bestanden of bestanden met gevoelige informatie. In een [.gitignore](https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files) bestand kun je aangeven welke files en folders niet op GitHub moeten komen.

Opdracht: maak in je eigen repository een .gitignore file aan en zet hierin de te negeren files en folders.

## 7. Wiki

Alle research die je tijdens Project Tech doet, documenteer je op je eigen wiki. De docenten zullen deze regelmatig bekijken en hier ook feedback op geven. Op dit moment kun je in elk geval al een pagina op je wiki maken, waarin je vertelt over de verschillende alternatieven die je hebt gevonden voor het gebruiken van Git/GitHub en de uiteindelijk door jou gekozen strategie.

## 8. Markdown

Markdown wordt gebruikt om eenvoudige tekstdocumenten (plain text) toch van een beetje structuur en opmaak te voorzien. Markdown is erg populair onder developers en wordt ook op veel plekken op Github gebruikt: voor het schrijven van documentatie, in je readme, bij het aanmaken van issue, je wiki, bij code reviews en ook in het document wat je nu aan het lezen bent. Gebruik onderstaande resources om meer over Markdown te leren:

- [Wes Bos Mastering Markdown course](https://www.youtube.com/watch?v=Je5w18nn-e8&list=PLu8EoSxDXHP7v7K5nZSMo9XWidbJ_Bns3)
- [Interactive markdown tutorial](https://www.markdowntutorial.com/)
- [Markdown git reference](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

Tip: als je in VSCode een Markdown bestand bewerkt, kun je een preview venster openen naast je codevenster, zodat je meteen ziet hoe het er uit komt te zien. Je opent de preview met CTRL-K en dan V.

## 9.Readme

Opdracht:

- Bekijk de readme's van een aantal populaire repo’s. Wat voor onderwerpen worden besproken in deze readme’s en hoe zijn ze opgebouwd?
- Lees het artikel: [About readmes](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)
- Schrijf in je eigen readme - in je repository - een inhoudsopgave, met daarin alvast de onderwerpen die je tijdens project uiteindelijk verder zult gaan uitwerken. Hierbij gebruik je natuurlijk markdown!

## 10. License & Open Source

Lees de onderstaande artikelen:

- [Starting an Open Source Project](https://opensource.guide/starting-a-project/)
- [The Legal Side of Open Source](https://opensource.guide/legal/)

Opdracht: kies nu een eigen License voor je project en voeg deze toe aan je repo. Gebruik eventueel [choosealicence.com](https://choosealicense.com/) om je te helpen bij je keuze.

## 12. Bronnen
Roger Dudler heeft een [praktisch overzicht](https://rogerdudler.github.io/git-guide/) gemaakt voor Git-beginners. 
