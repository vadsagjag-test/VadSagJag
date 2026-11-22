# VadSågJag PWA – version 0.1

En fristående svensk mobilwebbapp med kamera/bildval, flyttbar beskärningsram, frivillig titel, tjänster, noteringar, två sorteringslägen, vänstersvep för att visa redigering/borttagning och lokal IndexedDB-lagring. Ingen backend, inget konto och inga externa bibliotek.

## Publicera gratis

1. Skapa ett konto på GitHub och ett **publikt** repository, t.ex. `vadsagjag-test`. (Publikt innebär att källkoden kan läsas av andra, inte att dina privata programbilder laddas upp.)
2. Ladda upp **filerna i denna mapp** till repositoryts rot (`index.html`, `app.js`, `sw.js`, `manifest.webmanifest`, ikonerna).
3. Öppna Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)` → Save.
4. Vänta tills GitHub Pages visar din HTTPS-adress, normalt `https://DITT-NAMN.github.io/vadsagjag-test/`.
5. Öppna adressen i **Safari på iPhone**. Tryck Dela → Lägg till på hemskärmen → Lägg till.
6. Starta VadSågJag från hemskärmsikonen. Testa att fotografera, beskära och spara en post. Prova därefter flygplansläge.

Du behöver inget Apple Developer Program. GitHub Pages är en statisk webbvärd; bilder och programuppgifter skickas inte till GitHub utan sparas i iPhones lokala IndexedDB. Använd inte privat information i repositoryts filer.

## Begränsningar

- Webbappen använder iPhones kamera via bildväljaren (`capture=environment`), inte en kontinuerlig live-kameravy med ram. Ramen visas i **beskärningssteget efter fotografering**.
- Första besöket kräver internet och HTTPS. Därefter kan cachade filer fungera offline.
- Safari och hemskärmsappen kan i vissa fall ha separata lagringsutrymmen; använd konsekvent hemskärmsappen efter installation.
- Om webbplatsdata raderas, lagringsutrymme frigörs av systemet eller appen avinstalleras kan data gå förlorade. Export/backup ingår inte ännu.
- Prototypen är inte verifierad på en fysisk iPhone; testning återstår.
