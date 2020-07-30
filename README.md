# Synthea_DE # 

## Hinweis ##
Der Synthea_DE Ordner enthält die Konfigurationsdateien um mit Synthea deutsche Daten generieren zu können. Derzeit sind lediglich die Städte Leipzig und Dresden vorhanden, weitere Städte und Bundesländer können jedoch nach der Anleitung [hier](https://github.com/synthetichealth/synthea/wiki/Other-Areas) ersetzt oder ergänzt werden.

Da diese Anpassungen im Rahmen meiner Bachelorarbeit stattfanden, stelle ich die Arbeit in Zukunft hier ebenfalls zur Verfügung.  

Im Output/Fhir Ordner befinden sich bereits ca. 100 Patienten die testweise im Fhir R4 Standard erzeugt wurden.  


## Nutzung ##
Syntheas Ressourcenordner synthea\src\main kann durch diesen main Ordner hier ersetzt werden. Die synthea.properties Datei kann noch nach Wunsch angepasst werden. Kompilieren Sie den Code (Gradle build erneut durchführen) und anschließend können deutsche Patienten generiert werden. 

Eine allgemeine Anleitung ist für Synthea [hier](https://github.com/synthetichealth/synthea/wiki/Developer-Setup-and-Running) zu finden. 

Beispiele für das Ausführen von Synthea zur Erzeugung deutscher Patienten:  
./run_synthea Sachsen  
./run_synthea Sachsen "Leipzig"  
./run_synthea Sachsen "Dresden" -p 10  
  
Bitte beachten: da der Quellcode teilweise verändert wurde,  
kann es zu Fehlern kommen beim generieren amerikanischer Patienten.  
Falls Fehler beim build auftreten kann evtl. der Befehl 'gradle build check test --debug' helfen. 

## mögliche Verbesserungen ##

Weitere deutsche Städte in verschiedenen Bundesländern ergänzen;   
Kosten anpassen bzw. entfernen;  
siehe BA für mehr... 
