# Onderzoek
In dit bestand komt alle onderzoek te staan die wij voor dit project hebben uitgevoerd.

## Table of Contents
1. [Data van websites afhalen](#data-van-websites-afhalen)
  1.1 [Scraper taal](#scraper-taal)
  1.2 [Opties](#opties)
  1.3 [Gekozen optie](#gekozen-optie)

## Data van websites afhalen
Wij moeten voor WoC een oplossing vinden om data te kunnen controleren bij retailers. Hiervoor hebben wij onderzoek gedaan om de beste methode hiervoor te gebruiken en we hebben gekeken naar de taal die wij gaan gebruiken.

### Scraper taal

Er zijn veel mogelijkheden voor het selecteren van een taal bij het maken van een scraper. Daarom is het belangrijk om eerst een goede programmeertaal te kiezen. Volgens de eisen en wensen van WoC moet de manier waarop het programma geschreven wordt onderhoudbaar en scalable zijn. Hierdoor wordt de scope van de programmeertaal al snel verkleind naar JavaScript of Python.

Python is momenteel de meest gekozen taal voor het maken van een web scraper. Dit omdat hier veel libraries voor zijn die regelmatig worden geüpdatet, die het maken van een scraper veel meer vereenvoudigen.

De opvolgers voor Python zijn Node.js of Ruby, deze twee talen worden een stuk minder gebruikt bij het maken van web scrapers. Node.js is veel gebruikt bij het maken van eenvoudige web scrapers, dit is niet helemaal bruikbaar voor onze toepassing. Ruby is ook een stukje trager dan de andere twee, daarbij komt ook nog eens kijken dat er weinig (duidelijke) libraries zijn.

### Opties
Voor het kunnen controleren van data heb je de volgende mogelijkheden:
- Web scraping en web crawling.
- Externe applicaties die tools beschikbaar hebben.
- Web scraping services, aangeboden door bedrijven.

### Gekozen optie
De oplossing die wij gekozen hebben is om web scraping en web crawling samen te gaan gebruiken. Hiemee kunnen wij pagina's zoeken en daar de content vanaf halen. Wij willen daarvoor frameworks gaan gebruiken in de taal python.

Naast het scrapen en web crawling willen wij een mappenstructuur opzetten aan de hand van retailers met daarin de bijbehorende excel bestanden. Wij willen dan met onze applicatie requests asynchronous en misschien zelf over meerdere threads gaan runnen die voor elk excel bestand van een retailer naast elkaar gaan zoeken en controleren. 

Om IP blokkering te voorkomen gaan we dan zorgen dat of na elke request een pauze van een halve of hele seconden genomen word of een proxy server gaan gebruiken die het IP na zoveel requests veranderd.
