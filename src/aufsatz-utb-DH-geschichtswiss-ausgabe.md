---
title: 'Daten und Schnittstellen: Die Ausgabeseite digitaler Editionen'
author: Stephan Kurz, ORCID 0000-0003-2546-2570, GND http://d-nb.info/gnd/13281899X
keywords: [TEI, Edition, Digitale Edition, Quellenedition]
language: 'de-DE, st-AN'
lang: 'de-DE, st-AN'
abstract: 'Ausgehend von der Codierung natürlichsprachlicher Quellen als strukturierte Daten im XML/TEI-Format stellt der Beitrag Wege vor, diese Daten zu publizieren. Vorgestellt werden konkrete Infrastrukturen und technische Implementationen. Anforderungen an unterschiedliche Ausgabeformate werden anhand von webbasierten und gedruckten Editionen vorgestellt. Neben dem Fokus auf Editionsdaten und ihre Modellierung steht auch die Notwendigkeit im Zentrum, verschiedenen Medien zur Speicherung, Zirkulation und Konsumption entsprechende Aufmerksamkeit zu widmen.'
bibliography: [file:bib/references.bib]
---
 
# Daten und Schnittstellen: Die Ausgabeseite digitaler Editionen
 
## Ausgabe: Schnittstellen

Die im Abschnitt „Transkribieren – Annotieren“ anlässlich der Eingabeseite digitaler Editionen skizzierten Abläufe bringen mit sich eine Zunahme an technischer (nicht unbedingt: konzeptioneller) Komplexität und an etwa für Geschichtswissenschaftler:innen oder Philolog:innen unbekanntem und in den Curricula auch nicht verankertem Werkzeugwissen. Dies erzeugt gegenüber der traditionellen Art, aus in Manuskripten und Karteikästen gespeichertem Wissen gedruckte Editionen zu erzeugen, neu hinzukommenden Bedarf an Expertise im Bereich der Vermittlung zwischen Editionsfachleuten und Techniker:innen in den verschiedenen Bereichen der digitalen Edition. 

