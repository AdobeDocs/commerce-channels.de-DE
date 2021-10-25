---
title: Listen von Drittanbietern
description: Über die Aktualisierung der Drittanbieterlisten-Einstellungen bestimmen Sie, ob Ihr Commerce-Katalog Produkte aus Ihren bestehenden Amazon Seller Central-Listen importiert.
redirect_from: /sales-channels/asc/ob-third-party-listings.html
exl-id: bc82775a-6f29-49b5-a80b-20e171eaf8f4
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# Listen von Drittanbietern

Die Einstellungen für die Drittanbieter-Auflistung sind Teil der Einstellungen für die Store-Auflistung. Auf die Listseinstellungen kann über folgende Optionen zugegriffen werden: [Dashboard speichern](./amazon-store-dashboard.md).

Diese Einstellungen bestimmen, ob Ihre [!DNL Commerce] Katalog importiert Produkte aus Ihren vorhandenen [!DNL Amazon Seller Central] Auflistungen. Es ist empfehlenswert, Listen aus Amazon zu importieren, um sicherzustellen, dass alle Auflistungen übereinstimmen. [!DNL Commerce] Produkte. Wenn Ihre Auflistungen Teil Ihrer [!DNL Commerce] können Sie alle Ihre Produkte aus einem einzigen Katalog verwalten und Amazon Sales Kanal-Funktionen verwenden. Zu diesen Funktionen gehören Fulfillment- und Auftragsmanagement mit Amazon, intelligente Preisgestaltung und Mengenmanagement.

Wenn Amazon Sales Kanal für den Import Ihrer Amazon-Listen konfiguriert ist, importiert er Ihre Amazon-Einträge in Ihre [!DNL Commerce] Katalog, der versucht, sie mit vorhandenen Produkten abzugleichen. Wenn eine Übereinstimmung nicht automatisch gefunden wird, können Sie die Amazon-Liste als neue importieren. [!DNL Commerce] oder ordnen Sie die Auflistung einem Produkt manuell zu.

Wenn Sie Ihre Amazon-Listen importieren möchten, wählen Sie [!DNL Commerce] Attribute mit Werten für Amazon Seller SKU und Amazon ASIN. Wenn Sie [!DNL Commerce] [Produktattribute](./ob-creating-magento-attributes.md), erwägen Sie, sie zu erstellen und zuzuweisen. Durch Zuordnen dieser Attribute werden importierte Amazon-Listen Ihren [!DNL Commerce] Produkte.

Der Import der ursprünglichen Liste wird gestartet, wenn [Speicherintegration](./store-integration.md) ist abgeschlossen. Anschließend und basierend auf Ihren cron-Einstellungen [!DNL Commerce] fortlaufend nach neu hinzugefügten Amazon-Listen (nicht im Amazon-Sales Channel erstellt) und aktualisiert Ihre [!DNL Commerce] Katalog gemäß Ihren Drittanbieter-Listings-Einstellungen.

## Einstellungen für Liste von Drittanbietern konfigurieren

1. Klick **[!UICONTROL Listing Settings]** auf dem Dashboard.

1. Erweitern der _[!UICONTROL Third Party Listings]_Abschnitt.

1. für **[!UICONTROL Import Third Party Listings]** (erforderlich), wählen Sie eine Option aus:

   - `Import Listing` - (Standard) Wählen Sie aus, wann Produktinformationen aus Ihren Amazon-Listen in Ihre [!DNL Commerce] Produktkatalog. Diese Option ist die Standardeinstellung und wird empfohlen.

   - `Do Not Import Listing` - Auswählen, wenn Sie manuell [neue Produkte erstellen und zuweisen](https://docs.magento.com/user-guide/catalog/products.html){Zielgruppe=&quot;_blank&quot; [!DNL Commerce] Katalog für Ihre Amazon-Listen.
   >[!NOTE]
   >Die folgenden Optionsfelder sind nur aktiv, wenn sie auf `Import Listing`.

1. für **[!UICONTROL Attribute That Contains Amazon Seller SKU]**, wählen Sie [!DNL Commerce] -Attribut, das dem Amazon Seller-SKU-Wert entspricht.

1. für **[!UICONTROL Attribute That Contains Amazon ASIN]**, wählen Sie [!DNL Commerce] Attribut, das Sie erstellt haben, und passend zum Amazon ASIN.

   >[!NOTE]
   >Wenn Sie diese nicht erstellt haben [!DNL Commerce] -Attribute für Ihre Amazon-Auflistungen, siehe [Erstellen von Attributen für Amazon Matching](./ob-creating-magento-attributes.md).

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save listing settings]**.

![Listen von Drittanbietern](assets/amazon-third-party-listings.png)

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Import Third Party Listings] | Erforderlich. Optionen:<ul><li>**[!UICONTROL Import Listing]** - (Standard) Wählen Sie aus, wann Produktinformationen aus Ihren Amazon-Listen in Ihre [!DNL Commerce] Produktkatalog. </li><li>**[!UICONTROL Do Not Import Listing]** - Auswählen, wenn Sie manuell [neue Produkte erstellen und zuweisen](https://docs.magento.com/user-guide/catalog/products.html){Zielgruppe=&quot;_blank&quot; [!DNL Commerce] Katalog für Ihre Amazon-Listen.</li></ul> |
| [!UICONTROL Attribute That Contains Amazon Seller SKU] | Nur aktiv, wenn auf `Import Listing`.<br>Wählen Sie [!DNL Commerce] -Attribut als Übereinstimmung mit dem Amazon-Attribut für die Amazon Seller SKU. Wenn dieses Attribut nicht vorhanden ist, siehe [Erstellen von Amazon-Produktattributen für Amazon Matching](./ob-creating-magento-attributes.md). Überprüfen Sie bei Bedarf Ihre [!DNL Commerce] [Attribute](./managing-attributes.md) und erstellen oder bearbeiten Sie ein Attribut, das diesen Amazon-Daten entspricht. |
| [!UICONTROL Attribute That Contains Amazon ASIN] | Nur aktiv, wenn auf `Import Listing`.<br>Wählen Sie [!DNL Commerce] -Attribut, das mit dem Amazon-Attribut für das Amazon ASIN übereinstimmt. Wenn dieses Attribut nicht vorhanden ist, siehe [Erstellen von Amazon-Produktattributen für Amazon Matching](./ob-creating-magento-attributes.md). Überprüfen Sie bei Bedarf Ihre [!DNL Commerce] [Attribute](./managing-attributes.md) und erstellen oder bearbeiten Sie ein Attribut, das diesen Amazon-Daten entspricht. |

**Schnellzugriff** - [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
