---
title: Amazon-Listendetails anzeigen
description: Um Wettbewerbsmetriken in Ihren Amazon-Listen und individuellen SKU-/Produktänderungen zu verstehen, lesen Sie die Seite Produktlistendetails .
feature: Sales Channels, Products, Merchandising
exl-id: faece1b1-b4fb-4506-bf77-576ae445ed28
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# Amazon-Listendetails anzeigen

Die _[!UICONTROL Product Listing Details]_-Seite enthält zusätzliche Informationen zu Ihren aktiven Produktlisten, einschließlich des Protokolls zu Listing-Aktivitäten, das die Änderungen an einer einzelnen SKU/einem einzelnen Produkt anzeigt. Diese Informationen helfen Ihnen dabei, die Wettbewerbsmetriken Ihrer Produkte und der einzelnen SKU/Produktänderungen zu verstehen. Weitere Informationen auf dieser Seite sind:

- **[!UICONTROL Listing Details]** - Produktdetails wie Name und Amazon Seller SKU
- **[!UICONTROL Listing Activity Log]** - Historische Aufzeichnung aller Änderungen, die für diese Auflistung vorgenommen wurden, wie Preisänderungen und Änderungen der Menge/des Bestands. Es sind keine weiteren Maßnahmen erforderlich. Dieses Protokoll wird zur Überprüfung bereitgestellt, um den Änderungsverlauf zu verstehen.
- **[!UICONTROL Buy Box Competitor Pricing]** - Daten für Amazon [[!DNL Buy Box]](./buy-box-competitor-pricing.md) Status und Preise der Wettbewerber
- **[!UICONTROL Lowest Competitor Pricing]** - Informationen über die Preise und Feedback-Informationen des niedrigsten Amazon-Konkurrenten

Die Startseiten der Amazon-Vertriebskanäle teilen sich einige gemeinsame [Arbeitsbereichssteuerelemente](./workspace-controls.md) die es Ihnen ermöglichen, die angezeigten Daten anzupassen.

## Auflistungsdetails

Die angezeigten Produktinformationen umfassen:

- _[!UICONTROL Amazon Name]_
- _[!UICONTROL Catalog (Magento) SKU]_
- _[!UICONTROL Amazon Seller SKU]_

![Auflistungsdetails](assets/amazon-product-listing-details.png){width="600" zoomable="yes"}

## Protokoll zu Listening-Aktivitäten {#listing-activity-log}

Zeigt alle zuletzt durchgeführten Aktivitäten für die Amazon-Auflistung an. Zu den angezeigten Informationen gehören:

- Amazon Seller SKU: Identifiziert die für die Auflistung definierte Bestandseinheit (Stock Keeping Unit, SKU).
- ASIN: Identifiziert die 10-stellige Amazon-Produktkennung.
- Auflistungsaktion: Identifiziert den Aktionstyp, der für die Auflistung aufgetreten ist.
- Kommentare: Bietet zusätzliche Details zum Typ der aufgetretenen Auflistungsaktion.
- Ausgeführt am: Identifiziert das Datum und die Uhrzeit der Aktion.

![Produktlistendetails - Protokoll zu Listening-Aktivitäten](assets/amazon-listing-activity-log.png){width="600" zoomable="yes"}
__

## Buy Box-Mitbewerber-Preise {#buy-box-competitor-pricing}

Auf dieser Registerkarte werden Informationen zum Amazon-Händler angezeigt, der die [[!DNL Buy Box]](./buy-box-competitor-pricing.md) Position für die Auflistung. Anhand dieser Informationen können Sie die Preispositionierung Ihrer Wettbewerber in Amazon nachvollziehen. Zu den angezeigten Informationen gehören:

- ASIN: Die 10-stellige Amazon-Produktkennung.
- Is Seller: Identifiziert, ob Sie der [!DNL Buy Box] Verkäufer. Optionen Ja/Nein.
- Bedingung: Identifiziert die für die Auflistung definierte Bedingung.
- Listingpreis: Identifiziert den Preis, zu dem die Liste veröffentlicht wurde.
- Versandpreis: Identifiziert den der Auflistung hinzugefügten Versandpreis.
- Anlandepreis: Identifiziert den Börsennotierungspreis zuzüglich des Versandpreises für die Auflistung.
- Zuletzt aktualisiert: Identifiziert Datum und Uhrzeit der Aktualisierung der Preisinformationen von Amazon.

![Details zur Produktliste: Buy Box-Mitbewerber-Preise](assets/amazon-listing-details-buy-box-2.png){width="600" zoomable="yes"}

## Niedrigste Preise für Wettbewerber {#lowest-competitor-pricing}

Auf dieser Registerkarte werden Informationen zu Amazon-Konkurrenten für dieselbe Auflistung angezeigt. Diese Informationen können zum Verständnis der Preispositionierung und [niedrigste Preise für Wettbewerber](./lowest-competitor-pricing.md). Zu den angezeigten Informationen gehören:

- ASIN: Die 10-stellige Amazon-Produktkennung.
- Bedingung: Identifiziert die für die Auflistung definierte Bedingung.
- Fulfillment-Kanal: Identifiziert den für die Erfüllung Verantwortlichen. Optionen: Händler/Amazon.
- Listingpreis: Identifiziert den Preis, zu dem die Liste veröffentlicht wurde.
- Versandpreis: Identifiziert den der Auflistung hinzugefügten Versandpreis.
- Anlandepreis: Identifiziert den Börsennotierungspreis zuzüglich des Versandpreises für die Auflistung.
- Feedback-Bewertung: Identifiziert die Feedback-Bewertung von Amazon für den niedrigsten Preis-Händler.
- Feedback-Anzahl: Identifiziert die Feedback-Anzahl von Amazon für den niedrigsten Preis-Händler.
- Zuletzt aktualisiert: Identifiziert Datum und Uhrzeit der Aktualisierung der Preisinformationen von Amazon.

![Details zur Produktliste - niedrigste Preise für Wettbewerber](assets/amazon-listing-details-lowest-comp.png){width="600" zoomable="yes"}
