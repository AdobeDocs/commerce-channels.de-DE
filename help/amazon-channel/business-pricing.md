---
title: "[!DNL (B2B) Business Price] für Amazon-Listen"
description: Sie können Ihre [!DNL Commerce] Store-Produkte auf der Amazon Business (B2B)-Site auflisten, indem Sie Ihr Amazon [!DNL Seller Central] -Konto für Unternehmen aktivieren.
role: Admin
level: Intermediate
feature: Sales Channels, Configuration, B2B, Tools and External Services, Merchandising, Integration
exl-id: 12a6cb2d-7a22-4b6d-9e94-ce91d564f42f
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# [!DNL (B2B) Business Price] für Amazon-Listen

(B2B) Die Business Price-Einstellungen sind Teil Ihrer Store-Listeneinstellungen. Auf Listening-Einstellungen kann über das [Dashboard für Amazon-Speicher](./amazon-store-dashboard.md) zugegriffen werden.

[!DNL Amazon Business] ist ein Marktplatz, der ausschließlich für in Amazon registrierte Geschäftskonten gilt und nur in den USA, Frankreich, Deutschland und Großbritannien verfügbar ist. Wenn der Marketplace B2B-Geschäftspreise zulässt, kann er in Ihren Listeneinstellungen bearbeitet werden.

Mit [!DNL B2B Business Pricing] können Händler mit Geschäftskonten untereinander Einkäufe tätigen und die erwartete Leistung des Amazon-Einkaufserlebnisses erzielen. Mit B2B-Geschäftspreisen können Unternehmen gestaffelte Preise anbieten, die auf der gekauften Menge basieren.

Damit Ihre Produkte auf der [!DNL Amazon Business (B2B)] -Site aufgeführt werden, müssen Sie zunächst Ihr Geschäft in Ihrem [!DNL Amazon Seller Central] -Konto aktivieren. Weitere Informationen zur B2B-Funktion finden Sie unter [Amazon: B2B Central](https://sellercentral.amazon.com/gp/help/G202161480/){target="_blank"} (Anmeldung von Seller Central erforderlich).

## Einstellungen für [!DNL (B2B) Business Price] konfigurieren

1. Klicken Sie im Store-Dashboard auf **[!UICONTROL Listing Settings]** .

1. Erweitern Sie den Abschnitt _[!UICONTROL (B2B) Business Price]_.

1. Wählen Sie für **[!UICONTROL Enable Business Pricing]** eine Option aus.

   - `Disabled` - (Standard) Wählen Sie aus, wann Sie den Business-to-Business-Vertrieb nicht aktivieren möchten. Alle anderen Felder in diesem Abschnitt sind bei Auswahl deaktiviert.

   - `Enabled` - Wählen Sie aus, wann Sie Ihren geschäftlichen Vertrieb aktivieren möchten. Wenn diese Option aktiviert ist, wird der Geschäftspreis auf den Listenpreis gesetzt, nachdem alle Preisregeln angewendet wurden. Der Geschäftspreis entspricht, sofern aktiviert, dem Umfang der Website-Preise. Ein Geschäftspreis darf nicht weniger als 1 Dollar betragen.

1. Wählen Sie für **[!UICONTROL Enable Tiered Pricing]** eine Option aus.

   - `Disabled` - (Standard) Wählen Sie aus, wann für alle Bestellmengen derselbe Listenpreis gelten soll. Wenn diese Option aktiviert ist, sind alle _[!UICONTROL Pricing Level]_-Felder in diesem Abschnitt deaktiviert.

   - `Enabled` - Wählen Sie aus, wann Sie Preisanpassungen basierend auf der Bestellmenge aktivieren möchten. Wenn diese Option aktiviert ist, sind die Felder _[!UICONTROL Pricing Level]_aktiviert.

1. Nehmen Sie die **[!UICONTROL Pricing Level]** -Einstellungen vor.

   Sie können bis zu fünf Quantitäts-/Rabatteinstellungen definieren, mit denen die Stufenpreise für Ihre Geschäftslisten festgelegt werden. Geben Sie in jeder Zeile den Schwellenwert für die Menge und den anzuwendenden Prozentsatz für den Rabatt an. Wenn Sie beispielsweise im ersten Feld der ersten Zeile den Wert `5` und im zweiten Feld den Wert `5` eingeben, wird beim Preis ein Rabatt von 5 % angewendet, wenn ein anderes Unternehmen eine Menge von 5 oder mehr kauft.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save listing settings]**.

![Amazon Business Pricing (B2B)](assets/amazon-business-pricing.png){width="500" zoomable="yes"}

| Feld | Beschreibung |
|----------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Enable Business Pricing] | Optionen: <ul><li>**[!UICONTROL Disabled]** - (Standard) Wählen Sie aus, wann Sie den geschäftlichen Vertrieb nicht aktivieren möchten. Wenn diese Option aktiviert ist, sind alle anderen Felder in diesem Abschnitt deaktiviert.</li><li>**[!UICONTROL Enabled]** - Wählen Sie aus, wann Sie Ihr Unternehmen für den Geschäftsverkauf aktivieren möchten. Wenn diese Option ausgewählt ist, wird der Geschäftspreis gleich dem Listenpreis festgelegt, nachdem alle Preisregeln angewendet wurden. Der Geschäftspreis entspricht, sofern aktiviert, dem Umfang der Website-Preise. Ein Geschäftspreis darf nicht weniger als 1 Dollar betragen.</li></ul> |
| [!UICONTROL Enable Tiered Pricing] | (Erforderlich) Optionen: <ul><li>**[!UICONTROL Disabled]** - (Standard) Wählen Sie aus, wann für alle Bestellmengen derselbe Listenpreis gelten soll. Wenn diese Option aktiviert ist, sind alle _[!UICONTROL Pricing Level]_-Felder in diesem Abschnitt deaktiviert.</li><li>**[!UICONTROL Enabled]** - Wählen Sie aus, wann Sie Preisanpassungen basierend auf der Bestellmenge aktivieren möchten. Wenn diese Option aktiviert ist, sind die Felder _[!UICONTROL Pricing Level]_aktiviert.</li></ul> |
| [!UICONTROL Pricing Level One-Five (qty/discount)] | Wenn die Option &quot;Tiered Pricing&quot;aktiviert ist, können Sie bis zu fünf Quantitäts-/Discount-Einstellungen definieren, die die Stufenpreise für Ihre Geschäftslisten festlegen. Geben Sie in jeder Zeile den Schwellenwert für die Menge und den anzuwendenden Prozentsatz für den Rabatt an. Wenn Sie beispielsweise im ersten Feld der ersten Zeile den Wert `5` und im zweiten Feld den Wert `5` eingeben, wird beim Preis ein Rabatt von 5 % angewendet, wenn ein anderes Unternehmen eine Menge von fünf oder mehr kauft. |

**Schnellzugriff** - [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
