---
title: "[!DNL (B2B) Business Price] für Amazon-Listen"
description: Sie können [!DNL Commerce] Store-Produkte auf der Amazon Business-Site (B2B), indem Sie Unternehmen in Ihrer Amazon aktivieren [!DNL Seller Central] -Konto.
role: Admin
level: Intermediate
feature: Sales Channels, Configuration, B2B, Tools and External Services, Merchandising, Integration
exl-id: 12a6cb2d-7a22-4b6d-9e94-ce91d564f42f
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# [!DNL (B2B) Business Price] für Amazon-Listen

(B2B) Die Business Price-Einstellungen sind Teil Ihrer Store-Listeneinstellungen. Auf die Listening-Einstellungen kann über die [Amazon Store-Dashboard](./amazon-store-dashboard.md).

[!DNL Amazon Business] ist ein Marktplatz, der ausschließlich für in Amazon registrierte Geschäftskonten gilt und nur in den USA, Frankreich, Deutschland und Großbritannien verfügbar ist. Wenn der Marketplace B2B-Geschäftspreise zulässt, kann er in Ihren Listeneinstellungen bearbeitet werden.

[!DNL B2B Business Pricing] Ermöglicht Händlern mit Geschäftskonten, untereinander mit der erwarteten Leistung des Amazon-Einkaufserlebnisses zu kaufen. Mit B2B-Geschäftspreisen können Unternehmen gestaffelte Preise anbieten, die auf der gekauften Menge basieren.

Damit Ihre Produkte im [!DNL Amazon Business (B2B)] Site müssen Sie zunächst in Ihrer [!DNL Amazon Seller Central] -Konto. Weitere Informationen zur B2B-Funktion finden Sie unter [Amazon: B2B Central](https://sellercentral.amazon.com/gp/help/G202161480/){target="_blank"} (erfordert die Anmeldung von Seller Central).

## Konfigurieren [!DNL (B2B) Business Price] settings

1. Klicken **[!UICONTROL Listing Settings]** im Dashboard speichern.

1. Erweitern Sie die _[!UICONTROL (B2B) Business Price]_Abschnitt.

1. Für **[!UICONTROL Enable Business Pricing]**, wählen Sie eine Option aus.

   - `Disabled` - (Standard) Wählen Sie aus, wann Sie den Business-to-Business-Vertrieb nicht aktivieren möchten. Alle anderen Felder in diesem Abschnitt sind bei Auswahl deaktiviert.

   - `Enabled` - Entscheiden Sie, wann Sie Ihren Business-to-Business-Vertrieb aktivieren möchten. Wenn diese Option aktiviert ist, wird der Geschäftspreis auf den Listenpreis gesetzt, nachdem alle Preisregeln angewendet wurden. Der Geschäftspreis entspricht, sofern aktiviert, dem Umfang der Website-Preise. Ein Geschäftspreis darf nicht weniger als 1 Dollar betragen.

1. Für **[!UICONTROL Enable Tiered Pricing]**, wählen Sie eine Option aus.

   - `Disabled` - (Standard) Wählen Sie aus, wann Sie denselben Listenpreis für alle Bestellmengen wünschen. Wenn ausgewählt, werden alle _[!UICONTROL Pricing Level]_-Felder in diesem Abschnitt sind deaktiviert.

   - `Enabled` - Wählen Sie aus, wann Sie Preisanpassungen basierend auf der Bestellmenge aktivieren möchten. Wenn ausgewählt, wird die _[!UICONTROL Pricing Level]_-Felder aktiviert sind.

1. Führen Sie die **[!UICONTROL Pricing Level]** -Einstellungen.

   Sie können bis zu fünf Quantitäts-/Rabatteinstellungen definieren, mit denen die Stufenpreise für Ihre Geschäftslisten festgelegt werden. Geben Sie in jeder Zeile den Schwellenwert für die Menge und den anzuwendenden Prozentsatz für den Rabatt an. Wenn Sie beispielsweise `5` im ersten Feld der ersten Zeile und `5` im zweiten Feld wird der Preis um 5 % ermäßigt, wenn ein anderes Unternehmen eine Menge von 5 oder mehr kauft.

1. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Save listing settings]**.

![Amazon Business Pricing (B2B)](assets/amazon-business-pricing.png){width="500" zoomable="yes"}

| Feld | Beschreibung |
|----------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Enable Business Pricing] | Optionen: <ul><li>**[!UICONTROL Disabled]** - (Standard) Wählen Sie aus, wann Sie den Business-to-Business-Vertrieb nicht aktivieren möchten. Wenn diese Option aktiviert ist, sind alle anderen Felder in diesem Abschnitt deaktiviert.</li><li>**[!UICONTROL Enabled]** - Entscheiden Sie, wann Sie Ihr Unternehmen für den Geschäftsverkauf aktivieren möchten. Wenn diese Option ausgewählt ist, wird der Geschäftspreis gleich dem Listenpreis festgelegt, nachdem alle Preisregeln angewendet wurden. Der Geschäftspreis entspricht, sofern aktiviert, dem Umfang der Website-Preise. Ein Geschäftspreis darf nicht weniger als 1 Dollar betragen.</li></ul> |
| [!UICONTROL Enable Tiered Pricing] | (Erforderlich) Optionen: <ul><li>**[!UICONTROL Disabled]** - (Standard) Wählen Sie aus, wann Sie denselben Listenpreis für alle Bestellmengen wünschen. Wenn ausgewählt, werden alle _[!UICONTROL Pricing Level]_-Felder in diesem Abschnitt sind deaktiviert.</li><li>**[!UICONTROL Enabled]** - Wählen Sie aus, wann Sie eine Preisanpassung basierend auf der Bestellmenge vornehmen möchten. Wenn ausgewählt, wird die _[!UICONTROL Pricing Level]_-Felder aktiviert sind.</li></ul> |
| [!UICONTROL Pricing Level One-Five (qty/discount)] | Wenn die Option &quot;Tiered Pricing&quot;aktiviert ist, können Sie bis zu fünf Quantitäts-/Rabatteinstellungen definieren, die die Stufenpreise für Ihre Geschäftslisten festlegen. Geben Sie in jeder Zeile den Schwellenwert für die Menge und den anzuwendenden Prozentsatz für den Rabatt an. Wenn Sie beispielsweise `5` im ersten Feld der ersten Zeile und `5` im zweiten Feld wird ein Rabatt von 5 % gewährt, wenn ein anderes Unternehmen eine Menge von fünf oder mehr kauft. |

**Schnellzugriff** - [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
