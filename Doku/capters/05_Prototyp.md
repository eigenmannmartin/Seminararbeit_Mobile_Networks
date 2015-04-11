

# Umsetzung

## Vorgehen und Messungen
Es wird nur eine Messung durchgeführt falls auch eine Verbindung hergestellt werden kann. Zur Messung der Signalstärke wird das Linux-Tool $wavemon$ verwendet. Zur Feststellung der Übertragungsgeschwindigkeit und Stabilität der Verbindung wird $iperf$ verwendet.
<!-- Tools zur Messung -->

## Richtstrahlantenne
<!-- Setup + Messungen -->
Um das WLAN-Signal zu verstärken, wird eine Yagi-Uda-Antenne mit einem Reflektor, einem Signalgeber und vier Direktoren verwendet.
![RouterYagi](img/router-yagi.jpg)

Der Antennengewinn liegt bei 9.8dBi. Bei einer Entfernung von 200 Metern und einer Ausgangsleistung von 16dB, ist mit -60dBm Empfangslevel zu rechnen. 

Bei einer Distanz von 200 Metern ist ohne ein modifiziertes Gegenstück immer noch eine sehr gute Verbindung erreichbar.
![RouterYagiErg](img/router-yagi-reg.jpg)

## Richtstrahlantenne II
<!-- Setup + Messunge -->
Die nächst grössere Distanz von ~1100 Metern ist keine ungestörte Sichtverbindung möglich und daher eine bessere Antenne nötig.
![Yagi](img/yagi-wald.jpg)

Mit zwei aufeinander ausgerichteten Yagi-Uda-Antennen vom Typ ABAKS YAGI-18 die jeweils einen Antennengewinn von 18dBi, einer Sendeleistung von 21.1dB $( 24dB - (2.4dB + 0.5dB) )$ bzw. 22.3dB $( 24dB - (1.2dB + 0.5dB) )$ ist idealerweise mit einem Empfangslevel von -60dBm zu rechnen.

Das gemessene Empfangslevel von -80dBm bzw. die Differenz von 20dBm zu dem erwarteten Ergebniss, ist den störenden Objekten im Funkpfad geschuldet.
![YagiReg](img/yagi-reg.jpg)

## Parabolspiegel
<!-- Setup + Messunge -->
Die grösste mögliche Distanz mit Sichtverbindung, welche im Rahmen dieser Arbeit betrachtet wird, beträgt bei 8340 Metern.
![Parabolantenne](img/parabol-point.jpg)

Die WLAN-Parabolantenne ist eine Improvisation um die Richtwirkung der Yagi-Uda-Antenne weiter zu erhöhen. Es handelst sich dabei um einen Handelsüblichen Parabolspiegel, der auch für Satellitenfernsehen eingesetzt wird. Der Antennengewinn beträgt ~30dBi.
![Parabolantenne](img/parabol.png)

Mit der Parabol-Antenne mit einer Sendeleistung 22.3dB und einer darauf ausgerichteten Yagi-Uda-Antenne mit einem Antennengewinn von 18dBi und einer Sendeleistung von 21.1dB ist idealerweise ein Empfangslevel von -66dBm erreichbar.
![YagiReg](img/parabol-reg.jpg)