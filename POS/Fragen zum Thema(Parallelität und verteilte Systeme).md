# Fragen zum Thema Parallelität und verteilte Systeme

Von Klemens Gassner und Johannes Neuper

„Bei der Herstellung dieses Textes [oder wahlweise Bildes oder des Programmiercodes etc.] wurde ChatGPT eingesetzt. Mit folgenden Prompts habe ich die KI gesteuert: "1. Parallelität bei Programmen
Was versteht man darunter?
Anwendungsbereiche und Beispiele?
Welche Vor- und Nachteile ergeben sich aus der Parallelität von Programmen., 2. Verteilte Systeme?
Was versteht man darunter?
Anwendungsbereiche und Beispiele?
Welche Vor- und Nachteile ergeben sich aus der Verteilung von Programmen., 3. Was versteht man unter einem Prozess?
Welche Eigenschaften hat ein Prozess?
Was versteht man unter einem Thread?
Zusammenhang/Unterscheidung von Prozess und Thread?, 4. Was versteht man unter Multithreading und was sind desen Vor und Nachteile?“

## Parallelität bei Programmen

1. Was versteht man darunter?
   - Parallelität bei Programmen bezieht sich darauf, dass ein Programm in mehrere gleichzeitig ausgeführte Teilprozesse oder Threads aufgeteilt wird, die gleichzeitig auf verschiedenen Prozessoren oder Kernen ausgeführt werden können. Das Ziel der Parallelisierung besteht darin, die Leistung des Systems zu verbessern, indem mehrere Aufgaben gleichzeitig ausgeführt werden, anstatt dass sie sequenziell auf einem Kern ausgeführt werden.

2. Anwendungsbereiche und Beispiele?
   - Anwendungsbereiche für die Parallelisierung von Programmen sind unter anderem:
     - High-Performance-Computing (HPC): Hier werden parallelisierte Programme eingesetzt, um komplexe Berechnungen auf Supercomputern oder Clustern auszuführen.
     - Datenverarbeitung: Parallelisierte Programme können große Datenmengen schneller verarbeiten und analysieren.
     - Grafikverarbeitung: Parallelisierte Programme können auf mehrere Grafikprozessoren verteilt werden, um eine schnelle Bild- und Videobearbeitung zu ermöglichen.
   - Beispiele für parallelisierte Programme sind:
     - Ein Webserver, der mehrere Anfragen gleichzeitig bearbeitet
     - Eine Bildverarbeitungssoftware, die Filter auf mehrere Bilder gleichzeitig anwenden kann
     - Eine Simulation, die mehrere Szenarien gleichzeitig berechnet

3. Welche Vor- und Nachteile ergeben sich aus der Parallelität von Programmen?
   - Vorteile der Parallelität von Programmen sind:
     - Schnellere Ausführungszeit: Wenn ein Programm parallelisiert wird, können mehrere Aufgaben gleichzeitig ausgeführt werden, wodurch die Gesamtausführungszeit reduziert wird.
     - Bessere Systemnutzung: Durch die Verteilung der Last auf mehrere Prozessoren oder Kerne wird die Auslastung des Systems verbessert und es wird mehr Ressourcen für andere Aufgaben freigegeben.
     - Skalierbarkeit: Parallelisierte Programme können einfacher auf größere Systeme und Cluster skaliert werden, um höhere Leistungsanforderungen zu erfüllen.
   - Nachteile der Parallelität von Programmen sind:
     - Komplexität: Das Design und die Entwicklung parallelisierter Programme sind oft komplexer und erfordern spezielle Kenntnisse.
     - Synchronisation: Bei der parallelen Ausführung müssen Daten und Ressourcen zwischen den Threads synchronisiert werden, was zu Problemen wie Deadlocks und Race Conditions führen kann.
     - Overhead: Die Koordination der Threads und die Synchronisation erzeugen einen zusätzlichen Overhead, der die Leistung beeinträchtigen kann.

## Verteilte Systeme

