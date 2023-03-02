# Fragen zum Thema Code "Smells"

Von Klemens Gassner

„Bei der Herstellung dieses Textes [oder wahlweise Bildes oder des Programmiercodes etc.] wurde ChatGPT eingesetzt. Mit folgenden Prompts habe ich die KI gesteuert: "1. Parallelität bei Programmen
Was versteht man darunter?
Anwendungsbereiche und Beispiele?
Welche Vor- und Nachteile ergeben sich aus der Parallelität von Programmen., 2. Verteilte Systeme?
Was versteht man darunter?
Anwendungsbereiche und Beispiele?
Welche Vor- und Nachteile ergeben sich aus der Verteilung von Programmen., 3. Was versteht man unter einem Prozess?
Welche Eigenschaften hat ein Prozess?
Was versteht man unter einem Thread?
Zusammenhang/Unterscheidung von Prozess und Thread?, 4. Was versteht man unter Multithreading und was sind desen Vor und Nachteile?“1. Duplicate Code:
Vermeiden Sie doppelten Code, indem Sie eine Funktion oder eine Klasse erstellen und den Code darin wiederverwenden. Eine andere Möglichkeit ist die Verwendung von Vererbung, um gemeinsame Funktionalitäten in einer Basis-Klasse zu definieren und diese in abgeleiteten Klassen zu erweitern.


## 1. Parallelität bei Programmen

1. Wie können die folgenden typischen "Fehler" beim Programmieren vermieden werden (Code Smells)
   - Long Methods:
Aufteilen von langen Methoden in kleinere, wiederverwendbare Funktionen. Stellen Sie sicher, dass jede Funktion nur eine einzige Aufgabe hat und gut benannt ist.

   - Large Classes:
Versuchen Sie, eine Klasse auf eine einzige Verantwortlichkeit zu beschränken und delegieren Sie andere Aufgaben an andere Klassen. Vermeiden Sie auch die Verwendung von globalen Variablen oder Funktionen, die sich auf viele verschiedene Klassen auswirken.

   - Shotgun surgery:
Konsolidieren Sie Code, der in vielen verschiedenen Klassen oder Methoden dupliziert ist, in einer einzigen Stelle. Wenn Sie Änderungen an dieser Funktion vornehmen, müssen Sie nur an einer einzigen Stelle Änderungen vornehmen, anstatt an vielen verschiedenen Stellen.

   - Feature envy:
Wenn eine Methode in einer Klasse mehr Zeit damit verbringt, auf die Daten einer anderen Klasse zuzugreifen, sollten Sie wahrscheinlich die Funktionalität in die entsprechende Klasse verschieben. Stellen Sie sicher, dass jede Klasse ihre eigenen Daten verarbeitet und so wenig wie möglich von anderen Klassen abhängt.

2. Was versteht man unter den folgenden Ausdrücken im Zusammenhang mit Code smells (Nennen Beispiele hierfür)
   
   - Object-Orientation Abusers:
Diese Code Smells treten auf, wenn Entwickler grundlegende Prinzipien der objektorientierten Programmierung (OOP) missachten. Beispiele hierfür sind Klassen, die zu viele Verantwortlichkeiten haben (z.B. eine Klasse, die sowohl für die Verarbeitung von Daten als auch für die Darstellung von Benutzeroberflächen zuständig ist), oder die Verwendung von Vererbung, wo dies nicht angebracht ist. OOP-Abuser-Smells führen dazu, dass der Code schwer zu verstehen, zu testen und zu warten ist.
Beispiel: Eine Klasse, die sowohl für die Verarbeitung von Daten als auch für die Erstellung von Benutzeroberflächen zuständig ist. In diesem Fall sollte die Klasse aufgeteilt werden, um nur eine Verantwortlichkeit zu haben.

   - Change Preventers:
Diese Code Smells treten auf, wenn der Code so geschrieben ist, dass er Änderungen verhindert oder erschwert. Beispiele hierfür sind hartcodierte Werte, die an vielen Stellen im Code verwendet werden, oder das Festlegen von Funktionalitäten in Beton gegossenen Strukturen, die schwer zu ändern sind. Änderungsverhindernde Code-Smells führen dazu, dass der Code schwer zu warten und zu aktualisieren ist.
Beispiel: Ein hartcodierter Dateipfad, der an vielen Stellen im Code verwendet wird. Wenn der Pfad geändert werden muss, muss der Code an vielen verschiedenen Stellen aktualisiert werden.

   - Dispensables:
Diese Code Smells treten auf, wenn der Code unnötig ist oder nicht ausgeführt wird. Beispiele hierfür sind tote oder unbenutzte Codeabschnitte, redundante Funktionen oder ungenutzte Variablen. Entfernung von unnötigem Code kann die Lesbarkeit und Wartbarkeit verbessern.
Beispiel: Eine Funktion, die im Code definiert ist, aber nicht aufgerufen wird. Diese Funktion sollte entfernt werden, um den Code übersichtlicher zu gestalten.

   - Couplers:
Diese Code Smells treten auf, wenn die Abhängigkeiten zwischen verschiedenen Teilen des Codes zu eng sind. Beispiele hierfür sind globale Variablen, die von vielen verschiedenen Klassen verwendet werden, oder enge Kopplung zwischen Klassen, die dazu führen, dass Änderungen an einer Klasse Auswirkungen auf viele andere Klassen haben. Gute Softwareentwicklung sollte eine lose Kopplung zwischen verschiedenen Teilen des Codes fördern.
Beispiel: Eine Klasse, die eine globale Variable verwendet, die von vielen anderen Klassen im Code verwendet wird. Die Verwendung von globalen Variablen sollte vermieden werden, um den Code besser zu strukturieren und zu isolieren.

## 2. Why Software Architectur matters?

1. Welche Anforderungen werden von unterschiedlicher Seite an die SW gestellt?