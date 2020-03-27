# YACoVV Monitoring
Bei der Beatmung kann es zu einer Vielzahl von Problemen kommen die zeitnah detektiert werden müssen.

## Überlegungen
- Das Monitoring sollte unabhängig von der Steuerung der Beatmung sein.
- Erreichen des Beatmungsdruck muss detektiert werden.
- Halten des PEEP muss überwacht werden
- Anzeige der Fehler per akustischem und optischem Signal

## Umsetzung
In einem ersten Ansatz haben wir eine kapazitative Messung von mehreren Höhen an der Wassersäule getestet.
Die Messtechnik besteht aus einem isolierten Kabel das innerhalb der Wassersäule des Manometers geführt ist, sowie weiteren isolierte Kabeln die am Manometer um die Stelle der zu detektierenden Druckwerten gewickelt sind.

Mit dieser Messtechnik lässt sich feststellen ob der Druck bei jedem Beatmungszyklus zwischen dem Beatmungsdruck und dem PEEP pendelt. Mit diesen Messungen können folgende Fehler im System detektiert werden:
- Beatmungsdruck wird nicht erreicht. Beispiele: Undichtigkeit im Schlauch zum Patienten oder auf dem Weg bis zum Auslassventil, Wassersäule für Beatmungsdruck nicht richtig eingestellt, Flüssgkeitsverlust im Druckregler
- PEEP wird unterschritten. Beispiele: Undichtigkeit im Beatmungsschlauch, Undichtigkeit zwischen Auslassventil und Wassersäule des Druckreglers, Flüssigkeitsverlust im Druckregler.
- Beatmungsfrequenz: Aus der Pendelfrequenz der Wassersäule im Manometer kann die Atemfrequenz berechnet werden. Über Min und Maxwerte im Monitoring kann ein Alarm ausgelöst werden wenn die Atemfrequenz unter oder überschritten wird.

[Video mit der Detektierung von 2 Druckwerten](https://youtu.be/_2SUDyStXJM)

Über eine kapazitative Messung wäre es auch möglich die absolute Höhe der Flüssigkeit im Manometer zu messen, das würde jedoch eine aufwendige Kalibierung des Systems erfordern. Des Weiteren lassen sich die fixen Messpunkte einfach auf dem Manometer verschieben um die Werte anzupassen. Soll beispielsweise der Beatmungsdruck bei einem Patienten erhöht werden reicht ein einfaches verschieben der Messstelle nach oben aus. 

## Anzeige der Fehler
Die Anzeige des Systemstatus kann auf mehrere Arten erfolgen.
### Farbige LEDs
- rot: Störung
- grün: Beatmung stabil
- gelb: Es gab eine Fehler in der Beatmung, dieser ist aber von selbst wieder verschwunden. Durch drücken eines Tasters kann der Fehler zurückgesetzt werden.
Die grüne und gelbe LED können auch im Takt der Beatmung blinken. Dadurch kann auch aus gröserer Entfernung die Frequenz erkannt werden.
### Display
Über ein Display kann die Atemfrequenz exakt angezeigt werden und eine genauere Beschreibung eines Fehlers. Das Display ist kein Ersatz für die LEDs sondern eine Ergänzung.
### Akustischer Alarm
Ein akustischer Alarm sollte auf jeden Fall eingebaut werden. Zusammen mit den LEDs kann ein fehlerhaftes System so auch bei einer grösseren Anzahl von Geräten die dicht nebeneinander stehen schnell und eindeutig identifiziert werden.
