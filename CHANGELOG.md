# Changelog

Alle nennenswerten Änderungen am UI-Atlas (früher Daumenregel, Repo pattern-library).
Die Einträge beschreiben,
was das Projekt danach kann bzw. was sich für den Nutzer ändert – kein Commit-Protokoll.

**Regel:** Jeder Commit bekommt seinen Eintrag, im selben Commit. Neues kommt oben unter
„Unveröffentlicht“ dazu; beim Release wird daraus ein Abschnitt mit Versionsnummer und Datum.

Kategorien: **Neu** (neue Funktionen), **Verbessert** (bestehendes Verhalten), **Behoben**
(Fehler), **Intern** (Struktur, Tooling, nicht sichtbar).

## Unveröffentlicht

### Neu
- Neuer Bereich „Feinschliff“ in Gut & Schlecht mit 27 Paaren: Details, die man leicht
  übersieht und die eine App erst rund machen – Spinner mit Verzögerung, Skeleton in Form des
  Inhalts, Vorladen bei Hover, Hover-Intent im Mega-Menü, Entwürfe wiederherstellen, Warnen
  beim Verlassen, Sitzungsende ankündigen, Offline-Warteschlange, automatisches Wiederholen,
  tolerante Eingaben, passende Handy-Tastatur, Einmalcode einfügen, Zeichenzähler kurz vor dem
  Limit, letzte Wahl merken, Strg+Enter zum Senden, Scrollposition beim Zurück, Zustand in der
  URL, Fokus nach dem Löschen, „neue Beiträge“-Hinweis, Status im Tab-Titel, Umschalt+Klick,
  „Kopiert ✓“ am Knopf, mitlaufende Zeitangaben, Mehrzahl und Zahlenformat, Bilder mit
  reserviertem Platz, auffindbare Tastenkürzel und Namen eintippen bei großem Löschen. Filter und
  Quiz kennen den neuen Bereich.
- Neuer Name: Aus „Daumenregel“ wird „UI-Atlas“, passend zu CSS-Atlas und HTML-Atlas. Die
  App liegt jetzt unter daniel-hopium.github.io/ui-atlas/; die alte Adresse
  …/pattern-library/ funktioniert nicht mehr. Gespeicherte Einstellungen bleiben erhalten.
- Sonne/Mond-Knopf in der Kopfleiste: schaltet zwischen hellem und dunklem Design um. Die
  Wahl bleibt gespeichert und ist dieselbe wie die Theme-Auswahl in der Token-Lektion; ohne
  eigene Wahl gilt weiter die Systemeinstellung.
- Neue Startseiten-Kachel für den ARIA-Kompass, die Schwester-App zu WAI-ARIA. Die Buttons
  zu CSS-Atlas und ARIA-Kompass tragen ein Symbol für externe Links.
- Zweisprachig: Die ganze App gibt es auf Deutsch und Englisch – Lektionen, Live-Beispiele,
  Negativbeispiele, WCAG-Kompass, alle 50 Paare von Gut & Schlecht und das Quiz. Ein Link oben
  rechts wechselt die Sprache; sie steht als `?lang=en` in der Adresse und wird gemerkt.
- Ein Klick auf das Logo führt zur Startseite.
- Gut & Schlecht wächst auf 50 Paare, mit dem neuen Bereich „Navigation & Inhalte“:
  unter anderem Passwort anzeigen, IBAN-Kästchen, `type="number"` bei der PLZ,
  Fokus im Löschdialog, Fortschritt statt Spinner, Hellgrau als Textfarbe,
  selbstlaufende Karussells, „hier“-Links und Popups beim Laden.
- Quiz mit Einstellungen: 10, 20 oder alle Paare, ein Bereich oder alle, wahlweise nur
  Paare, die man noch nicht erkannt hat. Dazu Serien-Anzeige, Auswertung pro Bereich,
  „Fehler üben“ und ein Lernstand, den auch die Galerie zeigt.
- Die Startseite verweist auf den CSS-Atlas, der als eigene App weiterlebt
  (daniel-hopium.github.io/css-atlas); alte Adressen wie `#css-flex/gap` leiten dorthin
  weiter. Der UI-Atlas bleibt damit bei UI-Regeln.
- Gut & Schlecht: UI-Details als Paar zum Ausprobieren – vom klickbaren Radio-Text
  über Doppelklick-Bestellungen bis zu springendem Inhalt –, dazu ein Quiz, das die
  Paare ohne Etikett zeigt.
- WCAG-Kompass: WCAG 2.2 auf Stufe A und AA, übersetzt für Frontend-Devs – Überblick
  mit Rechtslage, zehn Bauteile mit Angular-Hinweisen und Code „so nicht / so“, alle 55
  Kriterien filterbar, Test-Routine mit CI-Setup und eine Checkliste für den Pull Request.
- WCAG-Chips in den Lektionen führen direkt zum passenden Kriterium im Kompass.
- Eigenes Favicon: ein Daumenabdruck im Linienstil und in den Farben der mind app, als
  SVG für moderne Browser, ICO als Rückfall und PNG für den iOS-Homescreen.
- Selbsterklärende UI-Pattern-Library als einzelne Web-App: 29 Lektionen in 8 Kapiteln,
  jeweils mit Regel, Kennzahlen, Live-Beispiel, Richtig-Liste, Negativbeispielen und
  dem Hinweis, wo die Regel in der App selbst steckt.
- White-Label mit drei Marken (Fjord, Glut, Moos), Hell/Dunkel-Umschaltung und
  automatischer Kontrastprüfung der Markenfarbe.
- „Bauteile zeigen“ beschriftet alle Oberflächenelemente mit ihrem Fachbegriff.
- Lernfortschritt pro Lektion, Suche über alle Lektionen, eigene Adresse je Lektion.

### Verbessert
- Die Schwester-Apps HTML-Atlas und Angular-Patterns erscheinen als Kacheln bei den
  Schwester-Apps; die Kachel zum ARIA-Kompass nennt dessen neuen Screenreader-Trainer.
- Die Kachel zum CSS-Atlas nennt dessen neuen Umfang: über 100 Einträge.
- Die Kacheln zu CSS-Atlas und ARIA-Kompass stehen jetzt in einem eigenen Abschnitt „Die
  Schwester-Apps“ unter den Kapiteln – an derselben Stelle wie in den beiden anderen Apps.

### Behoben
- Live-Beispiele laufen auf schmalen Bildschirmen nicht mehr seitlich aus dem Bild (etwa bei
  Overlays, UX-Gesetzen und Dark Patterns); breite Tabellen scrollen weiter in ihrem eigenen
  Bereich.
- Fachliche Durchsicht aller Lektionen, des WCAG-Kompass und der 50 Paare: rund 40 Aussagen
  korrigiert – etwa dass Links nur auf Enter reagieren, dass `aria-invalid` eine Fehlermeldung
  nicht verknüpft, Details zu Angular Material, die Stufen „Tool hilft“ bei 1.4.1, 1.4.4 und
  3.1.2, die Spacing-Demo auf der eigenen Skala und veraltete Leseforschung bei Großbuchstaben.
- „Bauteile zeigen“ beschriftet jetzt auch die Seiten des WCAG-Kompass; die Etiketten
  verdecken keine Chips und Links mehr.
