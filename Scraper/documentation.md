# Documentatie linkscraper
## Beschrijving
De applicatie wordt gestart via een cmd terminal. Na het starten gaat het script checken welke retailers het scrapen hebben aan staan. Daarna gaat er een check langs of er al logs zijn aangemaakt voor die retailers. Als dat zo is krijg je een vraag via de terminal die aangeeft dat er al een keer gerund is vandaag en of dat nog een keer mag. Zoniet, dan gaat het script beginnen met crawlen in de link die in de retailer tabel staat. Vervolgens stript de crawler alle link tags (anchor tags) met de reference (href attribuut) van de pagina af. Waarna dit gedaan is wordt de link met de opgegeven start link vergeleken. Bevat de link die gevonden is hetzelfde als de start link, dan wordt de link opgeslagen in een lijstje met alle links die gevonden zijn.
Daarna gaat het script kijken of er producten vanuit de database zich bevinden in de gevonden linkjes. Ook checkt deze functie of er al een URL bij het product staat in de database, zoniet, wordt de gevonden link gebruikt en deze wordt geupdate in de database. Als er een link bij het product gevonden is worden deze meegegeven aan het 'vergelijk script'. Daarna begint het complete script opnieuw tot dat de lijst met retailers leeg is.

## Hoe werkt het
Als je een cmd terminal geopend hebt op de locatie waar het checker.py script staat, start je het programma door in de terminal te typen: 
```shell
python3 checker.py
```
Het script draait continu, deze checkt om de seconde de waarde van het scrapen in de database wordt aangepast naar 'True', als dit gebeurd dan roept het checker.py script het main.py script aan.

Als het programma helemaal is opgestart, kan er een waarschuwing komen bij welke retailer het scrapen niet enabled is. Dit kun je gewoon aangeven met y/n te typen in de terminal en vervolgens op enter te klikken.

```shell
[WARN] Retailer 'Dirk' is disabled for scraping.
[WARN] Retailer 'test' is disabled for scraping.
```

Ook kan er een vraag komen of je het script nog een keer wilt runnen als deze op de zelfde dag al gerund heeft.

```shell
[SYSTEM] The scraper as already completed once with this retailer today.
If you continue a new history entry will be created.
Do you want to continue? y/n
```

De scraper gaat vervolgens automatisch alle links ophalen en opslaan die beginnen met de link van de retailer:  
Retailer URL: https://www.ah.nl/producten

```shell
[INFO] Crawling: https://www.ah.nl/producten/frisdrank-sappen-koffie-thee/frisdrank/energy-drinks
[INFO] Crawling: https://www.ah.nl/producten/frisdrank-sappen-koffie-thee/frisdrank/energy-drinks/
[INFO] Crawling: https://www.ah.nl/producten/frisdrank-sappen-koffie-thee/frisdrank/energy-drinks/?kenmerk=nieuw/
```

Wanneer de scraper alle links heeft gevonden en ook alle links heeft bezocht, worden deze opgeslagen in een lijstje, en wordt er in de terminal weergegeven hoeveel links er gevonden zijn, en hoe lang het script er over gedaan heeft.

```shell
[INFO] Total links: 367
[INFO] Duration: 0:00:09.689614
```

Nu gaat het script uit de gevonden linkjes kijken of er ook een product in zit die zich in de database bevind. Als dat het geval is wordt er een log geprint in de terminal nadat alle matches gevonden zijn.

```shell
[INFO] Product: Red-Bull-Energy-drink-24-pack
URL: https://www.ah.nl/producten/product/wi476617/red-bull-energy-drink-24-pack/
[INFO] Product: Bullit-Energy-drink-suikervrij
URL: https://www.ah.nl/producten/product/wi229611/bullit-energy-drink-suikervrij/
```

Het complete product object vanuit de database samen met de gevonden URL wordt doorgestuurd naar het 'vergelijk script'.

Het vergelijk script haalt de gegeven URL op van het internet. De opgehaalde pagina wordt terug gegeven in HTML, dit wordt in een beautifullsoup object gezet. Beatifullsoup maakt het een stuk eenvoudiger om data van de pagina's af te halen.

Alle tekst bevattende elementen worden van de pagina af gehaald. Er wordt dan in een loopje constant over de elementen heen geloopt. Bij dit loopen wordt de gevonden tekst op van de URL vergeleken met de correcte teksten uit de database. Zijn de teksten 100% hetzelfde, dan wordt dit aangegeven als gevonden in de database. Nadat alles is vergeleken op 100% correct wordt er gekeken of er teksten zijn op de website die lijken op de correcte teksten. ALs laatste wordt dit aan de database toegevoegd en kan het in de front-end verwerkt worden.

Nadat alles is vergeleken geeft het script aan of je het nog een keer wilt laten draaien. Als je 'y' intypt, gaat het script nog een keer draaien en zal dus nieuwe logs, en history points aanmaken in de database. Als er 'n' of iets anders willekeurigs wordt ingevoerd, wordt het script beëindigd. Deze gaat dan terug naar het checker.py script, waar wordt gekeken wanneer de waarde in de database weer op 'True' wordt gezet.

```shell
[SYSTEM] Do you want to run the script again? y/n
n
[SYSTEM] Goodbye
```

## Wat moet er zijn geïnstalleerd
Om dit programma te laten werken moet Python versie 3.10 op de pc zijn geïnstalleerd, zorg ervoor dat er geen ander versies van
python zijn geïnstalleerd zijn.

### Gebruikte libraries
```python
from datetime import datetime  
from datetime import date  
from typing import re  
from bs4 import BeautifulSoup  
from urllib.parse import urlparse, urljoin 
from bson.objectid import ObjectId   
import time  
import requests  
import pymongo  
import sys  
import re  
import certifi  
```
