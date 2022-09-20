[TOP](../../)

# Solution Design für Szenario "Reimplementierung"

## Einführung

[…] siehe Szenario […] soll von jedem Stakeholder auf jeden Fall verstanden werden.

## Zusammenfassung der existierenden Funktionalitäten

Nutzer können aktuell Vorgänge X, Y, Z mit dem gegebenen System erledigen.
Das Erledigen ist allerdings nur unter Schwierigkeiten möglich wie schlechte Reaktionszeiten/UX der GUIs.

## Anforderungen an neues System

Listung aller Vorgänge X1, Y1, Z1 die auf IST Stand gemappt sind.

Non-funktionale Anforderung zu (**Annahmen aus Szenario**):
* Wartbarkeit
* Anpassbarkeit
* Performance
* UX

## Umgebung und Vorraussetzungen

* wie beispielsweise Windows Clients, Schnittstellen wie bisher, Datenformate, …

## Lösung (High Level)

* Diagramme auf Prozessfluss-Ebene, Integration/Schnittstellen nach außen (außerhalb dieser Lösung)

## Lösung (Low Level)

**Annahmen aus Szenario**

* Komponenten in Zukunft sind:
  * Cloud gehostet Server Software 
    * Technologie: Elixir Programmiersprache
    * Transportsicherheit mittels VPN (Authentifikation in VPN-Standardsoftware)
    * alle Geschäftslogiken am Server -> zentrales Logging, Fehlererkennung,
      Auslieferung von Updates einfacher
    * skaliert horizontal
  * Persistenzschicht
    * Datenbank (ohne Geschäftslogik) gemappt mittels ORM
    * Dateisystem mit vordefinierten Dateiformaten (siehe Umgebung/Vorraussetzungen)
  * Client Software
    * in Windows integriert sein: Webapp mit modernen UX/UI Frameworks in Typscript     

## Out-of-scope

Ähnlich negativen Anforderung, Beschreibung was nicht bestandteil sein soll.

**Annahmen aus Szenario** Reimplementierung von Authentifikation/Athorisationsschichten

## Risiken und Mitigation

**Annahmen aus Szenario** Bestellte Perfomance kann nicht geliefert werden -> Caches einsetzen, Horizontal Massiv skalieren, Lastests vorab


## Iteration
Prinzip für Messbarkeit der Zwischenergebnisse
