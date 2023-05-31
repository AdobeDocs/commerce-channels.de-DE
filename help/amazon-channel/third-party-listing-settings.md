---
title: Amazon-Vertriebskanal - [!UICONTROL Third-party Listings]
description: Aktualisieren Sie die Einstellungen für die Drittanbieterliste, um festzustellen, ob Ihr Commerce-Katalog Produkte aus Ihren bestehenden Amazon Seller Central-Listen importiert.
redirect_from: /sales-channels/asc/ob-third-party-listings.html
exl-id: bc82775a-6f29-49b5-a80b-20e171eaf8f4
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# [!UICONTROL Third-party Listings]

Die Einstellungen für die Drittanbieterliste sind Teil Ihrer Einstellungen für die Speicherauflistung. Auf die Listening-Einstellungen kann über die [Store-Dashboard](./amazon-store-dashboard.md).

Diese Einstellungen bestimmen, ob Ihre [!DNL Commerce] -Katalog importiert Produkte aus Ihrem bestehenden [!DNL Amazon Seller Central] Auflistungen. Es empfiehlt sich, Listen aus Amazon zu importieren, um sicherzustellen, dass alle Auflistungen übereinstimmen. [!DNL Commerce] Produkte. Wenn Ihre Auflistungen Teil Ihrer [!DNL Commerce] -Katalog können Sie alle Ihre Produkte aus einem einzigen Katalog verwalten und die Funktionen des Amazon-Vertriebskanals verwenden. Zu diesen Funktionen gehören die Erfüllung und Auftragsverwaltung mit Amazon, intelligente Neupreisentwicklung und Mengenverwaltung.

Wenn der Amazon-Vertriebskanal für den Import Ihrer Amazon-Listen konfiguriert ist, importiert er Ihre Amazon-Listen in Ihre [!DNL Commerce] -Katalog, der versucht, sie mit vorhandenen Produkten abzugleichen. Wenn eine Übereinstimmung nicht automatisch gefunden wird, können Sie die Amazon-Liste als neue [!DNL Commerce] Produkt oder die manuelle Zuordnung der Liste zu einem Produkt.

Wenn Sie Ihre Amazon-Listen importieren möchten, wählen Sie die [!DNL Commerce] -Attribute mit Werten für Amazon Seller SKU und Amazon ASIN. Wenn Sie [!DNL Commerce] [Produktattribute](./ob-creating-magento-attributes.md), sollten Sie sie erstellen und zuweisen. Die Zuordnung dieser Attribute erleichtert die korrekte Zuordnung importierter Amazon-Listen zu Ihren [!DNL Commerce] Produkte.

Der erste Listenimport wird beim [Store-Integration](./store-integration.md) ist abgeschlossen. Anschließend und basierend auf Ihren Cron-Einstellungen [!DNL Commerce] sucht kontinuierlich nach neu hinzugefügten Amazon-Listen (nicht im Amazon-Sales Channel erstellt) und aktualisiert Ihre [!DNL Commerce] Katalog entsprechend Ihren Drittanbieter-Listening-Einstellungen.

## Einstellungen für die Drittanbieterliste konfigurieren

1. Klicken **[!UICONTROL Listing Settings]** im Dashboard speichern.

1. Erweitern Sie die _[!UICONTROL Third Party Listings]_Abschnitt.

1. Für **[!UICONTROL Import Third Party Listings]** (erforderlich), wählen Sie eine Option aus:

   - `Import Listing` - (Standard) Wählen Sie aus, wann Produktinformationen aus Ihren Amazon-Listen in Ihre [!DNL Commerce] Produktkatalog. Diese Option ist die Standardoption und wird empfohlen.

   - `Do Not Import Listing` - Legen Sie fest, wann Sie manuell [Erstellen und Zuweisen neuer Produkte](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html) auf [!DNL Commerce] Katalog für Ihre Amazon-Auflistungen.
   >[!NOTE]
   >Die folgenden Optionsfelder sind nur aktiv, wenn auf `Import Listing`.

1. Für **[!UICONTROL Attribute That Contains Amazon Seller SKU]**, wählen Sie die [!DNL Commerce] -Attribut, das mit dem Amazon Seller-SKU-Wert übereinstimmt.

1. Für **[!UICONTROL Attribute That Contains Amazon ASIN]**, wählen Sie die [!DNL Commerce] -Attribut, das Sie erstellt haben, und ordnen Sie es dem Amazon-ASIN zu.

   >[!NOTE]
   >Wenn Sie diese nicht erstellt haben [!DNL Commerce] -Attribute für Ihre Amazon-Listen finden Sie unter [Erstellen von Attributen für Amazon-Übereinstimmung](./ob-creating-magento-attributes.md).

1. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Save listing settings]**.

![Drittanbieterlisten](assets/amazon-third-party-listings.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Import Third Party Listings] | Erforderlich. Optionen:<ul><li>**[!UICONTROL Import Listing]** - (Standard) Wählen Sie aus, wann Produktinformationen aus Ihren Amazon-Listen in Ihre [!DNL Commerce] Produktkatalog. </li><li>**[!UICONTROL Do Not Import Listing]** - Legen Sie fest, wann Sie manuell [Erstellen und Zuweisen neuer Produkte](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html) auf [!DNL Commerce] Katalog für Ihre Amazon-Auflistungen.</li></ul> |
| [!UICONTROL Attribute That Contains Amazon Seller SKU] | Nur aktiv , wenn auf `Import Listing`.<br>Wählen Sie die [!DNL Commerce] als Übereinstimmung mit dem Amazon-Attribut für die Amazon Seller-SKU. Wenn dieses Attribut nicht vorhanden ist, lesen Sie [Erstellen von Amazon-Produktattributen für Amazon-Übereinstimmung](./ob-creating-magento-attributes.md). Überprüfen Sie bei Bedarf Ihre [!DNL Commerce] [attributes](./managing-attributes.md) und erstellen oder bearbeiten Sie ein Attribut, das diesen Amazon-Daten entspricht. |
| [!UICONTROL Attribute That Contains Amazon ASIN] | Nur aktiv , wenn auf `Import Listing`.<br>Wählen Sie die [!DNL Commerce] -Attribut, das mit dem Amazon-Attribut für Amazon ASIN übereinstimmt. Wenn dieses Attribut nicht vorhanden ist, lesen Sie [Erstellen von Amazon-Produktattributen für Amazon-Übereinstimmung](./ob-creating-magento-attributes.md). Überprüfen Sie bei Bedarf Ihre [!DNL Commerce] [attributes](./managing-attributes.md) und erstellen oder bearbeiten Sie ein Attribut, das diesen Amazon-Daten entspricht. |

**Schnellzugriff** - [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
