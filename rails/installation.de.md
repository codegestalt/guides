# Rails Installation (Linux/Windows/OSX)

Diese Anleitung beschreibt die Installationsschritte für die Betriebssysteme Linux, Windows und OSX.

## Linux

## Windows

## OSX

### Überprüfe die Version deines Betriebssystems

Klicke auf das Apfelmenu und wähle den Punkt **Über diesen Mac**:

![](http://codegestalt-guides.s3.amazonaws.com/rails/installation/installation-osx-01.png)

Anschliessend öffnet sich ein Dialogfenster in dem man die aktuelle Versionsnummer des Betriebssystems ausgelesen werden kann:

![](http://codegestalt-guides.s3.amazonaws.com/rails/installation/installation-osx-02.png)

Basierend auf dieser Nummer wird nun der entsprechende Installer gedownloadet.

### Rails downloaden und installieren

Die folgenden Downloads stammen von der Seite http://railsinstaller.org/en:

* [Mac OSX 10.7 & 10.8](http://railsinstaller.s3.amazonaws.com/RailsInstaller-1.0.4-osx-10.7.app.tgz)
* [Mac OSX 10.6](http://railsinstaller.s3.amazonaws.com/RailsInstaller-1.0.4-osx-10.6.app.tgz) (64bit only)

Mittels Doppelklick auf das gedownloadete File wird der RailsInstaller ausgepackt.
Mittels einem weiteren Doppelklick auf die entpackte Datei (**RailsInstaller-1.0.4-osx-10.6.app** oder **RailsInstaller-1.0.4-osx-10.7.app**) beginnt der Installationsprozess von Rails.
Folge den Anweisungen im Installationsprozess. Nach dem Installationsprozess öffnet sich eine **README** Datei, ignoriere dessen Inhalt.

### Rails updaten

Falls es sich bei der gedownloadeten Version nicht um die aktuellste Rails Version handelt, kann man mit folgendem Befehl Rails updaten:

    gem update rails --no-ri --no-rdoc
