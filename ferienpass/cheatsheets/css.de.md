# CSS Cheatsheet

Dieses Dokument dient als Spickzettel für die CSS Programmierung.

## In HTML einbinden

CSS Code kann man auf verschiedene Arten einbinden, für die ersten Schritte ist die einfachste Methode das direkte Einbinden in einem HTML Dokument.

```html
<head>
  <style>
    body {
      background: blue;
    }
  </style>
</head>
```

Einzelnen HTML Elementen kann man auch ein `style` Attribut zuweisen:

```html
<img src="http://linkzubild.jpg" style="width: 100px;">
```

## Selektoren

Mit Selektoren referenziert man mit CSS auf Elemente.

```css
selector {
  attribut: wert;
}
```

Beispiel: Links auf der Seite mit blauer Farbe versehen.


```css
a {
  color: blue;
}
```

Im HTML kann man einzelnen Elementen Klassen zuweisen und mit CSS darauf referenzieren:

```html
<div class="links">
</div>
```

```css
.links {
  float: left;
}
```

## Attribute

Die folgenden Beispiele zeigen Attribute die man verwenden kann, mit Beispielswerten.

### Hintergrund

```css
body {
  background: gray; /* Hintergrundfarbe */
}
```

Hintergrundfarben kann man auch auf anderen Elementen wie `a`, `p`, etc. verwenden.

### Schriften

```css
body {
  font-size: 16px; /* Schriftgrösse */
  font-weight: bold; /* Schriftdicke */
  font-family: "Helvetica", sans-serif; /* Schriftart */
  color: red; /* Schriftfarbe */
}
```