# Was ist NoSQL?

Die Bezeichnung NoSQL ist als Oberbegriff für einen nicht relationalen Ansatz zu verstehen. Anders als in einer klassischen relationalen Datenbank exisitert kein Tabellenschemata. Weitere Charakteristika einer NoSQL Datenbank bestehen darin, dass es vermieden wird Daten per "join" zusammenzuführen und die Datenbank selber horizontal skaliert wird. [www.datenbanken-verstehen.de/lexikon/nosql/]

Unter einer horizontalen Skalierbarkeit einer Datenbank ist zu verstehen, dass ein Gesamtsystem auf mehrere Server verteilt wird und durch das Hinzufügen weiterer Server erweitert werden kann. Dabei besteht kein Zwang, dass ein einzelner Server ausfallsicher ist, da das Gesamtsystem eine sehr hohe Ausfalltoleranz mit sich bringt. Auch bei einem Ausfall eines Serverknotens gehen, aufgrund der redundant gespeicherten Daten auf allen Servern, keine Daten verloren. Weiterhin ist eine sehr hohe Verfügbarkeit des Gesamtsystems gegeben, da die Leistungsfähigkeit mit jedem zusätzlichem Server steigt. Anders wird dies mit relationalen Datenbanken gehandhabt. Hier wird die Leistungsfähigkeit eines einzelnen Servers üblicherweise durch das Aufrüsten der vorhandenen Hardware erhöht. Je nach System können hier natürlich auch Grenzen erreicht werden, welche nur durch einen Austausch des gesamten Servers umgangen werden können. Somit kann der neue Server weiter in Zukunft den Anforderungen angepasst werden. Das verursacht unter Umständen nicht linear verlaufende Kosten, welche abhängig von der entsprechenden Hardware sind (Speicher, CPU, RAM ...). Auch die Ausfallsicherheit ist bei vertikal skalierten Systemen nicht annähernd so hoch wie bei horizontal skalierten Systemen. Hier kann schon das Aufrüsten eines Servers zu Ausfallzeiten führen.

http://wikis.gm.fh-koeln.de/wiki_db/Datenbanken/Skalierbarkeit

Anders als vermutlich gedacht, bedeutet die Bezeichnung NoSQL, dass auch SQL-Datenbanken eingesetzt werden. Demnach steht NoSQL für "Not only SQL". In den verschiedenen NoSQL Ausprägungen, welche im nächsten Unterkapitel weiter erläutert werden, ist auch zu erkennen, dass gemischte Datenbanken und auch Varianten ohne SQL Datenbanken unter dem Begriff NoSQL Bedeutung finden.

Durch die zuvor bereits erwähnte horizontale Lastenverteilung der Daten, bieten NoSQL Systeme eine sehr hohe Geschwindigkeit - je nach Einsatzweck kann das aber auch variieren. Aber auch hier kommt es auf den Anbieter einer NoSQL Datenbank an, wie die Daten skaliert oder abgefragt werden. Hierzu werden im späteren Verlauf dieses Kapitels einige Vertreter der verschiedenen Arten von NoSQL vorgestellt.

!!!CAP THEOREM erwähnen!!!

## Arten von NoSQL Datenbanken

Dokumentenorientierte Datenbanken

Graphendatenbanken

Key-Value-Datenbanken

## Vor- und Nachteile von NoSQL

Zu den großen Vorteilen von NoSQL Systemen gehört mit Sicherheit die gute Skalierbarkeit, um einen Verbund aus Datenbanken zu bilden. Als Stichwort sei hier die Bezeichnung "Big Data" zu nennen.

Auch der Open-Source Gedanke hinter NoSQL steht für sich alleine als Vorteile. Die Entwicklungen sowie Dokumentationen sind offen zugänglich und bieten somit unter anderem eine hohe Transparenz bei der Wahl eines geeigneten Anbieters.

Die genannten Vorteile bringen allerdings auch gleichzeitig Nachteile mit sich. Durch die horizontale Skalierbarkeit werden alle Daten Redundant gespeichert. Dies wirkt sich zwar auch positiv auf die Ausfallsichheit aus aber belegt somit auf jedem einzelnen Server entsprechend den verfügbaren Speicher. Wird diese Eigenschaft noch weiter betrachtet fällt auf, dass die Verfügbarkeit immer nur mit konsistenten Daten funktioniert oder geteilten Daten bei einem Kommunikationsausfall zwischen zwei oder mehreren Serverknoten eines Gesamtsystems. Die zuvor erwähnten Szenarien beschreiben dabei grob das CAP-Theorem.

![Schnittmengen des CAP-Theorems](/img/cap.png)



Die Schnitmengen der Kreise zeigen die zuvor beschriebene Problematik und geben einen Überblick über die möglichen Kombinationsmöglichkteiten.



http://www.se.uni-hannover.de/priv/lehre_2010sommer_wwwseminar/11-SQL_vs_NoSQL-Ausarbeitung.pdf



Bei Open Source Projekten im Allgemeinen muss darauf geachtet werden, dass die Dokumentationen vollständig und gepflegt gehalten werden. Ist das nicht der Fall, fehlen womöglich Informationen zur Nutzung oder Hinweise zum Beispiel zur Sicherheit eines Systems.

http://www.datenbanken-verstehen.de/lexikon/nosql/





 Vor- sowie Nachteil: Konsistenz und Redundanz

www.se.uni-hannover.de/priv/lehre_2010sommer_wwwseminar/11-SQL_vs_NoSQL-Ausarbeitung.pdf



## Populäre NoSQL Datenbanken

## Beispiele