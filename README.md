# Portfolio von mar-we-tech

Dieses Repository enthält verschiedene Programmierprojekte, die ich neben meinem Studium in meiner Freizeit erstellt habe. Die meisten Projekte sind dokumentiert, inklusive aufgetretener Fehler und deren Lösungen.

---

## 1. Zahlenraten (SwiftUI)

### Beschreibung
Ein einfaches Zahlenratenspiel, bei dem der Benutzer eine Zahl zwischen 1 und 100 erraten muss. Das Programm gibt Hinweise, ob die Zahl zu hoch oder zu niedrig ist.

### Herausforderungen & Lösungen
- **Fehlende Eingabevalidierung:** Anfangs konnte der Benutzer beliebige Zeichen eingeben. Gelöst durch `if let guess = Int(userGuess)`, um sicherzustellen, dass nur Zahlen akzeptiert werden.
- **Fehlende Spielneustart-Funktion:** Wurde später durch eine zusätzliche Schaltfläche ergänzt.

---

## 2. Taschenrechner 2.0 (SwiftUI)

### Beschreibung
Ein Taschenrechner mit den Grundrechenarten sowie Exponentialfunktion.

### Herausforderungen & Lösungen
- **Division durch Null:** Anfangs wurde bei `num1 / num2` kein Fehler abgefangen. Gelöst durch `num2 == 0 ? "Fehler: Division durch 0" : "Ergebnis: \(num1 / num2)"`.
- **Falsche Darstellung der Ergebnisse:** Problem mit der Formatierung der Zahlen, gelöst durch `String(format: "%.2f", result)`.

---

## 3. Memory Spiel 2.0 (SwiftUI)

### Beschreibung
Ein Memory-Spiel mit acht Kartenpaaren.

### Herausforderungen & Lösungen
- **Karten drehten sich nicht zurück:** Nach einem falschen Versuch blieben Karten offen. Gelöst durch `DispatchQueue.main.asyncAfter(deadline: .now() + 1) { ... }`, um eine Verzögerung beim Umdrehen der Karten zu ermöglichen.
- **Fehlende zufällige Anordnung:** Karten wurden immer in der gleichen Reihenfolge angezeigt. Gelöst durch `shuffled()`-Funktion auf die Kartensymbole.

---

## 4. Snake Game 1.0 (HTML, CSS, JavaScript)

### Beschreibung
Eine klassische Umsetzung des Snake-Spiels im Browser.

### Herausforderungen & Lösungen
- **Schlangenbewegung zu schnell/langsam:** Anpassung der `setInterval()`-Werte für eine gleichmäßige Geschwindigkeit.
- **Kollisionserkennung ungenau:** Verbesserte Berechnung der Kollision mit der Wand und dem eigenen Körper.

---

## Weitere Projekte
Zukünftige Projekte werden hier ergänzt. Jede Anwendung ist so strukturiert, dass sie leicht verständlich und erweiterbar ist. Feedback ist willkommen!
