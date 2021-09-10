---
title: Drittanbieterlisten
description: 'Aktualisieren Sie die Einstellungen für die Drittanbieterliste, um festzustellen, ob Ihr Commerce-Katalog Produkte aus Ihren bestehenden Amazon Seller Central-Listen importiert.'
redirect_from: /sales-channels/asc/ob-third-party-listings.html: 
exl-id: bc82775a-6f29-49b5-a80b-20e171eaf8f4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 519
ht-degree: 0%

---

# Drittanbieterlisten

Die Einstellungen für die Drittanbieterliste sind Teil Ihrer Einstellungen für die Speicherauflistung. Auf die Listening-Einstellungen kann über das [Store-Dashboard](./amazon-store-dashboard.md) zugegriffen werden.

Diese Einstellungen bestimmen, ob Ihr [!DNL Commerce]-Katalog Produkte aus Ihren vorhandenen [!DNL Amazon Seller Central]-Listen importiert. Es empfiehlt sich, Listen aus Amazon zu importieren, um sicherzustellen, dass alle Listen die [!DNL Commerce] -Produkte aufweisen. Wenn Ihre Auflistungen Teil Ihres [!DNL Commerce]-Katalogs sind, können Sie alle Ihre Produkte aus einem einzigen Katalog verwalten und die Funktionen der Amazon-Vertriebskanäle nutzen. Zu diesen Funktionen gehören die Erfüllung und Auftragsverwaltung mit Amazon, intelligente Neupreisentwicklung und Mengenverwaltung.

Wenn der Amazon-Vertriebskanal für den Import Ihrer Amazon-Listen konfiguriert ist, importiert er Ihre Amazon-Auflistungen in Ihren [!DNL Commerce]-Katalog und versucht, sie mit vorhandenen Produkten abzugleichen. Wenn keine Übereinstimmung automatisch gefunden wird, können Sie die Amazon-Liste als neues [!DNL Commerce]-Produkt importieren oder die Liste manuell einem Produkt zuordnen.

Wenn Sie Ihre Amazon-Listen importieren möchten, wählen Sie die [!DNL Commerce]-Attribute mit Werten für Amazon Seller SKU und Amazon ASIN aus. Wenn Sie nicht über [!DNL Commerce] [Produktattribute](./ob-creating-magento-attributes.md) verfügen, sollten Sie diese erstellen und zuweisen. Die Zuordnung dieser Attribute erleichtert die korrekte Zuordnung importierter Amazon-Listen zu Ihren [!DNL Commerce] -Produkten.

Der erste Listenimport wird initiiert, wenn die [Speicherintegration](./store-integration.md) abgeschlossen ist. Anschließend sucht [!DNL Commerce] basierend auf Ihren Cron-Einstellungen kontinuierlich nach neu hinzugefügten Amazon-Listen (die nicht im Amazon-Sales Channel erstellt wurden) und aktualisiert Ihren [!DNL Commerce]-Katalog entsprechend Ihren Drittanbieter-Listeneinstellungen.

## Einstellungen für die Drittanbieterliste konfigurieren

1. Klicken Sie im Store-Dashboard auf **[!UICONTROL Listing Settings]** .

1. Erweitern Sie den Abschnitt _[!UICONTROL Third Party Listings]_.

1. Wählen Sie für **[!UICONTROL Import Third Party Listings]** (erforderlich) eine Option:

   - `Import Listing` - (Standard) Wählen Sie aus, wann Produktinformationen aus Ihren Amazon-Listen in Ihren  [!DNL Commerce] Produktkatalog importiert werden sollen. Diese Option ist die Standardoption und wird empfohlen.

   - `Do Not Import Listing` - Wählen Sie aus, wann Sie manuell  [erstellen und neue Produkte](https://docs.magento.com/user-guide/catalog/products.html){:target=&quot;_blank&quot;} Ihrem  [!DNL Commerce] Katalog für Ihre Amazon-Auflistungen zuweisen möchten.
   >[!NOTE]
   >Die folgenden Optionsfelder sind nur aktiv, wenn auf `Import Listing` gesetzt.

1. Wählen Sie für **[!UICONTROL Attribute That Contains Amazon Seller SKU]** das Attribut [!DNL Commerce] aus, das dem Amazon Seller SKU-Wert entspricht.

1. Wählen Sie für **[!UICONTROL Attribute That Contains Amazon ASIN]** das von Ihnen erstellte [!DNL Commerce]-Attribut aus und ordnen Sie es dem Amazon-ASIN zu.

   >[!NOTE]
   >Wenn Sie diese [!DNL Commerce]-Attribute nicht für Ihre Amazon-Auflistungen erstellt haben, finden Sie weitere Informationen unter [Erstellen von Attributen für die Amazon-Zuordnung](./ob-creating-magento-attributes.md).

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save listing settings]**.

![Drittanbieterlisten](assets/amazon-third-party-listings.png)

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Import Third Party Listings] | Erforderlich. Optionen:<ul><li>**[!UICONTROL Import Listing]** - (Standard) Wählen Sie aus, wann Produktinformationen aus Ihren Amazon-Listen in Ihren  [!DNL Commerce] Produktkatalog importiert werden sollen. </li><li>**[!UICONTROL Do Not Import Listing]** - Wählen Sie aus, wann Sie manuell  [erstellen und neue Produkte](https://docs.magento.com/user-guide/catalog/products.html){:target=&quot;_blank&quot;} Ihrem  [!DNL Commerce] Katalog für Ihre Amazon-Auflistungen zuweisen möchten.</li></ul> |
| [!UICONTROL Attribute That Contains Amazon Seller SKU] | Nur aktiv, wenn auf `Import Listing` gesetzt.<br>Wählen Sie das  [!DNL Commerce] Attribut als Übereinstimmung mit dem Amazon-Attribut für die Amazon Seller SKU aus. Wenn dieses Attribut nicht vorhanden ist, finden Sie weitere Informationen unter [Erstellen von Amazon-Produktattributen für Amazon-Übereinstimmungen](./ob-creating-magento-attributes.md). Überprüfen Sie bei Bedarf Ihre [!DNL Commerce] [Attribute](./managing-attributes.md) und erstellen oder bearbeiten Sie ein Attribut, das diesen Amazon-Daten entspricht. |
| [!UICONTROL Attribute That Contains Amazon ASIN] | Nur aktiv, wenn auf `Import Listing` gesetzt.<br>Wählen Sie das  [!DNL Commerce] Attribut aus, das dem Amazon-Attribut für Amazon ASIN entspricht. Wenn dieses Attribut nicht vorhanden ist, finden Sie weitere Informationen unter [Erstellen von Amazon-Produktattributen für Amazon-Übereinstimmungen](./ob-creating-magento-attributes.md). Überprüfen Sie bei Bedarf Ihre [!DNL Commerce] [Attribute](./managing-attributes.md) und erstellen oder bearbeiten Sie ein Attribut, das diesen Amazon-Daten entspricht. |

**Schnellzugriff**  -  [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
