# Pokermon
Must do!
Pillow Package muss in Visual Studio Code installiert werden.
Falls die Pfade nicht erkannt werden können, muss ggfs. der ganze Pfad im Code angegeben werden.

1.	Beschreibung des Programms
Das Programm Pokermon startet mit der Auswahl zweier Pokermon, von denen man sich über die eingefügten Infobuttons in der Terminausgabe anzeigen lassen kann welche Fähigkeiten und Attribute diesen Pokermons zugewiesen sind. Aufgrund dieser Attribute soll der Spieler per Mausklick auf das entsprechende Pokermon entscheiden welches er gerne spielen möchte.
Im zweiten Grundkonstrukt des Spiels wird der Spieler in die Kampfsituation befördert, welche sich aus der Anzeige beider Pokermons, der HP-Balken (Grün = eigene HP, Gelb = Gegner HP) und der Buttons für die unterschiedlichen Attacken zusammensetzt. Sobald einer der Buttons gedrückt wird erfolgt je nach Fähigkeit eine Animation der Pokermons, die Lebensbalken verändern sich und es kommt zu einer kurzen Textaugabe des geschehenen über die Terminalausgabe.
Das Spiel endet, sobald man es schafft, die Gegnerischen HP auf 0 oder niedriger zu bringen, oder die eigenen HP auf 0 bzw. darunterfallen. Sieg oder Niederlage wird in einem neu erscheinenden Fenster definiert, infolgedessen können die Fenster geschlossen werden.

2.	Aufbau des Programms
Das eigentliche Programm beginnt mit der Deklarierung der Klassen und deren Vererbungen, dazu wurde im Konstruktor der Elternklasse (Pokermon) zum einen alle Attribute genannt, welche alle Pokermons benötigen: Name, HP, Type, Attacken Info 1, Attacken Info 2, des Weiteren wurde auch die Methode „infos_ausgeben“ deklariert, da diese ebenfalls alle Pokermons benötigen. Die Spezifizierung der Attacken erfolgt daraufhin in den Kindklassen der Pokermons, da diese sich je Pokermon unterscheiden.
Zur Visuellen Darstellung des Programms wurde tk-inter bzw. ttk verwendet, welches sich durch die Darstellung in Buttons und die schnelle Aneignung außerhalb des Kurses anbietet.
Die Kampfszenarien finden eigens in definierten Methoden statt, um der Syntax von tk-inter gerecht zu werden.

3.	Nutzung des Programms
Um das Programm ausführen zu können muss die Pokermon.py Datei ausgeführt werden, da es sich dabei um die Main handelt. Das gesamte Programm lässt sich durch die Möglichkeiten von tk-inter über die Maus bedienen und bedarf keinerlei Eingaben über das Keyboard. Alle Befehle können über die Buttons interpretiert werden.

4.	Erweiterungsmöglichkeiten
4.1 Terminalausgabe
Die Ausgabe einiger Informationen, zb. Verlorene Lebenspunkte oder die Funktion „infos_ausgeben“, erfolgt über das Terminal. Um die Möglichkeiten von tk-inter vollends auszuschöpfen könnten diese Informationen ebenfalls im Spielfenster ausgegeben werden.

4.2 Weitere Pokermons
Eine weitere Möglichkeit der Erweiterung wäre zum einen das Einbinden mehrerer Auswahlpokermons und zum anderen das hinzufügen mehrerer Gegnerpokermons, um die Userexperience vielfältiger zu gestalten.

4.3 Attribute und Fähigkeiten der einzelnen Pokermons
Ebenfalls können den Pokermons weitere Fähigkeiten oder Attribute in Form von Funktionen hinzugefügt werden, welche beispielsweise einen Multiplikator innehaben, sobald ein Type Feuer gegen einen Type Pflanzenpokermon kämpft.

5.	Bugs
5.1 Buttons für Bilder der Pokermons verschwinden manchmal
In seltenen Fällen verschwinden die Buttons der Pokermons nach einer Animation, sobald man aber eine neue Animation anstößt tauchen diese wieder auf. Fehlerquelle leider unbekannt.

5.2 Glutkeks Animation
Bei der Fähigkeit des Pokermon wurde eingebaut, dass die Attacke „Pew“ erst einsetzbar ist und beginnt Rechnerische Operationen zum verändern der HP auszuführen, sobald das Pokermon sich unter 500 HP befindet, jedoch wird beim klicken der Fähigkeit die Animation ausgeführt, was leider im Rahmen des Projektes nicht lösbar war.

6.	Fazit
Durch die erlernten Fähigkeiten im Bereich der Objektorientierten Programmierung wird klar, dass die Skalierbarkeit des Projektes deutlich vereinfacht wird, sobald diese zum Tragen kommt. Das hinzufügen einzelner Klassen ist in wenigen Schritte Möglich und vereinfacht somit ebenfalls die Wiederverwendbarkeit von Code. Die selbsterlernten Fähigkeiten im Bereich von tk-inter waren ebenfalls ein großer Schritt, um erstmalig eine Visuelle Ausgabe außerhalb des Terminals vorweisen zu können 

Github Link:
https://github.com/Crang182/Pokermon.git
