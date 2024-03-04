# quickTools

#### VORWORT:
In dieser HTML-Seite werden verschiedene Tools angeboten, welche im Arbeitsalltag helfen möchten.
Zudem ist das Erstellen des Codes für mich eine Übung gewesen.
Der gesamte Code soll nur eine einzige Datei umfassen und muss daher eine hohe Qulität haben.
Also eine gute Struktur, sprechende Namen, effizenter und lesbarer Code, hilfreiche Kommentare.

		
#### TOOLS ÜBERSICHT:
- **Projekt Timer**:	Zwei Stoppuhren, eine für die gesamte Zeit und eine die man zurück setzten kann
- **Memory Note**:		Notizen die mit einer Erinnerung verknüpft werden können 
- **Commit Message**:	Formular zum Erstellen und Formatieren von Commits und Hilfe um die strengen Regeln einzuhalten
- **Commit History**:	Eine Liste der letzten Commits, eine Erweiterung zu den Commit Messages. Füllt sich automatisch
- **Calendar Note**:	Zeigt die aktuelle Arbeitswoche und ermöglicht zu jedem Tag eine kurze Notiz
- **Clipboard**:		Speichert kleine Texte und kopiert diese per Klick in die Zwischenablage
- **Collection List**:  Anlegen von Gruppen mit je mehreren kurzen Einträgen die verschiedene Eigenschaften haben können  



#### ANLEITUNG:
**Project Timer**  
Dieses Tool bietet für jeden Eintrag zwei Stoppuhren: Eine misst die gesamte Zeit, während die andere sich zurücksetzen lässt. Jeder Timer kann mit einem Namen versehen werden – sei es ein beliebiger Text, eine Ticketnummer oder eine spezifische Aufgabe.
- Mit [Go] starten beide Timer gleichzeitig, mit [Stop] werden beide angehalten.
- Über das Dropdown-Menü lässt sich eine Priorität für jeden Eintrag festlegen, wobei 1 die niedrigste und 4 die höchste Priorität bedeutet.
- Die Einträge können nach Erstellungsdatum oder Priorität sortiert werden.
- Um den Text eines Eintrags zu ändern, genügt ein Doppelklick darauf. Es erscheint ein Eingabefeld, in dem der neue Text eingegeben werden kann. Mit der Enter-Taste wird der neue Inhalt gespeichert. Verliert das Eingabefeld den Fokus, ohne dass Enter gedrückt wurde, wird die Bearbeitung abgebrochen.
- Mit [Delete] wird der Eintrag gelöscht.
  
---

**Memory Note**  
Dieses Tool bietet die Möglichkeit Notizen (zum Beispiel zu einem Projekt) zu erstellen. Jede Notiz hat einen Titel und einen Text. Zudem kann eine Erinnerung gesetzt werden, die sobald sie abgelaufen ist, den Text des Titels rot einfärbt. Auch der Rand dieses Tools wird rot.
- Mit [Add Note] wird eine neue Notiz erstellt, mit [Delete] neben dem Titel wird die Notiz gelöscht.
- Mit einem Doppelklick auf den Titel oder den Text öffnet sich ein Eingabefeld, in dem der neue Text eingegeben werden kann. Mit der Enter-Taste wird der neue Inhalt gespeichert. Verliert das Eingabefeld den Fokus, ohne dass Enter gedrückt wurde, wird die Bearbeitung abgebrochen.
- Mit einem Klick auf [Add Memo] kann eine Erinnerung gesetzt werden. Mit einem Klick auf [X] neben der Memo wird die Erinnerung gelöscht.

---

**Commit Message**  
Dieses Tool hilft bei der Erstellung von Commits, indem es die Einhaltung von Regeln unterstützt und die Message korrekt formatiert. Mit einem Klick kann die Message in die Zwischenablage kopiert werden. Zudem gibt es eine Hilfe, bei der Übersetzung vom Deutschen ins Englische (nur mit Internetverbindung).
- Typ: Wähle aus, ob es sich um ein Feature, ein Fix, eine Dokumentation oder eine andere Änderung handelt.
- Domain: Der Gültigkeitsbereich, zum Beispiel der Name der bearbeiteten Komponente, ist optional.
- Short Description: Eine kurze Beschreibung der Änderung, die in der Commit-Liste angezeigt wird. Sie darf maximal 72 Zeichen lang sein und muss mit einem Kleinbuchstaben beginnen. Zudem sollte sie im Präsens verfasst sein.
- Description: Eine ausführliche Beschreibung der Änderung, welche die Motivation für die Veränderung und die Auswirkungen beschreibt.
- Footer: Hier können zusätzliche Informationen wie Referenzen oder Schließungen von Tickets eingetragen werden. Mit /ready wird das Ticket als bereit zur Überprüfung markiert.

