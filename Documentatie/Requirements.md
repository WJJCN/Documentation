
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

**FR-05** Als gebruiker wil ik kunnen zien of de gegeven data overeenkomt met de retailer website doormiddel van een livescore, zodat ik een duidelijk overzicht heb.

### **Non-functionele requirements**

**NF-01** Als gebruiker wil ik dat de website zo snel mogelijk laad wanneer ik deze bezoek, zodat ik gelijk kan kijken of de content aanwezig is.

**NF-02** Als ontwikkelaar wil ik dat de live score wordt bijgehouden in een database, zodat deze makkelijk opgehaald kan worden.

**NF-03** Als ontwikkelaar wil ik dat de live score elke week geupdate word door opnieuw alle huidige data te scrapen, zodat de score up to date blijft.

**NF-04** Als ontwikkelaar wil ik dat alle applicaties maintainable en scalable zijn, zodat er in de toekomst gemakkelijk functionaliteit kan worden toegevoegd.

**NF-05** Als ontwikkelaar wil ik de state cachen, zodat als de applicatie crasht het niet opnieuw hoeft te beginnen.

**NF-06** Als ontwikkelaar wil ik na elke request dat er een seconden gewacht word, voordat er een nieuwe request word gemaakt bij een retailer website, zodat het ip niet geblokkeerd word.

### **Randvoorwaarden**

* Er word gebruik gemaakt van een web crawler en web scraper om content te controleren bij retailers.
* Er word gebruik gemaakt van Lambda functies binnen AWS voor de API.
* Er word gebruik gemaakt van localhost tijdens development.
* Er word gebruik gemaakt van Python voor de back-end.
* Er word gebruik gemaakt van Next.js voor de front-end.
* Er word gebruik gemaakt van een PostgreSQL database.
