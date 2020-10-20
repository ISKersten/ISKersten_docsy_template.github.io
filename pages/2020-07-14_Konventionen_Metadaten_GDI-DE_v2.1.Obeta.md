![Logo_GDI-DE_textstark-ansicht](media/image1.jpeg){width="2.0458333333333334in"
height="1.0375in"}

  -----------------------------------------------------------------------------------------------------------
  Dieses Dokument beschreibt die Konventionen zu Metadaten in der GDI-DE mit Erläuterungen und Beispielen. 
  -----------------------------------------------------------------------------------------------------------

Architektur der

Geodateninfrastruktur

Deutschland

Konventionen zu Metadaten

**Arbeitskreis Metadaten**

**14.07.2020**

**Version: 2.1.0 beta**

**\
**

*(Leerseite)*

 Dokumentinformation {#dokumentinformation .no-toc}
===================

+------------------------+-------------------------+----------------+
| Bezeichnung            | Architektur der         |                |
|                        | Geodateninfrastruktur   |                |
|                        | Deutschland --          |                |
|                        | Konventionen zu         |                |
|                        | Metadaten               |                |
+========================+=========================+================+
| Autor                  | AK Metadaten            |                |
+------------------------+-------------------------+----------------+
| Erstellt am            | 02.04.2019              |                |
+------------------------+-------------------------+----------------+
| Bearbeitungszustand    |                         | in Bearbeitung |
+------------------------+-------------------------+----------------+
|                        | x                       | Vorgelegt      |
+------------------------+-------------------------+----------------+
|                        |                         | Abgestimmt     |
+------------------------+-------------------------+----------------+
| Dokumentablage         | Kollaborationsplattform |                |
|                        | GDI-DE                  |                |
+------------------------+-------------------------+----------------+
| Arbeitskreis Metadaten | Peter Kochmann (GDI-NW  |                |
|                        | \| Bezirksregierung     |                |
|                        | Köln -- Abteilung       |                |
|                        | Geobasis NRW)           |                |
|                        |                         |                |
|                        | Steffen Bach (GDI-BW \| |                |
|                        | Landesamt für           |                |
|                        | Geoinformation und      |                |
|                        | Landentwicklung         |                |
|                        | Baden-Württemberg --    |                |
|                        | Kompetenzzentrum        |                |
|                        | Geodateninfrastruktur)  |                |
|                        |                         |                |
|                        | Andreas Berg (GDI-SN \| |                |
|                        | Staatsbetrieb           |                |
|                        | Geobasisinformation und |                |
|                        | Vermessung Sachsen      |                |
|                        | (GeoSN) --              |                |
|                        | Administration          |                |
|                        | Geodateninfrastruktur)  |                |
|                        |                         |                |
|                        | Valentina Gorsic        |                |
|                        | (GDI-HE \| Hessisches   |                |
|                        | Landesamt für           |                |
|                        | Bodenmanagement und     |                |
|                        | Geoinformation --       |                |
|                        | Geo                     |                |
|                        | informationsmanagement) |                |
|                        |                         |                |
|                        | Anja Jacobi (GDI-SN \|  |                |
|                        | Staatsbetrieb           |                |
|                        | Geobasisinformation und |                |
|                        | Vermessung Sachsen      |                |
|                        | (GeoSN) --              |                |
|                        | Koordinierung           |                |
|                        | Geodateninfrastruktur)  |                |
|                        |                         |                |
|                        | Robin Küspert (GDI-BY   |                |
|                        | \| LDBV Bayern)         |                |
|                        |                         |                |
|                        | Anja Loddenkemper (Kst. |                |
|                        | GDI-NI \| Landesamt für |                |
|                        | Geoinformation und      |                |
|                        | Landesvermessung        |                |
|                        | Niedersachsen --        |                |
|                        | Landesbetrieb --)       |                |
|                        |                         |                |
|                        | Stephanie Marstatt      |                |
|                        | (GDI-BY \| LDBV Bayern) |                |
|                        |                         |                |
|                        | Stefanie Nadler (BLE \| |                |
|                        | Bundesanstalt für       |                |
|                        | Landwirtschaft und      |                |
|                        | Ernährung --            |                |
|                        | Fachzentrum für         |                |
|                        | Geoinformation und      |                |
|                        | Fernerkundung für den   |                |
|                        | Geschäftsbereich des    |                |
|                        | BMEL)                   |                |
|                        |                         |                |
|                        | Andrea Pörsch (GDI-BB   |                |
|                        | \| LGB --               |                |
|                        | Landesvermessung und    |                |
|                        | Geobasisinformation     |                |
|                        | Brandenburg --          |                |
|                        | Kontaktstelle GDI-DE +  |                |
|                        | Metadatenmanagement)    |                |
|                        |                         |                |
|                        | Michael Räder (MDI-DE   |                |
|                        | \|                      |                |
|                        | Nationalpark-Verwaltung |                |
|                        | Niedersächsisches       |                |
|                        | Wattenmeer /            |                |
|                        | Niedersächsischer       |                |
|                        | Landesbetrieb für       |                |
|                        | Wasserwirtschaft,       |                |
|                        | Küsten- und             |                |
|                        | Naturschutz)            |                |
|                        |                         |                |
|                        | Sabine Schütze (BKG \|  |                |
|                        | Bundesamt für           |                |
|                        | Kartographie und        |                |
|                        | Geodäsie --             |                |
|                        | Geodateni               |                |
|                        | nfrastrukturleistungen) |                |
|                        |                         |                |
|                        | Martin Thal (GDI-HH \|  |                |
|                        | Landesbetrieb           |                |
|                        | Geoinformation und      |                |
|                        | Vermessung -- Urban     |                |
|                        | Platform \| Betrieb     |                |
|                        | Serversysteme)          |                |
|                        |                         |                |
|                        | Renate Zweer (GDI-BE \| |                |
|                        | Senatsverwaltung für    |                |
|                        | Stadtentwicklung und    |                |
|                        | Wohnen --               |                |
|                        | Geoinformation)         |                |
|                        |                         |                |
|                        | Anja Litka (Kst. GDI-DE |                |
|                        | \| Bundesamt für        |                |
|                        | Kartographie und        |                |
|                        | Geodäsie)               |                |
+------------------------+-------------------------+----------------+

Die Autoren danken den vielen Personen und Institutionen, die am
Entwicklungsprozess des Konventionendokuments aktiv beteiligt waren.

 {#section .no-toc}

 Änderungsverzeichnis {#änderungsverzeichnis .no-toc}
====================

+------------+-------------------+-------------------+--------------+
| Version    | Datum             | Änderung          | Ersteller    |
+============+===================+===================+==============+
| 0.9 beta   | 27.03.2013        | Aufbereitung als  | AK Metadaten |
|            |                   | Vorlage zur       |              |
|            |                   | Beschlussfassung  |              |
|            |                   | im LG GDI-DE      |              |
+------------+-------------------+-------------------+--------------+
| 0.9        | 13.05.2014        | Beschluss Nr. 69  | Vorsitz LG   |
|            |                   | im LG GDI-DE      |              |
+------------+-------------------+-------------------+--------------+
| 1.0 beta   | 17.11.2014        | Aufbereitung als  | AK Metadaten |
|            |                   | Vorlage zur       |              |
|            |                   | Beschlussfassung  |              |
|            |                   | im LG GDI-DE      |              |
+------------+-------------------+-------------------+--------------+
| 1.0        | 14.01.2015        | Beschluss Nr. 79  | Vorsitz LG   |
|            |                   | im LG GDI-DE      |              |
+------------+-------------------+-------------------+--------------+
| 1.1        | 21.04.2015        | Fehlerkorrektur   | AK Metadaten |
|            |                   | Codelisten,       |              |
| beta       |                   | Ergänzung Anhang  |              |
|            |                   | 2                 |              |
+------------+-------------------+-------------------+--------------+
| 1.1.0      | 27.07.2015        | Beschluss Nr. 88  | Vorsitz LG   |
|            |                   | im LG GDI-DE      |              |
+------------+-------------------+-------------------+--------------+
| 1.1.1      | 01.04.2016        | ATS-Referenzen    | AK Metadaten |
|            |                   | und Abschnitt 1.4 |              |
| beta       |                   | eingefügt; ed.    |              |
|            |                   | Korrekturen       |              |
+------------+-------------------+-------------------+--------------+
| 1.1.1      | 14.04.2016        | Aufbereitung zur  | Kst. GDI-DE  |
|            |                   | Veröffentlichung  |              |
+------------+-------------------+-------------------+--------------+
| 1.2.0      | 04.04.2017        | Kategorisierung   | AK Metadaten |
|            |                   | der Konventionen  |              |
| beta       |                   | bzgl. INSPIRE     |              |
|            |                   | und/oder GDI-DE   |              |
|            |                   | plus              |              |
|            |                   | entsprechende     |              |
|            |                   | Kennzeichnung in  |              |
|            |                   | jedem Kapitel     |              |
+------------+-------------------+-------------------+--------------+
| 1.2.0 beta | 18.04.2017        | Aufbereitung als  | Kst. GDI-DE  |
|            |                   | Vorlage zur       |              |
|            |                   | Beschlussfassung  |              |
|            |                   | im LG GDI-DE      |              |
+------------+-------------------+-------------------+--------------+
| 1.2.0      | 01.08.2017        | Korrekturen sowie | AK Metadaten |
|            |                   | Aktualisierung    |              |
| beta       |                   | als Vorlage zur   |              |
|            |                   | Beschlussfassung  |              |
|            |                   | im LG GDI-DE      |              |
+------------+-------------------+-------------------+--------------+
| 1.2.0      | 30.08.2017        | Beschluss Nr. 103 | Vorsitz LG   |
|            |                   | im LG GDI-DE      |              |
+------------+-------------------+-------------------+--------------+
| 1.3.0 beta | nicht             | interne Version;  | AK Metadaten |
|            | veröffentlicht    | Arbeitsdokument   |              |
|            |                   | bzgl. Anpassung   |              |
|            |                   | der Konventionen  |              |
|            |                   | an TG MD 2.0.1    |              |
+------------+-------------------+-------------------+--------------+
| 2.0.0 beta | 07.03.2019        | Anpassung der     | AK Metadaten |
|            |                   | Konventionen an   |              |
|            |                   | TG MD 2.0.1       |              |
+------------+-------------------+-------------------+--------------+
| 2.0.0 beta | 02.04.2019        | Aufbereitung als  | Kst. GDI-DE  |
|            |                   | Vorlage zur       |              |
|            |                   | Beschlussfassung  |              |
|            |                   | im LG GDI-DE      |              |
+------------+-------------------+-------------------+--------------+
| 2.0.0      | 06.06.2019        | Beschluss Nr. 121 | Vorsitz LG   |
|            |                   | im LG GDI-DE      |              |
+------------+-------------------+-------------------+--------------+
| 2.0.1      | 12.06.2019        | Anpassung der     | AK Metadaten |
|            |                   | Beispiele         |              |
|            |                   | aufgrund          |              |
|            |                   | Beschluss im LG   |              |
|            |                   | GDI-DE            |              |
+------------+-------------------+-------------------+--------------+
| 2.0.2      | 22.11.2019        | Redaktionelle     | AK Metadaten |
|            |                   | Anpassungen       |              |
+------------+-------------------+-------------------+--------------+
| 2.1.0 beta |                   | -   XML-Beispiele | AK Metadaten |
|            |                   |     3.2.1 und 3.5 |              |
|            |                   |     korrigiert    |              |
|            |                   |                   |              |
|            |                   | -                 |              |
|            |                   |   Konkretisierung |              |
|            |                   |     in 3.6 und    |              |
|            |                   |     XML-Beispiel  |              |
|            |                   |     korrigiert    |              |
|            |                   |                   |              |
|            |                   | -   Korrekturen   |              |
|            |                   |     in Abschnitt  |              |
|            |                   |     2.10 (Wegfall |              |
|            |                   |     NUTS/LAU)     |              |
|            |                   |                   |              |
|            |                   | -                 |              |
|            |                   |   Konkretisierung |              |
|            |                   |     in 2.7.1 und  |              |
|            |                   |     3.2.2         |              |
|            |                   |                   |              |
|            |                   | -   Korrektur im  |              |
|            |                   |     Anhang 3      |              |
|            |                   |     (Anpassungen  |              |
|            |                   |     an Änderungen |              |
|            |                   |     aus Version   |              |
|            |                   |     2.0.3)        |              |
|            |                   |                   |              |
|            |                   | -   Grafik aus TG |              |
|            |                   |     zum           |              |
|            |                   |                   |              |
|            |                   |   Geltungsbereich |              |
|            |                   |     eingefügt in  |              |
|            |                   |     1.2           |              |
|            |                   |                   |              |
|            |                   | -   Pfade zur ATS |              |
|            |                   |                   |              |
|            |                   |   (pdf-Dokumente) |              |
|            |                   |     überarbeitet  |              |
|            |                   |                   |              |
|            |                   | -                 |              |
|            |                   |   Konkretisierung |              |
|            |                   |     in 4.3.1:     |              |
|            |                   |     Verpflichtung |              |
|            |                   |     zu            |              |
|            |                   |     GetCap        |              |
|            |                   | abilities-Request |              |
|            |                   |     bei INSPIRE   |              |
|            |                   |                   |              |
|            |                   | -   Anhang 2: im  |              |
|            |                   |     Einzelfall    |              |
|            |                   |                   |              |
|            |                   |  deutschsprachige |              |
|            |                   |     Bezeichnung   |              |
|            |                   |     aus           |              |
|            |                   |     Übersetzung   |              |
|            |                   |     der ISO 19115 |              |
|            |                   |     ergänzt       |              |
|            |                   |                   |              |
|            |                   | -   neues Kapitel |              |
|            |                   |     2.13 zu       |              |
|            |                   |                   |              |
|            |                   |  Referenzsystemen |              |
|            |                   |                   |              |
|            |                   | -   Kapitel 3.1   |              |
|            |                   |     präzisiert    |              |
|            |                   |                   |              |
|            |                   | -                 |              |
|            |                   |   Konkretisierung |              |
|            |                   |     in Kapitel 6  |              |
|            |                   |                   |              |
|            |                   | -   weitere       |              |
|            |                   |     geringfügige  |              |
|            |                   |     redaktionelle |              |
|            |                   |     Anpassungen   |              |
+------------+-------------------+-------------------+--------------+

 {#section-1 .no-toc}

 Inhalt {#inhalt .no-toc}
======

1 Einführung 7

1.1 Die Architektur der Geodateninfrastruktur Deutschland 7

1.2 Konventionen zu Metadaten 8

1.3 Die Topologie der Metadatenkataloge 10

1.4 Hinweise zum Dokument 11

2 Grundsätzliche Konventionen für alle Metadaten 14

2.1 Multiplizität des identificationInfo-Elementes 14

2.2 Eindeutiger Metadatensatzidentifikator 14

2.3 Art der Ressource 15

2.4 Sprache der Metadaten 15

2.5 Kontakt (Verantwortliche Stelle Metadaten) 16

2.6 Kontakt (Verantwortliche Stelle für die Ressource) 17

2.7 Schlüsselwörter 18

2.7.1 Schlüsselwort „inspireidentifiziert" 19

2.8 Beschränkungen des öffentlichen Zugangs (\[INS VO MD\], B 8.2) 19

2.9 Nutzungs- und Zugriffsbedingungen 21

2.9.1 Nutzungs- und Zugriffsbedingungen in der GDI-DE (ohne INSPIRE) 21

2.9.2 Bedingungen für den Zugang und die Nutzung bei INSPIRE (\[INS VO
MD\], B 8.1) 23

2.10 Regionalschlüssel 26

2.11 Kennzeichnung der Verbindlichkeit von per Darstellungs- und/oder
Downloaddienst bereitgestellten Daten 27

2.12 Konformität (Übereinstimmung mit Spezifikationen, \[INS VO MD\],
B 7) 29

2.13 Angaben zum Raumbezug / Koordinatenreferenzsystem (EPSG-Code) 30

3 Konventionen für Metadaten zu Datenbeständen und Anwendungen 32

3.1 Eindeutiger Ressourcenidentifikator (\[INS VO MD\], B 1.5) 32

3.2 Schlüsselwörter 33

3.2.1 Quellenangabe für Schlüsselwörter zu INSPIRE-Themen 33

3.2.2 Schlüsselwort „opendata" 34

3.3 Themenkategorie nach ISO (Zuordnung zum INSPIRE-Thema: \[INS VO
MD\], B 2.1) 35

3.4 Ressourcenverweis für Datensätze und -serien (transferOptions, \[INS
VO MD\], B 1.4) 36

3.5 Konformität (Übereinstimmung mit Spezifikationen, \[INS VO MD\],
B 7) 37

3.6 Nutzungsbedingungen und Lizenzinformationen für Open Data 39

3.7 Formatangaben 41

4 Konventionen für Metadaten zu Diensten 42

4.1 Schlüsselwörter 42

4.1.1 Schlüsselwörter zu Dienstkategorien bei INSPIRE 42

4.2 Verlinkung zum verwendeten Datenbestand (Daten-Dienste-Kopplung) 43

4.2.1 Gekoppelte Daten-Ressource (\[INS VO MD\], B 1.6) 43

4.2.2 Art der Kopplung zwischen Dienst und zugehörigen Daten 44

4.3 Ressourcenverweise für Dienste 44

4.3.1 Ressourcenverweis unter transferOptions (\[INS VO MD\], B 1.4) 44

4.3.2 Ressourcenverweis unter connectPoint 46

4.4 Art des Geodatendienstes bei INSPIRE (\[INS VO MD\], B 2.2) 47

4.5 Version des Geodatendienstes bei INSPIRE 47

4.6 Konformität (Übereinstimmung mit Spezifikationen, \[INS VO MD\],
B 7) 48

5 Daten-Dienste-Kopplung 51

6 Open Data-Informationen zu Datensätzen und -serien 54

7 Werkzeuge zur Überprüfung der Konventionen 55

Referenzen 56

Anhang 1: INSPIRE-Spezifikationen (Durchführungsbestimmungen) 58

Anhang 2: Zuordnung der INSPIRE-Annex-Themen zu ISO-Themenkategorien 59

Anhang 3: Beschränkungen des öffentlichen Zugangs bei INSPIRE 61

Anhang 4: Nachweis der Änderungen der Konventionen zu Metadaten Version
2.1.0 gegenüber Version 2.0.3 vom 27.04.2020 63

Einführung
==========

Die Architektur der Geodateninfrastruktur Deutschland
-----------------------------------------------------

Um ein reibungsloses Zusammenwirken der nationalen technischen
Komponenten der GDI-DE zu ermöglichen, sind organisatorische und
technische Rahmenvorgaben erforderlich, die zusammen­fassend als
Architekturkonzept der GDI-DE bezeichnet werden.

Zur leichteren Handhabung ist das Architekturkonzept der GDI-DE aus
einzelnen Dokumenten in drei verschiedenen Kategorien (grundsätzliche
Festlegungen, spezielle technische Festlegungen und Empfehlungen)
aufgebaut:

![Übersicht der Module.png](media/image2.png){width="6.3in"
height="3.245833333333333in"}

Abbildung 1: Architekturkonzept der GDI-DE -- Übersicht über die
Architekturdokumente

Grundsätzliche Festlegungen werden durch Beschluss des LG GDI-DE in
folgenden Dokumenten getroffen:

-   Das Dokument *„Architektur der GDI-DE - Ziele und Grundlagen"*
    erläutert die strategischen Ziele, fachliche und technische
    Grundsätze sowie die rechtlichen und organisatorischen
    Rahmenbedingungen der GDI-DE \[GDI-DE Architektur - Ziele\].

-   Das Dokument *„Architektur der GDI-DE - Technik"* beschreibt die
    verschiedenen Architektur­komponenten und referenziert hierfür
    relevante Normen, Standards und Spezifikationen \[GDI-DE
    Architektur - Technik\].

-   Das Dokument *„Architektur der GDI-DE - Maßnahmenplan"* zeigt die
    für die künftige Entwicklung der GDI-DE erforderlichen Schritte auf
    \[GDI-DE Architektur - Maßnahmen\].

Spezielle technische Festlegungen, vor allem in Bezug auf Technik und
Betrieb von Komponenten der GDI-DE, werden durch Beschluss des LG GDI‑DE
in folgenden Dokumenten getroffen:

-   Profile der GDI-DE zu internationalen oder nationalen Normen und

-   Konventionen, die über eine Norm oder Spezifikation hinausgehen.

Darüber hinausgehende Informationen werden als Handlungsempfehlungen von
Arbeitskreisen weiter konkretisiert.

Konventionen zu Metadaten
-------------------------

Im vorliegenden Dokument werden Konventionen zu Metadaten sowie deren
Bereitstellung erläutert und zusammengefasst. Diese Konventionen werden
im Arbeitskreis (AK) Metadaten erarbeitet. Ältere Vorgängerversionen
gehen auch auf Arbeiten der Projektgruppe Geodatenkatalog.de und einen
Metadaten-Workshop mit Ansprechpartnern der GDI-DE aus Bund und Ländern
zurück. Weitere Hinweise, welche sich auf die Inhalte von Metadaten
beziehen, finden sich in eigenen Handlungsempfehlungen, z. B. der
Länder-GDIs[^1], wieder.

In Geodateninfrastrukturen gibt es grundsätzlich zwei unterschiedliche
Typen von Metadatendokumenten:

-   Typ1: Capabilities-Dokumente, mit welchen Dienste-Schnittstellen
    ihre Eigenschaften beschreiben.

-   Typ2: Metadaten nach ISO 19115/19119, welche in Katalogen erfasst
    und bereitgestellt werden.

Das vorliegende Dokument befasst sich überwiegend mit Konventionen zu
Typ 2. Typ 1 wird in den Konventionsdokumenten bzw.
Handlungsempfehlungen des AK Geodienste behandelt[^2].

Grundsätzlich sollen in der GDI-DE sowohl die Anforderungen aus der
INSPIRE-Richtlinie \[INS VO MD, INS TG MD\] (sofern relevant) als auch
die ISO-Festlegungen \[ISO 19115, ISO 19119, ISO 19139\] erfüllt werden.
Alle Vorgaben der ISO (Belegungspflichten bzw. -bedingungen,
Werteumfänge etc.) gelten somit auch für die GDI-DE. Das bedeutet, dass
es weitere, zwingend zu belegende Metadatenelemente geben kann, die
benötigt werden, um einen ISO- und/oder INSPIRE-konformen Metadatensatz
zu bilden, auch wenn das vorliegende Dokument keine Konvention dazu
aufführt.

Ergänzend bzw. vertiefend werden in diesem Dokument konkrete
Konventionen für einzelne Metadatenelemente in der GDI-DE beschrieben.
Die Festlegungen im vorliegenden Dokument betreffen Metadatenelemente,
für die Regelungsbedarf in der GDI-DE gesehen wird, der über die
grundsätzlichen Regelungen der ISO hinausgehen kann oder aus
verpflichtenden oder bedingten Angaben für INSPIRE resultiert.

Außerdem trifft dieses Dokument keine Festlegungen zur inhaltlichen
Strukturierung von Freitext-Elementen wie z. B. Titel und
Kurzbeschreibung. Etwaige Regelungen für eine einheitliche Vergabe von
Titeln, Kurzbeschreibungen etc. und die Festlegung von Benennungsmustern
liegen im Ermessen der einzelnen Fachnetzwerke und sind durch diese in
eigenen Leitfäden zu treffen.

Bzgl. der Vorgaben seitens INSPIRE wird an dieser Stelle explizit darauf
hingewiesen, dass zzt. für die GDI-DE keine Betrachtung der sog.
„aufrufbaren Geodatendienste", die keine INSPIRE-Netzdienste sind,
erfolgt. Aus der INSPIRE Technical Guidance zu Metadaten V2.0.1 wurden
daher nur die Belange für Metadaten zu Datensätzen und --serien
(geregelt in Chapter 2, 3.1 und 3.2 \[INS TG MD\]) sowie zu Netzdiensten
(geregelt in Chapter 4.1 und 4.2 \[INS TG MD\] berücksichtigt. Die
Vorgaben für aufrufbare Geodatendienste (geregelt in Chapter 4.3 bis 4.5
\[INS TG MD\]) gelten seitens INSPIRE davon unbenommen; eine
Präzisierung durch die GDI-DE bleibt jedoch zzt. aus, weil momentan
keine Anwendungsfälle existieren. Bei Bedarf wird dies zu einem späteren
Zeitpunkt im Rahmen der Fortschreibung dieses Dokumentes ergänzt.

![](media/image3.png){width="6.558333333333334in"
height="3.601350612423447in"}

Abbildung 2: „Figure 4: Structure of the conformance classes in this
Technical Guidance document" \[INS TG MD\] -- Metadaten für aufrufbare
Geodatendienste (rote Kennzeichnung) werden aktuell in diesem Dokument
nicht präzisiert.

Die Topologie der Metadatenkataloge
-----------------------------------

In der GDI-DE existieren eine Vielzahl verteilter, eigenständiger
Metadatenkataloge, deren Inhalte im zentralen Geodatenkatalog.de
zusammengeführt werden. Eine ähnliche Aggregation geschieht auch in
anderen Knoten. Beispielsweise laufen in den Katalogen der Bundesländer
die Metadaten aus verschiedenen Bereichen und Ebenen der Verwaltung
zusammen. 3Abbildung (Seite 9) verdeutlicht diesen Zusammenhang.

Eine Beschreibung der zentralen Komponente „Geodatenkatalog.de" der
GDI-DE erfolgt in diesem Dokument nicht, sondern ist im Dokument
„Architektur der GDI-DE -- Technik" zu finden \[[GDI-DE
Architektur](#REF12) - Technik\]. Dort werden auch die Voraussetzungen
für die Einbindung einer dezentralen Katalogschnittstelle in die GDI-DE
beschrieben.

![](media/image4.png){width="6.495833333333334in"
height="4.370833333333334in"}

Abbildung 3: Topologie der Metadatenkataloge

Durch die Topologie der Metadatenkataloge ist es notwendig, dass
Änderungen eines Katalogs überall dort nachvollzogen werden, wo dessen
Bestand übernommen wird. Wird also ein Metadatensatz in einem Katalog
gelöscht, so wird er auch in allen anderen Katalogen entfernt, welche
diesen Katalog harvesten, da der *fileIdentifier* des Metadatensatzes
und damit der Metadatensatz selbst nicht mehr auffindbar ist. Übernommen
werden zugleich alle „neuen" Metadaten mit einem bisher nicht
vorhandenen *fileIdentifier* und alle geänderten Metadaten, deren
*fileIdentifier* bereits bekannt sind, die jedoch einen aktualisierten
Zeitstempel tragen.

Hinweise zum Dokument
---------------------

Die Festlegungen in diesem Dokument sind für die Metadaten-Sprache
„Deutsch" getroffen, sofern durch ISO oder INSPIRE keine anderen
Forderungen bestehen.

Den einzelnen Festlegungen in diesem Dokument ist jeweils ein
XPath-Ausdruck vorangestellt:

Dieser adressiert bzw. beschreibt die Position des betreffenden
Metadatenelementes im XML-Dokument. Die Kodierung des Elementes in XML
wird jeweils wie folgt exemplarisch dargestellt:

Die einzelnen Festlegungen des Dokumentes enthalten am Anfang jeweils
folgende Tabelle:

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☐             ☐
  zusätzlich für INSPIRE   ☐               ☐             ☐

Diese Tabelle gibt einen Überblick über die jeweilige Forderung der
GDI-DE bzw. zusätzlich für INSPIRE. Dabei gelten folgende Festlegungen:

-   „GDI-DE" -- generelle Konventionen für [alle]{.ul} Metadaten, um
    eine Einheitlichkeit in den Metadaten der GDI-DE zu fördern und
    deren Interoperabilität zu gewährleisten. Diese Anforderungen können
    begründet sein

    -   über \[ISO 19115\] und \[ISO 19119\] hinausgehende Festlegungen
        zwecks Einheitlichkeit;

    -   durch die Verwendung der Metadaten für Open Data (siehe Kapitel
        6);

    -   durch Vorgaben seitens INSPIRE, für die eine Verallgemeinerung
        und Übertragung auf die gesamte GDI-DE als sinnvoll erachtet
        wurde.

-   „zusätzlich für INSPIRE" - Konventionen, die sich aus der RICHTLINIE
    2007/2/EG DES EUROPÄISCHEN PARLAMENTS UND DES RATES vom 14. März
    2007 zur Schaffung einer Geodateninfrastruktur in der Europäischen
    Gemeinschaft (INSPIRE), den INSPIRE Implementing Rules oder den
    zugehörigen Technical Guidance-Dokumenten ergeben. Hierbei handelt
    es sich um Klarstellungen oder Präzisierungen der GDI-DE, um die
    Metadaten, die Ressourcen für INSPIRE beschreiben, einheitlich zu
    gestalten (z. B. in Fällen, in denen INSPIRE Freiräume zulässt).
    Grundsätzlich betrifft dies nur Metadaten, die Datensätze, -serien
    oder Netzdienste für INSPIRE beschreiben. [Die Konventionen unter
    „GDI-DE" (s.o.) sind dabei ebenfalls zu beachten und
    einzuhalten]{.ul}.

-   *verpflichtend* -- generelle Verpflichtungen zur Erfüllung der
    Anforderungen seitens der GDI-DE bzw. für INSPIRE.

-   *konditional* - Verpflichtungen unter bestimmten Bedingungen, um die
    Anforderungen seitens der GDI-DE bzw. für INSPIRE zu erfüllen. Die
    jeweilige Konvention ist dann verpflichtend, wenn die benötigten
    Informationen vorliegen bzw. eine beschriebene Situation zutrifft.

-   *optional* - keine Verpflichtung zur Führung der jeweiligen
    Information. Für den Fall, dass diese Information aber erfasst
    werden soll, gelten die jeweils genannten Konventionen.

Im Fließtext sind die Bezeichnungen von Metadatenelementen kursiv
gesetzt, z. B.: *MD_Metadata*. Die Attributwerte sind in
Anführungszeichen angegeben, z. B.: „Es gelten keine Bedingungen".

Die dabei verwendeten Bezeichnungen von Metadatenelementen beziehen sich
auf die Nomenklatur der Spezifikationen der \[ISO 19115\] und \[ISO
19119\] sowie der INSPIRE-Verordnung für Metadaten \[INS VO MD\].

Jede Festlegung in diesem Dokument endet mit einem Verweis auf die
dazugehörige Testbeschreibung in Form einer *Abstract Testsuite* (ATS).
Dort sind die jeweiligen Testschritte, welche in der GDI-DE Testsuite
implementiert wurden, im Detail beschrieben:

Als Referenz werden unter

[*https://ims.geoportal.de/git/tree/AK-Metadaten.git/version2.0.0/konventionen!beispiel_xml*](https://ims.geoportal.de/git/tree/AK-Metadaten.git/version2.0.0/konventionen!beispiel_xml)

Beispieldokumente bereitgestellt:

-   *[dataset.xm](https://ims.geoportal.de/git/blob/AK-Metadaten.git/version0.9/konventionen!beispiel_xml!dataset.xml)l*
    (Daten-Metadatensatz)

-   [*service.xml*](https://ims.geoportal.de/git/blob/AK-Metadaten.git/version0.9/konventionen!beispiel_xml!service.xml)
    (Dienst-Metadatensatz)

-   [*wms.xml*](https://ims.geoportal.de/git/blob/AK-Metadaten.git/version0.9/konventionen!beispiel_xml!wms.xml)
    (WMS-Capabilities-Dokument)

-   *opendata_dataset.xml* (Daten-Metadatensatz)

In diesen Muster-Metadatensätzen sind die Konventionen, wie in diesem
Dokument dargelegt, umgesetzt.

Dieses Dokument wird in einem stetigen Prozess fortgeschrieben und
veröffentlicht. Je nach Veränderungen im Dokument werden die
Versionsnummern wie folgt angepasst:

  **Änderungen in der Versionsnummer**   **Anlass bzw. Umfang der Änderung**
  -------------------------------------- -----------------------------------------------------------------------------------------------------------------------
  1\.                                    Änderungen in den gesetzlichen Bestimmungen und damit grundsätzliche Änderungen im Dokument
  1.1                                    Geringfügige Änderungen oder Ergänzungen in den Kapiteln, Ergänzung von neuen Kapiteln
  1.1.1                                  Berichtigung von Schreibfehlern, Fehlerbehebung, redaktionelle Änderungen in den Kapiteln ohne fachliche Auswirkungen

**\
**

Grundsätzliche Konventionen für alle Metadaten
==============================================

Die Konventionen in diesem Kapitel betreffen die Metadaten zu allen
Ressourcen in der GDI-DE, unabhängig von der Art der Ressource im
*hierarchyLevel*-Element (siehe 2.3).

Multiplizität des identificationInfo-Elementes
----------------------------------------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☒               ☐             ☐
  zusätzlich für INSPIRE   ☐               ☐             ☐

Um die Einheitlichkeit und eindeutige Interpretierbarkeit der Metadaten
in der GDI-DE zu fördern, gilt als Konvention für [alle]{.ul} Metadaten
in der GDI-DE:

Alle relevanten Informationen sind im ersten
*identificationInfo*-Element anzugeben.

Gemäß \[ISO 19115\] kann das *identificationInfo*-Element innerhalb
eines Metadatensatzes mehrfach verwendet werden. Im Rahmen von INSPIRE
wird jedoch nur das erste *identificationInfo*-Element ausgewertet
(siehe \[[INS TG MD](#REF2)\], 2.3). Auch im Geoportal.de finden nur
Informationen Berücksichtigung, die im ersten
*identificationInfo*-Element angegeben sind.

Eindeutiger Metadatensatzidentifikator
--------------------------------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☒               ☐             ☐
  zusätzlich für INSPIRE   ☐               ☐             ☐

Ein Metadatensatz besitzt immer einen eindeutigen Identifikator. Die
Verwendung einer UUID gemäß RFC 4122[^3] wird empfohlen. Sollte der
bisher verwendete Metadatensatzidentifikator historisch bedingt nicht
den Regeln einer UUID entsprechen, so ist dieser im Sinne des
Bestandsschutzes weiterhin zulässig. Der Identifikator soll, unabhängig
von Überarbeitung am Metadatensatz selbst, nicht verändert werden. Beim
Replizieren muss dieser beibehalten und darf nicht überschrieben werden.
Nur so sind eine eindeutige Identifizierung von Metadaten, die
zuverlässige Filterung von Dubletten sowie die Aktualisierung
vorhandener Metadatensätze anhand von *fileIdentifier* (\[ISO 19115\],
B.2.1, No. 2) und *dateStamp* (\[ISO 19115\], B.2.1, No. 9) innerhalb
der GDI-DE möglich.

Art der Ressource
-----------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☒               ☐             ☐
  zusätzlich für INSPIRE   ☐               ☐             ☐

Ein Metadatensatz muss immer eine Information über die Art der
Ressource, die er beschreibt, beinhalten. Dies geht über die Regelungen
aus \[ISO 19115\] für das *hierarchyLevel*-Element (\[ISO 19115\],
B.2.1, No. 6) hinaus und soll eine eindeutige Interpretierbarkeit des
Metadatensatzes innerhalb der GDI-DE ermöglichen.

Sprache der Metadaten
---------------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☒               ☐             ☐
  zusätzlich für INSPIRE   ☐               ☐             ☐

Ein Metadatensatz muss immer eine Information über die in den Metadaten
verwendete Sprache beinhalten.

Diese Konvention beruht auf den Vorgaben aus \[INS TG MD\], 2.2.2
(Requirement C.5) und geht über die Regelungen aus \[ISO 19115\] für das
*language*-Element in \[ISO 19115\], B.2.1, No. 3, hinaus.

Um die Einheitlichkeit und die eindeutige Interpretierbarkeit der
Metadaten in der GDI-DE zu fördern, wird diese Konvention für
[alle]{.ul} Metadaten in der GDI-DE übernommen.

Kontakt (Verantwortliche Stelle Metadaten)
------------------------------------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☒               ☐             ☐
  zusätzlich für INSPIRE   ☐               ☐             ☐

Ein Metadatensatz muss immer eine Information über die für die
Erstellung und Pflege der Metadaten zuständige Stelle beinhalten. Diese
Information muss mindestens Folgendes beinhalten:

-   einen Namen im *organisationName*-Element*;*

-   eine E-Mail-Adresse im *electronicMailAddress*-Element;

-   die Rolle „pointOfContact" im *role*-Element.

Diese Konvention beruht auf den Vorgaben aus \[INS TG MD\], 2.2.3
(Requirement C.6) und geht über die Regelungen aus \[ISO 19115\] für das
*CI_ResponsibleParty*-Element in \[ISO 19115\], B.3.2.1, No. 374,
hinaus.

Um die Einheitlichkeit der Metadaten in der GDI-DE zu fördern, wird
diese Konvention für [alle]{.ul} Metadaten in der GDI-DE übernommen.

Kontakt (Verantwortliche Stelle für die Ressource)
--------------------------------------------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☒               ☐             ☐
  zusätzlich für INSPIRE   ☐               ☐             ☐

Ein Metadatensatz muss immer eine Information über die für die Ressource
zuständige Stelle beinhalten. Diese Information muss mindestens
Folgendes beinhalten:

-   einen Namen im *organisationName*-Element*;*

-   eine E-Mail-Adresse im *electronicMailAddress*-Element.

Diese Konvention beruht auf den Vorgaben aus \[INS TG MD\], 2.3.3
(Requirement C.10) und geht über die Regelungen aus \[ISO 19115\] für
das *CI_ResponsibleParty*-Element in \[ISO 19115\], B.3.2.1, No. 374,
hinaus.

Um die Einheitlichkeit der Metadaten in der GDI-DE zu fördern, wird
diese Konvention für [alle]{.ul} Metadaten in der GDI-DE übernommen.

Als **[zusätzliche Empfehlung]{.ul}** gilt: Im *role*-Element wird die
Rolle „pointOfContact" verwendet.

[Hintergrund]{.ul}: Sowohl die Auswertung in der GDI-DE zum
INSPIRE-Monitoring sowie die Ableitung der Metadaten für GovData
berücksichtigen diese Rolle in besonderer Art, d. h. derart
gekennzeichnete Kontakte sind diejenigen, die übernommen bzw. bevorzugt
werden.

Weitere Kontakte mit anderen Rollen bleiben davon unberührt.

Schlüsselwörter
---------------

Schlüsselwörter dienen der schnellen Auffindbarkeit von Daten und
Diensten. Häufig werden Schlüsselwörter verwendet, um Geodatenressourcen
zu bestimmten Fachthemen such- bzw. auffindbar zu machen oder um die
Geodatenressourcen in einem lokalen Zusammenhang, z. B. in einem Portal
gesammelt darstellen zu können. In diesem Dokument wird jedoch nur Bezug
auf Schlüsselwörter genommen, die für die GDI-DE in ihrer Gesamtheit
gültig sind.

### Schlüsselwort „inspireidentifiziert"

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☐             ☐
  zusätzlich für INSPIRE   ☒               ☐             ☐

Metadatensätze, die von INSPIRE betroffene Geodatensätze oder --dienste
beschreiben, werden mit dem Eintrag des Schlüsselworts
„**inspireidentifiziert**" im *keyword*-Element (\[[ISO 19115](#REF7)\],
B.2.2.3, No. 53) gekennzeichnet und werden dadurch beim
INSPIRE-Monitoring berücksichtigt.

Das Schlüsselwort „inspireidentifiziert" ist keinem Thesaurus entnommen
und ist ohne Quellenangabe in den Metadaten zu führen.

Beschränkungen des öffentlichen Zugangs (\[INS VO MD\], B 8.2)
--------------------------------------------------------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☐             ☐
  zusätzlich für INSPIRE   ☒               ☐             ☐

Dieser Abschnitt beschreibt, wie Zugriffseinschränkungen im Sinne des
INSPIRE-Elements \"Beschränkungen des öffentlichen Zugangs\"
entsprechend der \[INS TG MD\] zu erfassen sind. Dabei sind
Beschränkungen des öffentlichen Zugangs nur in den in Artikel
13(1) a) - h) der INSPIRE-Richtlinie genannten Fällen zulässig.

Die Beschränkungen des öffentlichen Zugangs sind nach \[INS TG MD\],
2.3.6 (Requirement C.17), innerhalb eines gemeinsamen
*MD_LegalConstraints*-Objekts in folgenden Elementen anzugeben:

-   [genau ein]{.ul} *accessConstraints*-Element, Codelisten-Wert
    \"**otherRestrictions**\" aus *MD_RestrictionCode* (\[ISO 19115\],
    B.5.24)

[und]{.ul}

-   [ein oder mehrere]{.ul} *otherConstraints*-Elemente; jedes enthält
    einen Grund für die Beschränkung des öffentlichen Zugangs nach
    Artikel 13(1) a) - h) der INSPIRE-Richtlinie als
    *gmx:Anchor*-Element (Verweis auf einen Eintrag in der seitens
    INSPIRE bereitgestellten Codeliste zu LimitationsOnPublicAccess). Da
    die Metadaten-Sprache Deutsch ist, soll die zusätzliche
    Text-Ausprägung die deutsche Übersetzung des angegebenen
    Codelisten-Wertes beinhalten. Die Tabelle im *Anhang 3:
    Beschränkungen des öffentlichen Zugangs bei INSPIRE* enthält die o.
    g. Gründe nach Artikel 13 der INSPIRE-Richtlinie und listet den
    jeweils benötigten Eintrag für das *gmx:Anchor*-Element sowie für
    den deutschsprachigen Begleittext auf.

Liegen [keine]{.ul} Beschränkungen vor, so ist im
*otherConstraints*-Element statt eines Grundes für die Beschränkung der
Verweis zum Codelisten-Wert \"**noLimitations**\" der INSPIRE-Codeliste
zu LimitationsOnPublicAccess[^4] ebenfalls als *gmx:Anchor*-Element
einzutragen. Zur semantischen Abgrenzung gegenüber den
Nutzungsbedingungen (siehe 2.9) wird als deutschsprachige Entsprechung
der Freitext „Es gelten keine Zugriffsbeschränkungen" empfohlen.
Alternativ kann der für diesen Zweck bisher dokumentierte Freitext „Es
gelten keine Bedingungen" beibehalten werden.

Nutzungs- und Zugriffsbedingungen
---------------------------------

### Nutzungs- und Zugriffsbedingungen in der GDI-DE (ohne INSPIRE)

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☒               ☐             ☐
  zusätzlich für INSPIRE   ☐               ☐             ☐

Dieser Abschnitt beschreibt, wie Nutzungs- und Zugriffsbedingungen in
den Metadaten der GDI-DE dokumentiert werden, sofern es sich um eine
Ressource handelt, die [nicht]{.ul} unter die INSPIRE-Richtlinie fällt.
Sonst gelten stattdessen die Regelungen für das INSPIRE-Element
\"Bedingungen für den Zugang und die Nutzung\" unter 2.9.2.

Die Bedingungen für den Zugang und die Nutzung sind innerhalb eines
gemeinsamen *MD_LegalConstraints*-Objekts anzugeben. Dadurch wird
sichergestellt, dass textliche Erläuterungen zweifelsfrei der ggf.
dokumentierten Beschränkungsart zugeordnet werden können.

In den Metadaten der GDI-DE besteht das *MD_LegalConstraints*-Objekt für
Nutzungs- und Zugriffsbedingungen aus folgenden Elementen:

-   [verpflichtend mindestens ein]{.ul} *useConstraints*-Element; Inhalt
    ist Codelisten-Wert aus *MD_RestrictionCode* (\[ISO 19115\],
    B.5.24); empfohlener Inhalt: „**otherRestrictions**";

[und]{.ul}

-   [bedingt verpflichtend]{.ul} (falls *useConstraints* mit
    „**otherRestrictions**" belegt wurde) [mindestens ein]{.ul}
    *otherConstraints*-Element; in welchem die Nutzungs- und
    Zugriffsbedingungen sowie Informationen über etwaige Gebühren in
    Textform oder als Verweis (URL) zu dokumentieren sind.

*Anmerkung: In Anlehnung an die INSPIRE-Anforderung, immer eine Aussage
zu Nutzungs- und Zugriffsbedingungen in den Metadaten zu führen und
diese in der GDI-DE ausschließlich und einheitlich in den ISO-Elementen
useConstraints/otherConstraints abzulegen (siehe* *2.9.2), wird an
dieser Stelle zwecks Einheitlichkeit auch für diejenigen Ressourcen, die
[nicht]{.ul} unter die INSPIRE-Richtlinie fallen, als GDI-DE-Konvention
festgelegt, die gleiche Struktur (d. h. die ISO-Elemente
useConstraints/otherConstraints) zu verwenden. Die inhaltliche Belegung
ist für Ressourcen, die unter die INSPIRE-Richtlinie fallen, jedoch
restriktiver.*

Für den Fall, dass [keine]{.ul} Bedingungen gelten oder die Bedingungen
[unbekannt]{.ul} sind, ist dies ebenfalls zu dokumentieren. Der Eintrag
erfolgt als deutschsprachiger Freitext „Es gelten keine Bedingungen"
(siehe folgendes Beispiel) oder „Bedingungen unbekannt".

*Anmerkung: Eine „unbekannte" Bedingung ist für den Nutzer nicht
hilfreich und sollte möglichst konkretisiert werden.*

### Bedingungen für den Zugang und die Nutzung bei INSPIRE (\[INS VO MD\], B 8.1)

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☐             ☐
  zusätzlich für INSPIRE   ☒               ☐             ☐

Dieser Abschnitt beschreibt, wie Nutzungs- und Zugriffsbedingungen im
Sinne des INSPIRE-Elements \"Bedingungen für den Zugang und die
Nutzung\" entsprechend der \[INS TG MD\] zu erfassen sind.

Die Bedingungen für den Zugang und die Nutzung sind nach \[INS TG MD\],
2.3.7 (Requirement C.18), innerhalb eines gemeinsamen
*MD_LegalConstraints*-Objekts nach einer vorgegebenen Bildungsregel
anzugeben. Für die GDI-DE wird diese zwecks Einheitlichkeit weiter
spezifiziert, so dass folgende Elemente erforderlich sind:

-   [genau ein]{.ul} *useConstraints*-Element, Codelisten-Wert
    \"**otherRestrictions**\" aus *MD_RestrictionCode* (\[ISO 19115\],
    B.5.24)

> [und]{.ul}

-   [mindestens ein]{.ul} *otherConstraints*-Element; in welchem die
    Nutzungs- und Zugriffsbedingungen sowie Informationen über etwaige
    Gebühren in Textform oder als Verweis (URL) zu dokumentieren sind.

*Anmerkung: Seitens INSPIRE besteht die Anforderung, immer eine Aussage
zu den Bedingungen für den Zugang und die Nutzung in den Metadaten zu
führen und diese entweder in den ISO-Elementen
useConstraints/otherConstraints oder accessConstraints/otherConstraints
abzulegen. Zwecks Einheitlichkeit in der GDI-DE und zur Abgrenzung von
den Beschränkungen des öffentlichen Zugangs (siehe* *2.8) wurde
festgelegt, hier ausschließlich die ISO-Elemente
useConstraints/otherConstraints zu verwenden.*

Für den Fall, dass [keine]{.ul} Bedingungen gelten oder die Bedingungen
[unbekannt]{.ul} sind, ist dies entsprechend \[INS VO MD\], Teil B 8.1,
zu dokumentieren. Die Einträge erfolgen gem. \[INS TG MD\], 2.3.7
(Requirement C.18), als *gmx:Anchor*-Element mit Verweis auf einen
Eintrag in der seitens INSPIRE bereitgestellten Codeliste
ConditionsApplyingToAccessAndUse[^5] über die Werte
\"**noConditionsApply"** bzw. „**conditionsUnknown**" sowie den
zugehörigen deutschsprachigen Texten (siehe folgende Beispiele).

*Anmerkung: Eine „unbekannte" Bedingung ist für den Nutzer nicht
hilfreich und sollte möglichst konkretisiert werden.*

Regionalschlüssel
-----------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☐             ☒
  zusätzlich für INSPIRE   ☐               ☐             ☐

**[Empfehlung:]{.ul}** Geodaten und Geodatendienste, die einen
räumlichen Bereich in Form einer bestimmten Verwaltungseinheit abdecken,
können über deren 12-stelligen Regionalschlüssel (RS) gezielt auffindbar
gemacht werden, wenn der entsprechende Schlüssel in den Metadaten
hinterlegt wird. Die Angabe in den Metadaten ist optional, wird aber
empfohlen, um Auswertungen zu ermöglichen.

Alternativ kann die Kodierung auch in einem *CharacterString*-Element
erfolgen:

Der Regionalschlüssel wird vom Statistischen Bundesamt veröffentlicht
\[DESTATIS\].

Die in den Beispielen genannten URL (z. B.
https://registry.gdi-de.org/id/\<namespaceRS\>/033595407004) enthalten
persistente Identifikatoren für den Schlüssel. Diese verweisen auf einen
WFS, der u. a. die Geometrie der Verwaltungseinheit ausgibt.

Kennzeichnung der Verbindlichkeit von per Darstellungs- und/oder Downloaddienst bereitgestellten Daten
------------------------------------------------------------------------------------------------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☐             ☒
  zusätzlich für INSPIRE   ☐               ☐             ☐

Um in Zukunft rechtsgültige Auskunftssysteme auf Basis von
Geodatendiensten zu ermöglichen, soll die Verbindlichkeit von Daten, die
mittels Diensten bereitgestellt werden, automatisiert ausgewertet werden
können. Eine mögliche Ausprägung dieser Verbindlichkeit kann der Status
„amtliche Daten" sein. Damit Planer und Entscheider unmittelbar erkennen
können, inwieweit die vorliegenden Informationen für die Beantwortung
ihrer jeweiligen Fragestellung ausreichend verbindlich sind, wird eine
Information darüber in der Qualitätsaussage in den Metadaten hinterlegt.

Die Angabe der Verbindlichkeit in den Daten- und den Dienst-Metadaten
ist optional, wird aber wie folgt empfohlen:

Unter *dataQualityInfo* wird im entsprechenden
*DQ_ConformanceResult*-Element in

-   *specification* die rechtliche Grundlage (z. B. Verordnung,
    gesetzlicher Rahmen) zitiert;

-   *explanation* ein Freitext wie z. B.

    -   „amtlicher Dateninhalt",

    -   „Bei diesen Daten handelt es sich um einen amtlichen
        Dateninhalt." oder

    -   „Dieser Dienst präsentiert amtliche Daten." angegeben;

-   *pass* der Wert „true" gesetzt, um zu kennzeichnen, dass die
    benannte Rechtsgrundlage tatsächlich zu Grunde liegt.

Das folgende Beispiel zeigt, wie die Verbindlichkeit in Bezug auf eine
konkrete gesetzliche Regelung im Metadatensatz abgebildet werden kann:

Konformität (Übereinstimmung mit Spezifikationen, \[INS VO MD\], B 7)
---------------------------------------------------------------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☐             ☐
  zusätzlich für INSPIRE   ☒               ☐             ☐

Gemäß \[INS VO MD\], B 7 und \[[INS TG MD](#REF1)\], 2.4.1 (Requirements
C.20 bis C.22) ist in den Metadaten zu dokumentieren, ob die
beschriebene Ressource gegenüber einer Spezifikation geprüft wurde und
ob diese Überprüfung erfolgreich war. Grundsätzlich ist die Konformität
mindestens bzgl. der jeweils relevanten Durchführungsbestimmung
anzugeben. Mit der Aussage zur Konformität wird ausgedrückt, ob

-   die Daten bereits im INSPIRE-Datenmodell vorliegen und
    bereitgestellt werden (Daten-Metadaten: Übereinstimmung mit der
    Durchführungsbestimmung zur Interoperabilität, IR 1089/2010);

-   der Dienst die Vorgaben (Funktionen, Performanz, Capabilities etc.)
    für Netzdienste einhält (Dienst-Metadaten: Übereinstimmung mit der
    Durchführungsbestimmung zu Netzdiensten, IR 976/2009);

In [zusätzlichen]{.ul} Elementen können weitere Spezifikationen wie
z. B. Änderungsverordnungen, die die Durchführungsbestimmungen
betreffen, sowie Technical Guidance-Dokumente, z. B.
Datenspezifikationen oder zu Darstellungs- bzw. Downloaddiensten,
referenziert werden.

Die Informationen werden je zitierter Spezifikation in einem eigenen
*DQ_ConformanceResult*-Element mit *specification*, *explanation* und
*pass* (\[ISO 19115\], B.2.4.4, No. 129 bis No. 132) angegeben:

-   *specification*-Element: Für den Titel der Spezifikation wird das
    *title*-Element (\[ISO 19115\], B.3.2.1, No. 360) aus *CI_Citation*
    verwendet. Das Element kann als Freitext (gco:CharacterString) oder
    Verweis (gmx:Anchor mit xlink:href auf einen seitens der EU
    festgelegten Link plus Freitext) codiert werden. Die Abschnitte 3.5
    (für Datensätze und -serien) bzw. 4.6 (für Netzdienste) regeln
    Benennung und Schreibweise der jeweiligen Durchführungsbestimmung,
    die zusammen mit dem angegebenen Veröffentlichungsdatum zu verwenden
    ist. Dort ist auch der jeweilige Link für den Verweis mittels
    gmx:Anchor dokumentiert und Beispiele abgebildet. Im *Anhang 1:
    INSPIRE-Spezifikationen (Durchführungsbestimmungen)* sind die in
    Frage kommenden INSPIRE Durchführungsbestimmungen abermals
    aufgelistet.

-   *explanation*-Element: Hier kann grundsätzlich Freitext eingetragen
    werden. Beispielsweise können Angaben zu den verwendeten Anwendungen
    bei der Überprüfung der Konformität gemacht werden (siehe Kapitel
    7).

-   *pass-*Element: Gemäß \[ISO 19115\] ist der Wertebereich von *pass*
    auf 0 (= nein) und 1 (= ja) festgelegt. INSPIRE definiert abweichend
    davon, aber in Übereinstimmung mit \[ISO 19139\], die zulässigen
    Werte als **true** und **false**. Wurde die Übereinstimmung mit der
    Spezifikation noch nicht überprüft, kann das Element leer bleiben,
    sofern im *pass-*Element das Attribut **nilReason="unknown"**
    angegeben wird.

Angaben zum Raumbezug / Koordinatenreferenzsystem (EPSG-Code)
-------------------------------------------------------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☒             ☐
  zusätzlich für INSPIRE   ☐               ☐             ☐

**Bedingung für das Gelten dieser Konvention:** Die zu beschreibende
Ressource besitzt einen absoluten Raumbezug.

Für Geodaten soll das Koordinatenreferenzsystem, in dem die
beschriebenen Geodaten tatsächlich vorliegen, als EPSG-Code[^6] in den
Metadaten hinterlegt werden. Für Geodatendienste sollen die EPSG-Codes,
in denen der Dienst die Geodaten bereitstellen kann, in den Metadaten
hinterlegt werden.

Der EPSG-Code (z. B. „4326" für das Koordinatenreferenzsystem „WGS 84")
ist ein konkreter Identifikator für das Referenzsystem gemäß
http://www.epsg-registry.org/. Im Zusammenspiel mit dem Namensraum kann
eine abstrakte und maschinenlesbare Beschreibung der Projektion im
GML-Format abgerufen werden[^7].

Für alle Daten und Dienste in der GDI-DE ist der entsprechende
Identifikator mindestens in Textform zu hinterlegen (siehe erstes
Beispiel). Alternativ kann dies in Form eines Verweises als gmx:Anchor
erfolgen (siehe zweites Beispiel). Für beide Varianten wird analog zu
den INSPIRE-Vorgaben als Identifier der HTTP URI Identifier für das
opengis.net-Repository[^8] vorgeschrieben.

In Metadaten zu INSPIRE-Datensätzen oder -serien ist bereits nach \[INS
TG MD\], 3.2.1.1 (Requirement 2.2) die Angabe des Referenzsystems als
HTTP URI Identifier verpflichtend, [sofern]{.ul} der anzugebende
Identifikator im Anhang D.4 „Default Coordinate Reference System
Identifiers" aufgeführt ist. Diese Verpflichtung gilt unverändert und
wird durch die vorliegende Konvention mit abgedeckt. Um die
Einheitlichkeit der Metadaten in der GDI-DE zu fördern, wird diese
Konvention für alle Metadaten in der GDI-DE übernommen.

Für die empfohlene Referenzierung mittels gmx:Anchor (\[INS TG MD\],
3.2.1.1, Recommendation 2.2) ist für den genannten HTTP URI Identifier
http://www.opengis.net/def/crs/EPSG/0/\[EPSG-Code\] zu verwenden (siehe
zweites Beispiel).

*Hinweis: Für Projektionen der World Meteorological Organisation (WMO)
ist das WMO-Register entsprechend zu zitieren*[^9]*.*

Konventionen für Metadaten zu Datenbeständen und Anwendungen
============================================================

Die Konventionen in diesem Kapitel betreffen die Metadaten zu allen
Ressourcen in der GDI-DE, die keine Dienste sind, d. h. deren Inhalt im
*hierarchyLevel*-Element [ungleich]{.ul} „service" ist (siehe 2.3).
Somit fallen auch Metadaten zu Anwendungen (z. B. Portale) darunter,
deren Metadatenstruktur in ISO 19115 analog zu Metadaten zu
Datenbeständen geregelt ist.

Eindeutiger Ressourcenidentifikator (\[INS VO MD\], B 1.5)
----------------------------------------------------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☒               ☐             ☐
  zusätzlich für INSPIRE   ☐               ☐             ☐

Die Angabe des eindeutigen Ressourcenidentifikators erfolgt im
*identificationInfo*-Element (ISO 19115, B.2.1, No. 15). Gemäß den
INSPIRE-Vorgaben in \[INS TG MD\], 3.1.2.1, Requirement 1.3, ist dieser
aus einem **Namensraum** (**namespace**) und einem lokalen
**Identifikator** (**localID**) zu bilden. Der lokale Identifikator ist
eine Zeichenkette und wird i. d. R. vom Eigentümer der Daten vergeben.
Der Namensraum, z. B. für eine Organisation, definiert den Kontext, in
dem der lokale Identifikator vergeben wird. Innerhalb eines Namensraumes
identifiziert ein lokaler Identifikator eindeutig eine Ressource (\[INS
VO MD\], B.1.5; \[INS Generic Conceptual Model\], 14.2).

Für die Bildung des eindeutigen Ressourcenidentifikators gelten folgende
Regeln:

1.  Der Ressourcenidentifikator ist ein gültiger „Unique Resource
    Identifier" (URI) \[RFC 3986\].

2.  Die Abbildung des Ressourcenidentifikators erfolgt über das
    *MD_Identifier/code*-Element (ISO 19115, B.2.7.3, No. 205/207)[^10].

3.  Der *code* wird aus Namensraum und lokalem Identifikator
    zusammengesetzt. Hierfür wird die localID an den namespace
    angehängt, getrennt durch „/" (namespace/localId).

4.  Nach Möglichkeit soll der verwendete Namensraum über die GDI-DE
    Registry[^11] verwaltet werden. Weitere Informationen dazu sind im
    GDI-DE Wiki[^12] zu finden.

5.  Sofern der verwendete Namensraum [nicht]{.ul} über die GDI-DE
    Registry verwaltet wird, ist (technisch) selbstständig
    sicherzustellen, dass dieser im Hinblick auf die gewünschte Funktion
    (Direktzugriff auf das XML des Daten-Metadatensatzes) dennoch
    aufgelöst werden kann, um die erforderliche Konformität zu
    gewährleisten.

*Hinweis: Der im Beispiel genannte Namensraum
„**https://registry.gdi-de.org/id/de.nw**" ist ein Platzhalter. Dieser
setzt sich aus einem für alle Namensräume festgelegten Prefix (z. B.
<https://registry.gdi-de.org/id/> ) und einem domänenspezifischen Teil
(z. B. „de.nw") zusammen. Der domänenspezifische Teil entsteht erst
durch Registrierung des Namensraums in der GDI-DE Registry.*

Schlüsselwörter 
---------------

### Quellenangabe für Schlüsselwörter zu INSPIRE-Themen

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☐             ☐
  zusätzlich für INSPIRE   ☒               ☐             ☐

In Metadaten zu INSPIRE-Datensätzen oder -serien ist nach \[INS TG MD\],
3.1.2.2 (Requirement 1.4) die Angabe mindestens eines Schlüsselworts
notwendig, das dem Thesaurus „GEMET - INSPIRE themes" entstammt. Dieser
Thesaurus ist zudem nach \[INS TG MD\], 2.3.5 (Requirement C.15) als
Quellenangabe anzugeben bzw. zu bennen.

Für die Metadaten in der GDI-DE werden die Anforderungen an die
Quellenangabe wie folgt präzisiert, um die Einheitlichkeit der Metadaten
zu fördern und Weiterverwendungen im EU-Kontext zu unterstützen:

-   *title*-Element: „GEMET - INSPIRE themes, version 1.0"

-   *date*-Element: „2008-06-01" mit *dateType*="publication"

### Schlüsselwort „opendata"

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☒             ☐
  zusätzlich für INSPIRE   ☐               ☐             ☐

**Bedingung für das Gelten dieser Konvention:** Die zu beschreibende
Ressource fällt unter Open Data.

Metadaten zu Datensätzen und -serien, die über den Geodatenkatalog.de
für GovData bereitgestellt werden sollen, müssen im *keyword*-Element
(\[[ISO 19115](#REF7)\], B.2.2.3, No. 53) das Schlüsselwort
„**opendata**" enthalten.

Das Schlüsselwort „opendata" ist keinem Thesaurus entnommen und ist ohne
Quellenangabe in den Metadaten zu führen.

Themenkategorie nach ISO (Zuordnung zum INSPIRE-Thema: \[INS VO MD\], B 2.1)
----------------------------------------------------------------------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☐             ☐
  zusätzlich für INSPIRE   ☒               ☐             ☐

In Metadaten zu Datensätzen oder -serien ist die Angabe mindestens einer
ISO-Themenkategorie notwendig (\[ISO 19115\], \[[INS VO MD](#REF1)\],
Teil B, 2.1[^13], \[INS TG MD\], 3.1.2.5, Requirement 1.7). Um für
INSPIRE darüber hinaus eine sachlich und inhaltlich richtige Zuordnung
von INSPIRE-Themen zu ISO-Themenkategorien zu gewährleisten, die durch
\[INS VO MD\], Teil D vorgegeben ist, ist die Zuordnungstabelle aus

*\
*anzuwenden. Dabei ist in der XML-Abbildung stets die Schreibweise der
Spalte ISO-Themenkategorie -- EN zu verwenden.

Handelt es sich beispielsweise um das INSPIRE-Thema Gewässernetz
(entscheidend ist die Angabe von INSPIRE-Themen und deren Schreibweise
gem. GEMET in den Schlüsselwörtern), ist hier die zugehörige
ISO-Themenkategorie „inlandWaters" (Binnengewässer) anzugeben:

Ressourcenverweis für Datensätze und -serien (transferOptions, \[INS VO MD\], B 1.4)
------------------------------------------------------------------------------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☐             ☐
  zusätzlich für INSPIRE   ☐               ☒             ☐

**Bedingung für das Gelten dieser Konvention:** Die für INSPIRE zu
beschreibende Ressource bzw. zu beschreibenden Informationen hierzu sind
online zugänglich.

Aufgrund der INSPIRE-Vorgaben (\[[INS VO MD](#REF2)\], B.1.4) sind die
Ressourcenverweise in den Metadaten für Datensätze und -serien bedingt
verpflichtend. Diese müssen angegeben werden, falls solche Ressourcen
(s. u.) vorhanden bzw. zugänglich sind. Gemäß \[[INS TG MD](#REF1)\],
3.1.3.1 (Requirement 1.8) ist der Zugriffspunkt unter *transferOptions*
(ISO 19115, B.2.10.1, No. 270 *MD_Distribution* / No. 274
*MD_DigitalTransferOptions*) einzutragen.

Im *CI_OnlineResource*-Element soll gemäß \[[INS TG MD](#REF1)\],
3.1.3.1 (Recommendation 1.9) eine gültige URL auf eine der folgenden
Ressourcen hinterlegt werden:

-   eine Möglichkeit zum direkten Download der beschriebenen Daten

-   ein Capabilities-Dokument eines Dienstes

-   eine WSDL-Datei (SOAP-Binding)

-   eine Client-Anwendung, die einen direkten Zugriff auf den
    beschriebenen Datensatz gewährt

-   eine Webseite, die weitere Anleitungen bzw. Informationen enthält

Die Funktion der hinterlegten URL in *CI_OnlineResource* kann im
*function*-Element über die Begriffe der Codeliste B.5.3
*CI_OnLineFunctionCode* aus \[[ISO 19115](#REF7)\] annotiert werden.
Dies wird durch \[INS TG MD\], 3.1.3.1 (Recommendation 1.8) empfohlen,
ist aber nicht verpflichtend. Eine naheliegende und sinnvolle Verwendung
in Metadaten zu Datensätzen und -serien wird dabei für folgende Begriffe
der Codeliste gesehen:

-   *information* - für den Link auf eine Webseite, die weitere
    Anleitungen bzw. Informationen enthält

-   *download* - für den Link zum unmittelbaren Herunterladen der
    beschriebenen Daten.

*Hinweis: Die Hinterlegung eines Links zum direkten Download der
beschriebenen Daten (s. o.) entbindet [nicht]{.ul} von der Verpflichtung
seitens INSPIRE, einen Datenbestand per Downloaddienst (z. B. WFS oder
Atom-Feed) verfügbar zu machen und diesen mittels eines eigenen
Dienst-Metadatensatzes zu dokumentieren.*

*Hinweis: Das im Beispiel verwendete Element „name" ist optional und
unterliegt [nicht]{.ul} der hier dokumentierten GDI-DE-Konvention. In
diesem Element [kann]{.ul} der hinterlegte Link (zusätzlich zur
Kennzeichnung im Element „function") näher erläutert werden.*

Konformität (Übereinstimmung mit Spezifikationen, \[INS VO MD\], B 7)
---------------------------------------------------------------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☐             ☐
  zusätzlich für INSPIRE   ☒               ☐             ☐

Ergänzend zu den grundsätzlichen Konventionen zur Konformitätsaussage in
2.12 wird an dieser Stelle das Zitat der anzugebenden Spezifikation
geregelt. In Metadaten zu INSPIRE-Datensätzen oder -serien ist gem.
\[INS TG MD\], 3.1.4.2, Requirement 1.10 die Verordnung 1089/2010
(Interoperabilität von Geodatensätzen und -diensten) zu zitieren, um
dokumentieren, [ob die Daten bereits im INSPIRE-Datenmodell
vorliegen]{.ul}.

Dazu sind folgende Angaben erforderlich:

-   Titel: **VERORDNUNG (EG) Nr. 1089/2010 DER KOMMISSION vom 23.
    November 2010 zur Durchführung der Richtlinie 2007/2/EG des
    Europäischen Parlaments und des Rates hinsichtlich der
    Interoperabilität von Geodatensätzen und -diensten**

-   Veröffentlichungsdatum: **2010-12-08**

Für die empfohlene Referenzierung mittels gmx:Anchor (\[INS TG MD\],
3.1.4.2, Recommendation 1.10) ist für die genannte
Durchführungsbestimmung <http://data.europa.eu/eli/reg/2010/1089> zu
verwenden (siehe zweites Beispiel).

Nutzungsbedingungen und Lizenzinformationen für Open Data
---------------------------------------------------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☒             ☐
  zusätzlich für INSPIRE   ☐               ☐             ☐

**Bedingung für das Gelten dieser Konvention**: Die zu beschreibende
Ressource fällt unter Open Data.

Dieser Abschnitt beschreibt, wie Nutzungsbedingungen bzw.
Lizenzinformationen zu Open Data in den Metadaten der GDI-DE
dokumentiert werden, um zentral bzw. einheitlich dem GovData-Portal
bereitgestellt und dort verarbeitet werden zu können.

Die Angaben zur Lizenz werden zunächst als Nutzungsbedingung erfasst,
wie es grundsätzlich in 2.9.1 (Nicht-INSPIRE) bzw. 2.9.2 (bei
gleichzeitiger Relevanz für INSPIRE) beschrieben ist.

Darüber hinaus sind die Lizenzinformationen in [genau]{.ul} [einem]{.ul}
zusätzlichen *otherConstraints*-Element (im selben
*MD_LegalConstraints*) im Datenformat JSON (JavaScript Object Notation)
strukturiert anzugeben: Die einzelnen Paare, gebildet aus Parametername
und -wert, werden durch Kommata getrennt und in geschweiften Klammern
eingeschlossen, angegeben. JSON eignet sich an dieser Stelle, da der
relevante Bereich innerhalb des Freitextfeldes recht einfach
identifiziert und ausgewertet werden kann. Mischformen aus JSON und
Freitext innerhalb eines *otherConstraints*-Element müssen zur
Vermeidung von Fehlinterpretationen verhindert werden. Mindestens
folgende Parameter sollen bei der Lizenzbeschreibung gesetzt werden:

-   id: Identifier der Lizenz [^14]

-   name: Name der Lizenz [^15]

-   url: URL, unter welcher der Lizenztext bezogen werden kann [^16]

-   quelle: Text der Namensnennung, unter welcher die Datenquelle bei
    einer Weiternutzung zitiert werden soll

Formatangaben
-------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☐             ☐
  zusätzlich für INSPIRE   ☒               ☐             ☐

Gemäß \[INS VO Interop\], Art. 13 (3) und \[[INS TG MD](#REF1)\],
3.2.3.1 (Requirement 2.6) ist in den Metadaten zu dokumentieren, in
welchem Format (die \[INS VO Interop\] beschreibt dies als
„Programmiersprachenkonstrukt") die Daten vorliegen. Dies fokussiert auf
das [Dateiformat]{.ul} und weniger auf die logische Struktur der
enthaltenen Daten. In der \[[INS TG MD](#REF1)\] wird dies im Anhang
unter C.3.3 am gewählten Beispiel für eine GML-Datei deutlich.
Gegenstand der hier beschriebenen Konvention ist nicht die
verpflichtende Formatangabe selbst (diese Verpflichtung gilt
unverändert), sondern die Betonung der Aussage im Kommentar unter \[[INS
TG MD](#REF1)\], Anhang C.3.3:

**[Empfehlung:]{.ul}** Die Formatangabe durch die Elemente *name* und
*version* unter *MD_Format* ist ausreichend. Informationen über die
zugrundeliegende logische Datenstruktur (z. B. eine
INSPIRE-Datenspezifikation) sollte entgegen dem Beispiel 3.18 der \[INS
TG MD\] nicht begleitend im *specification-*Element unter *MD_Format*,
sondern als eigenständige Information im separaten Zweig
*MD_ApplicationSchemaInformation* der \[ISO 19115\] geführt werden.

Konventionen für Metadaten zu Diensten
======================================

Die Konventionen in diesem Kapitel betreffen die Metadaten zu allen
Diensten in der GDI-DE, d. h. die Dienste, deren Inhalt im
*hierarchyLevel*-Element [gleich]{.ul} „service" ist (siehe 2.3).

Schlüsselwörter
---------------

### Schlüsselwörter zu Dienstkategorien bei INSPIRE

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☐             ☐
  zusätzlich für INSPIRE   ☒               ☐             ☐

In Metadaten zu Diensten für INSPIRE ist die Angabe mindestens eines
Schlüsselworts erforderlich, das aus dem Teil D (Ziffer 4) der \[[INS VO
MD](#REF1)\] stammt (\[INS VO MD\], Teil B, 3, \[INS TG MD\], 4.1.2.2,
Requirement 3.4). Diese Verpflichtung gilt unverändert.

**[Empfehlung]{.ul}**: Zur Förderung der Einheitlichkeit und der
eindeutigen Interpretierbarkeit der Metadaten sollen in der GDI-DE in
Abhängigkeit der Art des jeweils zu dokumentierenden Dienstes folgende
Schlüsselwörter verwendet werden:

  **Art des Dienstes**                              **Schlüsselwort**
  ------------------------------------------------- ------------------------------
  WMS, WMTS                                         infoMapAccessService
  WFS, predefinedAtom (Vektor)                      infoFeatureAccessService
  WFS-G                                             infoGazetteerService
  WCS, predefinedAtom (Raster)                      infoCoverageAccessService
  CSW                                               infoCatalogueService
  Sensordienste                                     infoSensorDescriptionService
  Anwendung zum Suchen von Geodatenbeschreibungen   humanCatalogueViewer

Verlinkung zum verwendeten Datenbestand (Daten-Dienste-Kopplung)
----------------------------------------------------------------

### Gekoppelte Daten-Ressource (\[INS VO MD\], B 1.6)

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☒             ☐
  zusätzlich für INSPIRE   ☐               ☐             ☐

**Bedingung für das Gelten dieser Konvention:** Es besteht eine
Verbindung zu einer ebenfalls mit Metadaten beschriebenen Datenquelle.

Das INSPIRE-Element „Gekoppelte Ressource / Coupled resource" (\[INS VO
MD\], B.1.6; \[INS TG MD\], 4.1.2.4, Requirement 3.6) wird verwendet, um
die Beziehung zwischen Dienst und zugehörigem Datensatz bzw. zugehörigen
Datensätzen auszudrücken. Die Referenzen auf die vom Dienst
bereitgestellten Datensätze werden dabei im *operatesOn*-Element (ISO
19119, C.1, No. 9) angegeben. Dies entspricht dem grundsätzlichen
Prinzip der Daten-Dienste-Kopplung in der GDI-DE (vgl. Kapitel 5) und
gilt für [alle]{.ul} Metadaten in der GDI-DE.

Laut (\[INS VO MD\], B.1.6; \[ISO 19119\]) kennzeichnet dieses Element
den bereitgestellten Datensatz durch den eindeutigen
Ressourcenidentifikator (URI) des Datensatzes (siehe 3.1). Gemäß \[INS
TG MD\] soll die Referenz dabei jedoch auf ein
*MD_DataIdentification*-Objekt eines Daten-Metadatensatzes verweisen.

Da nach \[INS VO MD\] die Art der Bezugnahme auf die Daten-Metadaten
nicht eindeutig vorgegeben ist, wird für die Gewährleistung der
Interoperabilität innerhalb der GDI-DE die Festlegung getroffen,
auflösbare URLs zu verwenden. Hierfür kann die GDI-DE Registry[^17]
verwendet werden. Zu den dort registrierten Namensräumen kann jeweils
ein Muster für einen Dienst-Aufruf hinterlegt werden. Beim Aufruf der
Referenz wird von der GDI-DE Registry eine Weiterleitung z. B. auf die
hinterlegte URL mit einem *GetRecords*-Aufruf eines CSW durchgeführt.
Weitere Informationen dazu sind im GDI-DE Wiki[^18] zu finden.

### Art der Kopplung zwischen Dienst und zugehörigen Daten

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☒             ☐
  zusätzlich für INSPIRE   ☐               ☐             ☐

**Bedingung für das Gelten dieser Konvention:** Es besteht eine
Verbindung zu einer ebenfalls mit Metadaten beschriebenen Datenquelle.

In den Dienst-Metadaten ist neben den verknüpften Daten-Metadaten auch
die Art der Kopplung anzugeben (ISO 19119, *SV_CouplingType*). Dabei
sind die Werte „eng" (tight), „gemischt" (mixed) und „lose" (loose)
zulässig.

Es ist davon auszugehen, dass in der Regel ein WMS „eng" (tight),
kaskadierende Dienste „gemischt" (mixed) und Downloaddienste ebenfalls
„eng" (tight) gekoppelt sind. Je nach Struktur der Katalogtopologie
können Suchdienste sowohl „lose", „eng" oder „gemischt" gekoppelt sein.

Ressourcenverweise für Dienste
------------------------------

### Ressourcenverweis unter transferOptions (\[INS VO MD\], B 1.4)

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☐             ☐
  zusätzlich für INSPIRE   ☐               ☒             ☐

**Bedingung für das Gelten dieser Konvention:** Die für INSPIRE zu
beschreibende Ressource bzw. Informationen dazu sind online zugänglich.

Aufgrund der INSPIRE-Vorgaben (\[[INS VO MD](#REF2)\], B.1.4) ist ein
Ressourcenverweis in den Metadaten für Dienste bedingt verpflichtend.
Dieser muss angegeben werden, falls solche Ressourcen (s. u.) vorhanden
bzw. zugänglich sind (\[INS VO MD\], Tabelle 2: „wenn ein Link auf den
Dienst verfügbar ist"). Gemäß \[[INS TG MD](#REF1)\], 4.1.3.1
(Requirement 3.7) ist der Zugriffspunkt unter *transferOptions* (ISO
19115, B.2.10.1, No. 270 *MD_Distribution* / No. 274
*MD_DigitalTransferOptions*) einzutragen.

Im *CI_OnlineResource*-Element soll gemäß \[[INS TG MD](#REF1)\],
4.1.3.1 (Recommendation 3.5) eine gültige URL auf eine der folgenden
Ressourcen hinterlegt werden:

-   ein Capabilities-Dokument eines Dienstes

-   eine WSDL-Datei (SOAP-Binding)

-   eine Webseite, die weitere Anleitungen bzw. Informationen enthält

Diese Alternativen sind jedoch nicht als gleichwertig zu betrachten, da
sich aus \[INS TG MD\], 4.1.3.1 (Requirement 3.7) weiter ergibt, dass
ein direkter Link (GetCapabilities-Request) gegenüber einem Link, der zu
ersatzweisen Informationen über den Dienst führt, zu bevorzugen ist.

Zusammengefasst ergibt sich für die GDI-DE die Pflicht, den
GetCapabilities-Request des Dienstes einzutragen, wenn der Online-Zugang
zum Dienst verfügbar ist.

Handelt es sich bei der Ressource um einen Atom-Download-Dienst, so ist
hier die URL des Service Feed einzutragen.

Die Funktion der hinterlegten URL in *CI_OnlineResource* kann im
*function*-Element über die Begriffe der Codeliste B.5.3
*CI_OnLineFunctionCode* aus \[[ISO 19115](#REF7)\] annotiert werden.
Dies wird durch \[INS TG MD\], 4.1.3.1 (Recommendation 3.4) empfohlen,
ist aber nicht verpflichtend. Eine naheliegende und sinnvolle Verwendung
in Metadaten zu Diensten wird dabei für folgenden Begriff der Codeliste
gesehen:

-   *information* -- für den Link auf das Capabilities-Dokument des
    Dienstes oder eine Webseite, die weitere Anleitungen bzw.
    Informationen enthält

### Ressourcenverweis unter connectPoint

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☒               ☐             ☐
  zusätzlich für INSPIRE   ☐               ☐             ☐

Für jeden Dienst-Metadatensatz gilt, dass die URL zum Dienst unter
*connectPoint* (\[ISO 19119\], Table C.2 No. 6) geführt werden muss.
Hier ist die URL einzutragen, unter der das Capabilities-Dokument bzw.
der Service Feed des Dienstes (Atom) bezogen werden kann (siehe auch
Kapitel 5).

Begleitet wird diese Angabe vom *operationName*-Element, das z. B.
aussagt, dass es sich bei dem angegebenen Link um ein Anfordern des
Capabilities-Dokumentes handelt. Unter dem XML-Element „gmd:URL" wird in
diesem Fall kein kompletter GetCapabilities-Request abgelegt. Bei
Atom-Feeds ist für *operationName* ein entsprechender Wert, z. B.
„Download", zu setzen.

Art des Geodatendienstes bei INSPIRE (\[INS VO MD\], B 2.2)
-----------------------------------------------------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☐             ☐
  zusätzlich für INSPIRE   ☒               ☐             ☐

Die Festlegung über die Art des Geodatendienstes wird mit dem
*serviceType*-Element (\[ISO 19119\], Table C.1) umgesetzt. Die von
INSPIRE vorgesehene Werteliste (\[[INS TG MD](#REF1)\], 4.2.1.1
(Requirement 4.1)) ist nicht konform zur OGC CSW-Spezifikation \[OGC CSW
ISO AP\]. Letztere verlangt die OGC-Bezeichnungen der Dienste. Trotzdem
muss die INSPIRE-Vorgabe umgesetzt werden. Danach sind nur die Werte
„view", „download", „discovery" und „transformation" zulässig. Daher
wird empfohlen, die Art des Geodatendienstes im
*serviceTypeVersion*-Element (4.5) weiter zu spezifizieren.

Version des Geodatendienstes bei INSPIRE
----------------------------------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☐             ☐
  zusätzlich für INSPIRE   ☒               ☐             ☐

Ergänzend zum *serviceType* (4.4) ist im Feld *serviceTypeVersion*
(\[[ISO 19119](#REF7)\], Table C.1 No. 2) die OGC-Bezeichnung in der
Form „OGC:\<Diensttyp\> \<Version\>" einzutragen, also z. B. „OGC:WMS
1.1.1" oder „OGC:WFS 2.0". Auf die Verwendung äquivalenter
ISO-Bezeichner (z. B. OGC:WMS 1.1.1 = ISO 19128) ist an dieser Stelle
aus Gründen der Einheitlichkeit zu verzichten. In Abhängigkeit vom
jeweiligen *serviceType* ist das *serviceTypeVersion*-Element wie folgt
zu belegen:

  **serviceType**   **serviceTypeVersion**
  ----------------- -------------------------------------------------------------------------
  discovery         „OGC:CSW \<Version\>"
  view              „OGC:WMS \<Version\>" oder „OGC:WMTS \<Version\>"
  download          „OGC:WFS \<Version\>" oder „OGC:WCS \<Version\>" oder „predefined ATOM"

Die Angabe der Versionsnummer ist außer bei „predefined ATOM"
verpflichtend. Die Versionsnummer richtet sich bezüglich ihrer
Schreibweise (2- oder 3-stellig) nach der Version der zugrundeliegenden
OGC-Spezifikation für den Dienst.

Konformität (Übereinstimmung mit Spezifikationen, \[INS VO MD\], B 7)
---------------------------------------------------------------------

                           verpflichtend   konditional   optional
  ------------------------ --------------- ------------- ----------
  GDI-DE                   ☐               ☐             ☐
  zusätzlich für INSPIRE   ☒               ☐             ☐

Ergänzend zu den grundsätzlichen Konventionen zur Konformitätsaussage in
2.12 wird an dieser Stelle das Zitat der anzugebenden Spezifikation
geregelt. In Metadaten zu INSPIRE-Netzdiensten ist gem. \[INS TG MD\],
4.2.2.1, Recommendation 4.1 die Verordnung 976/2009 (Netzdienste) zu
zitieren, um zu dokumentieren, [ob der Dienst die Vorgaben (Funktionen,
Performanz, Capabilities etc. ) für Netzdienste erfüllt]{.ul}.

Dazu sind folgende Angaben erforderlich:

-   Titel: **VERORDNUNG (EG) Nr. 976/2009 DER KOMMISSION vom 19. Oktober
    2009 zur Durchführung der Richtlinie 2007/2/EG des Europäischen
    Parlaments und des Rates hinsichtlich der Netzdienste**

-   Veröffentlichungsdatum: **2009-10-20**

Für die empfohlene Referenzierung mittels gmx:Anchor (\[INS TG MD\],
4.2.2.1, Recommendation 4.2) ist für die genannte
Durchführungsbestimmung <http://data.europa.eu/eli/reg/2009/976> zu
verwenden (siehe zweites Beispiel).

Daten-Dienste-Kopplung
======================

Das Konzept der dienstorientierten Architektur bildet die technische
Grundlage, um die Ziele und Grundlagen der GDI-DE \[GDI-DE Architektur -
Ziele\] umzusetzen. Um die verteilten Ressourcen über webbasierte
Dienste bereitzustellen und nutzbar zu machen, wird das
„Publish-Find-Bind-Muster" verwendet. Dieses wird im Dokument
„Architektur der GDI-DE -- Technik" \[GDI-DE Architektur - Technik\]
ausführlich beschrieben.

Ein wesentlicher Baustein, um das Publish-Find-Bind-Muster erfolgreich
umzusetzen, ist die Kopplung der Metadaten von Geodaten und
Geodatendiensten. Ein Geodatensatz kann dabei über einen oder mehrere
Geodatendienste bereitgestellt werden. Voraussetzung hierfür ist, dass
sowohl der Geodatensatz als auch der Geodatendienst mit Metadaten
beschrieben und diese Metadaten öffentlich zugänglich sind. Ein
Geodatendienst besitzt, zusätzlich zum Metadatensatz im Katalog, eine
technische Beschreibung seiner Funktionalitäten in Form eines
Capabilities-Dokumentes bzw. eines Service Feeds (Atom).

Die Metadaten eines Geodatensatzes geben i. d. R. keine Auskunft
darüber, über welche Geodatendienste der Geodatensatz bereitgestellt
wird. Daher wird die Suche auf die Dienst-Metadatensätze erweitert und
in diesen nach dem Vorkommen des Identifikators des Geodatensatzes
gesucht. Über die *GetCapabilities*-URL bzw. die URL zum Service Feed
(Atom) im Dienst-Metadatensatz ergibt sich die Referenz auf den Dienst
(vgl. Abbildung 3).

![DDK.png](media/image5.png){width="6.3in" height="4.75in"}

Abbildung 4: Kopplung der Geodaten und Geodatendienste

Für die Umsetzung der Daten-Dienste-Kopplung ergeben sich also folgende
Anforderungen:

-   Jeder **Geodatensatz** erhält durch die Beschreibung mit Metadaten
    einen eindeutigen Ressourcenidentifikator, \<ID\>
    ![zahlen](media/image6.png){width="0.14166666666666666in"
    height="0.14166666666666666in"}. Dieser ist nach festgelegten Regeln
    zu bilden und in dem zugehörigen Metadatensatz zu dokumentieren
    (Abschnitt 3.1);

-   Jeder **Metadatensatz**, der Datensätze oder Dienste beschreibt,
    besitzt einen eindeutigen Metadatensatzidentifikator, \<FID\>
    (Abschnitt 2.2);

-   Jeder **Metadatensatz**, der einen **Dienst** beschreibt, enthält
    Referenzen auf die Daten, welche der Dienst bereitstellt
    ![zahlen](media/image7.png){width="0.17916666666666667in"
    height="0.15in"} (Abschnitt 4.2.1);

-   Jeder **Metadatensatz**, der einen **Dienst** beschreibt, enthält
    Angaben über die Art der Kopplung (Abschnitt 4.2.2);

-   Jeder **Metadatensatz**, der einen **Dienst** beschreibt, enthält
    die URL für den GetCapabilities-Request des Dienstes bzw. den
    Service Feed des Dienstes (Atom)
    ![zahlen](media/image8.png){width="0.15in"
    height="0.12916666666666668in"} (Abschnitt 4.3.2);

-   Jedes **Capabilities-Dokument** bzw. jeder **Service Feed** (Atom)
    eines **Dienstes** enthält einen Link auf den Metadatensatz, der den
    Dienst beschreibt
    ![zahlen](media/image9.png){width="0.17083333333333334in"
    height="0.14166666666666666in"} [oder]{.ul} integriert die
    INSPIRE-Metadaten direkt im *ExtendedCapabilities*-Block des
    Capabilities-Dokumentes (\[GDI-DE HE ViewServices\] und \[GDI-DE HE
    DownloadServices\]);

-   Jedes **Capabilities-Dokument** eines **Darstellungsdienstes**
    enthält für jedes Layerelement einen Link auf den Metadatensatz, der
    die Daten beschreibt
    ![zahlen](media/image10.png){width="0.12916666666666668in"
    height="0.13333333333333333in"} sowie eine Referenz auf die Daten
    (genauer gesagt auf den in den Metadaten festgelegten
    Ressourcenidentifikator), die der Dienst visualisiert
    ![zahlen](media/image11.png){width="0.15in"
    height="0.14166666666666666in"} (\[GDI-DE HE ViewServices\]);

-   Jedes **Capabilities-Dokument** eines **Downloaddienstes** enthält
    in jedem *FeatureType*-Element einen Link auf den Metadatensatz, der
    die Daten beschreibt
    ![zahlen](media/image10.png){width="0.12916666666666668in"
    height="0.13333333333333333in"} sowie im
    *ExtendedCapabilities*-Block eine Referenz auf die Daten (genauer
    gesagt auf den in den Metadaten festgelegten
    Ressourcenidentifikator), die der Dienst bereitstellt
    ![zahlen](media/image11.png){width="0.15in"
    height="0.14166666666666666in"}. Beim Service Feed (Atom) wird auf
    den Service Metadatensatz, sowie für jeden eingebundenen
    „Dataset-Entry" auf den Daten-Metadatensatz verwiesen (\[GDI-DE HE
    DownloadServices\]).

Aus Sicht einer Anwendung (C*lient*) ergibt sich daraus z. B. der in
Abbildung 4 dargestellte Ablauf. Die Anwendung sendet z. B. eine
Suchanfrage nach **Datensätzen** an einen Suchdienst. Der Suchdienst
sendet die Antwort in Form von ISO 19139 XML-Dokumenten. Diese enthalten
einen eindeutigen **Ressourcenidentifikator** für die bekannten
Geodatensätze (\<ID\>). Um Dienste zu identifizieren, die diese
Ressourcen anbieten, sendet die Anwendung eine erneute Suchanfrage nach
**Diensten** an den Suchdienst. Dabei wird die **\<ID\> des Datensatzes
als Teil der Suchanfrage** übermittelt. Als Antwort erhält die Anwendung
ein oder mehrere ISO 19139 XML-Dokumente, die die Dienste beschreiben,
welche den gesuchten Datensatz anbieten. Über einen
*GetCapabilities-*Request bzw. *GetDownloadServiceMetadata-*Request
(Atom) erhält die Anwendung Informationen über angebotene Layer bzw.
FeatureTypes der Dienste, wobei jeweils die \<ID\> des angebotenen
Geodatensatzes im Capabilities-Dokument enthalten ist. Mit diesen
Informationen ist die Anwendung nunmehr in der Lage, Darstellungen bzw.
Downloads des Geodatensatzes anzufordern.

![sequenz.png](media/image12.png){width="6.079166666666667in"
height="2.1875in"}

Abbildung 5: Sequenzdiagramm zur Daten-Dienste-Kopplung am Beispiel von
OGC:WMS/WFS

Open Data-Informationen zu Datensätzen und -serien
==================================================

Der IT-Planungsrat hat DCAT-AP.de[^19] als formalen Austauschstandard
für allgemeine offene Verwaltungsdaten festgelegt[^20]. Das bedeutet,
dass die Informationen über Geo-Ressourcen, die unter Open Data fallen
und mit entsprechenden Lizenz- bzw. Nutzungsbedingungen versehen sind,
ebenfalls in Strukturen gem. DCAT-AP.de zu dokumentieren sind. Zur
Vermeidung von Doppelerfassungen wurde eine Vorgehensweise[^21]
etabliert, um die Metadaten aus der GDI-DE auch unter DCAT-AP.de nutzbar
zu machen und eine Auffindbarkeit in Open Data-Portalen[^22] automatisch
zu ermöglichen.

Metadaten zu Datensätzen und -serien, die für GovData[^23]
bereitgestellt werden sollen, [müssen]{.ul} in ausgewählten Elementen
bestimmte Inhalte aufweisen:

1.  In den Schlüsselwörtern wird der Begriff „**opendata**" hinterlegt
    (Details siehe 3.2.2);

2.  Die Angaben zur Lizenz werden als Nutzungsbedingung gem. den
    Konventionen in den Abschnitten 2.9.1 bzw. 2.9.2 erfasst und
    [zusätzlich]{.ul} strukturiert im Datenformat JSON (JavaScript
    Object Notation) hinterlegt (Details siehe 3.6).

[Zusätzlich]{.ul} zu den o. g. Anforderungen müssen Zugriffswege
dokumentiert sein, die bei GovData als sog. „Distributionen"
(Online-Verfügbarkeit) dargestellt werden. Bei Fehlen jeglicher
Informationen über die Online-Verfügbarkeit eines Datensatzes erfolgt
keine Veröffentlichung im GovData-Portal. Daher [muss]{.ul} in den
Metadaten [mindestens eine der folgenden Verlinkungen]{.ul} existieren:

a.  [Daten-Dienste-Kopplung zu den Metadaten]{.ul} eines frei
    zugänglichen Dienstes für den Zugriff auf die dokumentierten Daten
    (siehe Kapitel 5);

b.  [Link zum unmittelbaren Download]{.ul} der dokumentierten Daten
    (siehe Kapitel 3.4).

Die gleichzeitige Verwendung beider Möglichkeiten ist ebenso zulässig
wie auch mehrere gleichartige Verlinkungen parallel.

Werkzeuge zur Überprüfung der Konventionen
==========================================

Für die Überprüfung der Gültigkeit der eigenen Metadaten existieren
verschiedene Anwendungen. Innerhalb der GDI-DE wird die Verwendung der
GDI-DE Testsuite[^24] empfohlen. Dort stehen Tests zur Prüfung von
Metadaten zur Verfügung. Die Tests sind dabei auf Metadaten in deutscher
Sprache ausgerichtet. So kann einerseits überprüft werden, ob die
Anforderung an Metadaten durch ISO und INSPIRE erfüllt werden,
andererseits kann auch die Erfüllung der in diesem Dokument vorliegenden
Konventionen geprüft werden.

Für die Überprüfung von Metadaten stehen verschiedene Testklassen zur
Verfügung:

-   „Metadaten \| Konventionen der GDI-DE für INSPIRE-relevante
    Metadaten"

-   „Metadaten \| Konventionen der GDI-DE für ISO-konforme Metadaten"

Bei den Testklassen mit Bezug auf die Konventionen der GDI-DE ist im
Namen der dieser immer die Version desjenigen Dokumentes \"Konventionen
zu Metadaten\" angegeben, dessen Vorgaben geprüft werden.

Die GDI-DE-Testklassen prüfen neben der Erfüllung der Anforderungen aus
ISO und/oder INSPIRE insbesondere die weitergehenden Anforderungen der
GDI-DE-Konventionen. Die Konformitätsklasse „Metadaten: GDI-DE INSPIRE"
innerhalb der Testklasse „Metadaten \| Konventionen der GDI-DE für
INSPIRE-relevante Metadaten" prüft hingegen nur die Konformität zu den
Anforderungen aus INSPIRE, welche nicht explizit im Konventionendokument
genannt bzw. aufgeführt sind und unverändert gelten.

Mithilfe der GDI-DE Testsuite können neben Metadaten auch
Katalog-/Suchdienste (CSW), Karten-/Darstellungsdienste (WMS) und
Downloaddienste (WFS, Atom) überprüft werden.

Neben der GDI-DE Testsuite gibt es noch weitere Anwendungen zur
Überprüfung der Gültigkeit der Metadaten. Eines dieser Werkzeuge ist der
EU INSPIRE Validator[^25], der zur Überprüfung der Übereinstimmung mit
den INSPIRE-Vorgaben entwickelt wurde. Ferner können Dienste und
INSPIRE-Datenmodelle mit dem Tool geprüft werden. Das Ergebnis der
Überprüfung im INSPIRE-Validator ist ein Richtwert, um die Konformität
der eigenen Metadaten im Hinblick auf INSPIRE festzustellen. Der
Validator wird beständig weiterentwickelt. Im Gegensatz zur GDI-DE
Testsuite können im INSPIRE-Validator die Konventionen dieses Dokumentes
[nicht]{.ul} überprüft werden. Daher ist innerhalb der GDI-DE die GDI-DE
Testsuite das maßgebliche Tool, um die Konformität von Metadaten im
Hinblick auf die vereinbarten Konventionen zu überprüfen.

Die Ergebnisse der Konformitätsprüfung gegenüber dem Datenmodell und den
Anforderungen an INSPIRE-Netzdienste werden in den Metadaten des
entsprechenden Geodatensatzes bzw. Geodatendienstes dokumentiert (siehe
2.12, bzw. 3.5 und 4.6). Die Einhaltung des INSPIRE-Datenmodells wird im
Daten-Metadatensatz dokumentiert. Die Einhaltung der Vorgaben zu einem
INSPIRE-Netzdienst wird im Dienst-Metadatensatz dokumentiert.

Referenzen {#referenzen .list-paragraph}
==========

\[**DESTATIS**\]: Gemeindeverzeichnis
(https://www.destatis.de/DE/ZahlenFakten/LaenderRegionen/Regionales/Gemeindeverzeichnis/Administrativ/Archiv/GVAuszugQ/AuszugGV4QAktuell.xlsx?\_\_blob=publicationFile)

\[**GDI-DE Architektur - Technik**\]: Architektur der GDI-DE -- Technik,
Version 3.4.0

\[**GDI-DE Architektur - Maßnahmen**\]: Architektur der GDI-DE --
Maßnahmenplan, Version 3.3.0

\[**GDI-DE Architektur - Ziele**\]: Architektur der GDI-DE -- Ziele und
Grundlagen, Version 3.1.1

\[**GDI-DE Architektur - Darstellung**\]: Architektur der GDI-DE --
Vorgaben zur Bereitstellung von Darstellungsdiensten, Version 1.0.1

\[**GDI-DE HE ViewServices**\]: Handlungsempfehlungen für die
Bereitstellung von INSPIRE konformen Darstellungsdiensten, Version 1.0

\[**GDI-DE HE DownloadServices**\]: Handlungsempfehlungen für die
Bereitstellung von INSPIRE konformen Downloaddiensten, Version 1.3.0

\[**INS Generic Conceptual Model**\]: INSPIRE Generic Conceptual Model,
Version 3.0, 2008-06-20

\[**INS TG Discovery Services**\]: Technical Guidance for the
implementation of INSPIRE Discovery Services, Version 3.1, 2011-11-07

\[**INS TG Download Services**\]: Technical Guidance for the
implementation of INSPIRE Download Services, Version 3.1, 2013-08-09

\[**INS TG MD**\]: Technical Guidance for the implementation of INSPIRE
dataset and service metadata based on ISO/TS 19139:2007, V. 2.0.1,
2017-03-02

**\[INS TG View Services\]**: Technical Guidance for the implementation
of INSPIRE View Services, Version 3.11, 2013-04-04

\[**INS VO MD**\]: VERORDNUNG (EG) Nr. 1205/2008 DER KOMMISSION vom 3.
Dezember 2008 zur Durchführung der Richtlinie 2007/2/EG des Europäischen
Parlaments und des Rates hinsichtlich Metadaten

\[**INS VO Interop**\]: VERORDNUNG (EG) Nr. 1089/2010 DER KOMMISSION vom
23. November 2010 zur Durchführung der Richtlinie 2007/2/EG des
Europäischen Parlaments und des Rates hinsichtlich der Interoperabilität
von Geodatensätzen und -diensten, geändert durch Verordnung (EU) Nr.
102/2011 der Kommission vom 4. Februar 2011, Verordnung (EU) Nr.
1253/2013 der Kommission vom 21. Oktober 2013 und Verordnung (EU) Nr.
1312/2014 der Kommission vom 10. Dezember 2014

\[**INS VO Netzdienste**\]: VERORDNUNG (EG) Nr. 976/2009 DER KOMMISSION
vom 19. Oktober 2009 zur Durchführung der Richtlinie 2007/2/EG des
Europäischen Parlaments und des Rates hinsichtlich der Netzdienste,
geändert durch Verordnung (EU) Nr. 1088/2010 der Kommission vom 23.
November 2010

\[**INS Generic Conceptual Model**\]: Generic Conceptual Model of the
INSPIRE data specifications, 2014-04-08

\[**ISO 19115**\]: ISO 19115:2003, Geographic information - Metadata
(with ISO 19115:2003/Cor. 1:2006, Geographic information - Metadata -
Technical Corrigendum 1)

\[**ISO 19115-D**\]: Deutsche Übersetzung der Metadatenfelder der ISO
19115, 2008-12-08

\[**ISO 19119**\]: ISO 19119:2005/PDAM 1, Geographic Information --
Services

\[**ISO 19139**\]: ISO/TS 19139 (10/2005), Geographic information -
Metadata - Implementation specification

\[**OGC CSW**\]: OpenGIS® Catalogue Services Specification 2.0.2,
2007-02-23

\[**OGC CSW ISO AP**\]: OpenGIS® Catalogue Services Specification 2.0.2
- ISO Metadata Application Profile, Version 1.0, 2007-07-19

\[**RFC 3986**\]: Uniform Resource Identifier (URI), Generic Syntax
(http://www.ietf.org/rfc/rfc3986.txt)

Anhang 1: INSPIRE-Spezifikationen (Durchführungsbestimmungen) {#anhang-1-inspire-spezifikationen-durchführungsbestimmungen .list-paragraph}
=============================================================

(zu Abschnitt 2.12, Konformität (Übereinstimmung mit Spezifikationen,
\[INS VO MD\], B 7))

Die folgende Tabelle enthält die relevanten
INSPIRE-Durchführungsbestimmungen, die als Inhalt für die Aussage zur
Konformität (*specification*-Element) in Frage kommen:

  **Titel der Spezifikation**                                                                                                                                                                                                  **Datum der Veröffentlichung**
  ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- --------------------------------
  VERORDNUNG (EG) Nr. 1089/2010 DER KOMMISSION vom 23. November 2010 zur Durchführung der Richtlinie 2007/2/EG des Europäischen Parlaments und des Rates hinsichtlich der Interoperabilität von Geodatensätzen und -diensten   2010-12-08
  VERORDNUNG (EG) Nr. 976/2009 DER KOMMISSION vom 19. Oktober 2009 zur Durchführung der Richtlinie 2007/2/EG des Europäischen Parlaments und des Rates hinsichtlich der Netzdienste                                            2009-10-20

Anhang 2: Zuordnung der INSPIRE-Annex-Themen zu ISO-Themenkategorien {#anhang-2-zuordnung-der-inspire-annex-themen-zu-iso-themenkategorien .list-paragraph}
====================================================================

(zu Abschnitt 3.3, Themenkategorie nach ISO (Zuordnung zum
INSPIRE-Thema: \[INS VO MD\], B 2.1))

+----------------------+----------------------+----------------------+
| **I                  | *                    | *                    |
| NSPIRE-Annex-Thema** | *ISO-Themenkategorie | *ISO-Themenkategorie |
|                      | - DE**[^29]          | - EN**[^30]          |
+----------------------+----------------------+----------------------+
| Adressen             | Ortsangaben          | location             |
+----------------------+----------------------+----------------------+
| Atmosphärische       | Klimatologie/Met     | climatologyM         |
| Bedingungen          | eorologie/Atmosphäre | eteorologyAtmosphere |
+----------------------+----------------------+----------------------+
| Bewirtschaftungsge   | Planung              | planningCadastre     |
| biete/Schutzgebiete/ | sunterlagen/Kataster |                      |
| geregelte Gebiete    |                      |                      |
| und                  |                      |                      |
| Bericht              |                      |                      |
| erstattungseinheiten |                      |                      |
+----------------------+----------------------+----------------------+
| Biogeografische      | Biologie             | biota                |
| Regionen             |                      |                      |
+----------------------+----------------------+----------------------+
| Boden                | Geowissenschaften    | geos                 |
|                      |                      | cientificInformation |
+----------------------+----------------------+----------------------+
| Bodenbedeckung       | Bilddaten/Basis      | image                |
|                      | karten/Landbedeckung | ryBaseMapsEarthCover |
|                      |                      |                      |
|                      | *Oberfläch           |                      |
|                      | enbeschreibung*[^31] |                      |
+----------------------+----------------------+----------------------+
| Bodennutzung         | Planung              | planningCadastre     |
|                      | sunterlagen/Kataster |                      |
+----------------------+----------------------+----------------------+
| Energiequellen       | Wirtschaft           | economy              |
+----------------------+----------------------+----------------------+
| Fl                   | Planung              | planningCadastre     |
| urstücke/Grundstücke | sunterlagen/Kataster |                      |
| (Katasterparzellen)  |                      |                      |
+----------------------+----------------------+----------------------+
| Gebäude              | Bauwerke             | structure            |
+----------------------+----------------------+----------------------+
| Gebiete mit          | Geowissenschaften    | geos                 |
| naturbedingten       |                      | cientificInformation |
| Risiken              |                      |                      |
+----------------------+----------------------+----------------------+
| Geografische         | Ortsangaben          | location             |
| Bezeichnungen        |                      |                      |
+----------------------+----------------------+----------------------+
| Geologie             | Geowissenschaften    | geos                 |
|                      |                      | cientificInformation |
+----------------------+----------------------+----------------------+
| Gesundheit und       | Gesundheitswesen     | health               |
| Sicherheit           |                      |                      |
+----------------------+----------------------+----------------------+
| Gewässernetz         | Binnengewässer       | inlandWaters         |
+----------------------+----------------------+----------------------+
| Höhe                 | Höhenangaben         | elevation            |
+----------------------+----------------------+----------------------+
| Landwirtschaftliche  | Landwirtschaft       | farming              |
| Anlagen und          |                      |                      |
| Aquakulturanlagen    |                      |                      |
+----------------------+----------------------+----------------------+
| Lebensräume und      | Biologie             | biota                |
| Biotope              |                      |                      |
+----------------------+----------------------+----------------------+

+----------------------+----------------------+----------------------+
| INSPIRE-Annex-Thema  | ISO-Themenkategorie  | ISO-Themenkategorie  |
|                      | - DE[^35]            | - EN[^36]            |
+----------------------+----------------------+----------------------+
| Meeresregionen       | Meere                | oceans               |
+----------------------+----------------------+----------------------+
| Meteoro              | Klimatologie/Met     | climatologyM         |
| logisch-geografische | eorologie/Atmosphäre | eteorologyAtmosphere |
| Kennwerte            |                      |                      |
+----------------------+----------------------+----------------------+
| Mineralische         | Wirtschaft           | economy              |
| Bodenschätze         |                      |                      |
+----------------------+----------------------+----------------------+
| Orthofotografie      | Bilddaten/Basis      | image                |
|                      | karten/Landbedeckung | ryBaseMapsEarthCover |
|                      |                      |                      |
|                      | *Oberfläch           |                      |
|                      | enbeschreibung*[^37] |                      |
+----------------------+----------------------+----------------------+
| Ozeanog              | Meere                | oceans               |
| rafisch-geografische |                      |                      |
| Kennwerte            |                      |                      |
+----------------------+----------------------+----------------------+
| Produktions- und     | Bauwerke             | structure            |
| Industrieanlagen     |                      |                      |
+----------------------+----------------------+----------------------+
| Schutzgebiete        | Umwelt               | environment          |
+----------------------+----------------------+----------------------+
| Statistische         | Grenzen              | boundaries           |
| Einheiten            |                      |                      |
+----------------------+----------------------+----------------------+
| Umweltüberwachung    | Bauwerke             | structure            |
+----------------------+----------------------+----------------------+
| Verkehrsnetze        | Verkehrswesen        | transportation       |
+----------------------+----------------------+----------------------+
| V                    | Ver- und             | ut                   |
| ersorgungswirtschaft | Entsorg              | ilitiesCommunication |
| und staatliche       | ung/Nachrichtenwesen |                      |
| Dienste              |                      |                      |
|                      | *Ver- und            |                      |
|                      | Entsorgung,          |                      |
|                      | Kommunikation*^26^   |                      |
+----------------------+----------------------+----------------------+
| Verteilung der Arten | Biologie             | biota                |
+----------------------+----------------------+----------------------+
| Verteilung der       | Gesellschaft         | society              |
| Bevölkerung **---**  |                      |                      |
| Demografie           |                      |                      |
+----------------------+----------------------+----------------------+
| Verwaltungseinheiten | Grenzen              | boundaries           |
+----------------------+----------------------+----------------------+

Anhang 3: Beschränkungen des öffentlichen Zugangs bei INSPIRE {#anhang-3-beschränkungen-des-öffentlichen-zugangs-bei-inspire .list-paragraph}
=============================================================

(zu Abschnitt 2.8, Beschränkungen des öffentlichen Zugangs (\[INS VO
MD\], B 8.2))

Die folgende Tabelle enthält die o.g. Gründe nach Artikel 13(1) a) - h)
der INSPIRE-Richtlinie, aus denen eine Beschränkung des öffentlichen
Zugangs überhaupt nur zulässig ist, und listet den jeweils benötigten
Eintrag für das *gmx:Anchor*-Element sowie für den deutschsprachigen
Begleittext auf:

+----------------------+----------------------+----------------------+
| **Grund nach Artikel | **Eintrag unter      | **deutschsprachiger  |
| 13(1) a) - h) der    | gmx:Anchor**         | Begleittext**        |
| I                    |                      |                      |
| NSPIRE-Richtlinie:** |                      |                      |
|                      |                      |                      |
| **Zugang beschränkt, |                      |                      |
| weil dieser          |                      |                      |
| nachteilige          |                      |                      |
| Auswirkungen hätte   |                      |                      |
| auf...**             |                      |                      |
+======================+======================+======================+
| \... a) die          | xlink:href=\"http    | Öffentlicher Zugriff |
| Vertraulichkeit der  | ://inspire.ec.europa | beschränkt           |
| Verfahren von        | .eu/metadata-codelis | entsprechend Artikel |
| Behörden, sofern     | t/LimitationsOnPubli | 13(1)(a) der         |
| eine derartige       | cAccess/INSPIRE_Dire | INSPIRE-Richtlinie:  |
| Vertraulichkeit      | ctive_Article13_1a\" | a) aufgrund          |
| gesetzlich           |                      | nachteiliger         |
| vorgesehen ist;      |                      | Auswirkungen auf die |
|                      |                      | Vertraulichkeit der  |
|                      |                      | Verfahren von        |
|                      |                      | Behörden             |
+----------------------+----------------------+----------------------+
| ... b)               | xlink:href=\"http    | Öffentlicher Zugriff |
| internationale       | ://inspire.ec.europa | beschränkt           |
| Beziehungen, die     | .eu/metadata-codelis | entsprechend Artikel |
| öffentliche          | t/LimitationsOnPubli | 13(1)(b) der         |
| Sicherheit oder die  | cAccess/INSPIRE_Dire | INSPIRE-Richtlinie:  |
| Landesverteidigung;  | ctive_Article13_1b\" | b) aufgrund          |
|                      |                      | nachteiliger         |
|                      |                      | Auswirkungen auf     |
|                      |                      | internationale       |
|                      |                      | Beziehungen, die     |
|                      |                      | öffentliche          |
|                      |                      | Sicherheit oder die  |
|                      |                      | Landesverteidigung   |
+----------------------+----------------------+----------------------+
| ... c) laufende      | xlink:href=\"http    | Öffentlicher Zugriff |
| Gerichtsverfahren,   | ://inspire.ec.europa | beschränkt           |
| die Möglichkeiten    | .eu/metadata-codelis | entsprechend Artikel |
| einer Person, ein    | t/LimitationsOnPubli | 13(1)(c) der         |
| faires Verfahren zu  | cAccess/INSPIRE_Dire | INSPIRE-Richtlinie:  |
| erhalten oder die    | ctive_Article13_1c\" | c) aufgrund          |
| Möglichkeiten einer  |                      | nachteiliger         |
| Behörde,             |                      | Auswirkungen auf     |
| Untersuchungen       |                      | laufende             |
| strafrechtlicher     |                      | Gerichtsverfahren    |
| oder                 |                      |                      |
| disziplinarischer    |                      |                      |
| Art durchzuführen;   |                      |                      |
+----------------------+----------------------+----------------------+
| ... d) die           | xlink:href=\"http    | Öffentlicher Zugriff |
| Vertraulichkeit von  | ://inspire.ec.europa | beschränkt           |
| Geschäfts- oder      | .eu/metadata-codelis | entsprechend Artikel |
| Be                   | t/LimitationsOnPubli | 13(1)(d) der         |
| triebsinformationen, | cAccess/INSPIRE_Dire | INSPIRE-Richtlinie:  |
| sofern das           | ctive_Article13_1d\" | d) aufgrund          |
| innerstaatliche      |                      | nachteiliger         |
| Recht oder das       |                      | Auswirkungen auf die |
| Gemeinschaftsrecht   |                      | Vertraulichkeit von  |
| diese                |                      | Geschäfts- oder      |
| Vertraulichkeit      |                      | B                    |
| vorsieht, um         |                      | etriebsinformationen |
| berechtigte          |                      |                      |
| wirtschaftliche      |                      |                      |
| Interessen,          |                      |                      |
| einschließlich des   |                      |                      |
| öffentlichen         |                      |                      |
| Interesses an der    |                      |                      |
| Wahrung der          |                      |                      |
| statistischen        |                      |                      |
| Geheimhaltung und    |                      |                      |
| des                  |                      |                      |
| Steuergeheimnisses,  |                      |                      |
| zu schützen;         |                      |                      |
+----------------------+----------------------+----------------------+

+----------------------+----------------------+----------------------+
| **Grund nach Artikel | **Eintrag unter      | **deutschsprachiger  |
| 13(1) a) - h) der    | gmx:Anchor**         | Begleittext**        |
| I                    |                      |                      |
| NSPIRE-Richtlinie:** |                      |                      |
|                      |                      |                      |
| **Zugang beschränkt, |                      |                      |
| weil dieser          |                      |                      |
| nachteilige          |                      |                      |
| Auswirkungen hätte   |                      |                      |
| auf...**             |                      |                      |
+======================+======================+======================+
| ... e) Rechte des    | xlink:href=\"http    | Öffentlicher Zugriff |
| geistigen Eigentums; | ://inspire.ec.europa | beschränkt           |
|                      | .eu/metadata-codelis | entsprechend Artikel |
|                      | t/LimitationsOnPubli | 13(1)(e) der         |
|                      | cAccess/INSPIRE_Dire | INSPIRE-Richtlinie:  |
|                      | ctive_Article13_1e\" | e) aufgrund          |
|                      |                      | nachteiliger         |
|                      |                      | Auswirkungen auf die |
|                      |                      | Rechte des geistigen |
|                      |                      | Eigentums            |
+----------------------+----------------------+----------------------+
| ... f) die           | xlink:href=\"http    | Öffentlicher Zugriff |
| Vertraulichkeit      | ://inspire.ec.europa | beschränkt           |
| personenbezogener    | .eu/metadata-codelis | entsprechend Artikel |
| Daten und/oder Akten | t/LimitationsOnPubli | 13(1)(f) der         |
| über eine natürliche | cAccess/INSPIRE_Dire | INSPIRE-Richtlinie:  |
| Person, sofern diese | ctive_Article13_1f\" | f) aufgrund          |
| der Bekanntgabe      |                      | nachteiliger         |
| dieser Informationen |                      | Auswirkungen auf die |
| an die               |                      | Vertraulichkeit      |
| Öffentlichkeit nicht |                      | personenbezogener    |
| zugestimmt hat und   |                      | Daten                |
| sofern eine          |                      |                      |
| derartige            |                      |                      |
| Vertraulichkeit nach |                      |                      |
| einzelstaatlichem    |                      |                      |
| oder                 |                      |                      |
| gemeinschaftlichem   |                      |                      |
| Recht vorgesehen     |                      |                      |
| ist;                 |                      |                      |
+----------------------+----------------------+----------------------+
| ... g) die           | xlink:href=\"http    | Öffentlicher Zugriff |
| Interessen oder den  | ://inspire.ec.europa | beschränkt           |
| Schutz einer Person, | .eu/metadata-codelis | entsprechend Artikel |
| die die angeforderte | t/LimitationsOnPubli | 13(1)(g) der         |
| Information          | cAccess/INSPIRE_Dire | INSPIRE-Richtlinie:  |
| freiwillig zur       | ctive_Article13_1g\" | g) aufgrund          |
| Verfügung gestellt   |                      | nachteiliger         |
| hat, ohne dazu       |                      | Auswirkungen auf den |
| gesetzlich           |                      | Schutz einer Person  |
| verpflichtet zu sein |                      |                      |
| oder verpflichtet    |                      |                      |
| werden zu können, es |                      |                      |
| sei denn, dass diese |                      |                      |
| Person der           |                      |                      |
| Herausgabe der       |                      |                      |
| betreffenden         |                      |                      |
| Informationen        |                      |                      |
| zugestimmt hat;      |                      |                      |
+----------------------+----------------------+----------------------+
| ... h) den Schutz    | xlink:href=\"http    | Öffentlicher Zugriff |
| der Umweltbereiche,  | ://inspire.ec.europa | beschränkt           |
| auf die sich die     | .eu/metadata-codelis | entsprechend Artikel |
| Informationen        | t/LimitationsOnPubli | 13(1)(h) der         |
| beziehen, wie z. B.  | cAccess/INSPIRE_Dire | INSPIRE-Richtlinie:  |
| die Aufenthaltsorte  | ctive_Article13_1h\" | h) aufgrund          |
| seltener Tierarten.  |                      | nachteiliger         |
|                      |                      | Auswirkungen auf den |
|                      |                      | Schutz von           |
|                      |                      | Umweltbereichen      |
+----------------------+----------------------+----------------------+

Anhang 4: Nachweis der Änderungen der Konventionen zu Metadaten Version 2.1.0 gegenüber Version 2.0.3 vom 27.04.2020 {#anhang-4-nachweis-der-änderungen-der-konventionen-zu-metadaten-version-2.1.0-gegenüber-version-2.0.3-vom-27.04.2020 .list-paragraph}
====================================================================================================================

  -- ------------------------------
     *NEU*
     *ÄNDERUNG (Struktur/Inhalt)*
  -- ------------------------------

  -- ------------
     *GELÖSCHT*
  -- ------------

     **Kapitel**   **Name des Kapitels**                                            **Beschreibung der Änderung**                                                                                                                                                  **Referenz auf Version** **2.0.3**
  -- ------------- ---------------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ ------------------------------------
     1.2           Konventionen zu Metadaten                                        Aufnahme der Grafik aus TG MD 2.0.1 zur Verdeutlichung des Geltungsbereichs dieses Dokuments                                                                                   
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
     2.7.1         Schlüsselwort „inspireidentifiziert"                             Anpassung des Textes bzgl. Nicht-Verwendung eines Thesaurus an den Meldungstext in der ATS                                                                                     
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
     2.10          Regionalschlüssel                                                Streichung der NUTS/LAU -Regionen aus Text und Beispielen                                                                                                                      
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
     2.13          Angaben zum Raumbezug / Koordinatenreferenzsystem                Neues Kapitel zur Regelung der Angabe von EPSG-Codes                                                                                                                           
                                                                                                                                                                                                                                                                   
     3.1           Eindeutiger Ressourcenidentifikator (\[INS VO MD\], B 1.5)       Präzisierung der Anforderung bzgl. der Auflösbarkeit des Ressourcenidentifikators durch die GDI-DE Registry oder eine anderweitige technische Unterstützung                    
                                                                                                                                                                                                                                                                   
     3.2.2         Schlüsselwort „opendata"                                         Anpassung des Textes bzgl. Nicht-Verwendung eines Thesaurus an den Meldungstext in der ATS                                                                                     
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
     3.6           Nutzungsbedingungen und Lizenzinformationen für Open Data        Konkretisierung, dass GENAU EIN Element für JSON-Ausdruck vorgesehen ist sowie Anpassung des Beispiels bzgl. angegebener URL                                                   
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
     4.3.1         Ressourcenverweis unter transferOptions (\[INS VO MD\], B 1.4)   Konkretisierung bzgl. Verpflichtung zu GetCapabilities-Request bei INSPIRE                                                                                                     
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
     Anhang 2      Zuordnung der INSPIRE-Annex-Themen zu ISO-Themenkategorien       Ergänzung der deutschsprachigen Übersetzung der ISO 19115 zu einzelnen Werten (sofern abweichend von der Aufzählung in der INSPIRE Implementing Rule Metadata \[INS VO MD\])   
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   
                                                                                                                                                                                                                                                                   

[^1]: <http://www.geoportal.de/DE/GDI-DE/Media-Center/Dokumente/dokumente.html?lang=de>

[^2]: <http://www.geoportal.de/DE/GDI-DE/Arbeitskreise/Geodienste/geodienste.html?lang=de>

[^3]: RFC 4122: <https://www.ietf.org/rfc/rfc4122.txt>

[^4]: http://inspire.ec.europa.eu/metadata-codelist/LimitationsOnPublicAccess

[^5]: http://inspire.ec.europa.eu/metadata-codelist/ConditionsApplyingToAccessAndUse

[^6]: Die EPSG Geodetic Parameter Registry ist ein Angebot der
    International Association of Oil&Gas Producers. Die Definition des
    Koordinatenreferenzsystems kann über die EPSG-Registry als textliche
    Beschreibung, als GML
    (http://www.epsg-registry.org/export.htm?gml=urn:ogc:def:crs:EPSG::4326)
    oder als WKT
    (http://www.epsg-registry.org/export.htm?wkt=urn:ogc:def:crs:EPSG::4326)
    versioniert abgerufen werden. Die EPSG-Registry basiert auf der ISO
    19111:2007 und kann demnach keine gitterbasierten Raumbezugssysteme
    wie MGRS / UTMREF abbilden. Raumbezugsinformationen, die
    ausschließlich in MGRS / UTMREF vorliegen, können aus diesem Grund
    nicht mit Hilfe eines EPSG-Codes beschrieben werden.

[^7]: Es gibt weitere Übersichten, die Definitionen der EPSG-Codes in
    unterschiedlichen Formaten für unterschiedliche Zwecke führen.
    Hierzu gehört beispielsweise http://epsg.io/4326 , wo auf
    Definitionen für PROJ4 (http://epsg.io/4326.proj4), zahlreiche
    weitere und ebenfalls XML bzw. GML (http://epsg.io/4326.xml)
    zurückgegriffen werden kann. Sämtliche Übersichten basieren auf den
    Informationen der EPSG-Registry.

[^8]: Das opengis.net-Repository ist vom Umfang her eine ebenfalls
    versionierte Kopie der EPSG-Registry. Es stellt den Versuch dar, die
    EPSG-Registry im Falle eines Ausfalls zu ersetzen und hat das
    Anliegen PURLs (Permanente URLs) im Sinne des W3C als dauerhafte und
    unabhängige Referenz zu den EPSG-Codes auszuweisen. Die Technical
    Guidance für Metadaten greift diesen Gedanken auf und weist das
    opengis.net- Repository ihrerseits als vorläufige Referenz für
    INSPIRE aus.

[^9]: WMO Codes Register: http://codes.wmo.int/ui/about. Beispiel für
    das Projektionssystem „ICAO Standard Atmosphere Reference Height":
    http://codes.wmo.int/grib2/codeflag/4.2/\_0-3-3

[^10]: Das queryable ‚ResourceIdentifier' wird lt. \[OGC CSW ISO AP\]
    auf MD_Identifier/code abgebildet.

[^11]: https://registry.gdi-de.org/

[^12]: *https://wiki.gdi-de.org/display/REGISTRYDE/Namensraum-Register*

[^13]: Nicht anwendbar auf Metadaten, die Dienste beschreiben

[^14]: gem. Liste unter <https://www.dcat-ap.de/def/licenses/>, Spalte
    „Lizenzcode"

[^15]: gem. Liste unter <https://www.dcat-ap.de/def/licenses/>, Spalte
    „Name"

[^16]: gem. Liste unter <https://www.dcat-ap.de/def/licenses/>, Spalte
    „Lizenztext"

[^17]: <https://registry.gdi-de.org/>

[^18]: <https://wiki.gdi-de.org/display/REGISTRYDE/Namensraum-Register>

[^19]: https://www.dcat-ap.de/

[^20]: https://www.it-planungsrat.de/SharedDocs/Sitzungen/DE/2018/Sitzung_26.html?pos=9

[^21]: https://github.com/GovDataOfficial/inspire-dcat-de-bridge

[^22]: u\. a. Europäisches Datenportal
    (https://www.europeandataportal.eu/de)

[^23]: https://www.govdata.de/

[^24]: <https://testsuite.gdi-de.org/gdi/>

[^25]: Der EU INSPIRE Validator ist zugänglich unter URL:
    http://inspire.ec.europa.eu/validator/

[^26]: Gemäß deutscher Fassung der \[INS VO MD\]

[^27]: Die Begriffe in der Spalte \'ISO-Themenkategorie-EN\' entsprechen
    der Codeliste B5.27 MD_TopicCategoryCode \[ISO 19115\] sowie der
    englischen Fassung der \[INS VO MD\]

[^28]: Gemäß deutscher Übersetzung zur \[ISO 19115-D\]

[^29]: Gemäß deutscher Fassung der \[INS VO MD\]

[^30]: Die Begriffe in der Spalte \'ISO-Themenkategorie-EN\' entsprechen
    der Codeliste B5.27 MD_TopicCategoryCode \[ISO 19115\] sowie der
    englischen Fassung der \[INS VO MD\]

[^31]: Gemäß deutscher Übersetzung zur \[ISO 19115-D\]

[^32]: Gemäß deutscher Fassung der \[INS VO MD\]

[^33]: Die Begriffe in der Spalte \'ISO-Themenkategorie-EN\' entsprechen
    der Codeliste B5.27 MD_TopicCategoryCode \[ISO 19115\] sowie der
    englischen Fassung der \[INS VO MD\]

[^34]: Gemäß deutscher Übersetzung zur \[ISO 19115-D\]

[^35]: Gemäß deutscher Fassung der \[INS VO MD\]

[^36]: Die Begriffe in der Spalte \'ISO-Themenkategorie-EN\' entsprechen
    der Codeliste B5.27 MD_TopicCategoryCode \[ISO 19115\] sowie der
    englischen Fassung der \[INS VO MD\]

[^37]: Gemäß deutscher Übersetzung zur \[ISO 19115-D\]
