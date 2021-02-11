Arbeitsauftrag 11.2
-------------------
## 1 Nennen Sie drei Beispiele für den Einsatz von Datenbanken und beschreiben Sie für jedes Szenario, WAS in der Datenbank verwaltet wird. 

### Nutzen zum Verwalten von Nutzerlogindaten
In der Datenbank würden gehashte Passworter und Nutzerdaten gespeichert werden.

### Speichern von Umfrageergebnissen
Pro Zeile würde man eine Umfrage und pro Spalte eine Frage speichern.

### Verwalten von Angestellten Daten
Die Namen werden zusammen mit anderen persönlichen Daten in einer Spalte gespeichert.  

## 2 Geben Sie die wesentlichen Probleme wieder, die bei der dateibasierten Datenverarbeitung auftraten und letztendlich zur Entwicklung und zum Einsatz von Datenbanksystemen geführt haben. 
- Daten werden mehrfach gespeichert
- Daten können sich so voneinander unterscheiden
- Kein standartisiertes Interface um auf Daten zu zugreifen
- Datenschutz sehe ich noch nicht ganz, man kann ja die Rechte entsprechend beschränken


## 3 Grenzen Sie die Begriffe Datenbanksystem, Datenbankmanagementsystem und Datenbank voneinander ab. 

### Datenbanksystem
Beschreibt das System in dem die Datenbank läuft. Ein Beispiel wäre ein MYSQL Server.

### Datenbankmanagementsystem
Ein System um eine Datenbank zu verwalten. z.B. ein MYSQL Client mit dem der Admin Änderungen an einer Datenbank vornehmen kann.
 

## 4 Beschreiben Sie, was eine Transaktion ist was durch Transaktionen ermöglicht wird. 
Eine Transaktion ist jedes Interagieren mit der Datenbank. So kann ich auf Daten Lesend oder Schreibend zugreifen und Zeilen und Spalte löschen bzw. hinzufügen.

 

### 5 Beschreiben Sie kurz die Drei-Ebenen-Architektur eines DBMS (Benennung der Ebene und Beschreibung, was darin festgelegt wird). 
| Ebene 		| Funktion 								|
|-----------------------|-----------------------------------------------------------------------|
| Externe Ebene		| Programme die die Datenbank benutzen (APIs, Benutzeroberflächen ...) 	|
| Konzeptionelle Ebene  | Daten/Beziehungen von Daten						|
| interne Ebene		| Speicherung, Zugriff							|
 

## 6 Welche Vorteile bietet die Drei-Ebenen-Architektur eines DBMS? 
Änderung auf einer Ebene wirken sich nicht auf eine andere an. Dies macht es deutlich einfacher z.B. Speichermedien auszutauschen und auch Änderungen an der Datenbank haben keine Auswirkungen auf andere Ebenen/auf die Technik außenrum.

## 7 Listen Sie die neun Ziele der Datenorganisation auf und beschrieben Sie jede mit einem kurzen Satz. 

### 1 Datenunabhängigkeit
Daten sind unabhängig von der Anwendung oder von logischen/physischen Datenorganisation gespeichert bzw. nutzbar/verarbeitbar.

### 2 Redundanzfreiheit
Jedes Datum sol möglichst nur einmal gespeichert werden

### 3 Datenintegrität
Die Daten müssen vollständig, korrekt und ohne wiederspruchsfrei gespeichert sein

### 4 Benutzerfreundlichkeit 
...komisches Ziel. 

### 5 Mehrfachzugriff, Synchronisation
jeder der darf kann auch jederzeit auf die Daten zugreifen. 

### 6 Datenschutz
Nur authorisierte Benutzer/Anwendungen haben Zugriff auf die Daten

### 7 Datensicherheit
Daten müssen geschütz sein vor Hard- und Softwarefehlern

### 8 Flexibilität
Daten müssen beliebig Verknüpfbar sein und Wahlfrei als auch sequenziell abrufbar sein.

### 9. Effizienz
Die Zugriffszeiten sollen kurz sein (schreibend sowie lesend)

## Zusatz: 8 Benennen Sie die gängigen Datenbankmodelle und beschrieben Sie jedes in 1-3 Sätzen 

### Hierarchische und Netzwerkartige
Die Datenfelder sind hierarchisch in einem Baum angeordnet und der Zugriff erfolgt von der Wurzel aus. Bei einer Netzartigen kann hingegen beliebig vermascht werden. Dies erhöht stark die Flexibilität

### Relationale Datenbanken
Besteht ausschließlich aus Tabellen. Zwischen verschiedenen Tabellen sind verknüpfungen, so genannte Beziehungen möglich.

### Objektorientierte Datenbanken
Besteht ausschließlich objekte. Oftmals als Erweiterung zu relationellen Datenbanken.

### No-SQL-Datenbanken
Geeignet um sehr große Datenmengen zu verwalten. Grob kann zwischen *Key-Value-Datenbanken* und *Dokument-Datenbanken* unterschieden werden.
 

 

## Zusatz 9: Unterscheide Sie Datenbanken nach ihrer Betriebsart. 

### Stand Alone Datenbank
Einfachste Form, Daten werden lokal in einer Datenbankdatei gespeichert. Kein Mehrfachbenutzersystem und keine Verwaltung von Zugangsberechtigungen

### File Share Datenbank
Übers Netzwerk geteilte Datenbank. Datenbankclients laufen auf allen beteiligten Rechnern. Auch Client-Server Datenbank genannt.

### Welche Betriebsart finden Sie heute überwiegend (ausschließlich?) in Unternehmen, wenn komplexe Datenbestände von mehreren Nutzergruppen ausgewertet werden müssen? 
Ausschließlich File Share Datenbanken da Standalone nicht den Mehrbenutzer-Betrieb ermöglichen.

