---
title: Erfüllen durch Einstellungen für Amazon-Listen
description: Verwenden Sie die Einstellungen Erfüllen von , um zu bestimmen, wie die Bestellungen aus Amazon-Auflistungen erfüllt (versandt) werden.
feature: Sales Channels, Products
exl-id: 240c2198-e23d-40e7-be39-b9a4f78565d2
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# Erfüllen durch Einstellungen für Amazon-Listen

_[!UICONTROL Fulfilled By]_-Einstellungen sind Teil Ihrer Einstellungen für die Store-Auflistung. Auf die Listening-Einstellungen kann über das [Dashboard speichern](./amazon-store-dashboard.md) zugegriffen werden.

Diese Einstellungen definieren die Partei, die Bestellungen erfüllt (oder ausführt). Wenn alle Ihre Bestellungen mit einer Methode erfüllt sind, wählen Sie zwischen Händler (Sie) oder Amazon. Wenn Sie Bestellungen von Ihren Standorten ausführen und Amazon verwenden möchten, empfiehlt es sich, die dritte Option zu verwenden und ein [!DNL Commerce] -Produktattribut zu konfigurieren.

- **[!UICONTROL Fulfilled by Merchant]** - Entscheiden Sie, ob Sie, der Händler, alle Bestellungen erfüllen. Wenn eine Bestellung aufgegeben wird, wird der Bestand aus Ihrem [!DNL Commerce] -Katalog abgezogen.

- **[!UICONTROL Fulfilled by Amazon]** - Entscheiden Sie, ob Amazon alle Bestellungen erfüllt. Mit dieser Option wird der Produktbestand nicht von Ihrem [!DNL Commerce] -Katalog abgezogen, wenn eine Bestellung aufgegeben wird. Lagerbestand für von Amazon erfüllte Bestellungen wird gespeichert und von ihren Lagern abgezogen. Bevor Sie diese Option zuweisen, müssen Sie in Ihrem [!DNL Amazon Seller Central]-Konto überprüfen, ob Ihre Produkte für die Erfüllung von _Fulfill By Amazon_ (FBA) geeignet sind. Der FBA-Bestand wird direkt über Ihr [!DNL Amazon Seller Central] -Konto verwaltet. Mit dieser Ausführungsmethode gibt der Amazon-Verkaufskanal keine Mengenaktualisierungen zwischen [!DNL Commerce] und Amazon frei. Daher stehen Ihnen nicht alle in den Mengeneinstellungen beschriebenen Marketing-Tools im Amazon-Vertriebskanal zur Verfügung.

- **[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - Wenn Ihre Produkte von Ihnen und Amazon möglicherweise erfüllt werden, sollten Sie ein [!DNL Commerce] -Produktattribut mit Werten für &quot;Fulfill By Merchant&quot;und &quot;Fulfill by Amazon&quot;erstellen. Wenn Sie diesen Wert pro Produkt festlegen, wird angegeben, wer die Bestellungen erfüllt.

Die Ausführungsmethode ist ein regionales Attribut, das auf der während der [Store-Integration](./store-integration.md) definierten Einstellung **[!UICONTROL Amazon Marketplace Country]** basiert. Wenn eine Änderung vorgenommen wird, wirkt sich die Änderung auf alle Amazon-Auflistungen aus, die den Wert [!DNL Amazon Seller SKU] in Ihren Amazon-Stores verwenden, die in derselben Region verkauft werden (wie in _[!UICONTROL Amazon Marketplace Country]_während der [Store-Integration](./store-integration.md) definiert). Eine Änderung an einem freigegebenen &quot;[!DNL Amazon Seller SKU]&quot;in den USA wirkt sich nicht auf Ihre Amazon-Stores aus, die für eine andere Region festgelegt wurden (wie in der Store-Integration definiert).

>[!NOTE]
>
>Wenn eine Bestellung von Amazon (FBA) erfüllt wird und die Bestellung importiert wird, können Sie Platzhalterdaten für einige Felder in den Bestelldetails sehen. Siehe [Amazon-Bestelldetails](./amazon-order-details.md).

## [!UICONTROL Fulfilled By]-Einstellungen konfigurieren {#configure-fulfilled-by-settings}

1. Klicken Sie im Store-Dashboard auf **[!UICONTROL Listing Settings]** .

1. Erweitern Sie den Abschnitt _[!UICONTROL Fulfilled By]_.

1. Wählen Sie für **[!UICONTROL Product Fulfilled By]** aus, wer die Reihenfolge erfüllt (ausführt):

   - `Fulfilled by Merchant` - Der Händler erfüllt die Bestellung.

   - `Fulfilled by Amazon` - Amazon Warehouse erfüllt die Bestellung.

   - `Assign Fulfilled By Using Magento Product Attribute` - Ein [!DNL Commerce] -Attribut gibt an, wer die Bestellung pro Produkt erfüllt.

     Wählen Sie, falls ausgewählt, das Attribut [!DNL Commerce] aus, das Sie in **[!UICONTROL Fulfilled by Attribute]** zuordnen möchten.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save listing settings]**.

