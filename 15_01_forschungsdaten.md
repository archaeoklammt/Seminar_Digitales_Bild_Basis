# Forschungsdaten

### Was sind eigentlich Forschungsdaten?

* Publikationsbezogenen Daten (z.B. Studien bei "Nature" sind hinterlegt mit Messdaten)
* Katalog und Listenanhänge in geisteswissenschaftlichen Publikationen
* Materialsammlungen:
  * Zettelkasten
  * Notizbücher
  * Bildkollektionen (Aby Warburgs "Mnemosyne Atlas" [Forschungsprojekt](https://warburg.library.cornell.edu/)) 
  * Trainingsdaten für KI-Anwendungen

### Definitionen für Forschungsdaten?

DARIAH-DE Definition (DARIAH-DE Forschungsinfrastruktur für die Geisteswissenschaften) 

> _"Unter digitalen geistes-und kulturwissenschaftlichen Forschungsdaten werden all jene Quellen/Materialien und Ergebnisse verstanden, die im Kontext einer geistes-und kulturwissenschaftlichen Forschungsfrage gesammelt, erzeugt, beschrieben und/oder ausgewertet werden und in maschinenlesbarer Form zum Zwecke der Archivierung, Zitierbarkeit und zur weiteren Verarbeitung aufbewahrt werden können.“_ Gradl/Schmuck 2017 (<https://www.uni-bamberg.de/fileadmin/uni/fakultaeten/wiai_lehrstuehle/medieninformatik/Bilder/Projekte/DARIAH-DE/dhd2017/DHd2017-4-StefanTobi.pdf>)

Definition der Deutschen Forschungsgemeinschaft (DFG) 

> _"Zu Forschungsdaten zählen u.a. Messdaten, Laborwerte, audiovisuelle Informationen, Texte, Surveydaten, Objekte aus Sammlungen oder Proben, die in der wissenschaftlichen Arbeit entstehen, entwickelt oder ausgewertet werden. Methodische Testverfahren, wie Fragebögen, Software und Simulationen können ebenfalls zentrale Ergebnisse wissenschaftlicher Forschung darstellen und sollten daher ebenfalls unter den Begriff Forschungsdaten gefasst werden."_ DFG: Leitlinien zum Umgang mit Forschungsdaten, 8.4.2020 (<https://www.dfg.de/download/pdf/foerderung/antragstellung/forschungsdaten/richtlinien_forschungsdaten.pdf>) 

Begriffsbestimmung Forschungsdaten des mainzed

> _"Unter Forschungsdaten sind sämtliche Daten zu verstehen, die im Laufe von Forschungsprozessen entstehen. Der hier verwendete Begriff von Forschungsdaten umfasst daher gleichermaßen Rohdaten, wie auch die aus ihnen abgeleiteten Forschungsergebnisse in Form von Publikationen der Daten und Resultate inklusive der jeweils dazugehörigen Metadaten und Dokumentationen. Die Verwendung von Forschungsdaten in Lehre und Transfer kann die Erzeugung spezifi-scher Datenprodukte erfordern. Ihre Erstellung ist Teil der wissenschaftlichen Arbeit und entsprechend sind diese für Vermittlung und Qualifikation erzeugten Datenbestände  als Transferdaten auf gleiche Weise wie Forschungsdaten als eine Ressource von hohem Wert zu behandeln."_ mainzed-Empfehlungen.Daten in Forschung, Lehre und Transfer, Vers. 1.1 2018, <https://doi.org/10.5281/zenodo.1442528>   

### Der sogenannte Lebenszyklus der Forschungsdaten

* Datensätze, die veröffentlicht werden, bilden oftmals nur Teilausschnitt aller Daten, die erhoiben wurden ab und dies oft in bereits stark bereinigter Art -> Planübersicht einer Grabung, vereinheitlichte Schreibweisen und Transkriptionen. Bezogen auf Bilder etwa nur die Bilder in der Auflösung und dem Format, wie sie in der Veröffentlichung gezeigt werden. bearbeitungsschritte sind weder nachvollziehbar, noch kann der Anteil einzelner an der Bearbeitung erfasst werden. Forschung ist nicht reproduzierbar und nicht nachprüfbar.
* Die Entwicklung von Strategien zum Umgang mit Forschungsdaten hat zunächst wesentliche generische Etapen oder auch Prozessschritte ausgemacht, die bei der wissenschaftlichen Arbeit mit Daten über alle Domänen hin erkannt werden können und die wiederkehrend ähnliche Bedarf der Dokumentation und Betreuung der Daten entfalten.
  * Erfassung
  * Verarbeitung (Prozessierung was auch Analyseschritte beinhaltet)
  * Veröffentlichung (was gleichbedeutend mit "Zugang geben" ist)
  * Sichere Speicherung -> Langzeitarchivierung
* Forschungsdaten werden und sollen als Grundlage weiterer Forschungen dienen, daher wird als weiterer Prozessschritt die "Wiedernutzung" angesehen, die dann in einer Schleife erneut alle weiteren Schritte aufruft. Daher hat sich auch das Bild des Forschungsdatenlebenszyklus etabliert, das rhetorisch zudem eine starke Wirkung entfaltet. 
* Die Anordnung der Schritte, die genaue Benennung und auch ihre Anzahl - somit Granularität der Beschreibung - variiert in den zahlreichen Varianten, die von diesem Zyklus-Modell veröffentlicht wurden.

![](https://seafile.rlp.net/lib/972cd770-66a2-415a-b25e-1ebcd8cd7e09/file/images/auto-upload/image-1610704265678.png?raw=1)
Lebensdatenzyklus von IANUS - Forschungsdatenzentrum Archäologie & Altertumswissenschaften (<https://www.ianus-fdz.de/>)

#### FAIR
* FAIR-Data ist ein seit einigen Jahren etabliertes Schlagwort, das für ein Konzept steht, dass Daten (und somit auch Forschungsdaten) zugänglich und nutzbar machen will. Die vier Buchstaben stehen für die wesentlichen Herausforderungen auf technischer, juristischer und semantischer Ebene. 

> * **F**indable
> * **A**ccessible
> * **I**nteroperable
> * **R**e-usable

* An FAIR knüpfen sich auf europäischer Ebene große Vorhaben, wie die EOSC (European Open Science Cloud (s. https://www.fairsfair.eu/)) und damit auch ihre spezifische Ausprägung für die Geistes- und Sozialwissenschaften (Social Sciences and Humanities Open Cloud [SSHOC](https://sshopencloud.eu/).
* Auch für FAIR gibt es eine große Anzahl an Informationsangeboten, die ausführen, wie konkret die vier Herausforderungen hinter F, A, I und R anzugehen sind.

> To be **Findable**:
F1. (meta)data are assigned a globally unique and eternally persistent identifier.
F2. data are described with rich metadata.
F3. (meta)data are registered or indexed in a searchable resource.
F4. metadata specify the data identifier.

>To be **Accessible**:
A1  (meta)data are retrievable by their identifier using a standardized communications protocol.
A1.1 the protocol is open, free, and universally implementable.
A1.2 the protocol allows for an authentication and authorization procedure, where necessary.
A2 metadata are accessible, even when the data are no longer available.

>To be **Interoperable**:
I1. (meta)data use a formal, accessible, shared, and broadly applicable language for knowledge representation.
I2. (meta)data use vocabularies that follow FAIR principles.
I3. (meta)data include qualified references to other (meta)data.

>To be **Re-usable**:
R1. meta(data) have a plurality of accurate and relevant attributes.
R1.1. (meta)data are released with a clear and accessible data usage license.
R1.2. (meta)data are associated with their provenance.
R1.3. (meta)data meet domain-relevant community standards.


https://www.force11.org/group/fairgroup/fairprinciples
