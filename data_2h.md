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

# Datenumgang (Daten speichern und teilen) 💾



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


## Ziele dieses Workshops 🎯

<img src="/images/nachnutzung-fdm-zyklus_2022.png" alt="Goals today" width="200" align="right">

Lernende können ...

* ... allgemeine Anforderungen an Datenspeicherung benennen.
* ... den Unterschied zwischen Speicherung und Backup erläutern.
* ... Beispiele für Datenspeicherung benennen.
* ... Risiken der Datenspeicherung bewerten.


## Überblick

* Datenspeicherung und Backup: Einführung 📝

* Datenspeicherung in der CAU-Cloud ☁ 

* Daten mit anderen teilen (während der Arbeit daran) 📚 



# Datenspeicherung und Backup: Einführung 📝

<div style="float:right; width:40%;">
  <img src="/images/backup.png" alt="No back up? No mercy!">
</div>


{{0-1}}
****************
Wo und wie speichern wir unsere (Forschungs)Daten? 🗨️


****************

{{1-2}}
****************

- Eigener PC

- Mobiles Speichermedium 

    - USB-Stick
    - Externe Festplatte 

- Institutionelle Speicherorte

    - Cloud
    - Virtuelle Laufwerke

* Externe Speicherorte (Cloud eines Anbieters)

****************

## Vor- und Nachteile


{{1-2}}
****************

<!--
style="
  max-width: 500px;
  background-color: #fee1ff;
  stroke: #9a047f;" -->
``` ascii
+-----------------+
| Eigener PC 💻  |            +-----------------+
+-----------------+            | Mobile 💽      |
                               | Speichermedien  |
                               +-----------------+


+-----------------+                    +-----------------+                
| Institutionelle |                    | Externe         |
| Speicherorte    |                    | Speicherorte    |
+-----------------+                    +-----------------+
                   

```


****************

{{2}}
****************


``` ascii
+-----------------+---------------------------------------------+-----------------------------------------------+
|                 |                                             |                                               | 
| Speichermedium  |                 Vorteile                    |                  Nachteile                    |
|                 |                                             |                                               |
+-----------------+---------------------------------------------+-----------------------------------------------+ 
|                 | Verantwortung & Sicherheit bei einem selbst | bei Verlust keine Datenrettung möglich        | 
| Eigener PC      | maximale Kontrolle                          | kooperatives Arbeiten Schwierig               |
|                 |                                             |                                               |
+-----------------+---------------------------------------------+-----------------------------------------------+
|                 | leichter Transport                          | Verlust oder Diebstahl möglich                | 
| Mobile          | Aufbewahrung im Safe möglich                | Inhalte separat verschlüsseln, da sonst       |
| Speichermedien  |                                             | nicht geschützt                               |
+-----------------+---------------------------------------------+-----------------------------------------------+ 
|                 | Backup & Wartung wird übernommen            | Möglicherweise langsam                        | 
| Institutionelle | Datenschutz der Institution berücksichtigt  | Sicherheitsstrategien evtl. intransparent     |
| Speicherorte    |                                             |                                               |
+-----------------+---------------------------------------------+-----------------------------------------------+ 
|                 | Einfache Nutzung und Verwaltung             | Datenschutz unklar                            | 
| Externe         | Backup und Wartung vorhanden                | Abhängigkeit von einem Anbieter               |
| Speicherorte    |                                             |                                               |
+-----------------+---------------------------------------------+-----------------------------------------------+ 

```


****************

## Cloudlösungen ☁ 

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


## Lebensdauer von Speichermedien ⚠️

> **Speichermedien haben unterschiedlich lange Lebensdauer**:

<div style="float:left; width:80%;">
  <img src="/images/Lebensdauer.png" alt="Lebensdauer">
</div>



<!--
style="
  float: right;
  max-width: 500px;
  background-color: #fee1ff;
  stroke: #9a047f;" -->
``` ascii
.--------------------.-------------.
| Speichermedium     | Lebensdauer |
|                    |  in Jahren  |
.--------------------.-------------. 

.--------------------+------+------.
| Externe Festplatte |   5  |  10  |
.--------------------+------+------. 
| Festplatte HDD     |   3  |   5  | 
.--------------------+------+------.
| Festplatte SSD     |   5  |  10  |
.--------------------+------+------. 
| SD-Speicherkarte   |  10  |  30  |
.--------------------+------+------.
| USB-Stick          |  10  |  30  |
.--------------------+------+------. 
| CD/DVD gebrannt    |   5  |  10  |
.--------------------+------+------. 
| CD/DVD gepresst    |  10  |  30  |
.--------------------+------+------. 
| Blu-ray            |  30  |  80  |
.--------------------+------+------. 

```

in Abhängigkeit von:

* Temperatur
* Feuchtigkeit
* Beanspruchung
* Lagerung


## 3-2-1 Regel


