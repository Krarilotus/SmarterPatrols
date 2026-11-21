# Smarter Patrols

**Autor**: Monsterfish
**Version**: 1.0.1

Sorgt dafür, dass die Patrouillen- und Belagerungsschutztruppen der KI bei einem Angriff tatsächlich alle ihre Gruppen nutzen. Beide Bereiche lassen sich in den Einstellungen getrennt deaktivieren.

## Angriffspatrouillen

Im Originalspiel erhält nur die erste Patrouillengruppe jemals Befehle. Die zweite bleibt den gesamten Angriff über am Sammelpunkt stehen.

Mit diesem Modul bekommt jede Patrouillengruppe eine eigene Route rund um die angegriffene Burg:

- **Gruppe 1** umkreist die Burg in einer Richtung.
- **Gruppe 2** umkreist sie in der Gegenrichtung.
- **Gruppe 3** läuft an der Vorderseite der Burg (der dem Angreifer zugewandten Seite) hin und her.
- **Gruppen 4, 5, 6** machen dasselbe wie 1, 2 und 3, jedoch um eine Viertelrunde dahinter versetzt. Die Gruppen 7, 8, 9 folgen wiederum dahinter und so weiter.

Sie laufen in einem festgelegten Laufabstand außerhalb der Burg (standardmäßig 12 Felder, wie die spielinterne Patrouille), sodass sie Mauern und Burggräben umlaufen, statt hineinzulaufen. Trifft eine Gruppe auf Feinde, kämpft sie zuerst und zieht danach weiter.

## Belagerungsschutz

Diese Truppen laufen zwar bereits von einem Belagerungsgerät zum nächsten, aber beide Gruppen folgen gleichzeitig derselben Route und wirken daher wie eine einzige Gruppe.

Mit diesem Modul:

- startet jede Gruppe an einem anderen Belagerungsgerät, und jede zweite Gruppe läuft in die Gegenrichtung, sodass alle Geräte abgedeckt werden;
- laufen Gruppen, die überwiegend aus Nahkämpfern bestehen, einige Felder vor den Belagerungsgeräten (Richtung Burg), damit die Verteidiger auf sie statt auf die Geräte feuern – Bogenschützen bleiben bei den Geräten;
- greifen alle Gruppen wie im Originalspiel mit an, sobald der Sturm auf die Mauern beginnt.

## Mehr Gruppen

Das Spiel kann von Haus aus nur 2 Patrouillen- und 2 Belagerungsschutzgruppen verwalten. Verlangt eine KI-Datei mehr, landen die zusätzlichen Einheiten in falschen Truppen (Grabenausheber oder Hauptarmee). Dieses Modul erlaubt bis zu 12 Gruppen je Art. Die Anzahl stammt aus der KI-Datei, sofern du in den Einstellungen keinen eigenen Wert vorgibst (Belagerungsschutz: standardmäßig 4). Eine Truppe wird nur so weit geteilt, dass jede Gruppe noch mindestens 4 Einheiten behält (einstellbar).

Die zusätzlichen Gruppen bestehen nur während des laufenden Angriffs. Sobald eine Bresche geschlagen ist, der Lord fällt oder sich die KI zurückzieht, schließen sie sich wieder dem Rest an und folgen den normalen KI-Befehlen.

## Gut zu wissen

- Betrifft nur Angriffe der KI; deine eigenen Truppen bleiben unverändert.
- Funktioniert zusammen mit Lord Hunt.
- In Spielständen wird nichts zusätzlich gespeichert.
