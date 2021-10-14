# NodeRed-eFriends-Heating
Heizung Kontrolle mit eFriends SmartMeter

<!-- GETTING STARTED -->
## Übersicht

[![Product Name Screen Shot][product-screenshot]]

Der NodeRed Flow liest alle 10 Sek. das eFriends Meter aus und wenn der Einspeisewert über 100W liegt, dann wird die Stromsteckdose eingeschalten.
Als Stromsteckdose wurde die HS100 von TpLink verwendet. Zusätzlich wird auch der aktuelle Wert an den Schalter übermittelt.

HS100 gibt es inzwischen fast nicht mehr der Nachfolger ist [KP105](https://www.amazon.de/TP-Link-Kasa-KP105-funktionieren-erforderlich/dp/B08339SP84/tag=wurmcoat-21)<br>
HS110 hab ich für die Messung verwendet hier gibt es inzwischen [KP115](https://www.amazon.de/TP-Link-KP115-Energieverbrauchskontrolle-funktioniert-Sprachsteuerung/dp/B08X18FXWS/?tag=wurmcoat-21)

## Einrichtung

Für die Einrichtung müssen 2 Werte eingstellt werden - die URL zum eFriends Meter mit IP Adresse und die IP Adresse der Steckdose.

Die IP Adresse des eFriends Meter am besten am Router rausfinden und fix einstellen.
Folgende Mac Adressen werden verwendet:
B8:27:EB:xx:xx:xx
DC:A6:32:xx:xx:xx
E4:5F:01:xx:xx:xx

Sonst geht es auch über den Browser
Zur URL kommt ihr in ein paar einfachen Schritten:
1. Browser Chrome/Firefox öffnen
2. app.efriends.at aufrufen
3. F12 drücken um in die Entwicklerkonsole zu gelange
4. In der Entwicklerkonsole den Tab "Network" bzw. "Netzwerkanalyse" öffnen
5. Hier nochmal F5 drücken
6. Suche nach AppConfig (Filter links oben)
7. auf der rechten Seite unter Preview ist die lokale IP Adresse zu finden

![image](https://user-images.githubusercontent.com/40350124/137376846-94f031d8-da44-4676-a65c-343012b56122.png)




[product-screenshot]: images/screenshot.jpg