Mindestens 3 Kopien der Daten 📝 📝 📝

... auf mindestens 2 unterschiedlichen Speichermedien 💾 💽

... wovon mindestens 1 Kopie dezentral ist. ☁

Datenwiederherstellung zu Beginn sowie in regelmäßigen Abständen testen!

## Sensible Daten 🔒 

Besondere Aufmerksamkeit bei sensiblen Daten:

> **Schützen Sie sensible Daten!** 
>
>- Hardware (z. B. in einem abschießbaren Raum gelagert)
>- Dateiverschlüsselung
>- Passwortsicherheit
>- Mindestens zwei Personen sollten Zugang zu den Daten haben


## Backup vs. Langzeitarchivierung 📂 

| Back up                                                                          | Langzeit Speicherung            |
| -------------------------------------------------------------------------------- | ----------------------------- |
| Automatisches Backup von allen Daten   | Speicherung von ausgewählten Daten |
| All Versionen                                                                     | Nur die finale Version            |
|   zur Verhinderung von Datenverlust <br>(technisch, z.B. Defekt, oder menschlich, z.B. versehentlich gelöscht) | Integritätssicherung <br> (z. B. regelmäßige Überprüfung auf modifizierte oder beschädigte Daten, <br>Dateisystemkonsistenz)      |
|                                                                                  | Langzeitspeicherung             |
|                                                                                  | Durchsuchbar                 |



## Zusammenfassung ☝


**Risiken**

Technische Defekte, Katastrophen (Unwetter), Diebstahl, Vergesslichkeit...

**Strategien**

Speicherung auf institutionellen Servern mit automatischem regelmäßigem Backup, Sicherung wichtiger Daten in mindestens drei Kopien auf räumlich getrennten Datenträgern


# Datenspeicherung in der CAU-Cloud ☁ 

## Open-Source-Strategie

![Open-Source](/images/open-source.png)

* Digitale Souveränität

* Open Source

* Cloudlösungen (Seite 7)

* Ablösung proorietärer Software (Seite 9)

![Open-Source Säulen](/images/open-source_SH.png)

"Produkte von Microsoft versorgen nahezu vollständig die Arbeitsplatzsysteme, sind kriti
sche Komponenten im Backend und bilden zudem auf der Anwendungsebene die Basis für einige Dienste." (Seite 22)

![Kosten Microsoft Bund](/images/Kosten_Microsoft.png)



## Funktionen

## Vor- und Nachteile

* Gemeinsames Arbeiten möglich





# Daten mit anderen teilen 📚 

Per Mail

über die Cloud






📂 📁 📄 📑📒 📖 🧾 📚 

📀 💾 💿 💽 💼 💻 ☁ 🗂️🗃️ 🛍️ 🖨️ 

🎚️ 🔑 🔒 🔓 🗝️ 🔏 

⏱️ ⏳️ 

🎯 ⛑️ 🆚 ☠ ♲♻ ☝ ☚ ☛ 

🎬🍿 

✔️ ✖️ 

✒️ ✏️ ✍️ 

 💬

 🚨 🔎 🦖 🦉 🤝 💡 🌐 🏁 🍪 ❓️❗️


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












## Landesdatenstrategie

![Landesdatenstrategie]()

https://transparenz.schleswig-holstein.de/dataset/cb95db6d-126c-4201-82dd-758ff897558d/resource/7f86ebbc-0a3e-4bd0-a9f3-fc56f62de99b/download/20240119_landesdatenstrategie_sh.pdf








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

{{1}}
********************************************************************************

Ordner und Dateien sollten systematisch benannt und geordnet sein, damit

* die Dateien jetzt und in Zukunft leicht auffindbar und zugänglich sind,
* längeres Suchen von Dateien oder das Vergleichen verschiedener Versionen von Dateien vermieden wird,
* Änderungen nachvollziehbar sind,
* die Dateien nicht versehentlich gelöscht oder überschrieben werden,
* um die Zusammenarbeit zu verbessern und
* Automatisierungsprozesse zu ermöglichen.

********************************************************************************


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

{{1}}
********************************************************************************

Es gilt außerdem:

* Ausprobieren und anpassen
* Dokumentieren/Dokumentation bei Änderungen anpassen
* Für gemeinsam genutzte Dateien gemeinsame Regeln festlegen
* Konsequent bleiben

********************************************************************************


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

{{1}}
********************************************************************************

**Es gilt außerdem:**

* Prüfen, ob bereits etablierte Dateibenennungskonventionen existieren
* eigene Benennungsregeln in einer Dateibenennungskonvention festhalten
* Konventionen möglichst frühzeitig festlegen
* Unterschiedliche Konventionen für verschiedene Dateitypen sind erlaubt
* Dokumentieren/Dokumentation bei Änderungen anpassen

********************************************************************************


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

{{3}}
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


