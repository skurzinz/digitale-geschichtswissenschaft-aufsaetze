---
title: 'Transkription und Annotation: Die Eingabeseite digitaler Editionen'
author: Stephan Kurz, ORCID 0000-0003-2546-2570, GND http://d-nb.info/gnd/13281899X
keywords: [TEI, Edition, Digitale Edition, Quellenedition, Text Input]
language: 'de-DE, st-AN'
lang: 'de-DE, st-AN'
abstract: 'Der Artikel führt ein in den aktuellen Stand der Grundlagen und Techniken bei der Erstellung von (Quellen-)Editionen geschichtswissenschaftlicher und verwandter Art. Edition verfährt in Kenntnis der Quellenlage stets regelhaft; für digitale Editionen als den Normalfall jeden Edierens im 21. Jahrhundert werden die Vorschläge der Text Encoding Initiative (TEI) vorgestellt. Edition folgt grundsätzlich einer Logik von Eingabe, Verarbeitung und Ausgabe, sie trennt analytisch immer schon zwischen Struktur- und Darstellungsphänomenen. Das erste Ergebnis der Editionsarbeit sind strukturierte Daten.'
bibliography: [file:bib/references.bib]
---
 
 
# Transkription und Annotation: Die Eingabeseite digitaler Editionen
 
Es gibt für die geschichtswissenschaftliche Arbeit im analogen wie im digitalen Raum ganz unterschiedliche Quellen. Für Historiker:innen ist es nicht nur wichtig, darüber Bescheid zu wissen, welche Quelltypen und Quellen für ihre jeweilige Forschungsarbeit zur Verfügung stehen: Mitunter gehört es zu den Erfordernissen geschichtswissenschaftlicher Forschung, selbst Quellen zu edieren und aus unstrukturierter natürlicher Sprache in strukturierte Daten umzuwandeln. Der vorliegende Beitrag führt zunächst ein in Grundbegriffe der Edition, um dann anhand des wichtigsten Werkzeugs zur Bereitstellung digitaler wissenschaftlicher Editionen den Stand der Technik vorzustellen. Dabei werden beispielhaft zentrale Elemente der Textwiedergabe mithilfe des von der Text Encoding Initiative (TEI) vorgeschlagenen Vokabulars vorgestellt. 

## Edition

Aufgabe der Edition ist es, Quellen verfügbar zu machen. Je nach Ausprägung der spezifischen Edition und den Erfordernissen der betreffenden Quellen gehört dazu auch, Bestände und Zustände aus unterschiedlichen Überlieferungen zusammenzuführen und dabei Chronologie und Abhängigkeit zu etablieren, einen bestimmten textuellen Status nach transparenten Vorgaben herzustellen, etwa durch Kommentar zu kontextualisieren, um dadurch Quellen zu erschließen, in einen Zusammenhang zu stellen, zu bewahren und zu vervielfältigen. Dabei ist es zentral, die eigenen Eingriffe in einen Textzustand von dem durch die Urheber:innen Überlieferten zu trennen und das Vorgehen bei den Prozessen der Edition für die Leserin und den Leser zu dokumentieren. Ziel der wissenschaftlichen Edition ist es, das zu Edierende (zuletzt wurde der Begriff des *Edendums* gestärkt)^[@Manifest-fuer-digitale-Editionen2022, Absatz 2: „Die Grenzen der Edition liegen nicht an den Grenzen von Werken (z.B. literarische, musikalische, bildnerische), Texten (auch des weitesten Textbegriffs) oder Dokumenten (z.B. Briefe, Archivalien, Objekte, audiovisuelle Medien, born digital data). Grundsätzlich ist jede kulturelle Äußerung unabhängig von ihrer Herkunft, Modalität, Medialität und Materialität editionsfähig“.] in „möglichst authentischer Form“ zu bieten (@RLW-Grubmueller-Weimar-Edition-1997).

In diesem Sinne sind die Anfänge der Edition dort zu suchen, wo Texte überhaupt vervielfältigt wurden – *ad fontes* zu gehen hieße dann, mit der Geschichte der Schrift zu beginnen. Die wissenschaftliche oder kritische Edition, die ihre eigenen Voraussetzungen und Handlungen mit transportiert, hat ihre Ursprünge im Zeitalter des Humanismus, als zahlreiche Quellen der Antike neu herausgegeben wurden und mit dem beginnenden Druckzeitalter (@giesecke_frneuzeit spricht vom *Typographeum*) neu zirkulieren konnten. Eine besondere Bedeutung hat die Edition wissenschaftsgeschichtlich in den „positivistischen“ Unternehmungen der zweiten Hälfte des 19. Jahrhunderts gewonnen, als sowohl in der Geschichtsschreibung (Geschichtswissenschaft) als auch der Literaturgeschichtsschreibung (Literaturgeschichte als Königsdisziplin in den Philologien) große Editionsunternehmen begonnen wurden, die teilweise explizit als nationale Projekte begründet wurden. Im Spannungsfeld von Bewahrung alter Quellen und Erschließung im Horizont des jeweils aktuellen wissenschaftlichen Diskurses hat sich seit damals die Editionswissenschaft als eigenes Fach etabliert. 

