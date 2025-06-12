# Selenium IDE Övningar (med the-internet.herokuapp.com)

Detta repository innehåller en samling testfall automatiserade med Selenium IDE, skapade som en del av en övningsserie för att bygga upp praktiska färdigheter inom webbtestautomatisering. Fokus har legat på att förstå grundläggande interaktioner, synkronisering och verifieringar med Selenium IDE.

## Projektöversikt

Vi har utforskat olika scenarier och webbinteraktioner för att täcka vanliga testfall:

### 1. Google Sökning (Grundläggande interaktion)

* **Beskrivning:** Ett enkelt testfall som navigerar till Google, söker efter en specifik term och verifierar sökresultaten.
* **Syfte:** Lära sig grundläggande `open`, `type`, `click` och `assert title` eller `assert text`.
* **Färdigheter:** Grundläggande navigering och textinmatning.

### 2. Inloggning och Utloggning (Formulärhantering & Verifiering)

* **Beskrivning:** Automatiserar inloggningsprocessen på en testsida (`practicetestautomation.com/practice-test-login/`), verifierar lyckad inloggning och loggar ut.
* **Syfte:** Öva på formulärinmatning, knappar, samt **robust verifiering** av meddelanden efter lyckad inloggning, inklusive hantering av asynkrona element med `wait for element visible`.
* **Färdigheter:** `type`, `click`, `wait for element visible`, `assert text`, `click linkText`.

### 3. Checkboxar (Formulärinteraktion)

* **Beskrivning:** Testfall som interagerar med checkboxar på `the-internet.herokuapp.com/checkboxes`.
* **Syfte:** Lära sig att markera och avmarkera checkboxar och verifiera deras tillstånd.
* **Färdigheter:** `click`, `assert checked`, `assert not checked`.

### 4. Dropdown-menyer (Select-element)

* **Beskrivning:** Testfall som väljer alternativ från en dropdown-meny på `the-internet.herokuapp.com/dropdown`.
* **Syfte:** Förstå hur man interagerar med `select`-element och verifierar det valda alternativet.
* **Färdigheter:** `select`, `assert selected label`.

### 5. Dynamisk Laddning (Asynkron innehållshantering)

* **Beskrivning:** Testar en sida där innehåll laddas dynamiskt efter en fördröjning (`the-internet.herokuapp.com/dynamic_loading`).
* **Syfte:** Lära sig att hantera asynkront laddat innehåll genom att använda `wait for element visible` för att säkerställa att element är redo innan interaktion/verifiering.
* **Färdigheter:** `click`, `wait for element visible`, `assert text`.

### 6. Multiple Windows (Fönsterhantering)

* **Beskrivning:** Automatiserar ett scenario där en länk öppnar ett nytt webbläsarfönster/flik (`the-internet.herokuapp.com/windows`).
* **Syfte:** Lära sig att växla fokus mellan olika fönster, interagera med element i det nya fönstret, stänga det, och växla tillbaka till det ursprungliga fönstret.
* **Färdigheter:** `store window handle`, `select window handle=${latest}`, `wait for element visible`, `assert text`, `close`. Detta testfall utforskar även hur Selenium IDE implicit kan hantera fönsterväxling baserat på kommandon.

---

## Hur man kör testerna

1.  **Installera Selenium IDE:** Se till att du har Selenium IDE installerat som ett webbläsartillägg (t.ex. för Chrome eller Firefox). Observera att Selenium IDE-tillägget för Chrome för närvarande kan ha kompatibilitetsproblem, som visats i tidigare felsökning. Firefox-versionen är oftast mer stabil.
2.  **Klona detta repository:** `git clone [din_repos_URL]`
3.  **Öppna `.side` filerna:** I Selenium IDE, använd `Open an existing project` och navigera till de `.side`-filer som finns i respektive projektmapp.
4.  **Kör testerna:** Klicka på "Run current test" eller "Run all tests" i Selenium IDE för att exekvera testfallen.

---

## Bidrag

Förslag och förbättringar är välkomna!
