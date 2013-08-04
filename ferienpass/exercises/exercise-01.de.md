# Übung 1

Diese Übung enthält folgende Punkte:

* Erster Kontakt mit Ruby
* Kommandozeile
* IRB (Interactive Ruby Shell)

## Erster Kontakt mit Ruby

Ruby (die Programmiersprache) lebt in deinem Computer.
Die meisten Menschen kommunizieren mit einem Computer
indem sie mit der Maus auf Icons,
Bilder oder Schaltflächen klicken um ihm mitzuteilen,
was als nächstes geschehen soll.

Damit wir mit Ruby kommunizieren können,
müssen wir ihr mit unserer Tastatur sagen,
was wir von ihr wollen.

Dazu benötigen wir ein Programm, welches Kommandozeile oder Terminal genannt wird.

## Kommandozeile

Um die Kommandozeile auf deinem Computer zu öffnen, befolge die Anweisungen für das Betriebssystem deines Computers:

* **OSX**: Öffne das Programm **Terminal**
* **Windows**: Klicke auf **Start** --> Klicke auf **Ausführen...** --> Schreibe **cmd** und drücke die Eingabetaste
* **Linux**: Öffne das Programm **Terminal**

Du befindest dich nun in der Kommandozeile.

Die Kommandozeile unterscheidet sich nicht gross von dem was du bereits
sonst schon so vom Umgang mit deinem Computer kennst.

Der einzige Unterschied ist, dass die Kommandozeile keine Bilder anzeigen kann und anstelle der Maus und per Mausklick, du mit ihr über die Tastatur mittels Wörter kommunizieren musst.

Wie mit der Maus, kannst du dich auch in der Kommandozeile zwischen den verschiedenen Ordnern hin und her bewegen.

Um das ganze ein wenig zu verdeutlichen, machen wir doch am besten gleich ein gemeinsames Beispiel.
Falls du bereits schon einmal einen Computer bedient hast, kennst du sicher die Oberfläche mit dem Hintergrundbild auf dem Ordner und Dateien herumliegen, welche du dann mit der Maus öffnen kannst.
Dies ist nichts weiter als ein Ordner in der Kommandozeile, welcher **Desktop** genannt wird. Wenn wir mit der Kommandozeile in diesen Ordner wechseln möchten, führen wir den Befehl **cd** (change directory) aus:

> Den Befehl ausführen bedeutet nichts anderes, als die folgenden grau markierten Wörter in die Kommandozeile einzutippen und danach mit der Eingabetaste zu bestätigen.

* Windows: `cd ~\Desktop`
* OSX und Linux: `cd ~/Desktop`

Super! Du befindest dich nun auf dem **Desktop** mit der Kommandozeile.

Nun hast du sicher ein paar Dateien auf deinem Desktop liegen. Die Kommandozeile kann dir diese Dateien mit folgendem Befehl anzeigen:

* Windows: `dir`
* OSX und Linux: `ls`

Die Kommandozeile zeigt dir nun die Namen der verschiedenen Ordner und Dateien auf dem Desktop an.

> Zeigt dir die Kommandozeile keine Datei- und Ordnernamen an? Befindest du dich auf dem Desktop? Hast du überhaupt Dateien und Ordner auf dem Desktop? Falls nicht, erstelle ein paar Beispieldateien und wiederhole den oberen Befehl.

Nun weisst du sicher schon, dass man mit der Maus per Rechtsklick einen neuen Ordner erstellen kannst oder?

Die Kommandozeile kann auch neue Ordner erstellen. Führe den folgenden Befehl aus:

    mkdir Mein-Erster-Ordner

Nun werfe einen Blick auf deinen Desktop. Siehst du das? Dort befindet sich der Ordner **Mein-Erster-Ordner** den du gerade erstellt hast. Cool nicht?

Du kannst jetzt mittels Kommandozeile in den neuen Ordner wechseln: `cd Mein-Erster-Ordner` und dort einen weiteren Ordner erstellen: `mkdir Mein-Zweiter-Ordner`.

Sobald du dies gemacht hast kannst du dir den Ordner auf der Kommandozeile mit dem Befehl `ls` anzeigen lassen.

Bist du dir nicht sicher in welchem Ordner du dich mit der Kommandozeile befindest? Der Befehl `pwd` zeigt dir den aktuellen Standort der Kommandozeile an.

Mit dem Befehl `cd` kannst du vom Ordner **Mein-Erster-Ordner** auch wieder in den Ordner **Desktop** zurück wechseln. Führe folgenden Befehle dazu aus:

    cd ..

Die zwei Punkte **..** sagen der Kommandozeile sie soll einen Ordner weiter nach oben gehen. Da sich der Ordner **Mein-Erster-Ordner** im Ordner **Desktop** befindet, wechselst du somit zum Ordner **Desktop**.

Damit hätten wir unseren ersten Schritt in der Kommandozeile erfolgreich abgeschlossen. Die Kommandozeile beherscht noch eine Vielzahl an weiteren Befehlen, die sie für dich ausführen kann.
Du brauchst längst nicht alle zu kennen, falls du willst, findest du hier noch weitere [Linux](http://www.lugs.ch/lib/doc/befehle.phtml) oder [Windows](http://www.script-example.com/themen/cmd_Batch_Befehle.php) Befehle, welche du dir beibringen kannst.

Im nächsten Schritt kommunizieren wir erstmals mit Ruby und werfen einen kleinen Blick darauf was sie so alles Grundlegendes für dich machen kann.

> Falls du das ganze hier noch nicht so richtig verstanden hast, brauchst du dir keine Sorgen zu machen.
> Dies geht den meisten so beim ersten mal.
> Wichtig ist einfach, dass du diese ersten Schritte einmal gemacht hast und dich nicht davon abschrecken lässt.
> Je länger du dich damit beschäftigst, desto verständlicher wird das ganze.

## IRB

IRB ist die Abkürzung für **Interactive Ruby Shell**.

Dies ist ein Befehl, welcher durch die Installation von Ruby der Kommandozeile zur Verfügung gestellt wird.

Wir können IRB auf der Kommandozeile wie folgt aufrufen:

    irb

Danach sollte uns die Kommandzeile eine ähnliche Antwort, wie die folgende geben:

    $ irb
    irb(main):001:0>

Dies bedeutet, dass wir nun IRB gestartet haben und Ruby direkt Befehle erteilen können.

Probiere folgende Befehle aus:

* `1 + 100`
* `1 - 100`
* `10 / 2`
* `2 * 5`
* `"Hallo" + "Ruby"`
* `"Hallo Ruby".reverse`
* `5.times { puts "Hello Ruby" }`
