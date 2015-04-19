

# Analyse

## Fachliche Grundlagen

<!-- Beschreibung des vorliegenden Materials zum Problem 
Was sagt das Schrifttum aus? Wie können die Aussagen geordnet werden?
-->

<!-- Definitionen wichtigstes begriffliches Handwerkszeug definieren. Umfangreiche Definitionslisten in den Anhang übernehmen
-->
Mit Wireless Local Area Network, kurz WLAN, wird gemeinhin der IEEE-802.11  Standard assoziiert. Die Tabelle \ref{standards} zeigt die bisher definierten Standards (Stand 2015).

-----------------------------------------------
Standard    Frequenzband    Datenrate (max)
----------  --------------- -------------------
802.11      2.4 GHz         2 Mbit/s
802.11b     2.4 GHz         6 Mbit/s
802.11g     2.4 GHz         22 Mbit/s
802.11a     5 GHz           22 Mbit/s
802.11h     5 GHz           54 Mbit/s
802.11n     2.4 GHz         450 Mbit/s
802.11n     5 GHz           450 Mbit/s
802.11ac    5 GHz           660 Mbit/s
802.11ad    60 GHz          6,7 Gbit/s
--------------------------------------------
Table: Standards \label{standards}
<!-- Quelle? -->

### Antenne
Idealerweise ist eine Antenne ein Rundstrahler, welcher eine in alle Richtungen gleiche Sendeleistung aufweist. Üblicherweise werden aber Antennen verwendet, welche das Signal richten, also zum Beispiel in der Vertikalen weniger Leistung aufweisen aber in der Horizontalen dafür weitreichender sind. So haben handelsübliche Stabantennen von Routern etwa eine Verstärkungswirkung um den Faktor zwei in der horizontalen Ebene.

### Sendeanlage
Eine Sendeanlage umfasst die Sendeeinheit (WLAN-Karte), Antennenkabel und Antenne. Dazugehörend sind auch allfällige Steckverbinder.

## Technische Limitationen
<!-- Was ist bekannt, wo können wir ansetzten -->

<!-- Ergebnis und Diskussion des vorliegenden Materials
Kritische Auseinandersetzung mit dem vorliegenden Material. Gibt es Hinweise auf Widersprüche, offene Fragen oder gänzlich unbearbeitete Felder? Schlussfolgerungen daraus ziehen und das (Zwischen-)Ergebnis zusammenfassen.
-->

<!-- http://www.bb-elec.com/Learning-Center/All-White-Papers/Wireless-Cellular/Wireless-Antenna-Installation-Guide-10-Tips-for-Ma.aspx -->

<!-- http://de.wikipedia.org/wiki/Freiraumd%C3%A4mpfung -->

Das elektromagnetische Signal einer WLAN Anlage wird durch das Übertragungsmedium (Luft) gedämpft. Dies wird als Freiraumdämpfung wie folgt beschreiben wenn $f$ die Frequenz und $c$ die Lichtgeschwindigkeit ist. 

$F = (\frac{4\pi r * f }{c})^2$

Für die Frequenz 2.4GHz ergibt sich eine Freiraumdämpfungs-Kurve wie in Abbildung {@fig:fa} gezeigt.

![Freiraumdaempfung](img/Freiraumdaempfung.png) {#fig:fa} \

<!-- Sys.setlocales("LC_ALL", "en_US.UTF-8")
curve(20*log(x,10)+20*log(2400000000,10)-147.55, 0, 10000000,  xlab='Distanz (d/m)', ylab='Freiraumdämpfung (dB)')
-->

Neben der Freiraumdämpfung, vermindern auch das Signalkabel vom Sender zur Antenne und Steckverbinder die Ausgangsleistung der gesamten Anlage. Gängige Antennenkabel weisen eine Dämpfung von etwa 117.9dB/100m und hochwertige Kabel sogar nur eine Dämpfung von 16.0dB/100m.<!-- http://www.profi-wlan.de/info_pages.php/pages_id/13 --> Steckverbinder dämpfen zusätzlich mit 0.2dB bis 0.5dB.

Moderne Wlan-Geräte besitzen eine Empfangsempfindlichkeit von bis zu -96dBm bei 1Mbps. Bei höheren Übertragungsraten nimmt die Empfangsempfindlichkeit systembedingt ab. So sind bei 54Mbps und hochwertigen Endgeräten -73dBm zu erwarten.

Bei einer Sendeleistung von genau 20dBm (entspricht 100mW) und unter Verwendung eines isotropen Kugelstrahler (einer idealen Rundstrahlentanne) können bei einer Empfangsempfindlichkeit von -73dBm maximal 443m Distanz überwunden werden. In der Praxis werden weder 20dBm Ausgangsleistung erreicht noch existieren absolut störungsfreie Räume.


## Rechtliche Limitationen
Die rechtliche Beschränkungen sind je nach Einsatzgebiet unterschiedlich und werden in der Schweiz vom Bundesamt für Kommunikation vorgegeben.

### 2.4 GHz Frequenzband
Die Leistung der gesamten Anlage ist im 2.4 GHz Band auf maximal 100mW begrenzt. [@bakomwlan]

### 5 GHz Frequenzband
Die Leistung der Anlage ist für das untere 5 GHz Frequenzband (5.15 - 5.35 GHz) ist auf maximal 100mW (200mW falls die Anlage TPC unterstützt) und für das obere 5 GHz Frequenzband (5.47 - 5.725 GHz) auf maximal 500mW (1000mW falls die Anlage TPC unterstützt) begrenzt. [@bakomwlan]