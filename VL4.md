---
title: "Vorlesung 4"
---

### Vorlesung 4: Agile Workflows und Tools
-------------


**Inhalt:** Was bedeutet Continuous Integration, Continuous Delivery und Continuous Deployment und wie unterscheiden Sie sich? Was sind Build-Server und wof�r werden Sie ben�tigt?

----------

**Continuous Integration:** 
ist eine Praxis in der Softwareentwicklung. Dabei werden isolierte �nderungen sofort gepr�ft und zur Gesamtcodebasis einer Software hinzugef�gt.

> **Um dies zu erreichen, umfasst Continuous Integration folgendes:**

> - Entwickler f�hren mindestens einmal am Tag einen Check-In ihres Codes durch
> - Der Code wird bei jedem Check-In gebaut
> - Code wird bei jedem Check-In automatisch mit Unit-Tests getestet
> - Jeder hat Zugriff auf den Build und die Testreports
> - Der Build ist schnell, sodass Entwickler schnell Feedback bekommen
> - Tests werden in einer herunterskalierten Version der Produktionsumgebung ausgef�hrt

Wird kontinuierliche Integration richtig angewandt, bietet der Ansatz verschiedene **Vorteile**, wie z.B. st�ndige Feedbacks zum Status der Software. Zudem k�nnen M�ngel bereits in einem fr�hen Entwicklungsstadium erkannt werden, sodass zuk�nftige Softwarefehler kleiner sowie weniger komplex ausfallen und sich somit einfacher beseitigen lassen. 

**Ziel** der kontinuierlichen Integration ist es, ein unmittelbares Feedback bieten zu k�nnen, so dass ein versehentlich integrierter Fehler so schnell wie m�glich identifiziert und korrigiert wird. 

Wenn diese Bedingungen umgesetzt werden, ist man auf einem �reifen� CI-Level und bereit f�r den n�chsten Schritt: **Continuous Delivery**.

Bildliche Veranschaulichung des Continuous Integration:
<img src="./images/continuous integration.png" id="img_reg_web" width="340">

----------

**Continuous Delivery:** 
bezeichnet in der Softwareentwicklung eine Sammlung von Techniken, Prozessen und Werkzeugen, welche kurze Entwicklungszyklen mit h�ufigen Softwareupdates bis hin zum produktiven System erm�glicht. Dies wird erm�glicht durch eine weitgehend automatisierte �Deployment pipeline� bzw. �Delivery pipeline� mit automatisierten Build-Prozessen, Auslieferungen, Installationen, Tests (Continous Integration) und Deployments. 

Die **Vorteile** dieses Vorgehens sind zum einen geringere Kosten wegen h�herer Automatisierung und h�here Zuverl�ssigkeit durch mehr automatisierte Tests sowie schnelleres Entdecken von Fehlern.

**Ziel:** Mit jeder erfolgreich durchlaufenden Umgebung w�chst die Wahrscheinlichkeit, dass die Software auch in der Produktiv-Umgebung lauff�hig sein wird. Ziel ist es somit, den Schritt in die Produktion soweit vorzubereiten, dass im Prinzip �per Knopfdruck� in die Produktion gegangen werden kann.

----------

Der letzte Schritt ist **Continous Deployment**. Beim Continous Delivery legt man fest, wann man in Produktion geht, beim Continous Deploment hingegen ist es keine Wahl die sich manuell steuern l�sst, sondern ein automatisierter Prozess.

Die **Vorteile** sind ein noch schnelleres Feedback, da jede �nderung direkt in Produktion geht und somit das Zeitfenster f�r eine verlorene Gelegenheit sehr klein ist. 

Continuous Integration vs. Continous Deployment:
<img src="./images/delivery vs. deployment.gif" id="img_reg_web" width="340">

----------

**Build-Server:**
stellen einen zentralen Ort dar, an dem der aktuelle Stand der Software (in Form von Testergebnissen und kompilierten Artefakten) einsehbar ist. Build-Server werden �blicherweise als Continuous Integration Server oder einfach CI-Server bezeichnet, wobei alle Prozesse innerhalb eines Build-Server vollautomatisch ablaufen und somit Fehler durch falsche, ausgelassene oder vertauschte Prozess-Schritte ausgeschlossen werden. �ber die kontinuierliche Integration hinaus k�nnen Build-Server Continuous Deployment erm�glichen und Updates f�r die Produktion bereitstellen, wenn Builds erfolgreich sind und alle Tests bestehen. 
**Beispiele** f�r einen Build-Server sind z.B. Jenkins und Travis CI.

----------

>**Quellenverzeichnis:**

> - Informationen zu Continuous Integration [hier][1]
> - Informationen zu Continuous Delivery [hier][2]
> - Informationen zu Continous Deployment [hier][3]
> - Unterschiede dieser Workflows [hier][4]
> - Informationen zu Build-Server [hier][5]


  [1]: http://www.searchenterprisesoftware.de/definition/Kontinuierliche-Integration-Continuous-Integration
  [2]: http://www.torsten-horn.de/techdocs/ContinuousDelivery.html
  [3]: https://de.wikipedia.org/wiki/Continuous_Delivery
  [4]: https://www.scrum.de/unterschiede-zwischen-continuous-integration-continuous-delivery-und-continuous-deployment/
  [5]: http://deviq.com/build-server/
