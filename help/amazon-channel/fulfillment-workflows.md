---
title: Amazon-Ausführungsarbeitsabläufe
description: Die Erfüllung einer Bestellung aus einer Amazon-Auflistung folgt einer bestimmten Sequenz von der Auftragseinsendung bis zum Versand.
exl-id: 30dd9f97-9193-4c98-bded-e5d8d35b0d05
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 2%

---

# Amazon-Ausführungs-Workflows

## Beispiel: vom Händler erfüllt

| Schritt | Beschreibung |
|----|----|
| 1 | **Ein Kaufauftrag wird auf Amazon erteilt.** Amazon weist den Status von zu,  `Pending` bis die Kreditkarteninformationen des Kunden verifiziert sind. Bestellungen im Status `Pending` werden automatisch in den Amazon-Verkaufskanal importiert, nicht jedoch auf der Registerkarte _[!UICONTROL Orders]_. |
| 2 | **Die Bestellung wird von Amazon überprüft.** Nach der Überprüfung ändert Amazon den Status in  `Unshipped`. Mit dieser Statusänderung wird die Bestellung im Amazon-Vertriebskanal aktualisiert und auf der Registerkarte _[!UICONTROL Orders]_angezeigt. |
| 1 | **Die Bestelldetails werden aktualisiert.** Der Amazon-Vertriebskanal aktualisiert die Bestelldetails mit dem Preis, der E-Mail-Adresse und dem Kundennamen. Bei dieser Aktualisierung erstellt die Amazon-Bestellung die entsprechende [!DNL Commerce]-Bestellung auf der Bestellverwaltungsseite. Die Bestellnummer [!DNL Commerce] wird mit den Bestellinformationen auf der Registerkarte _[!UICONTROL Orders]_angezeigt. |
| 4 | **Ein neues Kundenkonto wird erstellt.** Wenn der Kunde in Ihren Bestelleinstellungen konfiguriert wurde und nicht in Ihrer  [!DNL Commerce] Datenbank vorhanden ist, wird ein neuer Kunde mithilfe der entsprechenden Kundeninformationen aus der Amazon-Bestellung in Ihrer  [!DNL Commerce] Datenbank erstellt. Wenn Sie in Ihren Bestelleinstellungen `No Customer Creation (guest)` ausgewählt haben, folgt die Bestellung dem Gastprozess [!DNL Commerce] und erstellt keinen Kunden in Ihrer Datenbank. Wenn Ihr [!DNL Commerce]-System in ein ERP/OMS/WMS integriert ist, wird die Bestellung nach der Integration einer neuen Bestellung aufgenommen, die innerhalb von [!DNL Commerce] platziert und erstellt wird. |
| 5 | **Die Bestellung wird versandt.** Auf der  [!DNL Commerce] Bestellverarbeitungsseite versenden Sie die Bestellung und fügen eine Nachverfolgungsnummer hinzu. Wenn alle Elemente mit dem Status `Shipped` markiert sind:<ul><li>Der Status der [!DNL Commerce]-Reihenfolge ändert sich in `Complete`.</li><li>Der Status der Bestellung des Amazon-Vertriebskanals ändert sich in `Shipped`.</li><li>Die Trackingnummer wird mit Amazon synchronisiert und der Status der Bestellung in Amazon ändert sich in `Shipped`.</li><li>Versandbenachrichtigungen werden über Amazon an den Kunden gesendet, nicht von [!DNL Commerce] (gemäß den Richtlinien von Amazon). |

## Beispiel: erfüllt von Amazon (FBA)

| Schritt | Beschreibung |
|---|---|
| 1 | **Eine von Amazon erfüllte Bestellung wird auf Amazon aufgegeben.** |
| 2 | **Die Bestellung wird importiert.** Die Bestellung wird erst dann in den Amazon-Vertriebskanal importiert, wenn der Bestellung der  `Shipped` Status von Amazon zugewiesen wurde. Da Amazon über das Inventar für dieses Produkt verfügt, verhindert es Eingriffe in Ihr Lager-/Lagerbestandsmanagement. |
| 1 | **Die Bestelldetails werden aktualisiert.** Wenn diese in Ihren  [Bestelleinstellungen](./order-settings.md) konfiguriert ist, erstellt die Amazon-Bestellung die entsprechende  [!DNL Commerce] Bestellung und wird als Bestellung mit dem Status  `Complete`erstellt. |
