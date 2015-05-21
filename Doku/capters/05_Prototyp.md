

# Umsetzung

## Vorgehen und Messungen
Es wird nur eine Messung durchgeführt falls auch eine Verbindung hergestellt werden kann. Zur Messung der Signalstärke wird das Linux-Tool $wavemon$ verwendet.

Die Abbildung {@fig:androidap} zeigt einen beispielhaften Screenshot des Linux-Tools. Das UI ist unterteilt in die Sektionen Interface, Levels, Statistics, Info und Network.

![Screenshot: Wavemon Android AP](img/androidap.png) {#fig:androidap}

Die Sektion __Interface__ zeigt die verwendete Netzwerkkarte, in diesem Fall "wlan0", deren Eigenschaften (802.11bg) sowie die ESSID des verbundenen AccessPoints an.

Im Bereich __Levels__ wird die aktuelle Signalstärke in dBm angezeigt. Die Verbindungsqualität (link quality) gibt an, zu welchem Grand die maximale Bandbreite ausgenutzt werden kann.

Die Sektion __Info__ zeigt unter anderem auch, mit welcher Sendeleistung der AccessPoint sendet.

Die Bereiche __Statistics__ und __Network__ zeigen allgemeine Informationen über die Verbindung, den AccessPoint und aufgetretene Fehler während der Verbindung.

## Richtstrahlantenne
Um das WLAN-Signal zu verstärken, wird eine Yagi-Uda-Antenne mit einem Reflektor, einem Signalgeber und fünf Direktoren verwendet. (Siehe Abbildung {@fig:routeryagi}) Dabei handelt es sich um einen Eigenbau. Bauanleitungen mit detaillierten Beschreibungen und Hintergrundinformationen sind online verfügbar. [@eigenbauyagi]

![RouterYagi](img/router-yagi.jpg) {#fig:routeryagi}

Der Antennengewinn liegt bei 9.8dBi. Bei einer Entfernung von 200 Metern und einer Ausgangsleistung von 16dB, ist mit -60dBm Empfangslevel zu rechnen. 

Bei einer Distanz von 200 Metern ist ohne ein modifiziertes Gegenstück also immer noch eine sehr gute Verbindung erreichbar. Mit einem handelsüblichen Notebook sind genau -60dBm gemessen worden. (dazu Abbildung {@fig:router-yagi-reg})

<!-- additional text needed, description -->


## Richtstrahlantenne II
<!-- Setup + Messunge -->
Die nächst grössere Distanz, die überwunden werden soll, beträgt mehr als 1100 Meter. Da mit der selbst gebauten Yagi-Uda-Antenne kein Verbindungsaufbau möglich war, ist eine bessere Antenne nötig.

Mit zwei aufeinander ausgerichteten Yagi-Uda-Antennen vom Typ ABAKS YAGI-18 die mit jeweils 15 Direktoren einen Antennengewinn von 18dBi aufweisen und einer Sendeleistung von 21.1dB bzw. 22.3dB ist idealerweise mit einem Empfangslevel von -60dBm zu rechnen.

Die Sendeleistung von 21.1dB bzw. 22.3dB ergibt sich aus den 24dB maximaler Sendeleistung der WLAN-Karte abzüglich der 2.9dB bzw. 1.7dB Dämpfung für Kabel und Verbinder. 

![ABAKS YAGI-18 im Wald](img/yagi-wald.jpg) {#fig:yagi-18}

Das gemessene Empfangslevel von -80dBm (dazu Abbildung {@fig:yagi-reg}) bzw. die Differenz von 20dBm zu dem erwarteten Ergebniss von -60dBm, ist den störenden Objekten (Bäume) im Funkpfad geschuldet. 

## Parabolspiegel
<!-- Setup + Messunge -->
Die grösste mögliche Distanz mit Sichtverbindung, welche im Rahmen dieser Arbeit betrachtet wird, beträgt 8340 Meter.

![Parabolantenne ausgerichtet auf das 8340 Meter entfernte Gegenstück](img/parabol-point.jpg) {#fig:parabol-point}

Die WLAN-Parabolantenne ist eine Improvisation um die Richtwirkung der Yagi-Uda-Antenne weiter zu erhöhen. Es handelst sich dabei um einen Handelsüblichen Parabolspiegel, der auch für Satellitenfernsehen eingesetzt wird. Der Antennengewinn beträgt ca. 30dBi. (Abbildung {@fig:parabolantenne})

![Parabolantenne](img/parabol.png) {#fig:parabolantenne}

Mit der Parabolantenne mit ca 30dBi Antennengewinn, einer Sendeleistung 22.3dB und der darauf ausgerichteten Yagi-Uda-Antenne vom Typ ABAKS YAGI-18 mit einem Antennengewinn von 18dBi und einer Sendeleistung von 21.1dB ist idealerweise ein Empfangslevel von -66dBm erreichbar.

Der gemessene Signalpegel beträgt -67dBm. (dazu Abbildung {@fig:parabolantenne-reg})