1. Was versteht man darunter?
   - Ein verteiltes System ist ein System, in dem mehrere autonome Computer miteinander kommunizieren, um gemeinsam eine Aufgabe zu erledigen. Es handelt sich dabei um eine Sammlung von Rechnern, die über ein Netzwerk miteinander verbunden sind und zusammenarbeiten, um eine bestimmte Aufgabe zu erfüllen.

2. Anwendungsbereiche und Beispiele?
   - Anwendungsbereiche für verteilte Systeme sind unter anderem:
     - E-Commerce und Online-Shops: verteilte Systeme können genutzt werden, um Bestellungen zu verarbeiten, den Warenbestand zu verwalten, und Zahlungen zu autorisieren.
     - Soziale Netzwerke: verteilte Systeme können genutzt werden, um die riesigen Datenmengen von sozialen Netzwerken zu verarbeiten.
     - Wissenschaftliche Anwendungen: verteilte Systeme können genutzt werden, um große Datenmengen zu verarbeiten und komplexe Berechnungen durchzuführen.
     - Cloud Computing: Cloud-Computing-Systeme sind verteilte Systeme, die Rechenressourcen bereitstellen, die von Kunden genutzt werden können.
     - IoT (Internet of Things): verteilte Systeme können genutzt werden, um IoT-Geräte miteinander zu verbinden und Daten zu verarbeiten.
   - Beispiele für verteilte Systeme sind:
     - Das Domain Name System (DNS) ist ein verteiltes System, das verwendet wird, um Domainnamen in IP-Adressen umzuwandeln.
     - BitTorrent ist ein verteiltes System, das zum Teilen von Dateien zwischen vielen Benutzern verwendet wird.
     - Das Google File System ist ein verteiltes Dateisystem, das von Google verwendet wird, um riesige Datenmengen zu speichern und zu verwalten.
     - Blockchain ist ein verteiltes System, das zur Speicherung und Verarbeitung von Transaktionen verwendet wird.

3. Welche Vor- und Nachteile ergeben sich aus der Verteilung von Programmen?
   - Vorteile der Verteilung von Programmen sind:
     - Skalierbarkeit: Verteilte Systeme können einfach erweitert werden, indem zusätzliche Computer hinzugefügt werden.
     - Zuverlässigkeit: Wenn ein Computer ausfällt, kann das verteilte System immer noch funktionieren.
     - Höhere Leistung: Verteilte Systeme können in der Regel schneller arbeiten als einzelne Computer, da die Arbeit auf viele Computer aufgeteilt wird.
     - Bessere Ressourcennutzung: Verteilte Systeme können Ressourcen wie Speicherplatz, Bandbreite und Rechenleistung besser nutzen.
   - Nachteile der Verteilung von Programmen sind:
     - Komplexität: Die Entwicklung von verteilten Systemen ist in der Regel komplexer als die Entwicklung von einzelnen Anwendungen.
     - Kommunikation: Die Kommunikation zwischen den Computern im verteilten System kann schwierig sein.
     - Sicherheit: Verteilte Systeme können anfälliger für Angriffe von außen sein.
     - Koordination: Die Koordination der Arbeit auf vielen Computern kann schwierig sein.

## Prozesse und Threads in der Programmierung

1. Was versteht man unter einem Prozess?
   - Ein Prozess ist ein Programm in Ausführung. Es ist eine isolierte Instanz, die Speicher und Ressourcen wie CPU-Zeit, Arbeitsspeicher und Dateien verwendet. Jeder Prozess wird durch seinen eigenen Adressraum und Kontext gekennzeichnet. Ein Betriebssystem kann mehrere Prozesse ausführen, die auf Ressourcen zugreifen und miteinander kommunizieren können.
