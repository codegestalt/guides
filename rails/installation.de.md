# Rails Installation (Linux/Windows/OSX)

Diese Anleitung beschreibt die Installationsschritte für die Betriebssysteme OSX, Windows und Linux.

## OSX

### Überprüfe die Version deines Betriebssystems

Klicke auf das Apfelmenu und wähle den Punkt **Über diesen Mac**:

![](http://codegestalt-guides.s3.amazonaws.com/rails/installation/installation-osx-01.png)

Anschliessend öffnet sich ein Dialogfenster in dem man die aktuelle Versionsnummer des Betriebssystems ausgelesen werden kann:

![](http://codegestalt-guides.s3.amazonaws.com/rails/installation/installation-osx-02.png)

Basierend auf dieser Nummer wird nun der entsprechende Installer gedownloadet.

### Rails downloaden und installieren

Die folgenden Downloads stammen von der Seite http://railsinstaller.org/en

* [Mac OSX 10.7 & 10.8](http://railsinstaller.s3.amazonaws.com/RailsInstaller-1.0.4-osx-10.7.app.tgz)
* [Mac OSX 10.6](http://railsinstaller.s3.amazonaws.com/RailsInstaller-1.0.4-osx-10.6.app.tgz) (64bit only)

Mittels Doppelklick auf das gedownloadete File wird der RailsInstaller ausgepackt.
Mittels einem weiteren Doppelklick auf die entpackte Datei (**RailsInstaller-1.0.4-osx-10.6.app** oder **RailsInstaller-1.0.4-osx-10.7.app**) beginnt der Installationsprozess von Rails.
Folge den Anweisungen im Installationsprozess. Nach dem Installationsprozess öffnet sich eine **README** Datei, ignoriere dessen Inhalt.

### Rails updaten

Falls es sich bei der gedownloadeten Version nicht um die aktuellste Rails Version handelt, kann man mit folgendem Befehl Rails updaten:

    gem update rails --no-ri --no-rdoc

## Windows
### Rails downloaden und installieren

Die folgenden Downloads stammen von der Seite http://railsinstaller.org/en
https://github.com/railsinstaller/railsinstaller-windows/releases/download/2.2.2/railsinstaller-2.2.2.exe

Mittels Doppelcklick auf das heruntergeladene File wird die Installation gestartet. Falls das folgende Fenster auftaucht:
![](http://www.bedesign.ch/img/rails/sicherheitswarnung.png)

Klicke Ausführen. Danach sollte sich folgedes Fenster öffnen:
![](http://www.bedesign.ch/img/rails/setup1.jpg)

Hier klickst du Next und gelangst auf folgendes Fenster:
![](http://www.bedesign.ch/img/rails/setup2.jpg)

Hier ist es wichtig, dass du "I accept all of the Licenses" angewählt hast, und erst danach next klickst. 
Im folgenden Fenster klickst du dann Install

![](http://www.bedesign.ch/img/rails/setup3.jpg)

sobald die Installation abgeschlossen ist erscheint folgendes Fenster:
![](http://www.bedesign.ch/img/rails/setup4.jpg)

Hier klickst du auf Finish worauf dieses Fenster erscheinen wird:
![](http://www.bedesign.ch/img/rails/setup5.jpg)

Damit ist die Installation von Rails abgeschossen.

### Rails updaten

Falls es sich bei der gedownloadeten Version nicht um die aktuellste Rails Version handelt, kann man mit folgendem Befehl Rails updaten:

    gem update rails --no-ri --no-rdoc


## Linux

Für die Installation unter Linux müssen wir lediglich eine der beiden unteren Links kopieren und im Terminal eingeben:

**Unter Ubuntu:**

    bash < <(curl -s https://raw.github.com/railsgirls/installation-scripts/master/rails-install-ubuntu.sh)

**Unter Fedora:**

    bash < <(curl -s https://raw.github.com/railsgirls/installation-scripts/master/rails-install-fedora.sh)

Der Prozess dauert ein Weilchen.

# Bemerkungen

- Vielen Dank an Rails Girls für die Installationsscripts.
