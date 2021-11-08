# 13_11 Digitale Bilder

## Datenmodelle

Was sind die grundsätzlich zwei verschiedenen Modelle digitaler Bilder?

* Rastergrafiken
* Vektorgrafiken

* Rasterbilder bestehen aus einer Matrix von Werten, also z.B. Bildpunkten [https://upload.wikimedia.org/wikipedia/commons/8/8d/Kariertes_Papier_23-09-2016_PD.svg](https://upload.wikimedia.org/wikipedia/commons/8/8d/Kariertes_Papier_23-09-2016_PD.svg)
* Vektoren bestehen aus Knoten und Kanten, die sie verbinden [https://www.schule-und-familie.de/assets/images/Malen/Malen%20nach%20Zahlen/malen-nach-zahlen-clown.jp](https://www.schule-und-familie.de/assets/images/Malen/Malen%20nach%20Zahlen/malen-nach-zahlen-clown.jpg)

Es besteht zwischen den beiden Modellen ein grundlegender Unterschied darin, wie Attribute, etwa Farben, angelegt werden.

Für Vektor- und für Rastergrafiken gibt es jeweils eigene Dateiformate. Im alltäglichen Gebrauch sind z.B.:

> Aktivität: gemeinsames Sammeln von Dateiformaten auf dem Whitboard - dann sortieren zu den Formaten, dabei Vorbereitung: rechts "Vektordaten", mitte "Rasterdaten", links "anderes"

* TIF - Tagged Image File Format
* JPG - Joint Photographic Experts Group
* SVG - Scalable Vector Graphics
* bmp - bitmap image file
* png - Portable Network Graphics (Rastergrafik, verlustfreie Kompression)
* raw - Rasterdaten

Wenn wir im weiteren Verlauf des Seminars von digitalen Bildern sprechen, reden wir auf Ebene der Datenmodelle über Rasterbilder und in aller Regel repräsentieren die Werte pro Rasterzelle dabei Farbwerte.

---

## Rasterbilder 

### Bildraster - Bildpunkte und Rendern

Ein Rasterbild besteht aus einer Matrix aus gleichmäßig angeordneten Bildpunkten (oder auch _Pixel_) oder man könnte auch sagen, gleichmäßig angeordneten Messwerten. Dabei kann ein Messwert einen Grauwert, einen Farbwert wie z.B. einen Infrarotwert oder auch einen Messwert zur chemischen Zusammensetzung von Farbpigmenten enthalten. Die Messwerte können mit einer einzigen Zahl (so etwa Prozentanteil des Grauwerts) ausgedrückt werden, oder sich aus einer Kombination von Zahlen ergeben. 
Letzteres etwa ist der Fall, wenn RGB- oder CYMK-Farbwerte pro Zelle angegeben werden.

In der digitalen Fotografie und den vielen bildlichen Darstellungen, die wir alltäglich im Netz sehen, werden die Bildpunkte quadratisch gerendert. Das bedeutet, die Matrix der Bildpunkte wird in ein Raster aus gleichgroßen quadratischen Zellen umgesetzt. Es kann aber auch in rechteckige Zellen gerendert werden, was laut Wikipedia eine Rolle bei Videoformaten spielen soll, ebenso in kreisförmige Zellen, sechseckige Zellen usw.

Bei der Beschäftigung mit Rasterbildern sind drei verschiedene Maßzahlen zur Beschreibung von Bildern und ihrer Anzeige relevant. 

Und zwar 

* Bildgröße
* Farbtiefe
* Bildauflösung
---

### Bildgröße

Wenn wir eine Angabe, wie 1920 x 1080 Pixel finden, wissen wir, es handelt sich um ein Raster von 1920 Pixeln in der Breite und 1080 in der Höhe. Damit haben wir die **Bildgröße**. Sie kann entweder wie hier in ihrer Relation von Breite zu Höhe angegeben werden, oder aber in ihrer Summe, indem man beide multipliziert.

1920 x 1080 = 2073600 bits / 8000 = 295 Kilobyte

Hier machen wir einen kurzen Einschub zu **bits** und **bytes**.

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

In Frankreich werden englischsprachige Begriffe in der Regel übersetzt (es gibt hierzu auch eine gesetzliche Regelung, mit der der Anteil von fremdsprachigen Lehnwörtern beschränkt wird). Entsprechend gibt es den Begriff *bytes* nicht, sondern man nutzt die Bezeichnungen *octet* und *multiplet*. 

| englischer Begriff | französischer Begriff |
|--- | --- |
| bit | bit | 
| byte (8 bits) | octet (8 bits) | 
| kb (kilobits) | kb (kilobits) |
| KB (Kilobytes) | Ko (Kilooctets) |
| GB (Gigabytes) | Go (gigaoctets) |


mehr zum Thema: <https://web.stanford.edu/class/cs101/bits-bytes.html>

---

### Farbtiefe

Haben wir damit die Bildgröße behandelt, ist die **Farbtiefe** ein weiterer Wert, der in die Zahl der Bytes eines digitalen Bildes eingeht.


#### RGB

RGB steht für *red-green-blue* und bezeichnet ein additives Farbmodell, das für Bildschirme bzw. selbstleuchtende Medien eingesetzt wird. Indem die verschiedenen Farben durch den Anteil der drei Farben Rot, Grün und Blau erzeugt werden. technisch werden die drei Farben so eng nebeneinander gesetzt angezeigt, dass im menschlichen Auge die Wahrnehmung eines gemeinsamen Farbtons entsteht. 

Der Anteil der drei Farben pro Pixel bei einem 24bit System (pro Farbe 255 Werte) kann je nach Kontext unterschiedlich codiert werden (sprachlich z.B. "cornflowerblue", als Hexadezimal (#6495ED) oder auf 256 umgerechneter Wert 100,149,237  (100 = 39% von 256), 149 (= 58%), 237 (=93%)). 

Zurückkommend auf die eingangs gemachte Berechnung der Bits eines Bildes von 1920x1080 px wird deutlich, dass der errechnete Wert nur die Speicherung eines schwarzweißen Bildes erlaubt, während ein farbiges Bild bereits pro Pixel 24 bits (3 x 8 bits) ansetzen muss.

Auf Französisch wird für RGB entsprechend RVB (*rouge-vert-bleu*) als Bezeichnung verwendet.

#### CMYK

CMYK steht für *cyan-magenta-yellow-key* und bezeichnet ein substraktives Farbmodell, das für den Druck und für Lichttechnik (etwa bei Veranstaltungen) verwendet wird. Bei diesem Farbmodell werden dem Licht durch eine Oberfläche bestimmte Wellen entzogen und die Reflexion erscheint für das menschliche Auge farbig."Key" bezeichnet den Schwarzanteil. Die CYMK-Werte bezeichnen den Anteil der drei Farben und des Schwarzwertes.

Im frankophonen Raum wird CMYK als CMYJ (*cyan-magenta-jaune-noir*) oder auch *quadrichromie* bezeichnet, und damit direkt auf seinen Ursprung  im Vierfarbdruck verweist und tatsächlich werden die Farben beim Druck überlagert.

#### Farbe bei der Digitalisierung und im Druck

Bigitalkameras erfassen Bilder RGB-Farbwerte und die Betrachtung und Wiedergabe digitaler Bilder etwa auf Webseiten wird über RGB-Farbwerte gesteurt. Für den Druck - und speziell einen "farbechten" Druck - erfolgt erstens die Umrechnung in CMYK und zweitens werden für den professionellen Bereich Farbprofile erstellt, mit denen dann Drucker und Monitor so abgestimmt werden, dass der Ausdruck auf Papier (und hier den unterschiedlichen Qualitäten) und der Anschauung am Bildschirm, wo die Bildbearbeitung vorgenommen wurde, übereinstimmt.  

#### Datenformate

 * TIFF unterstützt CMYK-Farbmodell -> Druckausgabe
 * JPG  unterstützt ICC Profile RGB und CMYK-Farbmodell -> Druckausgabe
 * PNG unterstützt kein CYMK, nicht für Druck gedacht; unterstützt dafür 24-bit color und verlustfreie Kompression

### Bildauflösung

Und schließlich ist ein wichtiger Wert, die **Bildauflösung**.

Noch nicht festgelegt ist mit diesem Wert, wie groß die Rasterzellen angesetzt sind. So könnte theoretisch ein Bildpunkt auch 1 m umfassen. Wenn sie mit Geodaten arbeiten, gibt es z.B. Rasterbilder zur Vermessung der Geländehöhe. Bei ihnen werden etwa alle 90 m die Messhöhe gemessen und die "Pixel" geben hier 90x90 m wieder ([SRTM 90](https://cgiarcsi.community/data/srtm-90m-digital-elevation-database-v4-1/)). 

Für die Anzeige im Web hat sich die Einheit **px** etabliert. Das entspricht 1/100 inch bzw. 0,25 mm. Ein px bezeichnet die geringste Breite einer noch scharf darstellbaren Linie. 

Für die Anzeige im Web ist bezeichnend, dass die Bilder auf ganz verschiedenen Bildschirmen angezeigt werden. Für den Ausdruck, also die Nutzung von Druckern, wird dagegen von dpi (dots per inch) und im frankophonen Sprachraum auch von **ppp** (point par pouce) gesprochen und bezeichnet die Anzahl von Punkten, die auf einer Linie von 1 inch (= 2,54 cm) platziert werden können. 150 dpi sind also 150 Punkte auf 2,54 cm, 300 dpi entsprechend doppelt so viele.

Bei einem Digitalisat gibt schließlich die Einheit _ppi_ wieder, wie groß das Original war und bei Beibehaltung des ppi wird das Bild in der Größe des Originals ausgedruckt. Wird der PPI gesenkt, wird der Druck größer (weniger pixel pro ein Inch) und bei größeren Werten wird das Bild kleiner ausgedruckt. 

### Quellen

* <https://en.wikipedia.org/wiki/Pixel>
* [https://en.wikipedia.org/wiki/Dots_per_inch](https://en.wikipedia.org/wiki/Dots_per_inch) / [https://fr.wikipedia.org/wiki/Point_par_pouce](https://fr.wikipedia.org/wiki/Point_par_pouce)
* Rehbein, Malte. 2017. „Digitalisierung“. In Digital Humanities: Eine Einführung, herausgegeben von Fotis Jannidis, Hubertus Kohle, und Malte Rehbein, 179–198. Stuttgart: J.B. Metzler. 
* DFG-Praxisregeln "Digitalisierung"



