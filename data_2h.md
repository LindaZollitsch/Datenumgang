<!--

author:   Linda Zollitsch
email:    zollitsch@ub.uni-kiel.de
version:  0.1.0
language: de
narrator: UK English Female

icon:     images/Logo_cau-norm-de-lilagrey-rgb-0720_2022.png

link: https://raw.githubusercontent.com/RDM4CAU/Intro-to-RDM/refs/heads/main/cau-style.css


comment:  This document provides a brief introduction to data storage and backup.

-->

# Datenumgang (Daten speichern und teilen)



<script input="button">
alert("Disclaimer: Please note that you are leaving the CAU net once you open this presentation in your browser. This presentation includes links to other third party websites and services. These sites are not under our control. RDM@CAU is not responsible for the content of linked third party websites. Please be aware that the security and privacy policies on these sites may be different than CAU policies. Please read third party privacy and security policies closely.")

"Disclaimer"
</script>


<center><img src="./images/fdm_lehre.png" alt="workshop, teaching" height="40%" width="40%"></center>

<div style="page-break-after: always;"></div>

> To see this document as an interactive LiaScript rendered version, click on the
> following link/badge:
>
> [![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://raw.githubusercontent.com/RDM4CAU/TtL-FDM/main/TtL-FDM_Workshop.md#1)
>
> If you have questions, please contact us: [Central Research Data Management](https://www.datamanagement.uni-kiel.de/de)
>
> This work is licenced under CCBY (https://creativecommons.org/licenses/by/4.0/)


## Ziele dieses Workshops

<img src="/images/nachnutzung-fdm-zyklus_2022.png" alt="Goals today" width="200" align="right">

Lernende können ...

* ... allgemeine Anforderungen an Datenspeicherung benennen.
* ... den Unterschied zwischen Speicherung und Backup erläutern.
* ... Beispiele für Datenspeicherung benennen.
* ... Risiken der Datenspeicherung bewerten.


## Überblick

* Datenspeicherung und Backup: Einführung

* Datenspeicherung in der CAU-Cloud

* Daten mit anderen teilen (während der Arbeit daran)



# Datenspeicherung und Backup: Einführung

## Vorgedanken

<div style="float:right; width:40%;">
  <img src="/images/backup.png" alt="No back up? No mercy!">
</div>


{{0-1}}
****************
Wo und wie speichern wir unsere Forschungsdaten?


****************

{{1-2}}
****************

Eigener PC

Mobiles Speichermedium 

  USB-Stick
  Externe Festplatte

Institutionelle Speicherorte

  Cloud
  Virtuelle Laufwerke

Externe Speicherorte (Cloud eines Anbieters)

****************

## Vor- und Nachteile


{{1-2}}
****************


``` ascii
+-----------------++
|                 ||
| Eigener PC      || 
|                 ||           +-----------------++
+-----------------++           | Mobile          ||
                               | Speichermedien  ||
                               +-----------------++
+-----------------++
|                 ||                    +-----------------++
| Institutionelle ||                    |                 ||
| Speicherorte    ||                    | Externe         ||
+-----------------++                    | Speicherorte    ||
                                        +-----------------++ 

```


****************

{{2}}
****************


``` ascii
+-----------------++---------------------------------------------++-----------------------------------------------+
|                 ||                                             ||                                               | 
| Speichermedium  ||                 Vorteile                    ++                  Nachteile                    |
|                 ||                                             ||                                               |
+-----------------++---------------------------------------------++-----------------------------------------------+ 
+-----------------++---------------------------------------------++-----------------------------------------------+
|                 || Verantwortung & Sicherheit bei einem selbst || bei Verlust keine Datenrettung möglich        | 
| Eigener PC      || maximale Kontrolle                          ++ kooperatives Arbeiten Schwierig               |
|                 ||                                             ||                                               |
+-----------------++---------------------------------------------++-----------------------------------------------+ 
+-----------------++---------------------------------------------++-----------------------------------------------+
|                 || leichter Transport                          || Verlust oder Diebstahl möglich                | 
| Mobile          || Aufbewahrung im Safe möglich                ++ Inhalte separat verschlüsseln, da sonst       |
| Speichermedien  ||                                             || nicht geschützt                               |
+-----------------++---------------------------------------------++-----------------------------------------------+ 
+-----------------++---------------------------------------------++-----------------------------------------------+
|                 || Backup & Wartung wird übernommen            || Möglicherweise langsam                        | 
| Institutionelle || Datenschutz der Institution berücksichtigt  ++ Sicherheitsstrategien evtl. intransparent     |
| Speicherorte    ||                                             ||                                               |
+-----------------++---------------------------------------------++-----------------------------------------------+ 
+-----------------++---------------------------------------------++-----------------------------------------------+
|                 || Einfache Nutzung und Verwaltung             || Datenschutz unklar                            | 
| Externe         || Backup und Wartung vorhanden                ++ Abhängigkeit von einem Anbieter               |
| Speicherorte    ||                                             ||                                               |
+-----------------++---------------------------------------------++-----------------------------------------------+ 

```


****************

## Cloudlösungen

{{1-2}}
****************

Beispiel Cloudlösung

<!-- data-type="none" -->
| Cloudanbeiter           | Herkunft  | Open Source | Datenspeicherung | DSGVO  |
| ----------------------- | --------: | -----------:| ----------------:| ------:|
| Dropbox                 | USA       | nein        | unbekannt        | (ja)   |
| OneDrive (Microsoft)    | USA       | nein        | unbekannt        | (nein) |
| iCloud (Apple)          | USA       | nein        | unbekannt        | (nein) |
| Nextcloud (CAU)         | EU        | ja          | EU               | ja     |


****************

{{2}}
****************
Beispiele von zertifizierten Cloudlösungen

https://www.trusted-cloud.de/cloud-service-suche.html 

****************


## Lebensdauer von Speichermedien

> **Speichermedien haben unterschiedlich lange Lebensdauer**:

![Lebensdauer](/images/Lebensdauer.png)


<!-- data-type="BarChart" -->
| Speichermedium       | von | bis |
| -------------------- | ---:| ---:|
| externe Festplatte   |  5  | 10  |
| Festplatte HDD       |  3  |  5  |
| Festplatte SSD       |  5  | 10  |
| SD-Speicherkarte     | 10  | 30  |
| USB-Stick            | 10  | 30  |
| CD/DVD gebrannt      |  5  | 10  |
| CD/DVD gepresst      | 10  | 30  |
| Blu-ray              | 30  | 80  |


in Abhängigkeit von:

* Temperatur
* Feuchtigkeit
* Beanspruchung
* Lagerung


## 3-2-1 Regel

Mindestens 3 Kopien der Daten

... auf mindestens 2 unterschiedlichen Speichermedien

... wovon mindestens 1 Kopie dezentral ist.

Datenwiederherstellung zu Beginn sowie in regelmäßigen Abständen testen!

## Sensible Daten

Besondere Aufmerksamkeit bei sensiblen Daten:

> **Schützen Sie sensible Daten!**
>
>- Hardware (z. B. in einem abschießbaren Raum gelagert)
>- Dateiverschlüsselung
>- Passwortsicherheit
>- Mindestens zwei Personen sollten Zugang zu den Daten haben


## Backup vs. Langzeitarchivierung

| Back up                                                                          | Langzeit Speicherung            |
| -------------------------------------------------------------------------------- | ----------------------------- |
| Automatisches Backup von allen Daten   | Speicherung von ausgewählten Daten |
| All Versionen                                                                     | Nur die finale Version            |
|   zur Verhinderung von Datenverlust <br>(technisch, z.B. Defekt, oder menschlich, z.B. versehentlich gelöscht) | Integritätssicherung <br> (z. B. regelmäßige Überprüfung auf modifizierte oder beschädigte Daten, <br>Dateisystemkonsistenz)      |
|                                                                                  | Langzeitspeicherung             |
|                                                                                  | Durchsuchbar                 |



## Zusammenfassung


**Risiken**

Technische Defekte, Katastrophen (Unwetter), Diebstahl, Vergesslichkeit...

**Strategien**

Speicherung auf institutionellen Servern mit automatischem regelmäßigem Backup, Sicherung wichtiger Daten in mindestens drei Kopien auf räumlich getrennten Datenträgern


# Datenspeicherung in der CAU-Cloud



# Daten mit anderen teilen

Per Mail

über die Cloud








# Herzlichen Dank!

<img src="/images/rdmCAU.png" width="250" align="right">

Mehr zum FDM an der CAU finden Sie hier: https://www.fdm.uni-kiel.de/de

<div style="page-break-after: always;"></div>

# Quellen

https://mediafix.de/die-haltbarkeit-der-speichermedien/

https://forschungsdaten.info/themen/speichern-und-rechnen/datenspeicherung-und-die-lebensdauer-von-datentraegern/

https://www.bsi.bund.de/DE/Themen/Verbraucherinnen-und-Verbraucher/Informationen-und-Empfehlungen/Cloud-Computing-Sicherheitstipps/Cloud-Risiken-und-Sicherheitstipps/cloud-risiken-und-sicherheitstipps_node.html




Biernacka, K., Buchholz, P., Danker, S. A., Dolzycka, D., Engelhardt, C., Helbig, K., Jacob, J., Neumann, J., Odebrecht, C., Petersen, B., Slowig, B., Trautwein-Bruns, U., Wiljes, C., & Wuttke, U. (2021). Train-the-Trainer-Konzept zum Thema Forschungsdatenmanagement (Version 4). Zenodo. https://doi.org/10.5281/zenodo.5773203 

Biernacka, K., Dockhorn, R., Engelhardt, C., Helbig, K., Jacob, J., Kalová, T., Karsten, A., Meier, K., Mühlichen, A., Neumann, J., Petersen, B., Slowig, B., Trautwein-Bruns, U., Wilbrandt, J., & Wiljes, C. (2023). Train-the-Trainer-Konzept zum Thema Forschungsdatenmanagement (Version 5). Zenodo. https://doi.org/10.5281/zenodo.10122153

Engelhardt, C., Biernacka, K., Coffey, A., Cornet, R., Danciu, A., Demchenko, Y., Downes, S., Erdmann, C., Garbuglia, F., Germer, K., Helbig, K., Hellström, M., Hettne, K., Hibbert, D., Jetten, M., Karimova, Y., Kryger Hansen, K., Kuusniemi, M. E., Letizia, V., … Zhou, B. (2022). D7.4 How to be FAIR with your data. A teaching and training handbook for higher education institutions (V1.2.1). Zenodo. https://doi.org/10.5281/zenodo.6674301

Jaeger, Philipp, & Bode, Janice. (2021). Redet über die Daten! - Forschungsdatenmanagement und Hochschullehre in der Physik und darüber hinaus. Zenodo. https://doi.org/10.5281/zenodo.5168524

Klump, J., Wyborn, L., Downs, R., Asmi, A., Wu, M., Ryder, G., & Martin, J. (2020). Principles and best practices in data versioning for all data sets big and small. Version 1.1. Research Data Alliance. [DOI: 10.15497/RDA00042](https://doi.org/10.15497/RDA00042).

Petersen, B., Engelhardt, C., Hörner, T., Jacob, J., Kvetnaya, T., Mühlichen, A., Schranzhofer, H., Schulz, S., Slowig, B., Trautwein-Bruns, U., Voigt, A., & Wiljes, C. (2023). Lernzielmatrix zum Themenbereich Forschungsdatenmanagement (FDM) für die Zielgruppen Studierende, PhDs und Data Stewards (Version 2). Zenodo. https://doi.org/10.5281/zenodo.8010617

Positionspapier zu FAIR und Open Data im physikalischen Praktikum, ZaPF, 2020, online unter https://zapfev.de/resolutionen/wise20/opendata/opendata.pdf

Ryan, R. M., & Deci, E. L. (2000). Self-determination theory and the facilitation of intrinsic motivation, social development, and well-being. American psychologist, 55(1), 68.

Ryan, R. M., & Deci, E. L. (2017). Self-determination theory: Basic psychological needs in motivation, development, and wellness. Guilford Publications.
https://datamanagement.hms.harvard.edu/collect/file-naming-conventions

https://ddi-lifecycle-3-2-documentation.readthedocs.io/en/latest/generalstructures/versioning.html

https://de.creativecommons.net/was-ist-cc/ 

https://force11.org/info/the-fair-data-principles/ 

https://forschungsdaten.info/

https://learn.opengeoedu.de/

https://mantra.ed.ac.uk/

https://www.dfg.de/download/pdf/foerderung/grundlagen_dfg_foerderung/forschungsdaten/forschungsdaten_checkliste_de.pdf

https://www.fdm.uni-hannover.de/fileadmin/fdm/Dokumente/Schulungsunterlagen/Schulungsunterlagen_FDM_VertiefungDatenorganisation_Folien.pdf

https://www.forschungsdaten-bildung.de

https://www.gida-global.org/care 

https://www.nfdi.de/

https://opendata.uni-kiel.de/content/index.xml 

https://opendata.schleswig-holstein.de/dataset 

















# Erste Schritte im FDM

Wir werden uns eine Auswahl an Themenaspekten etwas näher anschauen:

* Dateibenennung & Versionierung
* Dokumentation von Forschungsdaten 
* Nachnutzung von Forschungsdaten

<div style="page-break-after: always;"></div>

## Ordner- und Dateibenennung
{{0-1}}
********************************************************************************
<div style="text-align:center">
><p style="color:#9a047f">**Es mag banal erscheinen, aber eine strukturierte Ordner- und Dateibenennung ist ein erster Schritt im Forschungsdatenmanagement!**</p>
</div>

<center><img src="images/naming-data-comic.png" alt="wild file names" height="150" width="200"></center>

<div style="text-align:center">
<P><SMALL>https://xkcd.com/1459. Shared under CC-BY-NC License</SMALL></P>
</div>

********************************************************************************

{{1-2}}
********************************************************************************
<img src="images/Dateibenennung_bad.png" alt="comic"  style="float:right"/>

* Haben Sie sich schon mal über sich selbst geärgert, weil Sie bestimmte Dateien nicht oder nur mit großem Aufwand finden konnten?

* Sind Ihnen vielleicht sogar schon mal Daten verloren gegangen, weil Dateien versehentlich überschrieben wurden?

---

********************************************************************************

<div style="page-break-after: always;"></div>

{{2}}
********************************************************************************

Ordner und Dateien sollten systematisch benannt und geordnet sein, damit

* die Dateien jetzt und in Zukunft leicht auffindbar und zugänglich sind,
* längeres Suchen von Dateien oder das Vergleichen verschiedener Versionen von Dateien vermieden wird,
* Änderungen nachvollziehbar sind,
* die Dateien nicht versehentlich gelöscht oder überschrieben werden,
* um die Zusammenarbeit zu verbessern und
* Automatisierungsprozesse zu ermöglichen.

********************************************************************************

<div style="page-break-after: always;"></div>

### Ordnerstrukturen

{{0-1}}
********************************************************************************

Folgende Punkte können bei der Erstellung einer nachvollziehbaren Ordnerstruktur helfen:

* Ordner fassen Dateien mit gemeinsamen Eigenschaften zusammen

  * Mögliche Ordnungskategorien: Teilprojekte, Arbeitspakete, Datum oder Zeitraum (z. B. Monate, Quartale), Datentypen, Datenanalysen, Literatur, Formate, ...

* Beschreibende Ordnernamen verweisen auf die Inhalte

* Ordner sind hierarchisch strukturiert

* Es sind nicht zu viele Unterordner angelegt worden (Pfadlänge)

* Laufende und abgeschlossene Arbeiten werden getrennt

* Rohdaten werden gesondert abgelegt

* Es gibt eine Zwischenablage, die regelmäßig aufgeräumt wird -->

* Nicht mehr benötigte Dateien werden regelmäßig gelöscht

********************************************************************************

{{1-2}}
********************************************************************************

Es gilt außerdem:

* Ausprobieren und anpassen
* Dokumentieren/Dokumentation bei Änderungen anpassen
* Für gemeinsam genutzte Dateien gemeinsame Regeln festlegen
* Konsequent bleiben

********************************************************************************

{{2}}
********************************************************************************
Beispiel Ordnerstruktur:

<img src="/images/Abb_OrdnerstrukturArchproject_2022_bp.png" width="350">

********************************************************************************

<div style="page-break-after: always;"></div>

### Dateibenennung
{{0-1}}
********************************************************************************
Die Art und Weise der Benennung von Dateien ist ein wichtiger Baustein im Forschungsdatenmanagement.

Folgende Punkte können bei der Erstellung nachvollziehbarer Dateinamen helfen:


* Weniger als 32 Zeichen (besser noch weniger) für Dateinamen benutzen

* Dateinamen sollten deutlich auf den Inhalt der Datei hinweisen

* Grundsätzlich keine unspezifischen Dateinamen (untitled3746.cvs, protokoll-final.docx) verwenden

* Keine Sonderzeichen, Umlaute oder Leerzeichen in Dateinamen benutzen

* Erlaubte Sonderzeichen sind Unterstrich ( _ ) und Bindestrich ( - )

* Führende Null(en) bei Nummerierungen verwenden

* Datumsangaben nach der ISO 8601 (YYYYMMDD oder YYYY-MM-DD oder YYYY_MM_DD)
********************************************************************************

{{1-2}}
********************************************************************************

**Es gilt außerdem:**

* Prüfen, ob bereits etablierte Dateibenennungskonventionen existieren
* eigene Benennungsregeln in einer Dateibenennungskonvention festhalten
* Konventionen möglichst frühzeitig festlegen
* Unterschiedliche Konventionen für verschiedene Dateitypen sind erlaubt
* Dokumentieren/Dokumentation bei Änderungen anpassen

********************************************************************************

{{2}}
********************************************************************************
Beispiele für Benennungskonventionen:

<img src="/images/Abb_Beispiele-Benennungskonvention_2022_bp.png">

********************************************************************************

<div style="page-break-after: always;"></div>

### Versionierung

{{0-1}}
********************************************************************************

<img src="/images/Comic_Dateibenennung_v2_2022-04-14_CM_web.jpg"> Illustration: Cleo Michelsen

********************************************************************************

<div style="page-break-after: always;"></div>

{{1-2}}
********************************************************************************

>* Um verschiedene Stadien der Bearbeitung von Dateien nachvollziehen und unterscheiden zu können, sollte eine konsequente Versionierung vorgenommen werden.
>
>* Das Vorgehen bei der Versionierung sollte allen, die gemeinsam an Datenmaterial arbeiten bekannt sein.
>
>* Versionierungen können im Dateinamen vorgenommen werden und die Vorgehensweise gemeinsam mit der Dokumentation zu Ordnerstruktur und Dateibenennung in einer README-Datei dokumentiert werden.
>
>* In einer **Versionskontrolltabelle** kann eine Dokumentation der vorgenommenen Änderungen erfolgen.
>
> * <p style="color:#9a047f">***Rohdaten immer separat und ggf. schreibgeschützt abspeichern***</p>

********************************************************************************

<div style="page-break-after: always;"></div>

{{2-3}}
********************************************************************************

**Versionierung im Dateinamen:**

Die Versionierung kann als Bestandteil des Dateinamens definiert werden und dabei zwischen größeren und kleineren Änderungen unterscheiden:

* Beispiel für größere Änderungen = Beispieldatei\_v1 -> Beispieldatei_v2
* Beispiel für kleinere Änderungen = Beispieldatei\_v1.1 -> Beispieldatei\_v1.2
* Beispiel für Major.Minor.Sub-Minor = Beispieldatei\_v0.1.0 -> Beispieldatei\_v0.1.1

><p style="color:#9a047f">**Unspezifische Bezeichnungen vermeiden!**</p>
>
>* ~original1~
>* ~neu~
>* ~bearbeitung2~
>* ~final~
>* ~final_2~


********************************************************************************
<div style="page-break-after: always;"></div>

{{3-4}}
********************************************************************************

**Beispiel für eine Versionskontrolltabelle**

| Versionsnr.  | Änderungen                       | Datum      | Bearbeitung durch |
| :----------  | :----------                      | ---        | ---               |
| 1.0          | Freigabe                         | 2016-11-2  | KL                |
| 1.1          | Verbesserung Rechtschreibfehler  | 2016-11-20 | KL                |
| 1.2          | Änderungen am Layout             | 2017-02-20 | GN                |
| 2.0          | Neues Kapitel (3.1.) hinzugefügt | 2017-02-20 | GN                |

Eine Versionskontrolltabelle kann innerhalb des bearbeiteten Dokuments oder als separate Datei angelegt werden.

********************************************************************************
<div style="page-break-after: always;"></div>

{{4-5}}
********************************************************************************
**Beispiel für eine Versionsinformation innerhalb eines Dokuments:**
<img src="/images/versionsdoku-beispiel-rda_2.png">

********************************************************************************

{{5}}
********************************************************************************

<div style="page-break-after: always;"></div>

**Beispiel eines dokumentierten Versionierungsschemas:**

<img src="/images/OstData_Versionierungsschema.png">

https://zenodo.org/record/6076538#.Y4pE63bMJPa

********************************************************************************
<div style="page-break-after: always;"></div>



### Forschungsdaten zitieren

Im Sinne der guten wissenschaftlichen Praxis müssen Forschungsdaten wie jede andere Quelle eindeutig zitiert werden.

Verschiedene Gruppen und wissenschaftliche Communities haben sich damit beschäftigt, Guidelines und Empfehlungen zur Zitation von Forschungsdaten zu erstellen. 

Hervorzuheben sind hier insbesondere die Empfehlung der Initiative [**Force11**](https://force11.org/) sowie des internationalen Registrierungsservice [**DataCite**](https://schema.datacite.org/).

Es existiert (noch) kein einheitlicher Standard für Datenzitationen.

>- **Nach FORCE11-Empfehlung**: Autor:in(nen) (Publikationsjahr): Titel der Forschungsdaten. Datenrepositorium oder Archiv. Version. Weltweit persistenter Identifikator (vorzugsweise als Link)

>- **Nach DataCite 2013**: Urheber:in (Veröffentlichungsdatum): Titel. Version. Publikationsagent. Genereller Ressourcentyp. Identifikator

---

<div style="page-break-after: always;"></div>


{{1}}
********************************************************************************
>**Aufgabe**: 
>
>Zitieren Sie folgende Publikation nach FORCE11-Empfehlung: http://dx.doi.org/10.13140/RG.2.2.34005.12001 

********************************************************************************

{{2}}
********************************************************************************
>**Lösung**:
>
>Risan, Patrick (2017): Accommodating Trauma in Police Interviews. An Exploration of Rapport in Investigative Interviews of Traumatized Victims. NSD - Norwegian Centre for Research Data. https://doi.org/10.13140/RG.2.2.34005.12001

********************************************************************************

{{3}}
********************************************************************************
>Für die Identifikation von elektronischen Textpublikationen existieren mittlerweile diverse Systeme von persistenten Identifikatoren. 
>
>Die ZBW nennt eine Reihe von existierenden Identifikatoren: https://auffinden-zitieren-dokumentieren.de/zitieren/ 
>
>**Welches ist laut des ZBW-Artikels das am häufigsten verwendete System für persistente Identifikatoren?**

[[ ]] Archival Research Key (ARK)
[[x]] Digital Object Identifier (DOI)
[[ ]] Handle
[[ ]] Persistent URL (PURL)
[[ ]] Uniform Resource Name (URN) 

********************************************************************************

<div style="page-break-after: always;"></div>

### Rechtslage einschätzen 

Um einschätzen zu können, ob und in welcher Form Datensätze und sonstige Materialien nachgenutzt werden dürfen, sollten Lizenzsysteme bekannt sein.

Durch freie Lizenzen wird die Nutzung eines urheberrechtlich geschützten Inhalts nachnutzenden erlaubt. Dabei können Einschränkungen in Hinblick auf den die Verbreitung von Bearbeitungen und Veränderungen oder in Bezug auf die Modalitäten einer weiteren Veröffentlichung bestehen. 

Die am häufigsten verwendeten Lizenzen sind:

- Creative Commons (CC) / für Texte, Abbildungen und Daten geeignet
- GNU General Public License (GPL) / für Software konzipiert
- Open Data Commons (ODC) / für Datenbanken konzipiert
- Community Data License Agreement / für Daten konzipiert

Das hierunter bekannteste Lizenzsystem sind die [Creative Commons Lizenzen](https://de.creativecommons.net/was-ist-cc/):

<div style="width:75%;">
![CCLizenzen](https://herrmayr.de/wp-content/uploads/2019/12/%C3%9Cbersicht_CC_Lizenzen-1024x529.png "Die Creative Commons Lizenzen im Überblick (Quelle: Symbole von Creative Commons Schweiz CC BY 4.0; Tabelle von Burgert/TU München CC BY 4.0)")
</div>

Informationen auf forschungsdaten.info: https://forschungsdaten.info/themen/rechte-und-pflichten/forschungsdaten-veroeffentlichen/creative-commons-lizenzen/

---
<div style="page-break-after: always;"></div>

{{1}}
********************************************************************************







# Orientierung im Themenbereich FDM

<!---
Orientierung im Themenbereich FDM, Grundbegriffe im FDM

Lernziele (LZM-FDM):
Lernende können	den Begriff Forschungsdaten	erläutern.(LZ-ID: 01_001_0007)

Lernende können	Beispiele für Forschungsdaten	benennen. (LZ-ID: 01_001_0008)

Lernende können Themen im Forschungsdatenmanagement (FDM) benennen. (neu)

--->

Der Themenbereich Forschungsdatenmanagement ist komplex. 

Wir wollen uns dem Themenbereich erstmal vorsichtig nähern...


## Begriffsdefinition Forschungsdatenmanagement

{{1}}
********************************************************************************
Das Portal **Forschungsdaten.info** definiert den Begriff **"Forschungsdatenmanagement"** folgendermaßen:

> Forschungsdatenmanagement (FDM) umfasst die Prozesse der **Transformation**, **Selektion** und **Speicherung** von Forschungsdaten mit dem gemeinsamen **Ziel**, diese *langfristig* und *personenunabhängig* **zugänglich**, **nachnutzbar** und **nachprüfbar** zu halten.
>
>(*forschungsdaten.info, letzter Zugriff 29.11.2022*)

********************************************************************************

<div style="page-break-after: always;"></div>

## Begriffsdefinition Forschungsdaten

**Und was sind Forschungsdaten?**

{{2}}
********************************************************************************
Die **DFG** definiert den Begriff **"Forschungsdaten"** folgendermaßen:

> „Zu Forschungsdaten zählen u. a. Messdaten, Laborwerte, audiovisuelle Informationen, Texte, Surveydaten oder Beobachtungsdaten, methodische Testverfahren sowie Fragebögen. Korpora und Simulationen können ebenfalls zentrale Ergebnisse wissenschaftlicher Forschung darstellen und werden daher ebenfalls unter den Begriff Forschungsdaten gefasst. Da Forschungsdaten in einigen Fachbereichen auf der Analyse von Objekten basieren (z. B. Gewebe-, Material-, Gesteins-, Wasser- und Bodenproben, Prüfkörper, Installationen, Artefakte und Kunstgegenstände), muss der Umgang mit diesen ebenso sorgfältig sein und eine fachlich adäquate Nachnutzungsmöglichkeit, wann immer sinnvoll und möglich, mitgedacht werden. Ähnliches gilt, wenn Software für die Entstehung oder Verarbeitung von Forschungsdaten erforderlich ist.“
>
> (*DFG 2021*)

********************************************************************************

{{3}}
********************************************************************************

Etwas weniger kompliziert definierte das PrePARe Projekt der Camebridge University den Begriff **Forschungsdaten** als:

> “Any any information you use in your research.”
>
> (*University of Camebridge PrePARe Project*)

********************************************************************************
<div style="page-break-after: always;"></div>

### Beispiele für Forschungsdaten

<img src="/images/forschungsdatenBSP.png" width="350" align="right">

- Audio- und Videoaufzeichnungen
- Tagebücher
- Daten aus geografischen Informationssystemen (GIS)
- Labor- und Feldnotizen
- Modell-, Skript- und Forschungssoftwarecode
- Bilder und Abbildungen
- Fragebögen und Codebücher
- Proben und Artefakte
- Sensor-Daten
- Sequenzierdaten
- Spektren
- Text- und Tabellenkalkulationsdokumente
- Textkorpora und Annotationen
- Topographie-Daten
- Abschriften

<div style="page-break-after: always;"></div>

## Forschungsdatenlebenszyklus
<!---
Lernende können	Phasen des Forschungsdatenlebenszyklus	benennen. (LZ-ID: 01_005_0079)
--->

<img src="/images/FDM_Zyklus_klein_ohneText.jpg" width="350" align="right">

<P><SMALL>Illustration: Cleo Michelsen, basierend auf dem Forschungsdatenlebenszyklus des UK Data Service</SMALL></P>

<div style="page-break-after: always;"></div>

{{1}}
********************************************************************************
<img src="/images/Planung_fdm-zyklus_2022.png" width="150" align="right">

**Planung**:

* Auf welche Weise entstehen neue Daten?
* Werden Daten wiederverwendet?
* Welche Datentypen, im Sinne von Datenformaten (z. B. Bilddaten, Textdaten oder Messdaten in Tabellen) entstehen?
* Welche Analysen sind geplant?
* Welches Datenvolumen ist zu erwarten?
* Welche rechtlichen und ethischen Aspekte müssen berücksichtigt werden?
* Wer ist verantwortlich?

---

********************************************************************************

<div style="page-break-after: always;"></div>

{{2}}
********************************************************************************
<img src="/images/erhebung-analyse_fdm-zyklus_2022.png" width="150" align="right">

**Erhebung und Analyse**:

* Welche Ansätze werden verfolgt, um die Daten nachvollziehbar zu dokumentieren?
* Welche Maßnahmen werden getroffen, um eine hohe Qualität der Daten zu gewährleisten?
* Welche digitalen Methoden und Werkzeuge (z. B. Software) sind zur Nutzung und Analyse der Daten erforderlich?
* Auf welche Weise werden die Daten während der Projektlaufzeit gespeichert und gesichert?
* Wie wird die Sicherheit sensibler Daten während der Projektlaufzeit gewährleistet (Zugriffs- und Nutzungsverwaltung)?

********************************************************************************
---

<div style="page-break-after: always;"></div>

{{3}}
********************************************************************************

<img src="/images/veroeffentl-archiv_fdm-zyklus_2022.png" width="150" align="right">

**Archivierung & Veröffentlichung**:

* Welche rechtlichen Besonderheiten bestehen im Zusammenhang mit dem Umgang mit Forschungsdaten in dem Forschungsprojekt?
* Sind Auswirkungen oder Einschränkungen in Bezug auf die spätere Veröffentlichung bzw. Zugänglichkeit zu erwarten?
* Auf welche Weise werden nutzungs- und urheberrechtliche Aspekte sowie Eigentumsfragen berücksichtigt?
* Existieren wichtige wissenschaftliche Kodizes bzw. fachliche Normen, die Berücksichtigung finden sollten?

---
********************************************************************************

<div style="page-break-after: always;"></div>

{{4}}
********************************************************************************

<img src="/images/nachnutzung-fdm-zyklus_2022.png" width="150" align="right">

**Nachnutzung**:

* Welche Daten bieten sich für eine Nachnutzung besonders an?
* Nach welchen Kriterien werden Forschungsdaten ausgewählt, um diese für die Nachnutzung durch andere zur Verfügung zu stellen?
* Planen Sie die Archivierung Ihrer Daten in einer geeigneten Infrastruktur?
* Falls ja, wie und wo? Gibt es Sperrfristen?
* Wann sind die Forschungsdaten für Dritte nutzbar?

********************************************************************************

<div style="page-break-after: always;"></div>

## FAIR-Prinzipien

<!---
Lernende können	die FAIR-Prinzipien	benennen. (LZ-ID: 01_007_0117)
Lernende können	die FAIR-Prinzipien	erläutern. LZ-ID: 01_007_0118)
--->


<img src="/images/fair2.jpg" width="250" align="right"> Illustration: Patrick Hochstenbach in Engelhardt, Claudia et. al. (2021).

Ein wichtiges Ziel des strukturierten Foschungsdatenmanagements ist es, Daten langfristig und personenunabhängig zugänglich, nachnutzbar und nachprüfbar zu halten. 

Die [**FAIR-Prinzpien**](https://www.nature.com/articles/sdata201618) dienen als Leitfaden für die Auswahl von Handlungsoptionen, die sicherstellen sollen, dass die im Rahmen von Forschung geschaffenen digitalen Artefakte auffindbar, zugänglich, interoperabel und wiederverwendbar sind.

<div style="page-break-after: always;"></div>

{{1}}
>**F**indable

{{2-3}}
****************
Der erste Schritt bei der (Wieder-)Verwendung von Daten besteht darin, sie zu finden. Metadaten und Daten sollten sowohl für Menschen als auch für Computer leicht zu finden sein. Maschinenlesbare Metadaten sind für das automatische Auffinden von Datensätzen und Diensten unerlässlich und daher ein wesentlicher Bestandteil des FAIRification-Prozesses.

F1. (Meta)data are assigned a globally unique and persistent identifier

F2. Data are described with rich metadata (defined by R1 below)

F3. Metadata clearly and explicitly include the identifier of the data they describe

F4. (Meta)data are registered or indexed in a searchable resource

***************


{{1}}
>**A**ccessible

{{3-4}}
***********************
Sobald der Nutzer die gewünschten Daten gefunden hat, muss er wissen, wie er auf sie zugreifen kann, möglicherweise einschließlich Authentifizierung und Autorisierung.

A1. (Meta)data are retrievable by their identifier using a standardised communications protocol

A1.1 The protocol is open, free, and universally implementable

A1.2 The protocol allows for an authentication and authorisation procedure, where necessary

A2. Metadata are accessible, even when the data are no longer available

******************

<div style="page-break-after: always;"></div>

{{1}}
>**I**nteroperable

{{4-5}}
**********************
Daten sollten in einer Form vorliegen, die die Nutzung mit diversen Anwendungen oder Arbeitsabläufen für die Analyse, Speicherung und Verarbeitung ermöglichen.

I1. (Meta)data use a formal, accessible, shared, and broadly applicable language for knowledge representation.

I2. (Meta)data use vocabularies that follow FAIR principles

I3. (Meta)data include qualified references to other (meta)data

**********************

{{1}}
>**R**eusable

{{5-6}}
***************
Das Ziel von FAIR ist es, die Wiederverwendung von Daten zu optimieren. Um dies zu erreichen, sollten Metadaten und Daten gut dokumentiert und beschrieben sowie mit einer eindeutigen Angabe bzgl. der Nutzungsbedingungen (Lizenzen) versehen sein.

R1. Meta(data) are richly described with a plurality of accurate and relevant attributes

R1.1. (Meta)data are released with a clear and accessible data usage license

R1.2. (Meta)data are associated with detailed provenance

R1.3. (Meta)data meet domain-relevant community standards

**************

<div style="page-break-after: always;"></div>




## Publikation


### Datenpublikation
Wie können Sie Daten veröffentlichen und weitergeben werden?
----

{{1}}
********************
> Ergänzung zu einem von peer-review Artikel („enhanced publication“)
********************

{{2-3}}
****************
- als Ergänzung zu dem zugehörigen Artikel
- als alleinstehenden Datensatz in einem Repository mit einem Link zum entsprechenden Artikel.

<div style="width:100%;">
  <img src="images/Example_R-R-Article.jpg" alt="Example R-R-Article">
</div>

**********************

<div style="page-break-after: always;"></div>

{{1}}
********************
> Unabhängiges Informationsobjekt in einem Repositorium
********************

{{3-4}}
********************

* disziplinspezifische Repositorien, z.B. [Datorium](https://data.gesis.org/sharing/#!Home), [Pangaea](https://www.pangaea.de/)

* fächerübergreifende Repositorien, z. B. [ZENODO](https://zenodo.org/)

* institutionelle Repositorien, z. B. [Refubium](https://www.fu-berlin.de/sites/open_access/refubium/index.html), [opendata@uni-kiel.de](https://opendata.uni-kiel.de/content/index.xml)

Beispiel:

<div style="float:left; width:45%;">
<img src="images/Example_Pangaea.jpg" alt="Example Pangea">
<sub>Source: https://www.pangaea.de/, Zugriff 10.02.2021</sub>

</div>

<div style="float:right; width:45%;">

<div style="width:100%;">
  <img src="images/Example_Zenodo.jpg" alt="Example Zenodo">
  <sub>Source: https://zenodo.org/, Zugriff 10.02.2021</sub>
</div>

</div>

*********************

<div style="page-break-after: always;"></div>

{{1}}
********************
> Data journals

********************

{{4-5}}
***************************

- detaillierte Beschreibung von Forschungsdaten

- teilweise peer-reviewed

Beispiel:

<div style="float:left; width:45%;">
<img src="images/example-datainbrief.png" alt="Example Data journal">
<sub>Source: https://www.earth-system-science-data.net, Zugriff 10.02.2021</sub>

</div>

<div style="float:right; width:45%;">

<div style="width:100%;">
  <img src="images/example-datainbrief.png" alt="Example Data journal">
  <sub>Source: https://www.journals.elsevier.com/data-in-brief, Zugriff 10.02.2021</sub>
</div>

</div>

***************************

<div style="page-break-after: always;"></div>

#### Open Data at Kiel University

>**Information und services @Kiel University:**
>
>* Es gibt keine Richtlinien zur Förderung von Open Data an der CAU :-(
>* [Central Research Data Management](https://www.fdm.uni-kiel.de/en?set_language=en) stellt Informationen, Hilfe und Dienstleistungen bereit
>* [**opendata@uni-kiel**](https://opendata.uni-kiel.de/content/index.xml?lang=en) ist das Open Data Repository der CAU

### Textpublikation

#### Open Access at Kiel University

>**Information und services @Kiel University:**
>
>* [Richtlinien zur Förderung von Open Access an der CAU](https://www.praesidium.uni-kiel.de/de/dokumente/leitlinien-der-cau-zu-open-access)
>* [Universitätsbibliothek](https://www.ub.uni-kiel.de/en/publishing/publishing/information?set_language=en) provides information, help and services.
>   * [Finanzierung von OA](https://www.ub.uni-kiel.de/en/publishing/funding-of-oa-publications?set_language=en)
>* [MACAU ist das Open Access Repository der CAU](https://macau.uni-kiel.de/content/publish/information.xml?lang=en)

<div style="page-break-after: always;"></div>




## Wrap Up

{{0-1}}
********************************************************************************

<img src="/images/kurzberichte.png" width="150" align="right">

**Wir schauen uns ein kurzes Video an. Dies verdeutlicht nochmal die Gründe, warum Forschungsdatenmanagement wichtig ist.**

Movie time!

---

<iframe width="560" height="315" src="https://www.youtube.com/embed/66oNv_DJuPc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---

********************************************************************************
<div style="page-break-after: always;"></div>


{{1}}
********************************************************************************
>**Gutes Forschungsdatenmanagement trägt bei zu ...**
>
> - Reproduzierbarkeit von Ergebnissen (GWP)
> - Rückverfolgbarkeit und Transparenz der Forschung (GWP)
> - gute Auffindbarkeit von Daten, z. B. durch aussagekräftige Benennung und beschreibende Metadaten
> - Wissenserhalt – Daten sollen unabhängig von einzelnen Menschen, Projekten oder Institutionen zugänglich sein (GWP)
> - Erleichterung der Zusammenarbeit
> - Vorbeugung von Datenverlusten
> - Kostenersparnis, z. B. durch Nachnutzung statt neuer Erhebung
> - Transfer der Daten in zukünftige Projekte
> - Erhöhung der Sichtbarkeit der eigenen Arbeit durch Forschungsdatenzitation
> - Erfüllung von Auflagen der Drittmittelgeber
> - ….

********************************************************************************
<div style="page-break-after: always;"></div>



# FDM an der CAU

{{0-1}}
***********

<div style="width: 50%; float:right">
![services](./images/cau-services.png)
</div>

website: https://www.fdm.uni-kiel.de/de

e-mail: <a href="info@fdm.uni-kiel.de">info@fdm.uni-kiel.de  </a>

***********

{{1-2}}
***********
**Beratung**

<div style="width: 20%; float:right">
![working](./images/consultation.png)
</div>

* Antragsberatung

* DMP Beratung

* technische Beratung (Storage, Backup, Tools, usw.)

* Unterstützung bei Peer Reviews

* Hilfe bei der Datenpublikation
***********

{{2-3}}
***********
**Unterstützung bei Training & Lehre**

<div style="width: 20%; float:right">
![working](./images/training.png)
</div>

* Workshops

 * beim Graduate Center, Wissenschaftliche Weiterbildung
 * kleine Gruppen
 * unterschiedliche Zielgruppen
 * grundsätzliche FDM-Grundlagen
 * Spezialisation, z.B. Einführung in Git (auf Anfrage)

* technische Unterstützung auf Anfrage
***********


{{3}}
***********
**Kontakt**

<div style="width: 20%; float:right">
![team](./images/team.png)
</div>

Zögern Sie nicht, uns zu kontaktieren:

>**DMP Beratung:**
>
>Thilo Paul-Stüwe
>paul-stueve@rz.uni-kiel.de
>
>Andreas Christ
>christ@ub.uni-kiel.de 

>**Workshops & Lehrunterstützung:**
>
>Britta Petersen
>b.petersen@rz.uni-kiel.de 
>
>Linda Zollisch 
>zollitsch@ub-uni-kiel.de

***********
