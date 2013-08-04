# Huusufgoobe Büechli

## 1. Terminal öffnen:

* Mac OS X: Öffne Spotlight, tippe Terminal und klicke auf die Terminal Applikation.
* Windows: Klicke Start und tippe im Suchfeld „Command Prompt“, klicke danach auf „Command Prompt with Ruby on Rails“ um das Terminal zu öffnen.
* Linux (Ubuntu): Suche nach dem  Terminal in der dash und klicke auf Terminal.

Als nächstes führe folgende Befehle im Terminal aus:

```bash
mkdir projects
cd projects
rails new ferienpass
cd ferienpass
rails server
```

> In der [Übung 1](/ferienpass/exercises/exercise-01.de.md) haben wir die Befehle `cd` und `mkdir` kennengelernt.
> `rails` ist lediglich ein weiterer Befehl, welcher unser Computer durch die [Installation von Ruby on Rails](/rails/installation.de.md) gelernt hat.

Öffne nun den Browser deiner Wahl und tippe in der Adresszeile `http://localhost:3000` ein.
Nun solltest du die **Welcome aboard** Seite sehen, was bedeutet, dass dein neues Projekt korrekt funktioniert.

Drücke **CTRL-C** im terminal um den Server zu beenden.

## 2. Erstelle das Hausaufgaben Gerüst

Nun werden wir die `scaffold` Funktion von Rails nutzen um deine erste Applikation zu erstellen, ein sogenanntes Grundgerüst (`scaffold` in Englisch).
Diese erlaubt dir eine Hausaufgaben Liste zu erstellen, in welcher zu Hausaufgaben hinzufügen, ändern, ansehen und entfernen kannst.

Wie du bereits weist, ist Ruby's Muttersprache **Englisch**. Darum verwenden wir beim Programmieren ausschliesslich Englische Begriffe.
Aus diesem Grund erstellen wir ein Grundgerüst mit dem Namen `task`, was übersetzt Aufgabe heisst:

```bash
rails generate scaffold task title:string description:text due_date:date status:boolean
rake db:migrate
rails server
```

Danach öffne `http://localhost:3000/tasks` in deinem Browser.
Klicke ein wenig herum und teste was du mit den wenigen Befehlen im Terminal erstellt hast.

Klicke **CTRL-C**  um den Server wieder zu beenden.

## 3. Design

Um das Design ein wenig schöner zu gestalten werden wir das Twitter Bootstrap Projekt verwenden. Dies tun wir folgendermassen:

Öffne `app/views/layouts/application.html.erb` in deinem Texteditor füge oberhalb dieser Zeile

```ruby
<%= stylesheet_link_tag "application", media: "all", "data-turbolinks-track" => true %>
```

folgende Zeile ein

```ruby
<link href="//netdna.bootstrapcdn.com/twitter-bootstrap/2.3.2/css/bootstrap-combined.min.css" rel="stylesheet">
```

und ersetze:

```ruby
<%= yield %>
```

mit

```ruby
<div class="container">
  <%= yield %>
</div>
```

Nun fügen wir eine Navigation zum Layout hinzu. Dafür fügen wir unter `<body>` folgendes hinzu:

```html
<div class="navbar navbar-fixed-top">
  <div class="navbar-inner">
    <div class="container">
      <a class="brand" href="/">Husufgoobe Büechli</a>
      <ul class="nav">
        <li class="active"><a href="/tasks">Tasks</a></li>
      </ul>
    </div>
  </div>
</div>
```

und vor `</body>` folgendes ein

```html
<footer>
  <div class="container">
    Ferienpass 2013
  </div>
</footer>
```

Nun wollen wir die Darstellung der Hausaufgaben Tabelle ändern.
Öffne `app/assets/stylesheets/application.css` und füge folgendes ein:

```css
body { padding-top: 100px; }
footer { margin-top: 100px; }
table, td, th { vertical-align: middle !important; border: none !important; }
th { border-bottom: 1px solid #DDD !important; }
```

Aktualisiere die Seite in deinem Browser und schau dir an was sich geändert hat.
Du kannst nun auch gerne noch weitere Änderungen an der Darstellung vornehmen um zu sehen wie sich die Seite verändert.

Eine Übersicht über die CSS Funktionen findest du auf dieser Seite: http://de.selfhtml.org/css/

## 4. Routes

Wenn du `http://localhost:3000` öffnest wird dort immer noch die  **Welcome aboard** Seite angezeigt.
Um dort direkt alle deine Hausaufgaben anzuzeigen machen wir folgendes:

Öffne `config/routes.rb` und füge nach der ersten Zeile folgendes hinzu:

```ruby
root :to => "tasks#index"
```

Teste die Änderung indem du `http://localhost:3000` in deinem Browser aufrufst.
Anstelle der **Welcome aboard** Seite solltest du nun die Indexseite aller deiner Hausaufgaben sehen.
