# **Requirements**
Dit zijn de requirements vormgegeven volgens Moscow, gesorteerd op functionele en non- functionele requirements.  
**FR** staat voor functionele requirement.  
**NF** staat voor non-functionele requirement.  
**B** staat voor beperking.  
**K** staat voor kwaliteitseis.

### **Functionele requirements**

**FR-01** Je krijgt verschillende retailers te zien op je dashboard.

	K-01: Alleen retailers die jouw brand hebben, worden laten zien.

**FR-02** Je kunt kiezen van welke retailers je de score wilt ontvangen.  
	
	K-01: Je kunt ze zelf toevoegen aan het dashboard.

**FR-03** Je kunt inloggen.

	B-01: Een account wordt aangemaakt door admins van de website.

	B-02: Geen lege velden.

	K-01: Wanneer je ingelogd bent zie je gelijk scores van de eerste paar retailers.

	K-02: Bij eerste keer inloggen moet je het wachtwoord veranderen.

**FR-04**  Je krijgt een live score te zien van correct geplaatste content per brand bij retailer.

	B-01: Live score is gehele percentages.

	B-02: Je hebt niet bij alle brands elke retailer.

	B-03: Score is niet voor iedere retailer aanwezig.

	B-04: Ophalen van scores kan wat langer duren.

	K-01: De score per retailer wordt gecategoriseerd op basis score per deel wat er gecontroleerd wordt (titel, beschrijving enzovoort).

**FR-05** Cache?

	B-01: Door de hoeveelheid scores kan niet alles gecached worden.

**FR-06** Admin kan een account aanmaken.

	B-01: Velden mogen niet leeg zijn.

	B-02: Wachtwoord moet langer zijn dan 7 letters.

**FR-07** Het bekijken van de live-score in het WoC-dashboard.

	B-01: Live score is gehele percentages.

	B-02: Systeem is gekoppeld aan het systeem van WoC.

### **Non-functionele requirements**

**NF-01** Database waar users worden opgeslagen.  

	B-01: Er kunnen niet meerdere users zijn met dezelfde gegevens (emailadres en  
gebruikersnaam).

**NF-02** Database waar de live score wordt bijgehouden.

**NF-03** Website is responsive.

**NF-04** Elke week nieuwe live-score ophalen.

**NF-05** Live-score opvragen binnen 5 seconden.

**NF-06** Alle applicaties zullen maintainable en scalable zijn.

	B-01: Doordat het maintainable moet zijn vallen er veel opties af.

	B-02: Om het scalable te maken moeten we gebruik maken van hele algemene functies.

**NF-07** Systeem koppelen met de database van WoC.

	B-01: WoC moet een API maken om deze data te integreren.

**NF-08** State cashen voor als de applicatie halverwege crashed.




|               |Functioneel		                       |Must    |Should  |Could   |Won't   |
|----------------|-----------------------------------------|--------|--------|--------|--------|
|FR-01|Je krijgt verschillende retailers te zien op je dashboard.|x|
|FR-02|Je kunt kiezen van welke retailers je de score wilt ontvangen.||x|
|FR-03|Je kunt inloggen.|x|
|FR-04|Je krijgt een live score te zien van correct geplaatste content per brand bij retailer.|x|
|FR-05|Cache?||x|
|FR-06|Admin kan een account aanmaken.||x|
|FR-07|Het bekijken van de live-score in het WoC-dashboard.||||x

|               |Non-Functioneel	                       |Must    |Should  |Could   |Won't   |
|----------------|-----------------------------------------|--------|--------|--------|--------|
|NF-01|Database waar users worden opgeslagen.|x|
|NF-02|Database waar de live score wordt bijgehouden.|x|
|NF-03|Website is responsive.|x|
|NF-04|Elke week een nieuwe live-score ophalen.|||x|
|NF-05|Live-score opvragen binnen 5 seconden.|x|
|NF-06|Alle applicaties zullen maintainable en scalable zijn.||x|
|NF-07|Systeem koppelen met de database van WoC.||||x|
|NF-08|State cachen voor als de applicatie halverwegen crasht.||x|