Die Daten der Edition in standardisiertem Format sind erstes und zentrales Ergebnis bei der Erstellung einer digitalen Edition. Sie sind es, die inklusive ihrer Metadaten archiviert werden und in Repositorien langzeitarchiviert werden. Viele Editionen legen ihre Daten zusätzlich zur eigenen Infrastruktur auch in großen digitalen Archiven ab; für die Europäische Union ist das relevante Repositorium das vom CERN betriebene Zenodo (<https://zenodo.org/>), auch das Internet Archive (<https://archive.org/>) wäre ein logischer Datenendlagerpunkt. Die Editionsdaten sind das Um und Auf: Sie sind im Kontext von nachhaltigen und nach den FAIR-Prinzipien bearbeiteten Forschungsdaten jedenfalls unter offener Lizenz zur Verfügung zu stellen;^[Vgl. zu den FAIR-Prinzipien im Zusammenhang mit der Standardisierung geisteswissenschaftlicher Forschungsdaten den Beitrag von Johannes Stigler, Lina Zangerl und Katharina Zeppezauer-Wachauer in diesem Band.] sie sind Rohdaten für die maschinengestützte Analyse, sie sind aber auch jenes Material, das in verschiedenen Formen in unterschiedlichen Medien publik gemacht wird. 

### Webapplikationen

 Zu einer digitalen Edition gehört denn denn üblicherweise nicht nur die Bereitstellung der Quelldaten, sondern auch eine im öffentlichen Web zugängliche Webapplikation, die die im Editionsprozess erarbeiteten Daten darstellt. Kriterien für deren Beurteilung hat das Rezensionsjournal RIDE des Instituts für Dokumentologie und Editorik e.V. erarbeitet (@SahleCriteriaReviewingScholarly2014). Diese Beurteilungskriterien geben abseits der fachspezifischen Gepflogenheiten ein gutes Bild von den tatsächlichen Erwartungen zumindest eines Teils der zu erwartenden Benutzer:innen einer digitalen Edition und sind insofern ein wichtiges Handwerkszeug schon bei der Planung einer wissenschaftlichen digitalen Edition.


___
#### Kasten Erprobte Tech Stacks für Webapplikationen zur Darstellung von TEI-Daten
 
- mithilfe von XML-Datenbanken wie eXist-db <http://exist-db.org/> (unter Zuhilfenahme verschiedener Frameworks wie z.B. teiPublisher <https://teipublisher.com/>; dsebaseapp <https://github.com/KONDE-AT/dsebaseapp>; wdb <https://github.com/dariok/wdbplus>) oder BaseX <https://basex.org/>
- repositoriengetrieben (für Österreich relevant sind z.B. GAMS der Universität Graz <http://gams.uni-graz.at/> (basierend auf Fedora-Commons, nicht quelloffen, übernommen auch an der Österreichischen Nationalbibliothek für <https://edition.onb.ac.at/>), ARCHE an der Österreichischen Akademie der Wissenschaften <https://arche.acdh.oeaw.ac.at/>, modular quelloffen unter <https://github.com/acdh-oeaw?q=arche>; die Fedora-Commons-basierte Repositorienlösung PHAIDRA an der größten Universität des Landes kann seit 2007 keine TEI-Daten darstellen, absolutes Negativbeispiel ist aber die nach mehreren Entwicklungsjahren eingestellte Eigenentwicklung der Universität Salzburg unter dem Titel „dh-Plus“)
- „infrastrukturlos“ (z.B. über die Continuous integration von GitHub Pages <https://pages.github.com/> und dem  JavaScript-Framework CeTEIcean <https://github.com/TEIC/CETEIcean/>, das einen parallelen, der TEI-Quelle isomorphen DOM-Baum generiert)
- aus TEI-Daten via XSL-T generierte statische HTML-Seiten (etwa mithilfe von <https://github.com/acdh-oeaw/dse-static-cookiecutter/>) 
- …

___

Einige unter offener Lizenz verwendbare Werkzeuge zur Veröffentlichung von TEI-Editionen im Web sind im Kasten „Erprobte Tech Stacks zur Darstellung von TEI-Daten“ aufgelistet; sie alle haben ihre Vor- und Nachteile und benötigen ein gewisses Maß an Verständnis von und technischer Erfahrung mit Webtechnologien (HTML/CSS/JavaScript). Dass verschiedene Implementationen verschiedene Funktionalitäten ermöglichen, liegt auf der Hand, doch nicht immer sind die Implikationen der technischen Umsetzung den Editor:innen von vorne herein bewusst (zu Schnittstellen allgemein vgl. @Digital-Scholarly-Editions-as-Interfaces2018). Eine standardisierte Beschreibung der Funktionalitäten von Editionsplattformen ist dem Verf. nicht bekannt – sie orientieren sich grundsätzlich meist an den Möglichkeiten des älteren Mediums Buch, erweitert durch automatisiert erzeugbare Navigationsmöglichkeiten (@CariaMinimalFunctionalityDigital2018). 

Die Anforderungen an Webauftritte sind komplex und ändern sich einerseits an den Linien dessen, was Benutzer:innen gewöhnt sind wahrzunehmen, andererseits durch technische Innovation und Weiterentwicklung von Standards. In den letzten Jahren maßgeblich ist das Anwachsen des Anteils an mobilen Endgeräten (Tablets, Smartphones), das an kleinere Bildschirmauflösungen und *touch events* (zusätzlich zum *click*) angepasstes sogenanntes *responsive* Design erforderlich macht. Hinzu kommen Vorgaben seitens der Gesetzgebung, sie betreffen konkret etwa die Impressumspflicht und die erforderliche Zustimmung der Benutzer:innen zur Speicherung und Weitergabe von personenbezogenen Daten. Für in Österreich vom Bund finanzierte Webauftritte gilt darüber hinaus auch das *Bundesgesetz über den barrierefreien Zugang zu Websites und mobilen Anwendungen des Bundes*,
^[Web-Zugänglichkeits-Gesetz – WZG, <https://www.ris.bka.gv.at/GeltendeFassung.wxe?Abfrage=Bundesnormen&Gesetzesnummer=20010727>. Das Gesetz implementiert die seit 2008 vom W3C-Konsortium standardisierten *Web Content Accessibility Guidelines (WCAG) 2.0*, <https://www.w3.org/TR/2008/REC-WCAG20-20081211/>.] sodass auch barrierefreier Zugang sichergestellt werden muss.^[Zur Prüfung gibt es Werkzeuge, die das W3C unter <https://www.w3.org/WAI/ER/tools/> listet; hervorzuheben ist z.B. das *WAVE Web Accessibility Evaluation Tool* <https://wave.webaim.org/>.] 

Die gerade umrissenen Anforderungen gelten für alle Webauftritte und die meisten Werkzeuge zur Erstellung von Webseiten bieten von Haus aus Hilfestellung zu ihrer Erfüllung. An spezifischen Funktionen digitaler Editionen sind darüber hinaus in Übereinstimmung mit den oberwähnten RIDE-Kriterien zu erwarten: 

- Textansicht inkl. allfälliger Schalter zur Anzeige codierter editorischer Entscheidungen oder Referenzen
- visueller HTML-Zugriff auf (Teile der) Metadaten
- Volltextsuchfunktion
- Faksimiles der Quelle/n 
- Verzeichnisse (je nach Quellengattung Register der Named Entities, Inhaltsübersicht, evtl. Zeitleiste/Kalender, Kartenansicht)
- transparente Dokumentation der Edition (Editionsrichtlinien, Lizenz, Verantwortlichkeiten, Finanzierung, technische Dokumentation) 
- Dokumentation von Programmierschnittstellen (APIs) und Datenzugriff
- stabile Identifikatoren zumindest auf Dokumentebene (gängig sind PURL, URN, Handle/DOI), evtl. Zitiervorschlag 

Der Anhang zu diesem Beitrag bietet eine Liste ausgewählter digitaler Editionen mit von geschichtswissenschaftlichem Interesse, die chronologisch nach ihren Edenda sortiert und thematisch kurz kommentiert ist. Ebendort sind weiters auch mehrere Kataloge digitaler Editionen aufgeführt, die zu weiteren Ressourcen führen. 

Zurück zur konkreten Aufgabenstellung, TEI-Daten via Hypertext Markup Language (HTML) in einer Webapplikation anzuzeigen, und zu einem Beispiel: 

Der Ausschnitt aus dem Briefindex der Großbotschaft Virmont in dem Projekt *Digitale Edition von Quellen zur habsburgisch-osmanischen Diplomatie 1500–1918* (QhoD), der bereits anlässlich von Transkription und Annotation im Beitrag d. Verf. eingeführt wurde, lautet in TEI-XML wie folgt: 

```
<list>
    <item corresp="o:vipa.l.hbg.17190527">
        <p><ref target="/o:vipa.l.hbg.17190527">Nr. 1</ref> <choice><abbr>d.d.</abbr><expan>de dato</expan></choice> <rs ref="#mpr9458" type="place">Erdöd</rs>
             <date when="1719-05-27">27. Maii 1719</date> ohne beylag. Berichtet den forthgang seiner raise und daß ein page des <rs type="person" ref="#mpr15403">grafen Bathyan</rs> einen laggey des <rs type="person" ref="#mpr15405">grafen von Türheimb</rs> erstochen.</p>
    </item>
    …
</list>^[@VirmontBriefindex1719_1720, <https://qhod.net/o:vipa.i.hbg.1720/TEI_SOURCE>, letzter Zugriff: 02.09.2022.]
```

Das QhoD-Projekt setzt auf einen repositoriengetriebenen Disseminationsansatz und verwendet das Fedora-Commons-basierte *Geisteswissenschaftliche Asset Management System (GAMS)*. GAMS unterstützt die oben angeführten Funktionalitäten, lediglich automatisierter Datenzugriff auf Sammlungs- oder Kontextebene ist in der verwendeten Softwarelösung nicht vorgesehen (@SteinerGAMSCiriloClient2017). Die Repräsentation der TEI-Daten in HTML wird hier durch XSL-Transformationen erzeugt.^[Die dazu verwendete „Regeldatei“ ist abrufbar unter <https://qhod.net/o:vipa.i.hbg.1720/STYLESHEET>.] Da der zitierte Indexeintrag nur einer von vielen ist, ist er nach den Kodierungsrichtlinien des Projekts in der Textstruktur als Eintrag `<item>` in einer Liste `<list>` gekennzeichnet. Dieses TEI-Element wird in die entsprechende HTML-Analogie mit <`ul`> (unordered list, im Gegensatz zu einer nummerierten ordered list) und `<li>` (list item) übersetzt. Dass der Listeneintrag dem Objekt mit dem Identifikator `o:vipa.l.hbg.17190527` entspricht, ist in TEI mit dem `@corresp`-Attribut gekennzeichnet; diese Information wird aber von den XSL-T-Stylesheets nicht weiterverarbeitet. Dem TEI-Absatz `<p>` (paragraph) innerhalb des Listeneintrags entspricht auch in HTML ein `<p>`. 

Der explizite Verweis auf den referenzierten und bereits edierten Brief, der mit dem TEI-Element `ref` und seinem Sprungzielattribut `@target` angegeben ist, wird dagegen in einen HTML-Link `<a href="">` übersetzt, sodass der Verweis im Browser per Klick/Touch auf das richtige Dokument führt. Das darauf folgende TEI-Element `<choice>` bezeichnet eine Auswahl-„Weiche“: Die im Original stehende Abkürzung (`<abbr>`) „d.d.“ könnte alterativ auch in der Auflösung (`<expan>`) „de dato“ aufgelöst werden. Hier zeigt sich der Vorteil der Trennung von Inhalt und Darstellung: Während die Abkürzungsauflösung in der aktuellen Implementation als *mouseover* mithilfe eines HTML-Attributs `@title` umgesetzt ist, sodass bei Bewegung des Mauszeigers (oder langes Tippen auf Touch-Geräten) der alternative Text angezeigt wird, ließen sich z.B. auch Ansichten erzeugen, die entweder nur die Abkürzung oder ihre Auflösung darstellen. Die Datumsangabe inklusive des normalisierten ISO-Datums wird ähnlich ausgewertet und in HTML überführt. 

Die im Beispiel auf Named Entities verweisenden *referencing strings* (`<rs>`) werden anhand ihres Typs (`@type`) unterschiedlich behandelt und erhalten in HTML mouseovers mit den Verweisen auf kanonische Identifikatoren aus der Gemeinsamen Normdatei und aus GeoNames. Die Daten zu den Named entities sind an die vom Projekt QhoD zur Kuratierung der Entitydaten verwendete APIS-Datenbank^[Modulare Prosopographische Registratur: <https://mpr.acdh.oeaw.ac.at>.] und an ein daraus erstelltes `<standOff>`-Verzeichnis ausgelagert; über den internen Identifikator im Attribut `@ref` ist auf den Eintrag <https://mpr.acdh.oeaw.ac.at/entity/15405> verwiesen, der bei der Darstellung der `<rs>` über <http://gams.uni-graz.at/o:qhod.standOff/TEI_SOURCE> ausgelesen wird. Die Faksimile-Ansicht <https://qhod.net/o:vipa.i.hbg.1720/sdef:TEI/get?mode=view:facs> verzichtet mit Bedacht darauf, die Verweisziele darzustellen: Im Originaldokument sind die gemeinten Orte und Personen ja auch nicht hinterlegt oder anklickbar. 

Anhand dieses Beispiels ist klar geworden, dass klar dokumentierte und bezeichnete Datenstrukturen für Editionen unumgänglich sind; ihre Darstellung in der Benutzerschnittstelle Browser (oder Screenreader u. dgl.) ist über Infrastrukturen wie die im Kasten „Erprobte Tech Stacks für Webapplikationen zur Darstellung von TEI-Daten“ genannten mithilfe einfacher Befehlssätze möglich. 

### Hybride Edition: Printausgabe aus Daten 

Alternativ oder zusätzlich zu einer Webapplikation als Schnittstelle zum Material erarbeiten manche digitale Editionen auch eine gedruckte Ausgabe. Dies wird häufig als *Single source publishing* bezeichnet, auch wenn die Quelldaten mitunter an unterschiedlichen Systemstellen voneinander abgezweigt werden und eine vollständige informationelle Deckungsgleichheit schwer zu erzielen ist (Beispiel: Seitenzahlen einer Druckausgabe in den Quelldaten). 

Eine gedruckte Ausgabe folgt dabei zwingend anderen Kriterien als eine Online-Präsentation durch eine Webapplikation. Sie hat sich an je eigenen (Darstellungs-)Gepflogenheiten des Faches und des spezifischen Editionstypus zu orientieren. Darüber hinaus hat sie gegenüber der grundsätzlich über Versionen veränderbaren digitalen Präsentationsform einen einmaligen Charakter, der keine Ad-hoc-Korrekturen im Nachhinein erlaubt. Weiters, und das ist vielleicht die Hauptherausforderung, sind gedruckte Bücher an eine jahrhundertealte typographische Tradition gebunden oder müssen sich zumindest daran messen: Ihre Produktion erfordert jedenfalls die Kenntnis typographischer Standards (@tschichold_aufs, @detailtypo, @Unger-Wie-Mans-Liest-2008) – nicht umsonst ist parallel zum verbreiteten Aufkommen von digitalen und hybriden Editionen auch eine verstärkte Auseinandersetzung mit der Buchkultur zu verzeichnen. Auch in den kulturwissenschaftlich verstandenen Geisteswissenschaften ist es nunmehr möglich, sich auseinanderzusetzen mit der „Schwarzen Kunst“, abseits der Arbeitsteilung von Wissensproduzent:innen und Vermittlerinstitutionen wie den Verlagen und ihrer ehemals hochgradig arbeitsteiligen Binnenorganisation (Satz, Grafik, Druck, Korrektorat, Lektorat, Vertrieb).^[Vgl. z.B. @Drucker-The-visible-word-1994, @ErnstWechselwirkung, @EderSeitenweiseWasdas2010, @KurzTheresMoreIt2011, @VanscheidtFontesLitterarum.Typographische2014, @FalkTypographie&Literatur2016, @MetzDieLesbarkeitder2019, @GorbachLesbar2019, @WissenundBuchgestalt2022.] Das Buch ist ein exzellentes Medium zur langfristigen Speicherung, zur Zirkulation und Präsentation von Wissen in einem haptisch zugänglichen Objekt: 

> Die Printedition hat weitere Mehrwerte: Sie ermöglicht dreidimensionale Navigation im Buchblock, mit dem Stift in der Hand, mit eingelegten Notizzetteln, Anstreichungen, als Objekt und als Ort des Studiums. Das gedruckte Buch ermöglicht durch saubere Mikrotypografie, ideale Kontrastverhältnisse und hohe Auflösung Lesbarkeit in längeren Aufmerksamkeitsspannen. Das gedruckte Buch ist ein haptisch greifbares und sinnlich erfahrbares Ding von Gewicht. Das gedruckte Buch ist mehr als die abstrakte Information, die es enthält, wir Menschen können zum Buchobjekt einen konkreten Bezug herstellen. (@KleteckaDieProtokolledes2022, IX)

Um zu diesem Ende aus den Daten einer digitalen Edition Druckdaten für den Digital- oder Offsetdruck zu erzeugen, müssen die in Struktur und Semantik kodierten Editionsdaten wieder in eine gemeinsame Darstellungsebene von Inhalt und Form gebracht werden – also in ein Satzdatenformat. Dies geschieht entweder mit XSL-FO (eXtensible Stylesheet Language-Formatting Objects), einem Werkzeug aus der Familie der X-Technologien, direkt nach PDF – oder durch Überführung in ein beliebiges Zwischenformat. Am gängigsten ist die Prozessierung mithilfe von LaTeX, eines für den hochwertigen Druck geschaffenen Satzsystems und der zugehörigen Auszeichnungssprache; dabei werden mit ähnlichen XSL-T-Routinen wie oben anhand der Webdarstellung LaTeX-Daten erzeugt (statt *mouseovers* für Personennennungen werden bspw. Registereinträge erzeugt). LaTeX folgt der Logik des traditionellen Buchsatzes und vermag daher schon ohne viele Adaptierungen konzeptionell alle Bedürfnisse des Buchs abzudecken. Da die LaTeX-Softwarefamilie (und Derivate wie das nativ XML-fähige ConTeXt) aus dem Open Source-Bereich kommt, sind Pakete für viele Aufgabenbereiche erhältlich – für die Registerprozessierung etwa MakeIndex und xindy, für mehrere Apparate und den klassischen Satz wissenschaftlicher Editionen etwa reledmac, für die Bibliografieformatierung BibTeX und BibLaTeX/biber. Das Prozessierungsmodell der oben erwähnten teiPublisher-Applikation für eXist-db erlaubt die Definition von LaTeX-Ausgabeblöcken aus (TEI-)XML-Daten auch in visueller Form. 

Auch in der Wissenschaftsverlagslandschaft werden die Vorteile standardisierter Datenquellen und adäquater -verarbeitung mittlerweile gesehen, sodass bis auf wenige Ausnahmen nicht mehr auf die Abgabe von Office-Dokumenten gepocht wird, welche doch eine unnötige und buchstäblich sinnbefreite Übung in technisch-semantischer Verflachung ist, die Editor:innen und Wissensarbeiter:innen von ihrer Denkarbeit nur abhält. Komplexitätsreduktion ist bei jedem Ausgabeformat vonnöten, aber bitte algorithmisch und ohne an den Quellen irreversible Abzweigungen als Fallstricke zu implementieren. Dokumente des Denkens und eine Darstellung als *What you see is what you mean* finden viel eleganter Platz in TEI-XML oder in noch reduzierteren Auszeichnungssprachen wie ReStructured Text oder Markdown.

### Sonderfall Retrodigitalisierte Edition: Daten aus Printausgaben

Viele länger bestehende Editionsprojekte haben in den letzten Jahren ihre Publikationspolitik und -technik auf digitales Edieren mit TEI-XML oder anderen standardisierten Formaten umgestellt. Viele davon erzeugen aus digitalen Daten auch weiterhin gedruckte Ausgaben. Sie haben andererseits aber auch Konvolute von mehr oder weniger im selben Layout erschienenen gedruckten Beständen aufzuweisen, deren Satzdaten nur in Ausnahmefällen komplett und in einheitlicher Formatierung überliefert sind: Die Edition der Ministerratsprotokolle Österreichs etwa hat ihre ersten Bände in den 1970er Jahren noch im Bleisatz vorgelegt, der letzte nicht mit TEI-Workflow erstellte Band erschien 2018 aus Word-Vorlagen im Indesign-Satz. Letzte Korrekturen in den Druckfahnen lagen selbst der Redaktion nicht digital vor. 

In solchen Fällen ist der Begriff der „Altbausanierung“ (@NeuberAltbausanierungmitNiveau2020) durchaus angebracht: Es geht dann darum, die impliziten Datenmodelle der Buchüberlieferung zu formalisieren (sie erst einmal auseinanderzulegen und auf ihre editorischen Intentionen zurückzuführen) und regelmäßige Oberflächenphänomene der Darstellung (Kursivierung, Überschriftensetzung) wiederum in strukturelle und funktional-semantisch angereicherte Daten zu überführen. Der Vorgang dabei kann als erneute Edition der Edition verstanden werden, jedenfalls beinhaltet er eine wissenschaftliche und editorische Leistung. Die dabei leitenden Prinzipien sind die gleichen wie bei der nativen Datenerstellung, und in vielen Fällen müssen die durch solches *reverse engineering* rückerschlossenen Editionskriterien dann mit dem Datenmodell der neu zu edierenden Bestände in Einklang gebracht werden. In Kombination entstehen bedeutende editorische Datensammlungen, die nicht nur der jeweiligen Fachwissenschaft zugutekommen. 

Deutlich ist auch bei diesen Unternehmungen: Jedes Eingabe- und Ausgabeformat benötigt spezielle Aufmerksamkeit, Aufwand, Zeit und finanzielle Ausstattung; der neoliberale Synergiensparstift führt nur zu einem: zu schlecht verwendbaren Applikationen und zu schlecht lesbaren Büchern. 

___
#### Übungsaufgabe 1

eBook-Dateien für E-Reader, etwa im EPUB-Format, sind im Wesentlichen HTML in einen Metadatenwrapper. Wandeln Sie den edierten Text einer der Beispieleditionen aus der Liste auf Seite XXX mithilfe von einfachen Transformationen in EPUB um.^[<https://github.com/jhellingman/tei2html> bietet einen Anfang für die Transformation von TEI Lite-Daten. Noch generischer ließe sich die Herausforderung mithilfe von Pandoc angehen (<https://www.pandoc.org/epub.html>, oder durch Kombination mit den Editierfunktionen von Calibre, vgl. dazu <https://manual.calibre-ebook.com/de/#editing-e-books>).]

#### Übungsaufgabe 2 

Schreiben Sie 500 Wörter zur Frage: Was entspricht dem Begriff der „(Buch-)Auflage“ bei einer digitalen Edition? Beachten Sie dabei die Trennung von Form/Darstellung/Präsentationslayer und Inhalt/Semantik/Editionsdaten und diskutieren Sie Möglichkeiten der eindeutigen Identifizierung einer Version. 

___

## Digitale Editionen: Beispiele 
 
(hier chronologisch nach Erfassungszeitraum gelistet)
 
- The Chronicle of St. Matthew of Edessa <https://editions.byzantini.st/ChronicleME/> (Frühmittelalter, graph based edition, armenisches Alphabet) 
- Cooking Recipes of the Middle Ages <https://gams.uni-graz.at/context:corema> (ab 1300, Mittelhochdt., handschriftliche Quellen)
- Jahrrechnungen der Stadt Basel 1535 bis 1610 <http://gams.uni-graz.at/context:srbas> (frühmoderne Rechnungsbücher als Quelle)
- Digitale Edition von Quellen zur habsburgisch-osmanischen Diplomatie 1500–1918 <https://gams.uni-graz.at/context:qhod> (langer Editionszeitraum, multilingual aus einer Vielzahl von Überlieferungen und Archiven, mehrere Alphabete)
- Sammlung Schweizerischer Rechtsquellen online <https://www.ssrq-sds-fds.ch/online/tei/> (Rechtstexte zwischen 9. und 19. Jh., mehrsprachig, textsortenübergreifend)
- Briefe und Texte aus dem intellektuellen Berlin um 1800 <https://www.berliner-intellektuelle.eu/> (raumorientierte Sammlung, 18. Jh./Aufklärung)
- Ministerratsprotokolle <https://mrp.oeaw.ac.at/> und <https://doi.org/10.5281/zenodo.4568291> (19. Jh., Textsorte Protokoll, polit. Geschichte)
- Korrespondenz Arthur Schnitzler <https://schnitzler-briefe.acdh.oeaw.ac.at/> (literarische Briefe als Quelle auch für Historiker/innen, frühes 20. Jh.)
- Ludwig von Ficker: Gesamtbriefwechsel. Kommentierte Online-Edition <https://edition.ficker-gesamtbriefwechsel.net/> (kulturhistorisch relevante Briefedition des *Brenner*-Herausgebers bis 1967)
 
___
#### Kasten Kataloge digitaler Editionen^[Gekürzt aus: @KurzKatalogedigitalerEditionenKlug2021.]

Nachdem Digitale Editionen nur in seltenen Fällen in Bibliothekskataloge aufgenommen wurden und sonstige zentrale Findemittel bislang nicht etabliert sind, haben Einzelne die Aufgabe übernommen, Metadaten zu Digitalen Editionen zu aggregieren und damit zur Wiederauffindbarkeit publizierter Editionen beizutragen.

- Patrick Sahle, Scholarly Digital Editions. An annotated List. <http://digitale-edition.de/>  
Der für den deutschsprachigen Raum aktuell mit über 700 Einträgen umfassendste Katalog ordnet nach Titel, Fachgebiet, Materialtyp, Sprache und Epoche und hebt eine kleine Shortlist von dzt. 30 Projekten als besondere Empfehlungen hervor.
- Greta Franzini, Catalogue of Digital Editions. <https://dig-ed-cat.acdh.oeaw.ac.at/>  
Der von Greta Franzini seit 2012 betreute Katalog hat die Besonderheit, dass er auch in DBIS gelistet ist. Zum Zeitpunkt der letzten Überprüfung werden Neueinreichungen über GitHub-Issues hinzugefügt.
- Roland S. Kamzelak und Lydia Michel, Marbacher Editionendatenbank. <https://www.dla-marbach.de/digital-humanities/editionen-db/>  
Die Datenbank wird seit 2012 betrieben und verzeichnet deutschsprachige Editionen. Der Datenzugang ist nur nach Anmeldung möglich.
- TEI, Projects Using the TEI <https://tei-c.org/activities/projects/>  
Auch das TEI-Konsortium betreibt einen eigenen Katalog von Editionen, die in diesem XML-Format codiert sind.

___

## Literatur^[Nicht zitiert, aber wichtig sind: @BleierKlugDiscussingInterfacesDigital2018;@KlugElementedigitalerEditionenKlugGalkaSteiner2021; @KurzDasProtokollals2022; @OhgePublishingScholarlyEditions2021; @W3CXMLBaseSecond2009; @NeuberAltbausanierungmitNiveau2020; @Vogelerassertiveedition2019.]


<!-- to build:
pandoc -s --bibliography bib/references.bib --citeproc --csl bib/my-german-apa7.csl --from markdown-footnotes+latex_macros aufsatz-utb-DH-geschichtswiss-ausgabe.md -o aufsatz-utb-DH-geschichtswiss-ausgabe.md.pdf
-->

