---
title: Amazon Fulfillment-Workflows
description: Die Erfüllung einer Bestellung aus einer Amazon-Liste folgt einer bestimmten Reihenfolge von der Bestellung bis zum Versand.
exl-id: 30dd9f97-9193-4c98-bded-e5d8d35b0d05
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 2%

---

# Amazon fulfillment Workflows

## Beispiel: vom Händler erfüllt

| Schritt | Beschreibung |
|----|----|
| 1 | **Amazon erhält einen Kaufauftrag.** Amazon weist folgenden Status zu: `Pending` bis die Kreditkarteninformationen des Kunden verifiziert sind. Bestellungen in `Pending` der Status automatisch in den Amazon Sales Kanal importiert wird, jedoch nicht auf _[!UICONTROL Orders]_Tabulator. |
| 2 | **Die Bestellung wird von Amazon überprüft.** Wenn bestätigt, ändert Amazon den Status in `Unshipped`. Mit dieser Statusänderung wird die Bestellung im Amazon Sales Kanal aktualisiert und im _[!UICONTROL Orders]_Tabulator. |
| 3 | **Die Auftragsdetails werden aktualisiert.** Amazon Sales Kanal aktualisiert die Auftragsdetails mit dem Preis, der E-Mail-Adresse und dem Kundennamen. Während dieser Aktualisierung erstellt die Amazon-Bestellung die entsprechende [!DNL Commerce] auf der Bestellverwaltungsseite bestellen. Die [!DNL Commerce] Bestellnummer wird mit den Bestellinformationen auf der _[!UICONTROL Orders]_Tabulator. |
| 4 | **Ein neues Kundenkonto wird erstellt.** Wenn in Ihren Bestelleinstellungen konfiguriert und der Kunde nicht in Ihrer [!DNL Commerce] Datenbank, ein neuer Kunde wird in Ihrer [!DNL Commerce] -Datenbank mit den entsprechenden Kundeninformationen aus der Amazon-Bestellung. Wenn Sie möchten `No Customer Creation (guest)` in Ihren Bestelleinstellungen folgt die Reihenfolge der [!DNL Commerce] Gastverarbeitung und keinen Kunden in Ihrer Datenbank erstellen. An dieser Stelle, wenn [!DNL Commerce] System ist mit einem ERP/OMS/WMS integriert, die Bestellung wird durch die Integration einer neuen Bestellung aufgegeben und erstellt in [!DNL Commerce]. |
| 5 | **Die Bestellung wird versendet.** Von [!DNL Commerce] Bestellungsseite, senden Sie die Bestellung und fügen Sie eine Nachverfolgungsnummer hinzu. Wenn alle Elemente in einem `Shipped` Status:<ul><li>Der Status der [!DNL Commerce] Änderungen bestellen an `Complete`.</li><li>Der Status des Amazon Sales Kanal-Auftrags ändert sich in `Shipped`.</li><li>Die Nachverfolgungsnummer wird mit Amazon synchronisiert, und der Status der Bestellung in Amazon ändert sich in `Shipped`.</li><li>Versandbenachrichtigungen werden über Amazon an den Kunden gesendet, nicht von [!DNL Commerce] (nach Amazon-Politik). |

## Beispiel: erfüllt von Amazon (FBA)

| Schritt | Beschreibung |
|---|---|
| 1 | **Amazon erhält eine Amazon-erfüllte Bestellung.** |
| 2 | **Die Bestellung wird importiert.** Die Bestellung wird erst dann in den Amazon-Kanal importiert, wenn der Auftrag der `Shipped` Status von Amazon. Da Amazon den Bestand für dieses Produkt besitzt, verhindert es Eingriffe in Ihr Lager-/Lagerbestandsmanagement. |
| 3 | **Die Auftragsdetails werden aktualisiert.** Wenn in Ihrem [Auftragseinstellungen](./order-settings.md), erstellt die Amazon-Bestellung die entsprechende [!DNL Commerce] Auftrag erstellen und als Auftrag mit dem Status `Complete`. |
