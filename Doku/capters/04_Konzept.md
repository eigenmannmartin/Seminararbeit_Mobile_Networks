

# Konzept

<!-- Konzept ist ein Modell, Hypothese die aufgestellt wird-->
<!-- Hypothese Erreichung von > 8KM Distanz-->


<!-- 2,4GHz besser geeignet, da bessere Ausbreitung -->

## Verminderung der Dämpfung
<!-- Bessere Antenne/Stecker  + Erklärung der Verbesserung, Verbesserung Empfang und Sende-Leistung-->
Um die Ausgangsleistung zu maximieren, muss die Dämpfung zwischen Sender und Antenne minimiert werden. Dies wird duch Qualitativ hochwertige Steckverbinder und kurze Signalkabel sichergestellt.

Auf der Basistation sind von der Antenne bis zum Sender nur 2 Meter Kabel verbaut. Das Gegenstück der Basistation kommt hingegen mit nur 1 Meter Antennenkabel aus. Verwendet wird ein Kabel mit einer Dämpfung von maximal 1.2dB/m.

## Erhöhung der Sendeleistung
<!-- Rechtliche Grenzen +  Erklärung der Verbesserung-->
Die maximal zulässige Sendeleistung vom 20dBm wird nicht von allen WLan-Karten untersützt. Der Ubiquiti SuperRange Cardbus kann bei einer Übertragungsrate von 54Mbps, immer noch mit einer Sendeleistung von 20dBm operieren. Unterhalb Übertragungsraten von 24Mbps sind sogar 24dBm möglich.
<!-- http://dl.ubnt.com/src_datasheet.pdf -->

## Richtstrahlantenne
<!-- Verbesserung Empfang und Sende-Leistung -->
Statt einen Rundstrahler zu verwenden, kann auch eine gerichtete Verstärkung des Signals vorgenommen werden. Dazu werden typischerweise Richstrahlantennen eingesetzt.
Neben der Yagi-Uda-Antenne, Wendelantenne und der Quadantenne gibt es auch Parabolantennen.
Yagi-Uda-Antennen erreichen eine Richtverstärkung von 3dBi bis 18dBi. Ähnlich stark sind auch Quadantennen sowie Wendelantennen. Parabolantennen erreichen hingegen Antennengewinne von 20dBi bis weit über 50dBi hinaus. Die Signalausbreitung der verschiedenen Antennen unterscheiden sich sehr im Öffnungswinkel (Strahlbreite) der Hauptkeule, sowie der Aubildung von Neben- und Rückkeulen.

Yagi-Uda-Antennen erreichen eine Richtverstärkung von 3dBi bis 18dBi. Ähnlich stark sind auch Quadantennen und Wendelantennen. Parabolantennen erreichen hingegen Antennengewinne von 20dBi bis weit über 50dBi hinaus.

Die Signalausbreitung der verschiedenen Antennen unterscheiden sich sehr im Öffnungswinkel (Strahlbreite) der Hauptkeule, sowie der Aubildung von Neben- und Rückkeulen.

Die verwendete Richstrahlantenne ist eine Yagi-Uda-Antenne mit einem Antennengewinn von 18dBi.
<!-- Bild Ausbreitungsgraph -->

Die verwendete Parabolantenne hat einen Antennengewinn von ~30dBi.
<!-- Bild Ausbreitungsgraph -->

Da die Funkverbindung über eine Distanz von 8.5 Km mit der Yagi-Uda-Antenne sehr instabil und langsam war, wurde eine Yagi-Uda-Antenne auf einem Parabol-Spiegel fixiert, um so eine improvisierte Parabolantenne zu erhalten.


## Abschluss

<!-- Zusannemfassung -->


<!-- Eigener Beitrag zur Lösung des Problems
Hier steht der eigene Beitrag zur Lösung der Aufgaben und Probleme im Vordergrund,
d.h.
- Beschreibung des verwendeten oder zur Verfügung gestandenen Materials [check]
- Begründung, warum dieses Material herangezogen wurde, zum Beispiel auf Grund von Standardliteratur, Fachartikeln oder eigener Berufserfahrung [check]
- Aufzeigen von Ungenauigkeiten, Rahmenbedingungen und Schwierigkeiten bei der Problemlösung [Messresultate abhängig vom Wetter]
- Beschreibung des methodischen Vorgehens, des Experiments usw. [Prototyp]
- Zusammenfassung der Ergebnisse aus dem eigenen Beitrag
-->