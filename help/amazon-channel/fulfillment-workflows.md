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
| 1 | **Eine Bestellung, die vom Händler erfüllt wurde, wird auf Amazon aufgegeben.** Amazon weist den Status `Pending` zu, bis die Kreditkarteninformationen des Kunden verifiziert sind. Bestellungen mit dem Status &quot;`Pending`&quot; werden automatisch in den Amazon-Verkaufskanal importiert, jedoch nicht auf der Registerkarte &quot;_[!UICONTROL Orders]_&quot;. |
| 2 | **Die Bestellung wird von Amazon überprüft.** Wenn überprüft, ändert Amazon den Status in `Unshipped`. Mit dieser Statusänderung wird die Bestellung im Amazon-Vertriebskanal aktualisiert und auf der Registerkarte _[!UICONTROL Orders]_angezeigt. |
| 3 | **Die Bestelldetails werden aktualisiert.** Der Amazon-Vertriebskanal aktualisiert die Bestelldetails mit dem Preis, der E-Mail-Adresse des Kunden und dem Kundennamen. Bei dieser Aktualisierung erstellt die Amazon-Bestellung die entsprechende [!DNL Commerce]-Bestellung auf der Bestellverwaltungsseite. Die Bestellnummer [!DNL Commerce] wird mit den Bestellinformationen auf der Registerkarte _[!UICONTROL Orders]_angezeigt. |
| 4 | **Ein neues Kundenkonto wird erstellt.** Wenn dies in Ihren Bestelleinstellungen konfiguriert wurde und der Kunde nicht in Ihrer [!DNL Commerce] -Datenbank vorhanden ist, wird ein neuer Kunde in Ihrer [!DNL Commerce] -Datenbank unter Verwendung der entsprechenden Kundeninformationen aus der Amazon-Bestellung erstellt. Wenn Sie in Ihren Bestelleinstellungen `No Customer Creation (guest)` ausgewählt haben, folgt die Bestellung dem Gastprozess [!DNL Commerce] und erstellt keinen Kunden in Ihrer Datenbank. Wenn Ihr [!DNL Commerce]-System zu diesem Zeitpunkt in ein ERP/OMS/WMS integriert ist, wird die Bestellung durch die Integration einer neuen Bestellung aufgenommen, die innerhalb von [!DNL Commerce] platziert und erstellt wird. |
| 5 | **Die Bestellung wird versandt.** Auf der Seite [!DNL Commerce] zur Bestellverarbeitung versenden Sie die Bestellung und fügen eine Trackingnummer hinzu. Wenn alle Elemente mit dem Status `Shipped` markiert sind:<ul><li>Der Status der [!DNL Commerce]-Reihenfolge ändert sich in `Complete`.</li><li>Der Status der Bestellung des Amazon-Vertriebskanals ändert sich in &quot;`Shipped`&quot;.</li><li>Die Tracking-Nummer wird mit Amazon synchronisiert und der Status der Bestellung in Amazon ändert sich in `Shipped`.</li><li>Versandbenachrichtigungen werden über Amazon an den Kunden gesendet, nicht über [!DNL Commerce] (gemäß den Richtlinien von Amazon). |

## Beispiel: erfüllt von Amazon (FBA)

| Schritt | Beschreibung |
|------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1 | **Eine von Amazon erfüllte Bestellung wird auf Amazon aufgegeben.** |
| 2 | **Die Reihenfolge wird importiert.** Die Bestellung wird erst dann in den Amazon-Vertriebskanal importiert, wenn Amazon der Bestellung den Status `Shipped` zugewiesen hat. Da Amazon über das Inventar für dieses Produkt verfügt, verhindert es Eingriffe in Ihr Lager-/Lagerbestandsmanagement. |
| 3 | **Die Bestelldetails werden aktualisiert.** Wenn in Ihren [Bestelleinstellungen](./order-settings.md) konfiguriert, erstellt die Amazon-Reihenfolge die entsprechende [!DNL Commerce]-Reihenfolge und wird als Bestellung mit dem Status `Complete` erstellt. |