---

**Commit History**  
Sobald ein Commit in die Zwischenablage kopiert wird, wird er der History hinzugefügt.
Es werden die letzten 10 Commits gespeichert, mit ihren Namen, dem Datum und der Zeit.
- Mit [X] wird der Eintrag gelöscht.
- Es können die letzten 3, 5 oder 10 Commits angezeigt werden.

---

**Calendar Note**  
Mit diesem Tool lassen sich kurze Notizen zu jedem Tag erstellen. Der Kalender zeigt die aktuelle Arbeitswoche an, der aktuelle Tag wird farblich markiert. Es kann genutzt werden um die wichtigsten Gedanken des Tages zu notieren, um sich später besser an die vergangene Woche zu erinnern.
- Mit [Last] und [Next] kann zwischen den Wochen gewechselt werden.
- Der Button dazwischen zeigt die aktuelle Woche und das Jahr an. Mit einem Klick auf das Kalender-Icon öffnet sich ein Datepicker, mit dem das Datum direkt ausgewählt werden kann.
- Mit einem Doppelklick auf den Text unter dem Datum öffnet sich ein Eingabefeld, in dem die Notiz eingegeben werden kann. Mit [Save] wird die Notiz gespeichert, mit [Cancel] wird der Vorgang abgebrochen.  

Issues: In Firefox wird das Datum nicht korrekt angezeigt. Das liegt daran, dass Firefox das `type="date"` nicht unterstützt. 

---

**Clipboard**  
Dieses Tool bietet die Möglichkeit, mehrere kurze Texte zu speichern und per Klick in die Zwischenablage zu kopieren. Das eignet sich beispielsweise, um häufig verwendete Texte wie URLs, Ticketnummern oder Befehle zu speichern und schnell in andere Anwendungen zu kopieren.
- Mit [Add Snippet] wird ein neuer Eintrag erstellt, mit [Delete] neben dem Eintrag wird dieser gelöscht.
- Mit [Copy] wird der Text in die Zwischenablage kopiert.
- Mit einem Doppelklick auf den Text öffnet sich ein Eingabefeld, in dem der neue Text eingegeben werden kann. Mit der Enter-Taste wird der neue Inhalt gespeichert. Verliert das Eingabefeld den Fokus, ohne dass Enter gedrückt wurde, wird die Bearbeitung abgebrochen.

---

**Collection List**  
Dieses Tool bietet die Möglichkeit, mehrere Gruppen anzulegen, die jeweils mehrere Einträge enthalten können. Jeder Eintrag kann mit einem Namen versehen werden, der in der Liste angezeigt wird, Zudem können Einträge aktiv oder inaktiv sein. Das eignet sich beispielsweise, um eine Liste von Aufgaben zu erstellen, die abgearbeitet werden müssen, oder regelmäßig wiederkehrende Tätigkeiten zu verwalten.
- Mit [Add List] wird eine neue Gruppe erstellt, mit [Delete List] neben dem Gruppennamen wird die Gruppe gelöscht.
- Mit [Add Entry] neben dem Gruppennamen wird ein Eintrag erstellt, mit [X] neben dem Eintrag wird dieser gelöscht.
- Linksklicks auf die Einträge toggeln diese von aktiv zu durchgestrichen und umgekehrt.
- Linksklicks auf die Gruppennamen klappen diese auf oder zu.
- Rechtsklick auf einen Eintrag in der Liste löscht diesen.
- Doppelklick auf einen Eintrag in der Liste oder dem Gruppennamen öffnet ein Eingabefeld, in dem der neue Name eingegeben werden kann. Mit der Enter-Taste wird der neue Inhalt gespeichert. Verliert das Eingabefeld den Fokus, ohne dass Enter gedrückt wurde, wird die Bearbeitung abgebrochen.