# OneFileTools

#### VORWORT:
In dieser HTML-Seite werden verschiedene Tools angeboten, welche im Arbeitsalltag helfen möchten.
Zudem ist das Erstellen des Codes für mich eine Übung gewesen.
Der gesamte Code soll nur eine einzige Datei umfassen und muss daher eine hohe Qulität haben.
Also eine gute Struktur, sprechende Namen, effizenter und lesbarer Code, hilfreiche Kommentare.

#### TOOLS SIND MODULE:
Die verschiedenen Tools sind als eigenständige Module zu sehen. 
Jedes Tool hat einen eigenen CSS-Block, HTML-Block und einen SCRIPT-Block. 
Zudem gibt es die Globalen Blöcke mit allgemeinen Layouts oder Verhaltenweisen wie EventListener.
Die einzelnen Tools lassen sich per Button im Header ein- und ausblenden.
Wichtig dabei ist die Namensgebung: der Toolname + Btn für die id des Buttons
Der dazu gehörende div-Kontainer hat die id des Toolnamen (gleiches Wort wie beim Button)
Dann kann die beim Klick ausgeköste Funktion mit dem Toolnamen als Parameter die Sichtbarkeit des Tools ändern  

#### TOOLTIPS:
Obwohl das UI der Seite englisch sein sollte, sind die Tooltipps auf deutsch. Ich mag verständliche Anleitungen.
Jede Überschrift eines Tools hat einen (?) Button, der beim Hovern eine Anleitung zum Tool zeigt.
Dieser div-Kontainer einhält ein span-Element welcher die gleiche id haben muss wie die Variable inder sein Text gespeichert ist.
Durch verschiedene CSS Klassen und einer Funktion die beim Start ausgeführt wird, werden die Tooltipps erstellt.
Im Gegensatz zum HTML-Attribut ``<titel>`` erscheint der Text sofort und ist optisch anpassbar.
		
#### TOOLS ÜBERSICHT:
- Projekt Timer:	Zwei Stoppuhren, eine für die gesamte Zeit und eine die man zurück setzten kann
- Projekt Note:		Notizen zu einem Projekt wie eine Aufgabenliste, eine Erweiterung zum Projekt Timer 
- Commit Message:	Formular zum Erstellen und Formatieren von Commits und Hilfe um die strengen Regeln einzuhalten
- Commit History:	Eine Liste der letzten Commits, eine Erweiterung zu den Commit Messages. Füllt sich automatisch
- Calenadar Note:	Zeigt die aktuelle Arbeitswoche und ermöglicht zu jedem Tag eine kurze Notiz
- Clipboard:		Speichert kleine Texte und kopiert diese per Klick in die Zwischenablage
	
#### SPEICHERORT:
Die Werte der Tools werden im LocalStorage des Browsers gespeichert.   
Projekt Timer speichert den Namen des Projektes, seine id, seine Prio, die gemessenen Zeiten und sein Erstellungsdatum in "saveProjectTime"
Projekt Note speichert seinen Text und seine id (gleiche id wie die des Projekt Timers) in "saveProjectNote"
Commit History speichert seinen Namen (Commit Message aus dem Formular) Datum und Zeit seines Erstellens in "saveCommit"
Calendar Note speichert seinen Text und das Datum zudem die Notiz gehört in "saveCalendarNote"
Clipboard speichert seinen Namen und den Text welcher im Zwischenspeicher kopiert werden soll in "saveSnippet"