2. Welche Eigenschaften hat ein Prozess?
   - Ein Prozess hat einen eigenen Adressraum, der ihm von einem Betriebssystem zugewiesen wird.
   - Ein Prozess kann mehrere Threads haben.
   - Ein Prozess kann auf Dateien, Netzwerkverbindungen und andere Systemressourcen zugreifen.
   - Ein Prozess hat mindestens einen Thread, der den Code des Programms ausführt.
   - Ein Prozess ist eine unabhängige Einheit und wird durch einen eigenen Prozess-Identifikator (PID) identifiziert.
3. Was versteht man unter einem Thread?
   - Ein Thread ist ein kleinerer Teil eines Prozesses und wird auch als leichte Einheit bezeichnet. Es handelt sich um eine sequenzielle Ausführungssequenz innerhalb eines Prozesses, die Ressourcen wie Speicher, Dateien und Netzwerkverbindungen gemeinsam mit anderen Threads des Prozesses teilt. Jeder Thread verfügt über einen eigenen Stack und kann auf dieselben Variablen und Daten zugreifen.
   - Einige Eigenschaften eines Threads sind:
     - Ein Thread teilt denselben Adressraum wie andere Threads desselben Prozesses.
     - Ein Thread kann gleichzeitig mit anderen Threads desselben Prozesses ausgeführt werden.
     - Ein Thread kann auf dieselben Ressourcen wie andere Threads desselben Prozesses zugreifen.
     - Ein Thread wird von einem eigenen Thread-Identifikator (TID) identifiziert.
4. Zusammenhang/Unterscheidung von Prozess und Thread?
   - Der Hauptunterschied zwischen einem Prozess und einem Thread besteht darin, dass ein Prozess eine unabhängige Einheit ist, während ein Thread innerhalb eines Prozesses existiert und Ressourcen mit anderen Threads des Prozesses teilt. Ein Prozess kann mehrere Threads haben, die gleichzeitig ausgeführt werden können, um die Leistung des Systems zu verbessern. Threads bieten die Möglichkeit, asynchrone Operationen durchzuführen, ohne die Ausführung des gesamten Programms zu blockieren.

## Multithreading

1. Was versteht man darunter?
   - Multithreading bezieht sich auf die Fähigkeit eines Computerprogramms, mehrere Threads oder Ausführungsfäden innerhalb desselben Prozesses gleichzeitig auszuführen. Ein Thread ist eine ausführbare Einheit, die einem Prozessor eine bestimmte Aufgabe zuweist. Multithreading ermöglicht es einem Programm, mehrere Aufgaben gleichzeitig auszuführen, anstatt sie sequentiell auszuführen.
2. Welche Vor- und Nachteile ergeben sich bei der Verwendung von Multithreading?
   - Vorteile von Multithreading
     - Verbesserte Leistung: Multithreading kann die Leistung eines Programms verbessern, indem es mehrere Threads parallel ausführt und somit die CPU-Auslastung optimiert.
     - Bessere Benutzererfahrung: Durch die Verwendung von Multithreading kann ein Programm auf Benutzerinteraktionen reagieren, ohne dass die Ausführung des Programms gestoppt wird.
     - Bessere Ressourcennutzung: Durch die Verwendung von Multithreading kann ein Programm die verfügbaren Ressourcen effektiver nutzen, z. B. indem es Daten schneller verarbeitet oder schneller auf Netzwerkverbindungen reagiert.
   - Nachteile von Multithreading
     - Komplexität: Multithreading kann die Komplexität eines Programms erhöhen, da es schwieriger wird, die Reihenfolge der ausgeführten Threads zu verwalten und sicherzustellen, dass sie sich nicht gegenseitig beeinträchtigen.
     - Synchronisationsprobleme: Wenn mehrere Threads auf gemeinsame Ressourcen zugreifen, besteht die Möglichkeit von Synchronisationsproblemen, die dazu führen können, dass das Programm fehlerhaft oder instabil wird.
     - Schwierige Fehlerbehebung: Es kann schwieriger sein, Fehler in einem Multithread-Programm zu diagnostizieren und zu beheben, da die Fehler möglicherweise nicht konsistent reproduzierbar sind und in verschiedenen Teilen des Codes auftreten können.
