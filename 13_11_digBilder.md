# 13_11 Digitale Bilder

## Datenmodelle

Was sind die grundsätzlich zwei verschiedenen Modelle digitaler Bilder?

* Rastergrafiken
* Vektorgrafiken

* Rasterbilder bestehen aus einer Matrix von Werten, also z.B. Bildpunkten [https://upload.wikimedia.org/wikipedia/commons/8/8d/Kariertes_Papier_23-09-2016_PD.svg](https://upload.wikimedia.org/wikipedia/commons/8/8d/Kariertes_Papier_23-09-2016_PD.svg)
* Vektoren bestehen aus Knoten und Kanten, die sie verbinden [https://www.schule-und-familie.de/assets/images/Malen/Malen%20nach%20Zahlen/malen-nach-zahlen-clown.jp](https://www.schule-und-familie.de/assets/images/Malen/Malen%20nach%20Zahlen/malen-nach-zahlen-clown.jpg)

Es besteht zwischen den beiden Modellen ein grundlegender Unterschied darin, wie Attribute, etwa Farben, angelegt werden.

Für Vektor- und für Rastergrafiken gibt es jeweils eigene Dateiformate. Im alltäglichen Gebrauch sind z.B.:

> Aktivität: gemeinsames Sammeln von Dateiformaten auf dem Whitboard, dabei Vorbereitung: rechts ""Vektordaten", mitte "Rasterdaten", links "anderes"

* TIF - Tagged Image File Format
* JPG - Joint Photographic Experts Group
* SVG - Scalable Vector Graphics
* bmp - bitmap image file
* png
* svg
* gif

Wenn wir im weiteren Verlauf des Seminars von digitalen Bildern sprechen, reden wir auf Ebene der Datenmodelle über Rasterbilder und in aller Regel repräsentieren die Werte pro Rasterzelle dabei Farbwerte.

---

## Rasterbilder - Größe, Farbtiefe, Auflösung

Wenn man sich mit Rasterbilder auf der grundlegenden Ebene beschäftigt, wird man sehr schnell mit bestimmten Begriffen konfrontiert und es werden verschiedene Masszahlen zur Beschreibung von Bildern und ihrer Anzeige verwendet. 
Und zwar 

* Bildgröße
* Farbtiefe
* Bildauflösung

Wir bauen das Stück für Stück auf, dabei nutze ich auch den Kursbaustein des e-Learningkurs für den Umgang mit digitalen Daten. 

> Orga. Alle bitten sich einzuschreiben, um zu prüfen, ob es bei allen funktioniert

Der Kurs wurde insgesamt von Kai-Christian Bruhn, Thomas Engel (einem ehmaligen Mitarbeiter am i3mainz) und mir erstellt. Diesen Baustein hat aber insbesondere Sarah Pittroff gestaltet, die heute an der Akademie Mainz tätig ist und damals als student. Hilfskraft das i3mainz unterstützt hat.

---

### Bildraster - Bildpunkte und Rendern

Ein Rasterbild besteht wie oben gesehen aus einer Matrix aus gleichmäßig angeordneten Bildpunkten (oder auch _Pixel_) oder man könnte auch sagen, Messwerten. Dabei kann ein Messwert einen Grauwert, einen Farbwert wie z.B. einen Infrarotwert enthalten. Die Messwerte können mit einer einzigen Zahl ausgedrückt werden, oder sich aus einer Kombination von Zahlen ergeben. 
Das sieht man am Beispiel des Smiley, wo die Farben in RGB (Red, Green, Blue) angegeben werden.

In der digitalen Fotografie und den vielen bildlichen Darstellungen, die wir alltäglich im Netz sehen, werden die Bildpunkte quadratisch gerendert. Das bedeutet, die Matrix der Bildpunkte wird in ein Raster aus gleichgroßen quadratischen Zellen umgesetzt. Es kann aber auch in rechtwinklige Zellen gerendert werden, was laut Wikipedia eine Rolle bei Videoformaten spielen soll, in punktförmige Zellen, sechseckige Zellen usw.

---

### Bildgröße

Wenn wir einen Angabe, wie 1920 x 1080 Pixel finden, wissen wir, es handelt sich um ein Raster von 1920 Pixeln in der Breite und 1080 in der Höhe. Damit haben wir die **Bildgröße**. Sie kann entweder wie hier in ihrer Relation von Breite zu Höhe angegeben werden, oder aber in ihrer Summe, indem man beide multipliziert.

1920 x 1080 = 2073600 bits / 8000 = 295 Kilobyte

Hier machen wir einen kurzen Einschub zu bits und bytes

* 1 bit erlaubt die Speicherung von einem einstelligen Wert, also üblicherweise "0" und "1".
* 2 bit erlauben bereits die Speicherung von vier verschiedenen Variationen

| bit | Variationen                            | Anzahl | Faktor   |
| --- | -------------------------------------- | ------ | -------- |
| 1   | 0, 1                                   | 2      | 2 hoch 1 |
| 2   | 00, 01, 10, 11                         | 4      | 2 hoch 2 |
| 3   | 000, 001, 011, 111, 010, 110, 100, 101 | 8      | 2 hoch 3 |
| 4   | 0000, 0001, 0010, ...                  | 16     | 2 hoch 4 |
| 8   | 00000000, 00000001, 00000010, ...      | 256    | 2 hoch 8 |

* 1 byte fasst 8 bits zusammen (1 byte = 8 bits)
* 1 kilobyte = 1000 bytes = 8000 bits

mehr <https://web.stanford.edu/class/cs101/bits-bytes.html>

---

### Farbtiefe

Haben wir damit die Bildgröße behandelt, ist die **Farbtiefe** ein weiterer Wert, der in die Zahl der Bytes eines digitalen Bildes eingeht.

In dem Smiley werden pro Zelle bzw. pro Pixel drei Farbwerte festgelegt, mit denen jeweils die Intensität des Anteils von Rot, Grün und Blau gespeichert wird. Die Intensität dereinzelnen Farben, oder auch Kanäle, reicht dabei jeweils von 0 bis 256. 

 * TIFF unterstützt CMYK-Farbmodell -> Druckausgabe
 * JPG  unterstützt ICC Profile RGB und CMYK-Farbmodell -> Druckausgabe

> Frage 1 in die Gruppe: Um diesen Zahlenraum in Bits zu speichern benötigt man insgesamt pro Pixel wieviele bits ? 
>
> Also landet man bei einem Bild von 1920 x 1080 Pixeln und einer Farbtiefe von 24 bit (sog. True-Color) bei wievielen Kilobyte?

### Bildauflösung

Und schließlich ist ein wichtiger Wert, die **Bildauflösung**.

Noch nicht festgelegt ist mit diesem Wert, wie groß die Rasterzellen angesetzt sind. So könnte theoretisch ein Bildpunkt auch 1 m umfassen. Wenn sie mit Geodaten arbeiten, gibt es z.B. Rasterbilder zur Vermessung der Geländehöhe. Bei ihnen werden etwa alle 90 m die Messhöhe gemessen und die "Pixel" geben hier 90x90 m wieder ([SRTM 90](https://cgiarcsi.community/data/srtm-90m-digital-elevation-database-v4-1/)). 

Für die Anzeige im Web hat sich die Einheit "px" etabliert. Das entspricht 1/100 inch bzw. 0,25 mm. Ein px bezeichnet die geringste Breite einer noch scharf darstellbaren Linie. Für die Anzeige im Web ist bezeichnend, dass die Bilder auf ganz verschiedenen Bildschirmen angezeigt werden. Für den Ausdruck, also die Nutzung von Druckern, wird von dpi (dots per inch) gesprochen und bezeichnet die Anzahl von Punkten, die auf einer Linie von 1 inch (2,54 cm) platziert werden können. 

Bei einem Digitalisat gibt schließlich die Einheit _ppi_ wieder, wie groß das Original war und bei Beibehaltung des ppi wird das Bild in der Größe des Originals ausgedruckt. Wird der PPI gesenkt, wird der Druck größer (weniger pixel pro ein Inch) und bei größeren Werten wird das Bild kleiner ausgedruckt. 

### Quellen

* <https://en.wikipedia.org/wiki/Pixel>
* <https://en.wikipedia.org/wiki/Dots_per_inch>
* Rehbein, Malte. 2017. „Digitalisierung“. In Digital Humanities: Eine Einführung, herausgegeben von Fotis Jannidis, Hubertus Kohle, und Malte Rehbein, 179–198. Stuttgart: J.B. Metzler. 
* DFG-Praxisregeln "Digitalisierung"

## Vorbereitung für die nächste Sitzung !

### Vorbereitende Lektüre zum Thema Digitalisierung

1. Rehbein, Malte. 2017. „Digitalisierung“. In Digital Humanities: Eine Einführung, herausgegeben von Fotis Jannidis, Hubertus Kohle, und Malte Rehbein, 179–192. Stuttgart: J.B. Metzler. 
2. Deutsche Forschungsgemeinschaft. 2016. DFG-Praxisregeln ‚Digitalisierung‘. <https://www.dfg.de/formulare/12_151/12_151_de.pdf> hier insbesondere 14-16

### Teilen in zwei Gruppen, die jeweils folgende Texte intensiv lesen

* **Gruppe 1** - DFG Parisregeln im Kapitel 3.2. die Seiten 17-20 (3.2.1.3 Digitaler Aufnahmeablauf)
* **Gruppe 2** - DFG Parisregeln im Kapitel 3.2. die Seiten 20-22 (3.2.1.4 Dateiformate)


