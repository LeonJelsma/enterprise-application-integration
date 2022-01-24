# Services beschrijven, SOAP, RAML en andere technieken - Week 2
De simulator en het inforbord verbinden
## Opdracht 1
1. receiveBusBijHalte toegevoegd aan flow
2. receiveBusBijEindpunt toegevoegd aan flow

![Mule Flow](https://i.imgur.com/f36leCV.png)

## Opdracht 2
Dit is een goede keuze omdat de acties in het asynchroon blok niet belangrijk zijn voor de rest van de flow. En dus geoptimalizeerd kunnen worden door deze asynchroon te maken.

## Opdracht 3
a. Maak een vergelijking tussen SOAP en RAML, beschrijf hierin de overeenkomsten en verschillen met betrekking tot de architectuur, gebruikte technieken, noodzakelijke onderdelen van de implementatie, etc.
SOAP vs RAML
SOAP is platform agnostisch, RAML moet HTTP gebruiken
SOAP gebruikt XML voor alle berichten, RAML gebruikt kleinere formaten zoals JSON
SOAP heeft ingebouwde error verhandeling, RAML niet

b1. Wat betekent de term contract-first met betrekking tot webservices?
Contract first betekend dat je begint te ontwikkelen door het contract eerst te verwerkelijken

b2. Welke tool kun je gebruiken om contract-first in Java te gebruiken bij SOAP servers?
Alle XSD enabled IDEAs
