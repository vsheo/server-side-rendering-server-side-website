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
Op de indexpagina ziet de gebruiker verschillende kaartjes. Elk kaartje heeft een titel. Wanneer de gebruiker op de titel klikt, wordt hij naar een detailpagina geleid waar hij meer over het cadeautje kan lezen.
![index_pagina](https://github.com/user-attachments/assets/01e30cb9-6a8a-455c-bb73-294575dff332)

## Gebruik
<!--Bij Gebruik staat hoe je project er uit ziet, hoe het werkt en wat je er mee kan. -->
Op de indexpagina staan verschillende cadeautjes. De gebruiker kan de naam en een afbeelding van het cadeau zien.
Als de gebruiker op de naam klikt, wordt hij of zij naar de detailpagina geleid.
Op deze pagina ziet de gebruiker ook de beschrijving van het cadeau.


https://github.com/user-attachments/assets/09f1eb4c-3ea9-4da4-a661-1ba09cebf143



## Kenmerken
<!-- Bij Kenmerken staat welke technieken zijn gebruikt en hoe. Wat is de HTML structuur? Wat zijn de belangrijkste dingen in CSS? Wat is er met Javascript gedaan en hoe? Misschien heb je een framwork of library gebruikt? -->
De stukken HTML-code die vaker herhaald worden op de website, zijn in een eigen Liquid file geplaatst. Dit is gedaan zodat ze met Liquid op de juiste plek ingeladen kunnen worden.
Als er een aanpassing in de HTML nodig is, hoeft dit maar op één plek te gebeuren.
Deze article:
https://github.com/vsheo/server-side-rendering-server-side-website/blob/791717c93a3c46a8ce76d2dc7e5d33fdc51b9932/views/partials/article-gift.liquid#L1-L8

wordt op de volgende plekken gebruikt:
https://github.com/vsheo/server-side-rendering-server-side-website/blob/791717c93a3c46a8ce76d2dc7e5d33fdc51b9932/views/index.liquid#L26-L29
https://github.com/vsheo/server-side-rendering-server-side-website/blob/791717c93a3c46a8ce76d2dc7e5d33fdc51b9932/views/details.liquid#L61-L62

### Styleguide
De huisstijl is gebaseerd op dit [figma design](https://www.figma.com/design/4NBbUuyXIrZ7VFHaDAHJLs/milledoni-design?node-id=6-23251&t=GgUuJZRB3GWeNTFB-1)
Dit is een [HTML-pagina]() met alle classes en custom properties van de Styleguide

De font sizes voor titels zijn responsive gemaakt met clamp, zodat ze niet te groot lijken op kleine schermen
voorbeeld van fontsizes met clamp:
https://github.com/vsheo/server-side-rendering-server-side-website/blob/7ac4e29f5be2bced1afadd0965dfd11c7088d742/public/styles/milledoni.css#L33-L37

font sizes met clamp
Naamgeving van custom properties: Het eerste woord (en soms ook het tweede) geeft aan waarvoor de custom property bedoeld is, en het laatste woord geeft aan wat er wordt veranderd.

Bijvoorbeeld, 'background-primary': het eerste woord geeft aan dat het voor de achtergrond bedoeld is, en het tweede woord geeft aan dat het de primaire kleur is.
https://github.com/vsheo/server-side-rendering-server-side-website/blob/7ac4e29f5be2bced1afadd0965dfd11c7088d742/public/styles/milledoni.css#L13-L16

In dit voorbeeld gebruik ik twee woorden om aan te geven voor welk element de custom property bedoeld is, en daarna wat het veranderd.
voorbeeld
--font-weight-regular
font-weight geeft aan dat het met de fonts te maken heeft, en regular geeft aan dat het de standaard font weight is.
https://github.com/vsheo/server-side-rendering-server-side-website/blob/7ac4e29f5be2bced1afadd0965dfd11c7088d742/public/styles/milledoni.css#L39-L44

voor de font weight benaming heb ik aangehouden hoe het in de font .ttf file heeft
hier zijn de font-weight cuistom properties in css stylesheet

### Responsive
#### Index pagina
Voor het grootste deel van de responsiveheid op de indexpagina heb ik een grid gebruikt om automatisch een nieuwe kolom te maken zodra er voldoende ruimte is.
Hiervoor heb ik in mijn grid-template-columns de functie repeat met auto-fit gebruikt om de kolommen te herhalen. Daarbij heb ik ook minmax toegepast om de minimale breedte te bepalen voordat er een nieuwe kolom wordt toegevoegd.
https://github.com/vsheo/server-side-rendering-server-side-website/blob/7ac4e29f5be2bced1afadd0965dfd11c7088d742/public/styles/style.css#L219

Dit heb ik gedaan zodat er automatisch een nieuwe kolom wordt gemaakt, waardoor er op hele grote schermen nooit te veel witruimte is.

De index pagina is responsief vanaf 320 pixels.
![responsive_320](https://github.com/user-attachments/assets/5e5238ab-f8fa-4796-85ed-0f4fb9b6628e)

De eerste breakpoint ligt bij 560 pixels.
![responsive_560_1](https://github.com/user-attachments/assets/e9e17d4c-1f68-4fa1-b1af-854010273f22)
![responsive_560_2](https://github.com/user-attachments/assets/c0d5d338-585d-4022-b930-2194b728d4e9)

Bij 700 pixels komt er een nieuwe kolom.
![responsive_700_1](https://github.com/user-attachments/assets/23bda5b0-c14e-4a8f-87cc-287791c88f17)
![responsive_700_2](https://github.com/user-attachments/assets/7ea7f234-877e-47a9-8504-8959da638ebf)

Bij 800 pixels komt er een derde kolom.
![responsive_870](https://github.com/user-attachments/assets/e943e5ce-48ad-4c56-a5b6-4837518404e9)

Vanaf 1100 pixels begint de desktop versie.
![responsive_1100](https://github.com/user-attachments/assets/a7fa9aac-6ce9-4b38-871a-464e66704ecf)

Bij 1440 pixels komt de versie die overeenkomt met het Figma-ontwerp.
![responsive_1440](https://github.com/user-attachments/assets/697b7a6b-08f7-424e-8ec3-e8d628d84b2e)

Na 1440 pixels wordt er een kolom toegevoegd zodra er voldoende ruimte is.


https://github.com/user-attachments/assets/bf59f787-5ee2-4212-a553-ea6840dc8758


#### Details pagina
De detailpagina is nog niet responsief, maar is goed te bekijken op een scherm van 320 pixels.
![responsive_details_320](https://github.com/user-attachments/assets/8e70026b-0f5a-4acd-abc2-b3d3197cccec)


## Installatie
<!-- Bij Instalatie staat hoe een andere developer aan jouw repo kan werken -->
- Download de nieuwste versie van Node.js (https://nodejs.org/en) op je laptop of computer.
- Fork deze repository en clone deze naar je laptop.
- Open de repository in GitHub.
- Open de terminal in VS Code en voer het volgende command uit:
    - 'npm install'
- Zodra de installatie klaar is, voer je het volgende commando uit om de website op localhost te starten:
    - 'npm start'
- Als alles goed is gegaan, krijg je in de terminal een link naar de juiste localhost. Klik hierop om de website in de browser te openen.
- Om de website te stoppen, voer je in de VS Code terminal het volgende command uit:
    - 'Ctrl + C'

## Bronnen

## Licentie

This project is licensed under the terms of the [MIT license](./LICENSE).
