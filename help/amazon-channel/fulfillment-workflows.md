---
title: Amazon-Ausführungs-Workflows
description: Die Erfüllung einer Bestellung aus einer Amazon-Auflistung folgt einer bestimmten Sequenz von der Auftragseinsendung bis zum Versand.
feature: Sales Channels, Orders, Shipping/Delivery
exl-id: 30dd9f97-9193-4c98-bded-e5d8d35b0d05
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 2%

---

# Amazon-Ausführungs-Workflows

## Beispiel: vom Händler erfüllt

| Schritt | Beschreibung |
|------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1 | **Ein Kaufauftrag wird auf Amazon erteilt.** Amazon weist den Status `Pending` bis die Kreditkarteninformationen des Kunden verifiziert sind. Bestellungen in `Pending` Status automatisch in den Amazon-Verkaufskanal importieren, jedoch nicht auf der Seite _[!UICONTROL Orders]_Registerkarte. |
| 2 | **Die Bestellung wird von Amazon überprüft.** Bei der Überprüfung ändert Amazon den Status in `Unshipped`. Mit dieser Statusänderung wird die Bestellung im Amazon-Vertriebskanal aktualisiert und im _[!UICONTROL Orders]_Registerkarte. |
| 3 | **Die Bestelldetails werden aktualisiert.** Der Amazon-Vertriebskanal aktualisiert die Bestelldetails mit dem Preis, der E-Mail-Adresse des Kunden und dem Kundennamen. Während dieser Aktualisierung erstellt die Amazon-Reihenfolge die entsprechende [!DNL Commerce] auf der Bestellverwaltungsseite. Die [!DNL Commerce] Bestellnummer mit Bestellinformationen auf der _[!UICONTROL Orders]_Registerkarte. |
| 4 | **Ein neues Kundenkonto wird erstellt.** Wenn dies in Ihren Bestelleinstellungen konfiguriert ist und der Kunde nicht in Ihrer [!DNL Commerce] Datenbank, wird ein neuer Kunde in Ihrer [!DNL Commerce] Datenbank mit den entsprechenden Kundeninformationen aus der Amazon-Bestellung. Wenn Sie `No Customer Creation (guest)` in Ihren Bestelleinstellungen folgt die Reihenfolge der [!DNL Commerce] -Gastverarbeitung und kein Kunde in Ihrer Datenbank erstellen. Wenn an dieser Stelle [!DNL Commerce] -System mit einem ERP/OMS/WMS integriert ist, wird die Bestellung durch die Integration einer neuen Bestellung aufgenommen, die in platziert und erstellt wird. [!DNL Commerce]. |
| 5 | **Die Bestellung wird versandt.** Aus dem [!DNL Commerce] Bestellverarbeitungsseite senden Sie die Bestellung und fügen eine Trackingnummer hinzu. Wenn alle Elemente in einem `Shipped` status:<ul><li>Der Status der [!DNL Commerce] Auftragsänderungen in `Complete`.</li><li>Der Status der Bestellung des Amazon-Vertriebskanals ändert sich in `Shipped`.</li><li>Die Tracking-Nummer wird mit Amazon synchronisiert und der Status der Bestellung in Amazon ändert sich in `Shipped`.</li><li>Versandbenachrichtigungen werden über Amazon an den Kunden gesendet, nicht von [!DNL Commerce] (gemäß den Richtlinien von Amazon). |

## Beispiel: erfüllt von Amazon (FBA)

| Schritt | Beschreibung |
|------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1 | **Eine von Amazon erfüllte Bestellung wird auf Amazon aufgegeben.** |
| 2 | **Die Bestellung wird importiert.** Die Bestellung wird erst dann in den Amazon-Vertriebskanal importiert, wenn der Bestellung die `Shipped` -Status von Amazon. Da Amazon über das Inventar für dieses Produkt verfügt, verhindert es Eingriffe in Ihr Lager-/Lagerbestandsmanagement. |
| 3 | **Die Bestelldetails werden aktualisiert.** Wenn in der [Bestelleinstellungen](./order-settings.md), erstellt die Amazon-Reihenfolge die entsprechende [!DNL Commerce] Bestellung und als Bestellung mit dem Status `Complete`. |