Die Edition geht in ihrem Tun geleitet von jeweils zu entwickelnden Editionsprinzipien vor. Die Editionswissenschaft hat ein ausdifferenziertes Instrumentarium entwickelt, um die Vorgänge der Textkritik zu systematisieren (eine Reihe von Fachbegriffen siehe Kasten). 

Edition befasst sich im Wesentlichen mit der kontextualisierenden Wiedergabe von materialgebundenen Inhalten. Für die Geschichtswissenschaften sind das hauptsächlich medial überlieferte Dokumente textueller Natur. Grenzwerte dazu wären etwa: die Musikedition, sie erfasst Notentexte; manche Altertumswissenschaften edieren Tonscherben als *text bearing objects*; die *Oral history* muss Tonbänder aus den 1950er Jahren erhalten. 

Wichtig ist für eine Bestimmung der Edition neben der Art ihrer Edenda aber auch, dass es in den meisten Fällen nicht um bloße Reproduktion geht, die der Erhaltung, Überlieferung und dem Zugänglichmachen des Kulturellen Erbes dienen würde, sondern dass die Edition ein Meta-Wissen über die edierten Quellen hinzufügt und im Minimalfall zumindest evidente Fehler der Überlieferung tilgt. Die bloße Sicherung von Archivquellen auf Mikrofilm oder in Bilddigitalisaten allein ist daher noch nicht Edition. Auch hier wieder ein Beispiel: Ausgehend von der Frankfurter Hölderlin-Ausgabe (D.E. Sattler, ab 1972) hat sich in der Germanistik für die textgenetische Edition ein spezifischer Typ der Edition bewährt, der ganz wesentlich auf Faksimiles und deren diplomatischer Umschrift beruht – auch in der Präsentation im Druck. Dieses Verfahren mag oberflächlich betrachtet als Anti-Edition erscheinen, es ermöglicht aber gerade ein Nachvollziehen editorischer Entscheidungen (für eine Lesart, für ein Komma statt eines physisch im Manuskript zu liegen gekommenen Fliegenbeins), die vor dem Hintergrund einer angenommenen auktorialen Intention dann transparent gemacht werden können.^[Beispiel für das Fehlen einer abschließenden auktorialen Intention und deren editorische Umsetzung ist die von Roland Reuß und Peter Staengle im Rahmen der Frankfurter Kafka-Ausgabe (FKA) herausgegebene Faksimile-Edition der *Zürauer Zettel*; die aktuell laufenden Editionsprojekte zu Arthur Schnitzler (Frühwerk: Wien, Mittlere Schaffensperiode: Cambridge, Spätwerk: Wuppertal) wenden ihre Editionsprinzipien auf einen textgenetisch wie durch zahllose autorisierte Drucke wesentlich „gesicherteren“ Autor an.] 

Festzuhalten bleibt: Edition ist stets mehr als Reproduktion. Eine edierte Quelle ist etwas anderes als die ihr zugrunde liegende Quelle erster Ordnung. Editionen „gehören, welchen Anspruch sie auch immer haben, zu wissenschaftlichen Großunternehmungen, sind zeit-, arbeits-, personal- und kostenintensiv.“ (@PlachtaEditionswissenschaft2019, 11)


___
#### Kasten Fachbegriffe der Editionswissenschaft, in der Reihenfolge der Textkritik

Heuristik
: Suche und Sammlung von Textzeugen

Kollation
: Abgleich zu edierender Textzeugen

Recensio
: Variantenanalyse, Auffinden von Lesarten, dabei entsteht nach Möglichkeit ein

Stemma
: „Stammbaum“ der Textzeugen, aus dem die Chronologie und Abhängigkeit ablesbar ist

Emendation
: Verbesserung, Fehlerkorrektur, mitunter auch 

Normalisierung
: von Schreibweisen, Abkürzungen, Rechtschreibung und Zeichensetzung

Konjektur
: „Deutung“, „Vermutung“, inhaltliche und stilistische Korrektur
  
___