![Erfüllt durch Einstellungen](assets/amazon-fulfilled-by.png){width="500" zoomable="yes"}

| Feld | Beschreibung |
|-------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product Fulfilled By] | Optionen:<ul><li>**[!UICONTROL Fulfilled by Merchant]** - (FBM) Wählen Sie aus, ob Sie die Bestellungen erfüllen. Wenn eine Bestellung aufgegeben wird, wird der Bestand aus Ihrem [!DNL Commerce] -Katalog abgezogen. Wenn ein neues Produkt erstellt wird, wird die Ausführungsmethode von Merchant Fulfill zugewiesen.</li><li>**[!UICONTROL Fulfilled by Amazon]** - (FBA) Entscheiden Sie, ob Amazon die Bestellungen erfüllt. Bei dieser Ausführungsmethode wird der Produktbestand nicht aus Ihrem [!DNL Commerce] -Katalog abgezogen, wenn eine Bestellung aufgegeben wird. Wenn ein Produkt erstellt wird, wird es mit _[!UICONTROL Fulfilled by Amazon (FBA)]_als Erfüllungstyp erstellt. Stellen Sie sicher, dass Ihre Produkte in Ihrem [!DNL Amazon Seller Central] -Konto FBA-Erfüllung erhalten. Der FBA-Bestand wird auch direkt über Ihr [!DNL Amazon Seller Central]-Konto verwaltet. Bei dieser Ausführungsmethode werden Mengenaktualisierungen nicht in Bezug auf Ihren [!DNL Commerce] -Katalog gesendet. Daher können Sie einige der unter [Lagereinstellungen/Mengeneinstellungen](./stock-quantity.md) beschriebenen Marketing-Tools nicht verwenden.</li><li>**[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - Entscheiden Sie, ob Sie über ein vorhandenes [!DNL Commerce] -Attribut verfügen, das bestimmt, ob es vom Händler erfüllt oder von Amazon erfüllt wird. Wenn diese Option ausgewählt ist, aktiviert **[!UICONTROL Fulfilled by Attribute]** .</li></ul> |
| [!UICONTROL Fulfilled By Attribute] | Wählen Sie das Attribut [!DNL Commerce] aus, das zur Bestimmung der Ausführungsmethode verwendet wird.<br><br>Wenn das Attribut beispielsweise _Fulfill By_ ist und Sie den Attributwert als `Fulfilled By Merchant` oder `Fulfilled By Amazon (FBA)` wählen, verwendet das System diesen Wert als Erfüllungstyp für ein neues Produkt. Als Händler sollten Sie sicherstellen, dass Ihre Produkte innerhalb Ihres [!DNL Amazon Seller Central]-Kontos für die FBA-Erfüllung infrage kommen. FBA Inventory wird auch direkt über Ihr Amazon-Verkaufskonto verwaltet.<br><br>Optionen hängen von den Attributen ab, die Sie für Ihre Amazon-Produkte einrichten. |

**Schnellzugriff** - [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
