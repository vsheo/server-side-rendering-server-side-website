> _Fork_ deze leertaak en ga aan de slag. Onderstaande outline ga je gedurende deze taak in jouw eigen GitHub omgeving uitwerken. De instructie vind je in: [docs/INSTRUCTIONS.md](docs/INSTRUCTIONS.md)

# Titel
<!-- Geef je project een titel en schrijf in één zin wat het is -->

## Inhoudsopgave

  * [Beschrijving](#beschrijving)
  * [Gebruik](#gebruik)
  * [Kenmerken](#kenmerken)
  * [Installatie](#installatie)
  * [Bronnen](#bronnen)
  * [Licentie](#licentie)

## Beschrijving
<!-- In de Beschrijving staat kort beschreven wat voor project het is en wat je hebt gemaakt -->
<!-- Voeg een mooie poster visual toe 📸 -->
<!-- Voeg een link toe naar Github Pages 🌐-->

## Gebruik
<!--Bij Gebruik staat hoe je project er uit ziet, hoe het werkt en wat je er mee kan. -->

## Kenmerken
<!-- Bij Kenmerken staat welke technieken zijn gebruikt en hoe. Wat is de HTML structuur? Wat zijn de belangrijkste dingen in CSS? Wat is er met Javascript gedaan en hoe? Misschien heb je een framwork of library gebruikt? -->
De stukken HTML code die vaker herhaald worden op de website zijn in hun eigen liquid file geplaatst. dit is gedaan zodat het met liquid op de juiste plaat ingeladen kan worden. als er een aanpassing nodig is, in de HTML, dan wordt dat op maar 1 plek gedaan.
voorbeeld van herhaalende code
Deze article:
https://github.com/vsheo/server-side-rendering-server-side-website/blob/791717c93a3c46a8ce76d2dc7e5d33fdc51b9932/views/partials/article-gift.liquid#L1-L8
wordt op de volgende plekken gebruikt:
https://github.com/vsheo/server-side-rendering-server-side-website/blob/791717c93a3c46a8ce76d2dc7e5d33fdc51b9932/views/index.liquid#L26-L29
https://github.com/vsheo/server-side-rendering-server-side-website/blob/791717c93a3c46a8ce76d2dc7e5d33fdc51b9932/views/details.liquid#L61-L62

### Styleguide
De huisstijl is gebaseerd op dit [figma design](https://www.figma.com/design/4NBbUuyXIrZ7VFHaDAHJLs/milledoni-design?node-id=6-23251&t=GgUuJZRB3GWeNTFB-1)
Dit is een [HTML-pagina]() met alle classes en custom properties van de Styleguide

De font sizes voor titels zijn responsive gemaakt met clamp, zodat ze niet te groot lijken op kleine schermen

font sizes met clamp
Naamgeving van custom properties Het eerste, en soms ook het tweede, woord geeft aan waarvoor de custom property bedoeld is, en het laatste woord geeft aan wat het verandert.

Bijvoorbeeld, 'background-primary': het eerste woord geeft aan dat het voor de achtergrond bedoeld is, en het tweede woord geeft aan dat het de primaire kleur is.
voorbeeld in stylesheet
In dit voorbeeld gebruik ik twee woorden om aan te geven voor welk element de custom property bedoeld is, en daarna wat het veranderd.
voorbeeld
--font-weight-regular
font-weight geeft aan dat het met de fonts te maken heeft, en regular geeft aan dat het de standaard font weight is.

voor de font weight benaming heb ik aangehouden hoe het in de font .ttf file heeft
hier zijn de font-weight cuistom properties in css stylesheet

## Installatie
<!-- Bij Instalatie staat hoe een andere developer aan jouw repo kan werken -->
download de nieuwste versie van Node.js (https://nodejs.org/en) op je laptop/computer.
fork deze repository, en clone het op je laptop.
open de repository in  github.
maak daarna de terminal in github open. en voer de volgende command uit:
npm install
als deze claar is kan je command
npm start
uitvoeren om de website op localhost op te starten.
als het goed is gegaan dan krijg je in de terminal een link naar de juiste localhost port.
als je hierop klikt dan open de website in de browser

als je de website wilt stoppen dan kan je in de vscode terminal de command:
"ctrl + c" 
uitvoeren om de localhost te stoppen

## Bronnen

## Licentie

This project is licensed under the terms of the [MIT license](./LICENSE).
