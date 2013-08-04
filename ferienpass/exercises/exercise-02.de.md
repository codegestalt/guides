# Übung 2

In der [ersten Übung](exercise-01.de.md) haben wir gelernt was die Kommandozeile ist und wie wir direkt Befehle an Ruby übergeben können.

Im zweiten Teil schreiben wir einen Brief (Program), welches wir mittels Brieftaube (Kommandozeile) an Ruby übergeben damit sie ihn lesen und den Inhalt für uns ausführen kann.

## Der Brief (das Program)

Dazu öffnen wir unseren Texteditor und erstellen eine neue Datei mit dem Namen `brief.rb`. 

Nun schreiben wir den folgenden Inhalt ab und fügen diesen in unseren `brief.rb` ein:

```ruby
#!/usr/bin/ruby

# Dies ist ein Kommentar
puts "Dies ist mein erster Brief an Ruby"

# Wir sagen Ruby sie soll etwas berechnen und sich das
# Resultat merken.
resultat = 100 * 100 / 2

# Nun sagen wir Ruby Sie soll das Resultat ausgeben
puts resultat

# Wir sagen Ruby sie soll dem Computer einen Befehl geben:
system("echo ‘Hallo Welt!’")
```

Danach speichern wir unseren Brief und übergeben ihn mittels Brieftaube an Ruby.

## Den Brief via Brieftaube (Kommandozeile) an Ruby übergeben

Damit wir Ruby unseren Brief übergeben können, wechseln wir zurück in die Kommandozeile.

Dort müssen wir zuerst in den richtigen Ordner wechseln, in welchem unser Brief hinterlegt ist (erinnerst du dich noch an die Befehle `cd`, `ls` oder `dir`, `pwd` aus dem [ersten Teil](exercise-01.de.md)?)

* Windows: `cd pfad\zum\ordner`
* OSX und Linux: `cd pfad/zum/ordner`

Mittels `ls` kannst du dir den Ordner Inhalt anzeigen lassen, dabei sollte unser Brief `brief.rb` angezeigt werden.

Sobald wir uns im korrekten Ordner befinden können wir den Brief mittels Brieftaube an Ruby übergeben. Dies machen wir wie folgt:

* Windows: `ruby.exe ./brief.rb`
* OSX und Linux: `ruby ./brief.rb`

Ruby führt nun die im Brief (Program) hinterlegten Anweisungen aus und gibt uns die angeforderten Resultate zurück:

    Dies ist mein erster Brief an Ruby
    5000
    ‘Hallo Welt!’