Editionen haben in der Textkritik ein standardisiertes Verfahren (s. Kasten, vgl. auch @SchwentnerTextkritikDigitalenEditionenKlugGalkaSteiner2021), das abhängig vom Editionsgegenstand und von den meist fachspezifischen Erkenntnisinteressen unterschiedlich gewichtet. Auch bedingen international unterschiedliche Wissenschaftstraditionen unterschiedliche Herangehensweisen an Edition und Konzepte davon (@PlachtaWieinternationalist2012). Die Editionen der philologischen Fächer fokussieren, da sie zumindest implizit dem Paradigma einer auktorialen Intention folgen (@Martus-Werkpolitik-zur-Literaturgeschichte-kritischer-2007, @Bosse-Autorschaft-ist-Werkherrschaft-uber-1981), auf die Herstellung gültiger Texte (auch sie, nicht nur die Kommentare einer Edition, sind stets Kinder ihrer Zeit und des je aktuellen Standes der Wissenschaft, was auch neue Editionen klassischer Autor:innen rechtfertigt), während andere Disziplinen die Quellenkritik im Editionsprozess eher auf den wissenschaftlichen Kommentar auslagern. Je nach Gattung oder Textsorte der Edenda erübrigt sich oft auch die Suche nach Varianten und Textzeugen – von eigenhändigen Briefen, Tagebüchern oder von geheimen Sitzungsprotokollen existieren üblicherweise schlicht keine Varianten, sondern allenfalls Abschriften oder technisch erzeugte Kopien. 

Wissenschaftliche Editionen haben wissenschaftliche Ziele. Diese können ganz unterschiedlich gesteckt sein – Geht es etwa um die dringende Konservierung eines Korpus von drei neu aufgefundenen fragilen Papyrusfragmenten durch Faksimilierung? Oder darum, der Forschung möglichst rasch einen Überblick über die Entscheidungsprozesse eines Regierungsorgans der Neuzeit über einige Jahrzehnte zu ermöglichen? Im ersten Fall wird die Edition allein aufgrund des geringeren Quellenumfangs ausführlicher auf Informationen zum Textträger abheben können und jedenfalls Abbildungen einbeziehen, im zweiten Fall werden aus Dutzenden Aktenlaufmetern vielleicht „nur“ Metadaten und Verschlagwortung zur besseren Auffindbarkeit als Regestenedition erstellt werden können. 

Je nach Zielgruppe, Umfang des Quellenbestandes, dem wissenschaftlichen Ziel der Edition, und nicht zuletzt auch der personellen und finanziellen Ausstattung eines Editionsunternehmens kommen dabei unterschiedliche Editionsmodelle zur Anwendung (siehe Kasten). 

___
#### Kasten Editionsmodelle

