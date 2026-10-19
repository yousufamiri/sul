# Für Sulaiman ❤️

Eine responsive Geburtstagsüberraschung auf Persisch, mit drei Szenen, goldener Geschenkbox, Konfetti, Torte und einer sanften, im Browser erzeugten Spieluhrmelodie.

## Dateien

- `index.html` – alle Texte und drei Szenen, mit `lang="fa"` und RTL
- `style.css` – Gestaltung, responsive Layouts und Animationen
- `script.js` – Szenenablauf, Konfetti und Musik
- `assets/favicon.svg` – eigenes Icon
- `vercel.json` – Vercel-Konfiguration

Keine Installation, kein Build, keine Umgebungsvariablen und kein Backend nötig.

## Lokal ansehen

`index.html` im Browser öffnen. Alternativ im Projektordner `python3 -m http.server 8000` starten und http://localhost:8000 öffnen.

## Kostenlos auf Vercel veröffentlichen – Schritt für Schritt

Sulaiman braucht weder ein Konto noch eine Anmeldung. Nur du benötigst zum Veröffentlichen ein kostenloses Vercel-Konto. Für dieses private, nicht kommerzielle Geschenk eignet sich der kostenlose Hobby-Tarif; aktuelle Tarifbedingungen bei Vercel prüfen.

### Weg A: Mit GitHub und ohne Terminal

 1. ZIP entpacken.
 2. Auf https://github.com anmelden und ein neues Repository anlegen, z. B. `sulaiman-birthday`. Es darf privat sein.
 3. Über „Add file“ → „Upload files“ alle Dateien aus dem entpackten Projektordner hochladen, einschließlich `assets`. `index.html` und `vercel.json` müssen auf der obersten Ebene des Repositorys liegen. „Commit changes“ anklicken.
 4. Auf https://vercel.com anmelden, „Add New…“ → „Project“ wählen und GitHub verbinden.
 5. Das Repository importieren. Als Framework „Other“ wählen. Root Directory auf `./` belassen, kein Build Command und keine Umgebungsvariablen setzen. Die beiliegende `vercel.json` legt das Ausgabeverzeichnis fest.
 6. „Deploy“ anklicken und auf den erfolgreichen Abschluss warten.
 7. Unter „Visit“ beziehungsweise „Domains“ die Produktionsadresse kopieren, z. B. `https://sulaiman-birthday.vercel.app`. Der tatsächliche Name kann abweichen.
 8. Den Link in einem privaten Browserfenster öffnen. Falls eine Vercel-Anmeldeseite erscheint: In den Projekteinstellungen unter „Deployment Protection“ den Schutz der Produktionsseite deaktivieren, damit Sulaiman ohne Anmeldung zugreifen kann. Verwende den Produktionslink und keinen geschützten Preview-Link.
 9. Den Link am iPhone testen: Geschenk öffnen, beide Witze abwarten, Musik an/aus und Wiederholung prüfen. Bei aktiviertem Stummmodus kann iOS die Musikwiedergabe unterdrücken.
10. Den öffentlichen Link in WhatsApp einfügen, z. B. mit „سلیمان جان، این هم یک سورپرایز کوچک برای تو ❤️🎁“.

### Weg B: Direkt über die Vercel CLI

Mit installiertem Node.js im entpackten Projektordner ausführen:

```sh
npx vercel --prod
```

Anmelden, neues Projekt erstellen und die Vorgaben für ein statisches Projekt übernehmen. Kein Build erforderlich. Die CLI gibt die fertige Produktionsadresse aus. Anschließend Schritte 8–10 oben durchführen.

## Ablauf und Anpassung

- Antippen der Box öffnet sie und startet die Musik, sofern sie nicht zuvor bewusst ausgeschaltet wurde.
- Der zweite Witz erscheint zwei Sekunden nach dem ersten. Anschließend folgt die Geburtstagsszene automatisch.
- „یک بار دیگر ببین 🎁“ setzt die Szenen zurück.
- Die Musik kann jederzeit über den Button oben rechts umgeschaltet werden; im Hintergrund wird sie pausiert.
- Texte in `index.html`, Farben oben in `style.css`, zeitliche Abstände in `script.js` bearbeiten.
- `prefers-reduced-motion` reduziert Bewegung und schaltet Konfetti aus.

## Datenschutz und Schrift

Die Seite verwendet keine Formulare, Cookies, Analysewerkzeuge oder Speicherung persönlicher Daten. Der Hostinganbieter verarbeitet technisch erforderliche Verbindungsdaten. Vazirmatn wird über Google Fonts geladen; dabei wird eine Verbindung zu Google aufgebaut. Ist die Schrift nicht erreichbar, erscheint eine lokale Ersatzschrift. Die Seite und die Musik funktionieren weiter. Für vollständig lokale Schriftbereitstellung kann die unter SIL Open Font License verfügbare Vazirmatn-Datei samt Lizenz in `assets/` abgelegt und per `@font-face` eingebunden werden.

Die Seite ist als fertiges statisches Projekt vorbereitet, aber noch nicht auf Vercel veröffentlicht. Ein Vercel-Konto wurde nicht verbunden. JavaScript-Syntax und Projektstruktur wurden geprüft; ein visueller Browser- oder echter iPhone-Test war in der Erstellungsumgebung nicht verfügbar.