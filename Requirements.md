
# **Requirements**
Dit zijn de requirements vormgegeven volgens Moscow, gesorteerd op functionele en non- functionele requirements.  
**FR** staat voor functionele requirement.  
**NF** staat voor non-functionele requirement.
___

### **Functionele requirements**

**FR-01** Als gebruiker wil ik verschillende brands op de landing page zien, zodat ik mijn brand kan kiezen.

**FR-02** Als gebruiker wil ik verschillende retailers zien die bij de brand horen die ik heb aangeklikt, zodat ik naar die retailer kan gaan.

**FR-03** Als gebruiker wil ik verschillende producten zien die bij de retailer beschikbaar zijn van de brand die eerder is gekozen, zodat ik de totale score kan zien.

**FR-04** Als gebruiker wil ik een specifiek product zien van een brand die bij de retailer beschikbaar is, zodat ik specifiekere data over de live score kan zien.

**FR-05** Als gebruiker wil ik kunnen zien of de titel, beschrijving en brand overeen komen bij de livescore.

**FR-06** Als ontwikkelaar wil ik requests maken op een retailers website waarbij er maar 1 request per seconde gemaakt wordt, zodat ik niet geblokkeerd word.

### **Non-functionele requirements**

**NF-01** Als gebruiker wil ik dat de website zo snel mogelijk laad wanneer ik deze bezoek, zodat ik gelijk kan kijken of de content aanwezig is.

**NF-02** Als ontwikkelaar wil ik dat de live score wordt bijgehouden in een database, zodat deze makkelijk opgehaald kan worden.

**NF-03** Als ontwikkelaar wil ik dat de live score elke keer bij een aanpassing van een excel bestand word gedraaid, zodat de live scores up to date blijven.

**NF-04** Als ontwikkelaar wil ik dat alle applicaties maintainable en scalable zijn zodat er in de toekomst gemakkelijk functionaliteit kan worden toegevoegd.

**NF-05** Als ontwikkelaar wil ik de state cachen zodat als de applicatie crasht hij niet opnieuw hoeft te beginnen.

### **Randvoorwaarden**

* Er word gebruik gemaakt van een web crawler en web scraper om content te controleren bij retailers.
* Er word gebruik gemaakt van AWS de applicatie(s) te draaien.
* Na elke request word er een seconden gewacht voordat er een nieuwe request word gemaakt bij een retailer website.
* Er word gebruik gemaakt van Python voor de back-end.
* Er word gebruik gemaakt van Next.js voor de front-end.
* Er word gebruik gemaakt van een PostgreSQL database.
