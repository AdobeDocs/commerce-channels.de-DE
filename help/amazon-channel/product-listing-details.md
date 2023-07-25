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

Die _[!UICONTROL Product Listing Details]_-Seite enthält zusätzliche Informationen zu Ihren aktiven Produktlisten, einschließlich des Protokolls zu Listing-Aktivitäten, das die Änderungen an einer einzelnen SKU bzw. einem einzelnen Produkt anzeigt. Diese Informationen helfen Ihnen dabei, die Wettbewerbsmetriken Ihrer Produkte und der einzelnen SKU/Produktänderungen zu verstehen. Weitere Informationen auf dieser Seite sind:

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

Zeigt alle aktuellen Aktivitäten für die Amazon-Auflistung an. Zu den angezeigten Informationen gehören:

- Amazon Seller SKU: Gibt die für die Auflistung definierte Bestandseinheit (Stock Keeping Unit, SKU) an.
- ASIN: Identifiziert die 10-stellige Amazon-Produktkennung.
- Auflistungsaktion: Gibt den Aktionstyp an, der für die Auflistung aufgetreten ist.
- Kommentare: Enthält zusätzliche Details zum Typ der aufgetretenen Auflistungsaktion.
- Ausgeführt bei: Gibt das Datum und die Uhrzeit der Aktion an.

![Produktlistendetails - Protokoll zu Listening-Aktivitäten](assets/amazon-listing-activity-log.png){width="600" zoomable="yes"}
__

## Buy Box-Mitbewerber-Preise {#buy-box-competitor-pricing}

Auf dieser Registerkarte werden Informationen zum Amazon-Händler angezeigt, der die [[!DNL Buy Box]](./buy-box-competitor-pricing.md) Position für die Auflistung. Anhand dieser Informationen können Sie die Preispositionierung Ihrer Wettbewerber in Amazon nachvollziehen. Zu den angezeigten Informationen gehören:

- ASIN: Die 10-stellige Amazon-Produktkennung.
- Ist Verkäufer: Identifiziert, ob Sie die [!DNL Buy Box] Verkäufer. Optionen Ja/Nein.
- Bedingung: Gibt die für die Auflistung definierte Bedingung an.
- Listenpreis: Gibt den Preis an, zu dem die Auflistung veröffentlicht wurde.
- Versandpreis: Identifiziert den der Auflistung hinzugefügten Versandpreis.
- Anlandepreis: Identifiziert den Börsennotierungspreis zuzüglich des Versandpreises für die Auflistung.
- Zuletzt aktualisiert: Identifiziert das Datum und die Uhrzeit, zu der die Preisinformationen von Amazon aktualisiert wurden.

![Details zur Produktliste: Buy Box-Mitbewerber-Preise](assets/amazon-listing-details-buy-box-2.png){width="600" zoomable="yes"}

## Niedrigste Preise für Wettbewerber {#lowest-competitor-pricing}

Auf dieser Registerkarte werden Informationen zu Amazon-Konkurrenten für dieselbe Auflistung angezeigt. Diese Informationen können zum Verständnis der Preispositionierung und [niedrigste Preise für Wettbewerber](./lowest-competitor-pricing.md). Zu den angezeigten Informationen gehören:

- ASIN: Die 10-stellige Amazon-Produktkennung.
- Bedingung: Gibt die für die Auflistung definierte Bedingung an.
- Fulfillment-Kanal: Identifiziert die für die Erfüllung verantwortliche Partei. Optionen: Händler/Amazon.
- Listenpreis: Gibt den Preis an, zu dem die Auflistung veröffentlicht wurde.
- Versandpreis: Identifiziert den der Auflistung hinzugefügten Versandpreis.
- Anlandepreis: Identifiziert den Börsennotierungspreis zuzüglich des Versandpreises für die Auflistung.
- Feedback-Bewertung: Identifiziert die Amazon-Feedback-Bewertung für den niedrigsten Preis.
- Feedback-Anzahl: Identifiziert die Amazon-Feedback-Anzahl für den niedrigsten Preis-Händler.
- Zuletzt aktualisiert: Identifiziert das Datum und die Uhrzeit, zu der die Preisinformationen von Amazon aktualisiert wurden.

![Details zur Produktliste - niedrigste Preise für Wettbewerber](assets/amazon-listing-details-lowest-comp.png){width="600" zoomable="yes"}
