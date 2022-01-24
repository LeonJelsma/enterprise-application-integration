# Nog meer verbindingen - Week 3
In deze opdracht is het de bedoeling om de logging en de synchronisatie van de tijd tussen de infoborden en de bussimulator te realiseren
## Opdracht 1
1. Tijdserver flow gemaakt
2. Tijdserver methodes aangeroepen in Inforborden en de Simulator

![Mule Flow](https://i.imgur.com/M9PnlfX.png)

## Opdracht 2
De drie bedrijven die bussen laten rijden (ARRIVA, QBUZZ en FLIXBUS) hebben alle drie een eigen methode van loggen.
1. QBUZZ web logging toegevoegd
2. Arriva java logging toegevoegd
3. FLIXBUS overgeslagen

![Mule Flow](https://i.imgur.com/eZ23Kin.png)

## Opdracht 3
Maak een schema van het uiteindelijke applicatie landschap
Schema:
![Ontwerp](https://i.imgur.com/AriAJVM.jpg)

Q: Wat voor technieken worden er gebruikt voor de verbindingen.
A: De applicaties worden verbonden via HTTP en ActiveMQ (over TCP)

Q: Zijn er eventueel alternatieve technieken die beter geschikt zijn.
A: Ja, er zou bijvoorbeeld gebruik van een andere message broker gemaakt kunnen worden zoals MQTT.

Q: Welke patterns worden er gebruikt.
A: Er wordt gebruik gemaakt van point-to-point doormiddel van queue's en publish-subscribe doormiddel van topics en een broken in de vorm van ActiveMQ.

Q: Beschrijf welke rol AnyPoint heeft in het proces (mediation of orchestration of beide).
A: Anypoint doet aan mediation omdat het data en protocollen transformeerd. Ook doet anypoint aan orchestration omdat het een compleet nieuwe HTTP listener opstart en realizeerd.