Regestenedition
: sie nimmt die Quelle/n dem Inhalt nach auf, indem sie (meist kurze) Zusammenfassungen – Regesten – erstellt. Beispiel: die *Regesta Imperii* (<http://www.regesta-imperii.de>)

Historisch-Kritische Edition
: nimmt alle verfügbaren Lesarten zu einer Quelle auf und unterzieht sie kritischer Bewertung sowie textgenetischer Analyse, meist mit einem ausführlichen Kommentar. Ausgeführt ist sie als

  - diplomatische Ausgabe – sie gibt eine Quelle anhand eines Leittextzeugen in dessen ursprünglicher Form wieder, oder als 
  - eklektische Ausgabe, welche Bestandteile verschiedener Zeugen kombiniert, wenn etwa kein Textzeuge einen vollständigen Text bietet. 

Wissenschaftliche Studienausgabe
: ermöglicht eine eingehende Beschäftigung mit der Quelle, der Kommentar (fallweise die Lesarten) sind weniger ausführlich gehalten. Dieses Editionsmodell verzichtet auf die Vollständigkeit der Erfassung aller Überlieferungen zugunsten eines gesicherten Textes.

Auswahleditionen
: sind darüber definiert, dass sie, anders als die meisten Historisch-Kritischen Editionen, keine vollständige Überlieferung ihres Editionsgegenstandes bieten, sondern eine – jeweils zu begründende – Auswahl daraus wiedergeben.

Leseausgabe
: verfolgt das Ziel, eine Quelle für die Lektüre verfügbar zu machen, nicht unbedingt für die wissenschaftliche Auseinandersetzung damit. Sie richtet sich an ein breiteres Publikum.
  
___

## Digitale Edition

![Abb. 1](DSE-workflow.svg "Abb. 1")

<!-- 
digraph DSE {
    Quelle -> 
    {rank = same; Bilddigitalisate; Metadaten;}
    Normdaten -> Semantik; 
  Bilddigitalisate -> "OCR/HTR" -> Editionsdaten;
  Bilddigitalisate -> "Transkription" -> Editionsdaten;
  Bilddigitalisate -> Struktur;
  Struktur -> Editionsdaten; Semantik -> Editionsdaten; Metadaten -> Editionsdaten; 
  Editionsdaten -> Editionsdaten; 
  Editionsdaten -> Langzeitarchivierung; 
  Editionsdaten -> Webapplikation;
  Editionsdaten -> Printausgabe;
  Editionsdaten -> "API-Zugriff";
  
  label = "\nSchematischer Abriss Vorgehensweise bei der Eingabe, Verarbeitung und Ausgabe von Daten
  für die digitale Edition; Eigenes Werk Stephan Kurz, \nCC-BY 4.0 https://creativecommons.org/licenses/by/4.0/deed.de";
}
-->
 
Im 21. Jahrhundert ist die digitale Edition der Normalfall des Edierens geworden (@Manifest-fuer-digitale-Editionen2022, Abs. 3); diesem Umstand tragen auch die Forschungsförderungsinstitutionen bei ihrer Förderpolitik Rechnung. Digitale Edition ist gewissermaßen die Fortsetzung der Editionspraxis mit Mitteln des digitalen Mediums. Die oft zitierte zirkelschlüssige Definition von Patrick Sahle – digitale Edition sei „Edition, die einem digitalen Paradigma folgt“ – lässt sich vor dem Hintergrund der von ihm klar ausdifferenzierten Textbegriffe nochmals herausarbeiten: Der Text (oder auch: das Edendum) kann betrachtet werden als abstrakte Idee, als Werk mit einer Struktur, als sprachlicher Ausdruck, als eine Fassung, als ein materielles Dokument und als Container visueller Zeichen.^[@SahleDigitaleEditionsformenZum2013b, 9–64, dort auch visualisiert als „Textrad“. Sahles Ausführungen beziehen sich klar auf Begriffe von Text, die der Edition zugrundeliegen; im Wesentlichen ließe sich dies aber auch zu beliebigen *Edenda* erweitern. Zum Textbegriff vgl. auch @reuss-textentwurfwerk.] 
 
In Bezug auf die Mittel der Produktion, Zirkulation und Rezeption gilt dabei: „die Essenz des gegenwärtigen Medienwandels ist nicht der Wechsel von analogen zu digitalen Medien, sondern der Übergang vom Denken in Medien zum Denken in Modellen und Daten.“ (@SahleZwischenMediengebundenheitund2010) Auch die damit ins Zentrum gerückten „Daten“ sind dabei nichts epochal Neues, sie waren schon in der Arbeit mit Karteien und Zettelkästen, wie sie die großen Editionsunternehmen des ausgehenden 19. Jh. geführt haben, letztlich Grundlage einer inhärent vernetzten Arbeit (vgl. @PetscharDer-Zettelkatal; @KrajewskiZettelwirtschaft2002; zur Methodenkritik digitaler Geschichtswissenschaft den Beitrag von Mareike König in diesem Band). Im digitalen Medium kommt die technische Vernetzbarkeit von Daten hinzu, weiters orientieren sich digitale Editionen an den FAIR-Prinzipien (Findable, Accessible, Interoperable, Reusable) und sind üblicherweise in Form frei lizenzierter Daten und Applikationen offen verfügbar. Die grundlegenden Abläufe bei der digitalen Edition (Eingabe – Verarbeitung – Ausgabe) zeigt die Abb. 1. Dieser Beitrag konzentriert sich auf Eingabe und Verarbeitung, zur Ausgabeseite des Editionsprozesses vgl. den Beitrag d. Verf. im Abschnitt „Publizieren – Präsentieren“. 

Zur Vernetzung von Wissensbeständen hier ein konkretes Beispiel aus der Edition zu einem Briefindex zur Korrespondenz des Großbotschafters Damian Hugo v. Virmont an Kaiser Karl VI. Im Rahmen des Friedens von Passarowitz/Požarevac 1718 war zwischen Sultan Ahmed III. und Karl VI. der Austausch von Großbotschaftern vereinbart worden. Die Korrespondenzen, wechselseitigen Reiseberichte, Zeitungsartikel, Protokollregistereinträge und anderes Material, das auf beiden Seiten zahlreich überliefert ist, werden in einem 2020 begonnenen Projekt unter Beteiligung des Verf. an der Österreichischen Akademie der Wissenschaften ediert. Die Dokumente der Großbotschaft Virmont 1719–1720 sind u.a. im Österreichischen Staatsarchiv überliefert – darunter befindet sich auch eine zeitgenössisch angefertigte handschriftliche Liste der 57 Stücke umfassenden Hofkorrespondenz des Großbotschafters „Sambt ainem indice und kurzen extract über die darinen enthaltene materias“. Der erste Eintrag bezieht sich auf einen Brief aus dem heutigen Rumänien auf der Hinreise der Gesandtschaft nach Konstantinopel. Er lautet: 

> Nr. 1 d.d.: Erdöd 27. Maii 1719 Berichtet den fortgang ohne beylag seiner raise, und daß ein page des grafen Bathyan einen laggey des grafen von Türheimb erstochen. (@VirmontBriefindex1719_1720)

Die Nummerierung verweist auf einen Brief, das Datum lässt sich ohne Schwierigkeiten als maschinell verarbeitbares ISO-Datum (1719-05-27) ausdrücken; die Referenz auf die Stadt Erdöd (heute rumänisch Ardud) lässt sich durch Identifizierung und Disambiguierung mithilfe eines Identifikators, z.B. jenem aus GeoNames – <https://sws.geonames.org/686206/> – vereindeutigen. Dass die Diener Carl Graf von Batthyánys (<https://d-nb.info/gnd/116082291>) und Johann Wilhelm Graf von Thürheims (kein GND-Eintrag) gemeint sind, die in den Quellen namenlos bleiben, lässt sich ebenso festmachen wie deren jeweilige Beziehung zu ihrem genannten Dienstherrn. – Ein Zettelkasten hätte bis hier Abteilungen zu führen für: Briefe/Dokumente, Orte, Daten, Personen und für die möglichen Relationen zwischen diesen (z.B. Person ist Diener von Person, Ort ist Geburtsort von Person, Person ist Mitglied von Institution, Datum ist Sterbedatum von Person, Person ist erwähnt in Werk/Brief usw.). Dass sowohl hinter dem Digitalisat des Briefs Nr. 1 (ediert als @VirmontAnHofkriegsrat17190527) als auch hinter jenem des edierten Briefverzeichnisses auch ein physisches Objekt mit Eigenschaften, einem Bestandsnachweis und einer digitalen Reproduktion mit einem bestimmten Dateinamen steht, macht die Datenstruktur nur größer, ohne sie konzeptuell überkomplex zu machen: All dies ließe sich auch mithilfe eines Zettelkastens abbilden. 

Derartige Datenstrukturen müssen erstens gut geplant sein, um alle möglichen Fälle abzudecken; zweitens müssen Eingabeformate und -Werkzeuge zur Verfügung stehen, um die Daten komfortabel erfassen und bearbeiten zu können, drittens müssen Darstellungsweisen gefunden oder geschaffen werden, um die Daten auch wieder zugänglich zu machen. Im Zeitalter der gedruckten Edition waren das Werkzeug für die drei Schritte erstens Zettelkästen, zweitens penible Datenein- und Ausgabe aus diesen Zettelkästen, drittens die Zusammenarbeit mit gut ausgebildeten Setzer:innen und Korrektor:innen. Die digitale Edition verfährt ähnlich, nur ist der Umgang mit Regeln und Werkzeugen des analogen Ordnens und des Buchdrucks ersetzt worden durch meist autodidaktisches Desktop-Publishing und durch die Vervielfältigung der Ausgabemedien. Der grundlegende Ablauf von Eingabe – Verarbeitung – Ausgabe hat sich allerdings nicht gewandelt. 

## Eingabe und Verarbeitung in TEI

Möglich gemacht wird die „Verdatung“ digitaler Editionen mithilfe technischer Lösungen. Die weitaus am häufigsten verwendeten Technologien bauen auf XML-Markup auf, das sich in den vergangenen Jahrzehnten gemeinsam mit den Schwestertechnologien XPath, XQuery, XSL-T und einigen weiteren als stabile technische Lösung für sämtliche oben angesprochenen Herausforderungen erwiesen hat (@Becher-XML-DTD-XML-Schema-2009; @W3CXMLBaseSecond2009; dazu vgl. auch @vogelerXML2017 sowie den Teil „Transkribieren und Annotieren“ in diesem Band). Als de-facto-Standard haben sich die Empfehlungen der Text Encoding Initiative (@teiconsortiumTEIGuidelines) herauskristallisiert, die von einer umfassenden Gemeinde von digitalen Editor:innen zum Zweck der gleich- oder doch ähnlichförmigen Kodierung von Textphänomenen seit 1994 (mit Vorstufen) entwickelt werden.^[Eine gute Einführung bietet @BurnardWhatisText2014. Die Vorschläge der TEI werden zumindest als menschen- und maschinenlesbares Archivierungs- und Datenaustauschformat Bestand haben. Alternativen zur Modellierung in TEI wären Text-as-Graph oder andere Markupsprachen; Reines JSON und JSON-LD sind an der Grenze des Menschenlesbaren, gewinnen aber in der Applikationsentwicklung für die Publikation von Editionsdaten an Bedeutung.] Dass damit ähnlich wie in der Bibliothekswelt Titel- und Personendaten maschinenlesbar austauschbar gemacht werden können, also beispielsweise eine Streichung in einem Brief von Karoline von Günderrode ebenso als `<del>` markiert wird wie jene in einem Konzept zu einem Großveziersbefehl, dass TEI-codierte Texte durch den Metadatenblock `<teiHeader>` auch ihre Beschreibung und die Dokumentation der Editionsprinzipien in einer einzigen Datei beinhalten können, dass durch strukturelles Markup Texte in hierarchisierte Abschnitte (z.B. `<front|body|back>` und `div`, welche Absätze `<p>`, Listen `<list>` uvm. enthalten) untergliedert werden können und all diese Informationen sowohl für den Menschen (der in den TEI-Guidelines nachlesen kann, wie das betreffende Element bestimmt ist) als auch für die Maschine auslesbar ist, zeigt die Wichtigkeit und Nützlichkeit so eines Standards auf: Ging es bei der maschinenlesbaren Erfassung von Metadaten darum, z.B. nur das „Titel“-Feld durchsuchbar zu machen, geht es bei der standardisierten Erfassung von Textdaten um die gleichartige Auffindbarkeit von Phänomenen des Textes (des Edendums) selbst. Mindestens ebenso wichtig ist, dass der TEI-Standard auch durch eigene Elemente erweitert werden kann.^[„In brief, the TEI Guidelines define a general-purpose encoding scheme which makes it possible to encode different views of text, possibly intended for different applications, serving the majority of scholarly purposes of text studies in the humanities. Because no predefined encoding scheme can possibly serve all research purposes, the TEI scheme is designed to facilitate both selection from a wide range of predefined markup choices, and the addition of new (non-TEI) markup options.“ (@teiconsortiumTEIGuidelines, <https://tei-c.org/release/doc/tei-p5-doc/en/html/AB.html#ABTEI2>).]

Mit TEI kodierte Texte lassen sich über ein Editionskorpus durch Festlegung des Vokabulars aus dem Gesamtumfang der bestehenden TEI-Module (etwa für Handschriften, für Dramentexte, für Wörterbücher usw.)^[Die TEI-Community stellt mit ROMA für diesen Zweck ein Tool zur Verfügung: <http://roma.tei-c.org/>.] gleichförmig machen, indem durch ein XML-Schema bestimmte Elemente in ihrer Kardinalität und Position festgelegt oder Attribute auf eine Auswahl bestimmter Werte begrenzt werden. Ein Korpus von einigen tausend Briefen lässt sich mit diesem Werkzeug innerhalb kurzer Zeit „validieren“, um zu prüfen, ob bspw. an einer Stelle ein Titel vergessen wurde oder eine Fußnote keinen Literaturnachweis beinhaltet. Solcherart mehr oder weniger „hart“ definierte Editionsrichtlinien müssen selbstverständlich in einem vorangegangenen Schritt der Datenmodellierung erarbeitet werden (@ResminiBriefHistoryInformation2011, @KlingnerForschungsdesign402019), sie erleichtern dann aber die Arbeit mit den Quellen. 

In der täglichen Arbeit mit digitalen Editionen in TEI-XML lässt sich grob unterscheiden zwischen der Aufnahme von 1) Metadaten, die Quelle und Edition beschreiben, 2) Strukturdaten, die die Textgliederung etwa in Absätze und Abschnitte wiedergeben, sowie 3) semantischem Markup, das einzelne Zeichenketten in ihrer kommunikativen Funktion kennzeichnet.

An dem obigen kurzen Zitat aus dem historischen Briefindex exemplifiziert hieße das: 

1. Erstens sind im `<teiHeader>` zumindest die Archivsignatur, Urheberschaften, Datierung und Titeldaten der Quelle und der Edition, ein Verweis auf die Editionsrichtlinien des Projekts verankert.
2. Das Element `<facsimile>` zweitens beinhaltet Verweise auf digitale Reproduktionen der Quelle und unter Umständen Koordinaten bestimmter Bereiche als `<zone>`.
3. Drittens, der gesamte zitierte Eintrag ist ein `<item>` in einer <`list`> von Briefen, er hat ein `<label>` mit einer Nummerierung (`@n`), deren Repräsentation verweist auf den an anderer Stelle edierten Brief und 
4. viertens wird semantisch erschlossen durch `<rs>`-Tags um Personen- und Ortsnamen (vgl. Kasten Named Entities) sowie die normalisierte Datierung (`<date>`) 

Ein wichtiges Prinzip von digitalen Editionen in diesem engeren Sinn ist die Trennung von Semantik und Darstellung: Während auf der Darstellungsebene z.B. eines Buches verschiedene textuelle Phänomene *kursiv* gedruckt erscheinen, lassen diese sich doch funktional und semantisch voneinander abtrennen: Der lebende Kolumnentitel einer Editionsreihe ist dann als solcher definiert (`<fw type="header" rend="#italic">Kapitelüberschrift</fw><fw type="pageNum" rend="#italic">Seitenzahl</fw>`), die Emphase innerhalb des edierten Textes (`<emph>`) hat einen anderen Stellenwert als der ebenfalls kursiv gesetzte Buchtitel im Zitat (`<title><hi rend="#italic">Titel</hi></title>`). Dies ermöglicht einerseits eine zielgenaue Adressierung aller Elemente einer Klasse (etwa, um Kolumnentitel für die Analyse aus den Textdaten wegzulassen), andererseits auch die Änderung der Darstellungsweise für eine Elementklasse (sollte z.B. eine Änderung des Zielformats für Titelangaben in den Fußnoten erwünscht sein, lassen sich alle `//note//title/hi[@rend='#italic']` auch in grün pulsierenden Kapitälchen wiedergeben. 

Die Trennung von Inhalt und Darstellungsweise ist erfahrungsgemäß eine konzeptionelle Hürde. Gewärtigt man allerdings, dass die unterschiedliche Darstellung gleicher wie die gleiche Darstellung unterschiedlicher Sachverhalte letztlich auch nur vorher vereinbarten Konventionen folgt, so liegt nahe, mit dem Vokabular etwa der TEI-Guidelines zunächst einmal den semantischen Gehalt aufzuzeichnen (ggf. zusätzlich dessen ursprüngliche Darstellungsweise in der Quelle über ein `@rend`- oder `@rendition`-Attribut). 

Ein oft diskutiertes Problemfeld der Edition ist jenes der Frage nach der zu erzielenden Erschließungstiefe. Sie richtet sich nach den Ansprüchen des Faches, ist aber auch Aushandlungssache zwischen dem technisch Machbaren und dem finanziell und zeitlich Umsetzbaren. Viele digitale Editionen der letzten Zeit haben z.B. die Auszeichnung von Metadaten, Schlagwörtern, Strukturdaten und Textsemantik inklusive der Named Entities (s. Kasten) an einzelnen Text- (oder Objekt-)zeugen in den Vordergrund gestellt und dabei den angestammt wichtigen wissenschaftlichen Beitrag der Kommentierung auf Grundlage der Textkritik hintangestellt. Das ergibt schon ein kursorischer Durchgang durch auch nur die aus den Philologien stammenden digitalen Editionen in den gängigen Katalogen (siehe Kasten Kataloge digitaler Editionen). Durch die Analyse solcher relativ oberflächlichen Strukturdaten lassen sich v.a. Fragen des *Distant Reading* systematisch bearbeiten.^[Zu den Möglichkeiten (v.a. literaturwissenschaftlicher) Analyse vgl. @SchoechEindigitalesTextformat2016; Korpora werden tw. ebenfalls international vergleichbar mit TEI analysierbar gemacht, vgl. dazu die COST-Action „Distant Reading“ (<https://www.distant-reading.net/>, letzter Zugriff 2.9.2022). Zu Begriff und Methoden von Distant Reading vgl. @MorettiDistantReading2013.]

___
#### Kasten Named Entities

Allgemeine Bezeichnung für benannte/benennbare Einheiten, die aus Texten heraus in der digitalen Edition referenziert werden. Üblich kommen Tags zur Anwendung für 

- Personen – in TEI als `<person>` mit dem Bezugselement `<persName>` oder `<name type="person">` für Namensnennungen, `<rs>` (referring string) für indirekte Bezüge („ihre Schwester“)
- Orte – in TEI als `<place>` mit dem Bezugselement `<placeName>` oder `<rs type="place">` und 
- Institutionen/Organisationen – in TEI als `<org>` mit dem Bezugselement `<orgName>` oder `<rs type="org">`

Weitere Entitätentypen etwa für Objekte `<object>` sind im TEI-Schema angelegt, ähnlich verhält es sich mit bibliographischen Einheiten `<bibl>` und `<biblStruct>`, mit Nymen als verallgemeinerte Namensstandardisierung `<nym>` oder mit Taxonomien `<taxonomy>` und `<category>`. Ausbaufähig ist die in TEI vordefinierte Verwendung von Ereignisdaten als `<event>`. Diese Liste ist jedoch – wie das TEI-Schema insgesamt – durch die Benutzer:in erweiterbar. 

In der digitalen Edition werden Named Entities üblicherweise in externen Listen bearbeitet, auf die über Identifikatoren in den edierten Dokumenten verwiesen wird. Zentrales Feature dabei ist das Kenntlichmachen (Identifikation) und die Vereindeutigung (Disambiguierung) von Namen (Bezeichnern) über Identifikatoren aus sogenannten Normdateien (engl. *authority files*), also Konkordanzen von Bezeichnern und Bezeichnetem. Im deutschsprachigen Raum wird meist der Identifikator der aus dem Bibliotheksbereich stammenden Gemeinsamen Normdatei (GND-Id) für Personen verwendet (die Gemeinsame Normdatei listet bspw. 25 distinkte Personen, auf die das Suchmuster „Mayer, Maria“ passt). Die GND umfasst auch Daten zu Institutionen und Organisationen. Für Ortsbezeichnungen bietet sich neben den GND-Daten die GeoNames-Id an, welche multilinguale Toponyme mit entsprechenden geographischen Koordinaten verknüpft (darunter drei in Deutschland und zwei in den USA gelegene Orte namens Salzburg).^[GND: Gemeinsame Normdatei, recherchierbar über <https://portal.dnb.de/>; GeoNames ist eine offene Datenbank von Ortsbezeichnungen und zugehörigen Geodaten, siehe <https://www.geonames.org/>.]

*Named Entity Recognition* (vgl. die Beiträge von Melanie Althage und Charlotte Schubert in diesem Band) ist der Prozess regel- oder modellgetriebener automatischer Erkennung von Eigennamen und Bezeichnern im Zuge der automatisierten Textverarbeitung etwa durch *Part-of-Speech-Tagging*. 

___

Im Gesamtgefüge der mit „digitalen“ Mitteln betriebenen Geschichtswissenschaft jinnt der wissenschaftlichen digitalen Edition ein zentraler Stellenwert zu. Sie ermöglicht einen standardisierten Zugriff auf edierte Quellen, der nicht nur auf die engen Grenzen des einzelnen Fachs beschränkt ist. Mit der an Standards wie dem TEI-Vokabular orientierten Wiedergabe der Edenda lässt sich neben dem „Inhalt“ einer Quelle auch deren Form in menschen- wie maschinenlesbarer Form abbilden. 

Grundsätze der Textwiedergabe wie individuelle Verantwortlichkeiten für Lesarten, Kommentare, Änderungen werden in der digitalen Edition mit dokumentiert.

Erstes Ergebnis der Tätigkeit wissenschaftlicher Editor:innen sind damit zunächst standardisierte (XML-)Dateien. Diese beinhalten die nach den Editionsgrundsätzen aufgenommenen Informationen zu Struktur und Semantik der Quelle/n und alle erforderlichen Metadaten dazu. Der Wiedergabe dieser Informationen in verschiedenen Ausgabeformaten – Webapplikationen, aber auch Druckerzeugnisse – ist im Abschnitt „Publizieren – Präsentieren“ ein eigener Beitrag gewidmet. 

## Literatur^[Nicht zitiert, aber wichtig sind: @BohnenkampRenkenMedienwandelMedienwechsel2012; @BurnardWhatisText2014; @CummingsworlddifferenceMyths2018; @DFGPraxisregelnDigitalisierung2016; @DiPietroInnovationConservationNarrow2018; @Edlex2016; @EarhartDigitalEditionDigital2012; @EferGraphdatenbankenfuerdie2016; @DumontEncodingCorrespondence2019; @HofmeisterTextkritik2005; @JannidisDigitalHumanities2017; @KlingnerForschungsdesign402019; @LukasAnnotierenKommentierenErlaeutern2020; @MartensTexteundVarianten1971; @NuttKofothEditionsphilologieAnz2007; @PlachtaWieinternationalist2012; @ResminiBriefHistoryInformation2011; @SchoechEindigitalesTextformat2016; @W3CXMLBaseSecond2009; @Kanzog-Einfuhrung-in-die-Editionsphilologie-1991; @giesecke_frneuzeit; @GorbachLesbar2019; @SteinerGAMSCiriloClient2017.]

<!-- to build this: 
pandoc -s --bibliography bib/references.bib --citeproc --csl bib/my-german-apa7.csl --from markdown-footnotes+latex_macros aufsatz-utb-DH-geschichtswiss-eingabe.md -o aufsatz-utb-DH-geschichtswiss-eingabe.md.pdf
-->