

# Analyse

## Fachliche Grundlagen

<!-- Beschreibung des vorliegenden Materials zum Problem 
Was sagt das Schrifttum aus? Wie können die Aussagen geordnet werden?
-->

<!-- Definitionen wichtigstes begriffliches Handwerkszeug definieren. Umfangreiche Definitionslisten in den Anhang übernehmen
-->

## Diskussion Aufgabenstellung

<!-- Beschreibung der Aufgabe oder des Problems und evtl. eine geschichtliche Einordnung des Themas (kann auch Teil der Einleitung sein). -->


## Technische Limitationen
<!-- Was ist bekannt, wo können wir ansetzten -->

<!-- Ergebnis und Diskussion des vorliegenden Materials
Kritische Auseinandersetzung mit dem vorliegenden Material. Gibt es Hinweise auf Widersprüche, offene Fragen oder gänzlich unbearbeitete Felder? Schlussfolgerungen daraus ziehen und das (Zwischen-)Ergebnis zusammenfassen.
-->

<!-- http://www.bb-elec.com/Learning-Center/All-White-Papers/Wireless-Cellular/Wireless-Antenna-Installation-Guide-10-Tips-for-Ma.aspx -->

<!-- http://de.wikipedia.org/wiki/Freiraumd%C3%A4mpfung -->

Das elektromagnetische Signal einer WLAN Anlage wird durch das Übertragungsmedium (Luft) gedämpft. Dies wird als Freiraumdämpfung wie folgt beschreiben wenn $f$ die Frequenz und $c$ die Lichtgeschwindigkeit ist. 

$F = (\frac{4\pi r * f }{c})^2$

Mit den eingesetzten Werten ergibt sich eine logarithmische Funktion.
<!-- Bild der Kurve-->
<!-- 
Sys.setlocales("LC_ALL", "en_US.UTF-8")
curve(20*log(x,10)+20*log(2400000000,10)-147.55, 0, 1000,  xlab='Distanz (d/m)', ylab='Freiraumdämpfung (dB)')
-->

Neben der Freiraumdämpfung, vermindern auch das Signalkabel vom Sender zur Antenne und Steckverbinder die Ausgangsleistung der Anlage. Gängige Antennenkabel weisen eine Dämpfung von 117.9dB/100m bis 16.0dB/100m auf.<!-- http://www.profi-wlan.de/info_pages.php/pages_id/13 --> Steckverbinder dämpfen zusätzlich mit 0.2dB bis 0.5dB.

Moderne Wlan-Geräte besitzen eine Empfangsempfindlichkeit von bis zu -96dBm bei 1Mbps. Bei höheren Übertragungsraten nimmt die Empfangsempfindlichkeit systembedingt ab. So sind bei 54Mbps bei guten Endgeräten -73dBm zu erwarten.

Bei einer Sendeleistung von genau 20dBm und unter Verwendung eines isotropen Kugelstrahler (einer idealen Rundstrahlentanne) können bei einer Empfangsempfindlichkeit von -73dBm maximal 443m Distanz überwunden werden. In der Praxis werden weder 20dBm Ausgangsleistung erreicht noch existieren störungsfreie Räume. 


## Rechtliche Limitationen
Die rechtliche Beschränkungen sind je nach Einsatzgebiet unterschiedlich und werden in der Schweiz vom Bundesamt für Kommunikation vorgeschrieben.

### 2.4 GHz Frequenzband
Die Leistung der gesamten Anlage ist im 2.4 GHz Band auf maximal 100mW begrenzt. [@bakomwlan]

### 5 GHz Frequenzband
Die Leistung der Anlage ist für das untere 5 GHz Frequenzband (5.15 - 5.35 GHz) ist auf maximal 100mW (200mW falls die Anlage TPC unterstützt) und für das obere 5 GHz Frequenzband (5.47 - 5.725 GHz) auf maximal 500mW (1000mW falls die Anlage TPC unterstützt) begrenzt. [@bakomwlan]