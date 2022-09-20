[TOP](../../)

# Was ist deine Strategie, um ein Solution Design zu erstellen und zu bewerten?

* Einteilung in feststehende Blöcke im Solution Design, wie bspw. Anforderung zu 
Nutzerzahlen, Schnittstellen, Entwicklerresourcen beim Kunden, Windows Umgebung 
auf Clientseite gegenüber modularen Möglichkeiten, v.a. eingesetzte Technologien
und Produkte.

* Iterativer Ansatz um frühzeitig mit Entwürfen fürs Solution Design mit allen 
  Stakeholdern ins Gespräch zu kommen.
  **RISIKO** Nicht-entscheidbarkeit wegen "zu viele Köche" Syndrom ; Mitigation Gilden Prinzip kann meist gut funktionieren.

## Modularer Aufbau

* Viele Fragen sind Abwägungssache mit Vor-/Nachteilen (**Annahmen im Hinblick auf Szenario**)
  * Programmiersprache, die nah genug an existierender Technologie ist (Smalltalk wird durch Elixir ersetzt)
  * Datenbank Geschäftslogik kann in Server Geschäftslogik konvertiert werden (Softwarecode anstatt SQL Trigger, Functions, …) 
  * Client wird leichtgewichtiger als derzeitge Lösung (Browser, Electron Runtime o.ä. ggü. Windows Software)
  * Gesicherter Transport zum Client (VPN Tunnel, HTTPS, verschieden Authentifizierungsverfahren bis hin zu PKI …)

Diese Dimensionen können in modularen Entwürfen unterschiedliche Konfiguration eines Solution Design ergeben

**RISIKO** Flut von Solution Designs kann überwältigen

## Bewertung der Entwürfe

Messbare KPIs der Entwüfe können zum Beispiel die folgenden 5 Dimensionen sein:

| Attribut          | Bestandsystem | Cloud gehostete Reimplementierung |
| :---------------: | :-----------: | :-------------------------------: |	
| Wirtschaflichkeit | Erfüllung vorrausgesetzt | Erfüllung vorrausgesetzt |	
| Nützlichkeit      | Erfüllung vorrausgesetzt | Erfüllung vorrausgesetzt |
| Availability	    | mittel                   | verbessert      |
| Performance	      | mittel                   | verbessert      |
| Technology        | EOL oder auslaufend      | State of the Art; Standardized |

Weiterhin kann jeder Entwurf im Hinblick auf Resourceneinsatz und die zu erreichenden
organisationsweiten Zielen (nach Anforderungsanalayse) bewertet werden.
