# Enterprise Application Integration - Week 1
De simulator en het inforbord verbinden
## Opdracht 1 - Oefening met JMS
1. ActiveMQ Service geinstalleerd
2. Methodes geimplementeerd in de code
3. Mule Flow gerealizeerd

![Mule Flow](https://i.imgur.com/QDAt0wB.png)

## Opdracht 2 - Queue patterns
Schema:
![Schema](https://i.imgur.com/gMo2EBx.png)
Patterns:
- DatabaseLogger: publish-subscribe
- InforbordSysteem: publish-subscribe
- Python_TimeServer: point-to-point
- Simulator: voor nu allen nog publish-subscribe, met tijdtools ook point-to-point
- Tijdtools: point-to-point

Extra patterns:
- Message Translator: In de mule flow wordt er een XML bericht getransformeerd naar een JSON bericht

## Opdracht 3 - Queue patterns
- Point-to-point: Grote data streams voor video, gaming of on-demand televisie.
- Publish-Subscribe: Evenement gedreven technologieen waar meerdere services bij moeten kunnen. Zoals bijvoorbeeld robotica, ROS.

## Opdracht 4 - Queues en loadbalancing
Met message queues kan je beschikbaarheid maximalizeren omdat tijdens een storing bij de service downstream de message queue gewoon door kan gaan met taken opvangen. Deze oplossing werkt niet als je directe symmetrische communicatie vereist, er kan alleen assymetrisch een antwoordt worden ontvangen van de service. 