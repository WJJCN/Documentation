# Onderzoek
In dit bestand komt alle onderzoek te staan die wij voor dit project hebben uitgevoerd.

## Table of Contents
1. [Data van websites afhalen](#data-van-websites-afhalen)
1.1 [Opties](#opties)
3. [Example2](#example2)
4. [Third Example](#third-example)
5. [Fourth Example](#fourth-examplehttpwwwfourthexamplecom)

## Data van websites afhalen
Wij moeten voor WoC een oplossing vinden om data te kunnen controleren bij retailers. Hiervoor hebben wij onderzoek gedaan om de beste methode hiervoor te gebruiken en we hebben gekeken naar de taal die wij gaan gebruiken.

### Opties
Voor het kunnen controleren van data heb je de volgende mogelijkheden:
- Web scraping en web crawling.
- Externe applicaties die tools beschikbaar hebben.
- Web scraping services, aangeboden door bedrijven.

### Gekozen optie
De oplossing die wij gekozen hebben is om web scraping en web crawling samen te gaan gebruiken. Hiemee kunnen wij pagina's zoeken en daar de content vanaf halen. Wij willen daarvoor frameworks gaan gebruiken in de taal python.

Naast het scrapen en web crawling willen wij een mappenstructuur opzetten aan de hand van retailers met daarin de bijbehorende excel bestanden. Wij willen dan met onze applicatie requests asynchronous en misschien zelf over meerdere threads gaan runnen die voor elk excel bestand van een retailer naast elkaar gaan zoeken en controleren. 

Om IP blokkering te voorkomen gaan we dan zorgen dat of na elke request een pauze van een halve of hele seconden genomen word of een proxy server gaan gebruiken die het IP na zoveel requests veranderd.
