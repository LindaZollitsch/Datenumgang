<!--

author:   Linda Zollitsch
email:    zollitsch@ub.uni-kiel.de
version:  0.1.0
language: de
narrator: UK English Female

icon:     images/Logo_cau-norm-de-lilagrey-rgb-0720_2022.png

link: LindaZollitsch/Datenumgang/style_css.css
  


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

* Datenspeicherung und Backup: Einführung

* Datenspeicherung in der CAU-Cloud

* Daten mit anderen teilen (während der Arbeit daran)



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
  background-color: #fee1ff;
  stroke: #9a047f;" -->
``` ascii
+-----------------+
| Eigener PC      |            +-----------------+
+-----------------+            | Mobile          |
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

{{1-2}}
****************

<section class="flex-container">

<!-- class="flex-child-1" style="background: lightgray; min-width: 100px; max-height:300px" -->
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

<!-- class="flex-child-2" style="background: lightgray; min-width: 100px; max-height:300px" -->
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

</section>

****************

{{2}}
****************
![img](/images/Lebensdauer-komplett.png)


in Abhängigkeit von:

* Temperatur
* Feuchtigkeit
* Beanspruchung
* Lagerung
****************

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



## Zusammenfassung 🦉


**Risiken**❗️

Technische Defekte, Katastrophen (Unwetter), Diebstahl, Vergesslichkeit...

-----

**Strategien** 💡

Speicherung auf institutionellen Servern mit automatischem regelmäßigem Backup, Sicherung wichtiger Daten in mindestens drei Kopien auf räumlich getrennten Datenträgern


# Datenspeicherung in der CAU-Cloud ☁ 

{{1-2}}
****************
![landing page](/images/CAU-cloud0.png)

****************

{{2-3}}
****************
![overview](/images/CAU-cloud1.png)

****************

{{3}}
****************
![left](/images/CAU-cloud3.png)

****************
{{4}}
****************
![top](/images/CAU-cloud2.png)

****************



## Funktionen

>* Gemeinsames Arbeiten online möglich
>
>* Zugang auch für CAU-externe möglich
>
>* Backup durch CAU
>
>* Datenschutz-konform



☛ **ABER** ☚


* Begrenzte Speichervolumen

* an eine Person an der CAU gebunden

* Speicherzeit an die Anstellung der Person an der CAU gebunden




## Open-Source-Strategie

{{1-2}}
****************
![Open-Source](/images/open-source.png)

* Digitale Souveränität

* Open Source

* Cloudlösungen (Seite 7)

* Ablösung proorietärer Software (Seite 9)
****************

{{2-3}}
****************
![Open-Source Säulen](/images/open-source_SH.png)

"Produkte von Microsoft versorgen nahezu vollständig die Arbeitsplatzsysteme, sind kritische Komponenten im Backend und bilden zudem auf der Anwendungsebene die Basis für einige Dienste." (Seite 22)
****************

{{3}}
****************
![Kosten Microsoft Bund](/images/Kosten_Microsoft.png)
****************




# Daten mit anderen teilen 📚 

* Per Mail 📄

* über die Cloud ☁

* über OpenData@CAU 




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


Jaeger, Philipp, & Bode, Janice. (2021). Redet über die Daten! - Forschungsdatenmanagement und Hochschullehre in der Physik und darüber hinaus. Zenodo. https://doi.org/10.5281/zenodo.5168524

Petersen, B., Altemeier, F., Boße, S., Dalby, M., Düvel, N., Engelhardt, C., Fichtner, M., Hastik, C., Haugwitz, J.-M., Jacob, J., Koch, K., Kuntz, A., Manske, A., Mühlichen, A., Murcia Serra, J., Ortmeyer, J., Richter, M., Schranzhofer, H., Slowig, B., … Zollitsch, L. (2025). Lernzielmatrix zum Themenbereich Forschungsdatenmanagement (FDM) (Version 3). Zenodo. https://doi.org/10.5281/zenodo.15025246

https://forschungsdaten.info/

https://mantra.ed.ac.uk/

https://www.fdm.uni-hannover.de/fileadmin/fdm/Dokumente/Schulungsunterlagen/Schulungsunterlagen_FDM_VertiefungDatenorganisation_Folien.pdf

https://www.forschungsdaten-bildung.de

https://www.gida-global.org/care 

https://opendata.uni-kiel.de/content/index.xml 

https://opendata.schleswig-holstein.de/dataset 

