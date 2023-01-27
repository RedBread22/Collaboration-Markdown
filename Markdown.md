# _Markdown-Dokumentation_
# Anleitung zu Markdown

Markdown ist eine leichtgewichtige Markup-Sprache, die verwendet wird, um Text in einfachem Format zu formatieren und es einfach lesbar und schreibbar zu machen. Es wird oft für Online-Inhalte wie Blogs, Foren und Dokumentationen verwendet und unterstützt von vielen beliebten Plattformen und Tools.


## Überschriften

Überschriften können in Markdown durch die Verwendung von Hashtags (#) erstellt werden. Je mehr Hashtags verwendet werden, desto kleiner wird die Überschrift.

```
# Überschrift 1
## Überschrift 2
### Überschrift 3
#### Überschrift 4
##### Überschrift 5
###### Überschrift 6
```
Alternativ können Überschriften auch mit Unterstrichen (_) erstellt werden.
```
Überschrift 1 =============  
Überschrift 2 --------------
```
## Trennstriche

Trennstriche können in Markdown durch die Verwendung von drei oder mehr Sternchen (*), Minuszeichen (-) oder Unterstrichen (_) erstellt werden.

```
---

***
```

## Hervorgehobene/betonte Wörter

Wörter können in Markdown hervorgehoben oder betont werden, indem sie kursiv oder fett formatiert werden. Kursive Formatierung erfolgt durch die Verwendung von Sternchen (*) oder Unterstrichen (_), fette Formatierung durch die Verwendung von zwei Sternchen (**) oder zwei Unterstrichen (__).

```
*kursiv*

_kursiv_

**fett**

__fett__
```

## Aufzählungen

Aufzählungen können in Markdown mit einem Pluszeichen (`+`), einem Bindestrich (`-`) oder einer Zahl (`1.`) und einem Punkt erstellt werden. Unterpunkte können mit zwei Leerzeichen vor dem Bullet-Zeichen erstellt werden.
```
1. geordnete Aufzählung
2. geordnete Aufzählung
3. geordnete Aufzählung
  - Unterpunkt
  - Unterpunkt
    - Unter-Unterpunkt
```

## Links

Links können in Markdown durch die Verwenden von eckigen Klammern und runden Klammern erstellt werden. Der Text, der angezeigt werden soll, steht in den eckigen Klammern, die URL des Links steht in den runden Klammern.

```
[Text des Links](https://www.example.com)
```
[Bsp.](https://www.example.com)


## Quellcode
```python
def say_hello():
    print("Hello, World!")
```

## Tabellen

Tabellen können in Markdown mit vertikalen Balken (`|`) und Bindestrichen (`-`) erstellt werden. Die Bindestriche dienen als Trennzeichen zwischen der Überschrift und dem Inhalt der Tabelle.

```
|Spalte 1|Spalte 2|
|--------|--------|
|    A    |    B    |
|    C    |    D    |
```
|Spalte 1|Spalte 2|
|--------|--------|
|    A    |    B    |
|    C    |    D    |
## Bilder

Bilder können in Markdown ähnlich wie Links durch die Verwendung von eckigen Klammern und runden Klammern eingefügt werden. Der Text, der als Alternativtext angezeigt werden soll, steht in den eckigen Klammern, die URL des Bildes steht in den runden Klammern.

```text
![Alt-Text](/Pfad/zum/Bild.jpg)
```

```
Bsp.
```



## Blockzitate

```
> Test1
> Test2
> Test3
> Test4
```
> Test1
> Test2
> Test3
> Test4


## Fußnoten

Fußnoten können in Markdown mit einem eckigen Klammern (`[]`) für den Text und einem runden Klammern (`()`) mit einer Nummer für die Fußnote erstellt werden. Der Text der Fußnote wird am Ende des Dokuments definiert.

```mixed
Im Fließtext [^1] können Sie ganz einfach Fußnoten [^2] unterbringen.
[^1]: Hier finden Sie den Text zu der Fußnote.
[^2]: **Fußnoten** selbst können auch *formatiert* werden.
Und diese umfassen sogar mehrere Zeilen.
```
Im Fließtext [^1] können Sie ganz einfach Fußnoten [^2] unterbringen.
[^1]: Hier finden Sie den Text zu der Fußnote.
[^2]: **Fußnoten** selbst können auch *formatiert* werden.
Und diese umfassen sogar mehrere Zeilen.


## Task Listen

Task Listen können in Markdown durch die Verwendung von Minuszeichen (-) und Leerzeichen, gefolgt von einem Häkchen (x) oder einem Leerzeichen erstellt werden. Ein Häkchen zeigt an, dass eine Aufgabe erledigt.
- [ ] Mercury - 
- [x] Venus - 
- [x] Earth (Orbit/Moon) - 
- [x] Mars -
- [ ]  [ ] Jupiter - 
- [ ] [ ] Saturn -
- [ ]  [ ] Uranus - 
- [ ] [ ] Neptune -
- [ ]  [ ] Comet Haley


## Durchgestrichene Absätze

In Markdown können per  (`~~`)  Text durchgestrichen werden.

~~Dieser Absatz ist durchgestrichen.~~

## Text Highlighting

Text kann mit zwei == markiert werden.

==Dieser Text ist markiert==

## Hochgestellte und tiefgestellte Zeichen

Zeichen können in Markdown hoch- oder tiefgestellt werden, indem man sie mit dem `^` oder `~` Zeichen einrahmt.
```
Hochgestellter Text:  4^4^
Tiefgestellter Text: 5~2~ 

Hochgestellter Text:  4^4^
Tiefgestellter Text: 5~2~ 
```
## Deaktivierte URL-Verknüpfungen

URLs können in Markdown deaktiviert werden, indem man sie mit dem `<` und `>` Zeichen einrahmt.

<https://www.example.com>


## Diagramme

And this will produce a flow chart:

```mermaid
graph LR
A[Square Rect] -- Link text --> B((Circle))
A --> C(Round Rect)
B --> D{Rhombus}
C --> D
