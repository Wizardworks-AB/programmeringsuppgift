# Wizardworks: Programmeringsuppgift

Se PDF för mer detaljerad vy över flödesdiagram etc. [PDF](https://github.com/Wizardworks-AB/programmeringsuppgift/blob/master/Wizardworks%20-%20programmeringsuppgift.pdf)

## Uppgift

Skapa en webbsida som genererar potentiellt oändligt med kvadrater i en kvadratisk form. För varje knapptryckning på "Lägg till ruta" ska en ny ruta läggas till, och färgen på rutan ska slumpas fram (dock aldrig samma färg som föregående ruta).

### Funktionalitet

1. **Frontend**:
    - Byggs med React.js.
    - Inget krav på CSS-ramverk, men TailwindCSS kan användas om så önskas.
    - För varje klick på "Lägg till ruta" ska en slumpmässigt färgad ruta läggas till.

2. **Backend**:
    - Ett API byggs med .NET/C#.
    - Vid varje knapptryckning ska position och färg på rutan sparas ner i en JSON-fil via API:et.
    - När webbsidan laddas om, ska det tidigare tillståndet återläsas från API:et för att bibehålla state.

## Teknisk stack

- **Frontend**: React.js
- **Backend**: .NET/C#
- **Lagring**: JSON-fil via .NET API

## Flöde

- En användare klickar på "Lägg till ruta", vilket triggar en händelse i React-applikationen som genererar en ny kvadrat.
- Varje ruta får en slumpmässig färg som inte är samma som föregående ruta.
- Position och färg på varje ruta skickas till API:et som sparar dessa värden till disk i JSON-format.
- När sidan laddas om, hämtar webbsidan den senaste layouten från API:et och återställer de genererade rutorna.

## Krav

- **React.js**: Applikationen ska kunna rendera kvadrater dynamiskt på sidan.
- **.NET/C# API**: Hantering av state (spara och läsa in data från en JSON-fil).
- **Inga CSS-ramverk krävs**, men TailwindCSS kan användas om önskas.

## FAQ

### Var ska koden sparas?
Koden ska sparas på ett publikt Github-repository.

### Kan jag använda AI-verktyg?
Absolut! Använd gärna verktyg som ChatGPT och Github Copilot för att underlätta din utveckling, men var beredd på att förklara dina val.

### Måste jag driftsätta lösningen?
Nej, det räcker med att köra den lokalt.

---

Lycka till med uppgiften! Om du har några frågor eller stöter på problem, tveka inte att höra av dig.
