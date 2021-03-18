# Normdaten

## LIDO Hands on

Beispiel 1: [https://commons.wikimedia.org/wiki/File:Vincent_van_Gogh_-_Self-Portrait_-\_Google_Art_Project.jpg](https://commons.wikimedia.org/wiki/File:Vincent_van_Gogh_-_Self-Portrait_-_Google_Art_Project.jpg)

XML Online Editor: <https://jsonformatter.org/xml-editor>

## Referat Getty

Fragen
Feedback-Bögen: <https://pad.gwdg.de/a0OBEO1HQm2sl-LHJpDVyQ?view>

Anwendung TGN und ULAN: <https://monsieur-park.github.io/Ownreality_visual/mapping.html>

## Fortsetzung LIDO

* Anreichern mit TGN, ULAN und Wikidata
* Abschluß XML kopieren und im Stud-Ordner ablegen

## Vorbereitung crosswalk iiif-APIs 11/12/2020

* Anreichern mit Subject ID: Orte, Institution, Künstler, ggfs. Sujet und Objekttyp
* ein Bild in das Internetarchive einstellen (bitte beachten Sie dazu sehr genau die Anleitung: <https://training.iiif.io/iiif-online-workshop/day-two/image-servers/iiif-hosting-ia.html> 
* für das Bild ein iiif-Manifest erzeugen, auch dies bitte genau entlang der Anleitung erstellen: <https://training.iiif.io/iiif-online-workshop/day-three/bodleian-editor/> ACHTUNG nutzen Sie bitte unbedingt de "Bodleian Manifest Editor" und hier die HTTP-version (nicht die HTTPS-version).
* so Sie Chrome haben, installieren Sie bitte einen Chrome Webserver: <https://training.iiif.io/iiif-online-workshop/day-three/chrome-web-server/>

## Übungsdaten

\<lido:lidoWrap xsi:schemaLocation="<http://www.lido-schema.org> <http://www.lido-schema.org/schema/v1.0/lido-v1.0.xsd">>
	\<lido:lido>\</lido:lido>
	\<lido:lido>
		\<lido:lidoRecID lido:source="Deutsches Dokumentationszentrum für Kunstgeschichte - Bildarchiv Foto Marburg" lido:type="local">DE-Mb112/lido-obj20344012,T,001\</lido:lidoRecID>
		\<lido:category>
			\<lido:conceptID lido:type="URI"><http://www.cidoc-crm.org/crm-concepts/E22>\</lido:conceptID>
			\<lido:term xml:lang="en">Man-Made Object\</lido:term>
		\</lido:category>
		\<lido:descriptiveMetadata xml:lang="de">
			\<lido:objectClassificationWrap>
				\<lido:objectWorkTypeWrap>
					\<lido:objectWorkType>
						\<lido:term lido:encodinganalog="5230/5230">Brunnen\</lido:term>
					\</lido:objectWorkType>
				\</lido:objectWorkTypeWrap>
				\<lido:classificationWrap>
					\<lido:classification lido:type="europeana:type">
						\<lido:term>IMAGE\</lido:term>
					\</lido:classification>
					\<lido:classification>
						\<lido:term lido:encodinganalog="5220/5220">Brunnenskulptur\</lido:term>
						\<lido:term lido:addedSearchTerm="yes" lido:encodinganalog="5220/520a">Skulptur\</lido:term>
					\</lido:classification>
				\</lido:classificationWrap>
			\</lido:objectClassificationWrap>
			\<lido:objectIdentificationWrap>
				\<lido:titleWrap>
					\<lido:titleSet>
						\<lido:appellationValue lido:pref="preferred">
Fontana del Moro — Brunnenbecken mit vier Tritonen und Masken
\</lido:appellationValue>
					\</lido:titleSet>
				\</lido:titleWrap>
				\<lido:inscriptionsWrap/>
				\<lido:repositoryWrap>
					\<lido:repositorySet lido:type="current">
						\<lido:repositoryLocation>
							\<lido:namePlaceSet>
								\<lido:appellationValue>Rom, Piazza Navona, Südseite\</lido:appellationValue>
							\</lido:namePlaceSet>
							\<lido:partOfPlace>
								\<lido:placeID lido:type="local" lido:source="TGN">7000874\</lido:placeID>
								\<lido:namePlaceSet>
									\<lido:appellationValue>Rom\</lido:appellationValue>
								\</lido:namePlaceSet>
											\<lido:appellationValue>Italien\</lido:appellationValue>
											\</lido:namePlaceSet>
                                \</lido:partOfPlace>
                            \</lido:partOfPlace>
                        \</lido:partOfPlace>
                    \</lido:repositoryLocation>
                \</lido:repositorySet>
                \</lido:repositoryWrap>
                \<lido:displayStateEditionWrap/>
                \<lido:objectDescriptionWrap/>
                \<lido:objectMeasurementsWrap/>
            \</lido:objectIdentificationWrap>
			\<lido:eventWrap>
				\<lido:eventSet>
					\<lido:event>
						\<lido:eventType>
							\<lido:term>Herstellung\</lido:term>
						\</lido:eventType>
						\<lido:eventActor>
							\<lido:actorInRole>
								\<lido:actor lido:type="person">
									\<lido:actorID lido:source="Bildindex-KUE-Datei" lido:type="local">kue 07600032\</lido:actorID>
									\<lido:nameActorSet>
										\<lido:appellationValue lido:pref="preferred">Porta, Giacomo della\</lido:appellationValue>
									\</lido:nameActorSet>
									\<lido:nationalityActor>
										\<lido:term>Italien\</lido:term>
									\</lido:nationalityActor>
									\<lido:vitalDatesActor>
										\<lido:earliestDate lido:type="estimatedDate">1537\</lido:earliestDate>
										\<lido:latestDate lido:type="deathDate">1602\</lido:latestDate>
									\</lido:vitalDatesActor>
									\<lido:genderActor>männlich\</lido:genderActor>
								\</lido:actor>
								\<lido:roleActor>
									\<lido:term>Bildhauer\</lido:term>
								\</lido:roleActor>
							\</lido:actorInRole>
						\</lido:eventActor>
						\<lido:eventDate>
							\<lido:date>
								\<lido:earliestDate>1575\</lido:earliestDate>
								\<lido:latestDate>1576\</lido:latestDate>
							\</lido:date>
						\</lido:eventDate>
					\</lido:event>
				\</lido:eventSet>
			\</lido:eventWrap>
			\<lido:objectRelationWrap>
				\<lido:subjectWrap>
					\<lido:subjectSet>
						\<lido:subject lido:type="Beschreibung">
							\<lido:subjectConcept>
								\<lido:conceptID lido:source="Iconclass" lido:type="local">92 H 39 1\</lido:conceptID>
								\<lido:term>92 H 39 1\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Triton(en)\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Triton & Triton\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Klassische Mythologie und Antike Geschichte\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">
Mythologie & antike Geschichte & Geschichte & Klassische Antike & Religion & griechisch & römisch
\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">die Götter in der klassischen Mythologie\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Gott (nicht-christlich)\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Wassergottheiten: Neptun und sein Gefolge\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Meeresgott & Gott (nicht-christlich)\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">die Geschichte von Triton\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Triton\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Nachkommenschaft, Begleiter, Gefolge, etc. Tritons\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Verwandtschaft & Zug & Gefolge & Triton\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Triton(en)\</lido:term>
							\</lido:subjectConcept>
						\</lido:subject>
					\</lido:subjectSet>
					\<lido:subjectSet>
						\<lido:subject lido:type="Beschreibung">
							\<lido:subjectConcept>
								\<lido:conceptID lido:source="Iconclass" lido:type="local">48 A 98 21 1\</lido:conceptID>
								\<lido:term>48 A 98 21 1\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Maske (mascaron) als Ornament\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Maske & Mascaron\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Gesellschaft, Zivilisation, Kultur\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Gesellschaft & Zivilisation & Kultur\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Kunst\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Kunst\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Kunst und Öffentlichkeit; Stile und Ornamente\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Öffentlichkeit & öffentlich & Kunst\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">stilistische und formale Kriterien für die Kunst\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Stil & Gestalt & Kunst\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Ornamente in der bildenden Kunst; naturalistisch\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Ornament & naturalistisch\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">antropomorphe Ornamente\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">menschliche Figur\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Ornamente in Form von menschlichen Körperteilen\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Glied (Körper)\</lido:term>
								\<lido:term lido:addedSearchTerm="yes">Maske (mascaron) als Ornament\</lido:term>
							\</lido:subjectConcept>
						\</lido:subject>
					\</lido:subjectSet>
		\</lido:descriptiveMetadata>
		\<lido:administrativeMetadata xml:lang="de">
			\<lido:rightsWorkWrap/>
			\<lido:recordWrap>
				\<lido:recordID lido:type="local">20344012,T,001\</lido:recordID>
				\<lido:recordType>
					\<lido:term>Einzelobjekt\</lido:term>
				\</lido:recordType>
				\<lido:recordSource>
					\<lido:legalBodyName>
						\<lido:appellationValue>
Deutsches Dokumentationszentrum für Kunstgeschichte - Bildarchiv Foto Marburg
\</lido:appellationValue>
					\</lido:legalBodyName>
					\<lido:legalBodyWeblink><http://www.fotomarburg.de>\</lido:legalBodyWeblink>
				\</lido:recordSource>
				\<lido:recordRights>
					\<lido:rightsHolder>
						\<lido:legalBodyName>
							\<lido:appellationValue>
Deutsches Dokumentationszentrum für Kunstgeschichte - Bildarchiv Foto Marburg
\</lido:appellationValue>
						\</lido:legalBodyName>
						\<lido:legalBodyWeblink><http://www.fotomarburg.de>\</lido:legalBodyWeblink>
					\</lido:rightsHolder>
				\</lido:recordRights>
				\<lido:recordInfoSet>
					\<lido:recordInfoLink lido:formatResource="html">
<http://www.bildindex.de/dokumente/html/obj20344012,T,001>
\</lido:recordInfoLink>
				\</lido:recordInfoSet>
			\</lido:recordWrap>
		\</lido:administrativeMetadata>
	\</lido:lido>
	\</lido:lido>
\</lido:lidoWrap>
