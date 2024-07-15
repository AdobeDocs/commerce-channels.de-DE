---
title: Amazon Sales Channel - [!UICONTROL Third-party Listings]
description: Aktualisieren Sie die Einstellungen für die Drittanbieterliste, um festzustellen, ob Ihr Commerce-Katalog Produkte aus Ihren bestehenden Amazon Seller Central-Listen importiert.
feature: Sales Channels, Products
exl-id: bc82775a-6f29-49b5-a80b-20e171eaf8f4
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 0%

---

# [!UICONTROL Third-party Listings]

Die Einstellungen für die Drittanbieterliste sind Teil Ihrer Einstellungen für die Speicherauflistung. Auf die Listening-Einstellungen kann über das [Dashboard speichern](./amazon-store-dashboard.md) zugegriffen werden.

Diese Einstellungen bestimmen, ob Ihr [!DNL Commerce] -Katalog Produkte aus Ihren vorhandenen [!DNL Amazon Seller Central]-Listen importiert. Es empfiehlt sich, Listen aus Amazon zu importieren, um sicherzustellen, dass alle Listen mit [!DNL Commerce] -Produkten übereinstimmen. Wenn Ihre Auflistungen Teil Ihres [!DNL Commerce]-Katalogs sind, können Sie alle Ihre Produkte aus einem einzigen Katalog verwalten und die Funktionen der Amazon-Vertriebskanäle verwenden. Zu diesen Funktionen gehören die Erfüllung und Auftragsverwaltung mit Amazon, intelligente Neupreisentwicklung und Mengenverwaltung.

Wenn Sie zum Importieren Ihrer Amazon-Listen konfiguriert sind, importiert der Amazon-Verkaufskanal Ihre Amazon-Listen in Ihren [!DNL Commerce] -Katalog, um sie mit vorhandenen Produkten abzugleichen. Wenn keine Übereinstimmung automatisch gefunden wird, können Sie die Amazon-Liste als neues [!DNL Commerce] -Produkt importieren oder die Liste manuell mit einem Produkt abgleichen.

Wenn Sie Ihre Amazon-Listen importieren möchten, wählen Sie die Attribute [!DNL Commerce] mit Werten für Amazon Seller SKU und Amazon ASIN aus. Wenn Sie nicht über [!DNL Commerce] [Produktattribute](./ob-creating-magento-attributes.md) verfügen, sollten Sie sie erstellen und zuweisen. Die Zuordnung dieser Attribute erleichtert die korrekte Zuordnung importierter Amazon-Listen zu Ihren [!DNL Commerce] -Produkten.

Der erste Listenimport wird initiiert, wenn die [Speicherintegration](./store-integration.md) abgeschlossen ist. Danach sucht [!DNL Commerce] basierend auf Ihren Cron-Einstellungen kontinuierlich nach neu hinzugefügten Amazon-Listen (die nicht in Amazon Sales Channel erstellt wurden) und aktualisiert Ihren [!DNL Commerce]-Katalog entsprechend Ihren Drittanbieter-Listeneinstellungen.

## Einstellungen für die Drittanbieterliste konfigurieren

1. Klicken Sie im Store-Dashboard auf **[!UICONTROL Listing Settings]** .

1. Erweitern Sie den Abschnitt _[!UICONTROL Third Party Listings]_.

1. Wählen Sie für &quot;**[!UICONTROL Import Third Party Listings]**&quot;(erforderlich) eine Option:

   - `Import Listing` - (Standard) Wählen Sie aus, wann Produktinformationen aus Ihren Amazon-Listen in Ihren [!DNL Commerce] Produktkatalog importiert werden sollen. Diese Option ist die Standardoption und wird empfohlen.

   - `Do Not Import Listing` - Wählen Sie aus, wann Sie manuell [ neue Produkte erstellen und ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html) Ihrem [!DNL Commerce] -Katalog für Ihre Amazon-Auflistungen zuweisen möchten.

   >[!NOTE]
   >Die folgenden Optionsfelder sind nur aktiv, wenn auf `Import Listing` gesetzt.

1. Wählen Sie für &quot;**[!UICONTROL Attribute That Contains Amazon Seller SKU]**&quot;das Attribut [!DNL Commerce] aus, das mit dem Amazon Seller SKU-Wert übereinstimmt.

1. Wählen Sie für **[!UICONTROL Attribute That Contains Amazon ASIN]** das von Ihnen erstellte [!DNL Commerce] -Attribut aus und ordnen Sie es dem Amazon-ASIN zu.

   >[!NOTE]
   >Wenn Sie diese [!DNL Commerce] -Attribute nicht für Ihre Amazon-Auflistungen erstellt haben, finden Sie weitere Informationen unter [Erstellen von Attributen für Amazon-Übereinstimmung](./ob-creating-magento-attributes.md).

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save listing settings]**.

![Drittanbieterlisten](assets/amazon-third-party-listings.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|--------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Import Third Party Listings] | Erforderlich. Optionen:<ul><li>**[!UICONTROL Import Listing]** - (Standard) Wählen Sie aus, wann Produktinformationen aus Ihren Amazon-Listen in Ihren [!DNL Commerce] Produktkatalog importiert werden sollen. </li><li>**[!UICONTROL Do Not Import Listing]** - Wählen Sie aus, wann Sie manuell [ neue Produkte erstellen und ](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html) Ihrem [!DNL Commerce] -Katalog für Ihre Amazon-Auflistungen zuweisen möchten.</li></ul> |
| [!UICONTROL Attribute That Contains Amazon Seller SKU] | Nur aktiv, wenn auf `Import Listing` gesetzt.<br>Wählen Sie das Attribut [!DNL Commerce] als Übereinstimmung mit dem Amazon-Attribut für die Amazon Seller-SKU aus. Wenn dieses Attribut nicht vorhanden ist, finden Sie weitere Informationen unter [Erstellen von Amazon-Produktattributen für Amazon-Übereinstimmung](./ob-creating-magento-attributes.md). Überprüfen Sie bei Bedarf Ihre [!DNL Commerce] [attribute](./managing-attributes.md) und erstellen oder bearbeiten Sie ein Attribut, das diesen Amazon-Daten entspricht. |
| [!UICONTROL Attribute That Contains Amazon ASIN] | Nur aktiv, wenn auf `Import Listing` gesetzt.<br>Wählen Sie das Attribut [!DNL Commerce] aus, das mit dem Amazon-Attribut für Amazon ASIN übereinstimmt. Wenn dieses Attribut nicht vorhanden ist, finden Sie weitere Informationen unter [Erstellen von Amazon-Produktattributen für Amazon-Übereinstimmung](./ob-creating-magento-attributes.md). Überprüfen Sie bei Bedarf Ihre [!DNL Commerce] [attribute](./managing-attributes.md) und erstellen oder bearbeiten Sie ein Attribut, das diesen Amazon-Daten entspricht. |

**Schnellzugriff** - [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
