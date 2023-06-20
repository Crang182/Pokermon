# Pokermon
Must do!
Pillow Package muss in Visual Studio Code installiert sein

1.	Beschreibung des Programms
Das Programm Pokermon startet mit der Auswahl zweier Pokermon, von denen man sich über die eingefügten Infobuttons in der Terminausgabe anzeigen lassen kann welche Fähigkeiten und Attribute diesen Pokermons zugewiesen sind. Aufgrund dieser Attribute soll der Spieler per Mausklick auf das entsprechende Pokermon entscheiden welches er gerne spielen möchte.
Im zweiten Grundkonstrukt des Spiels wird der Spieler in die Kampfsituation befördert, welche sich aus der Anzeige beider Pokermons, der HP-Balken (Grün = eigene HP, Gelb = Gegner HP) und der Buttons für die unterschiedlichen Attacken zusammensetzt. Sobald einer der Buttons gedrückt wird erfolgt je nach Fähigkeit eine Animation der Pokermons, die Lebensbalken verändern sich und es kommt zu einer kurzen Deklarierung des geschehenen über die Terminalausgabe.
Das Spiel endet, sobald man es schafft, die Gegnerischen HP auf 0 oder niedriger zu bringen, oder die eigenen HP auf 0 bzw. darunterfallen. Sieg oder Niederlage wird in einem neu erscheinenden Fenster definiert, infolgedessen können die Fenster geschlossen werden.

2.	Aufbau des Programms
Das eigentliche Programm beginnt mit der Deklarierung der Klassen und deren Vererbungen, dazu wurde im Konstruktor der Elternklasse (Pokermon) zum einen alle Attribute genannt, welche alle Pokermons benötigen: Name, HP, Type, Attacken Info 1, Attacken Info 2, des Weiteren wurde auch die Methode infos_ausgeben deklariert, da diese ebenfalls alle Pokermons benötigen. Die Spezifizierung der Attacken erfolgt daraufhin in den Kindklassen der Pokermons, da diese sich je Pokermon unterscheiden.
Zur Visuellen Darstellung des Programms wurde tk-inter bzw. ttk verwendet, welches sich durch die Darstellung in Buttons und die schnelle Aneignung außerhalb des Kurses anbietet.
Die Kampfszenarien finden eigens in definierten Methoden statt, um der Syntax von tk-inter gerecht zu werden.

3.	Nutzung des Programms
Das gesamte Programm lässt sich durch die Möglichkeiten von tk-inter über die Maus bedienen und bedarf keinerlei Eingaben über das Keyboard. Alle Befehle können über die Buttons interpretiert werden.
