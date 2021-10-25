---
title: Erfüllt von
description: Verwenden Sie die Fulfillment By-Einstellungen, um zu bestimmen, wie die Bestellungen aus Amazon-Listen ausgeführt (versendet) werden.
redirect_from: /sales-channels/asc/ob-fulfilled-by.html
exl-id: 240c2198-e23d-40e7-be39-b9a4f78565d2
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---

# Erfüllt von

_[!UICONTROL Fulfilled By]_-Einstellungen Teil Ihrer Einstellungen für die Ladenliste sind. Auf die Listseinstellungen kann über folgende Optionen zugegriffen werden: [Dashboard speichern](./amazon-store-dashboard.md).

Diese Einstellungen definieren die Partei, die Bestellungen erfüllt (oder ausführt). Wenn alle Ihre Bestellungen mit einer Methode erfüllt werden, wählen Sie zwischen Händler (Sie) oder Amazon. Wenn Sie planen, Aufträge von Ihrem Standort aus zu erfüllen und Amazon zu verwenden, sollten Sie die dritte Option verwenden und eine [!DNL Commerce] Produktattribut.

- **[!UICONTROL Fulfilled by Merchant]** - Wählen Sie aus, ob Sie, der Händler, alle Bestellungen erfüllen. Wenn eine Bestellung aufgegeben wird, wird der Lagerbestand von Ihrer Bestellung abgezogen [!DNL Commerce] Katalog.

- **[!UICONTROL Fulfilled by Amazon]** - Wählen Sie aus, ob Amazon alle Bestellungen erfüllt. Mit dieser Option wird der Produktbestand nicht von Ihrer [!DNL Commerce] Katalog, wenn eine Bestellung aufgegeben wird. Lagerbestände für Amazon-Aufträge werden gelagert und von ihren Lagern abgezogen. Bevor Sie diese Option zuweisen, müssen Sie Folgendes überprüfen: [!DNL Amazon Seller Central] Konto, für das Ihre Produkte berechtigt sind _Erfüllt von Amazon_ (FBA) Fulfillment. Die FBA-Bestandsaufnahme wird direkt über Ihre [!DNL Amazon Seller Central] Konto. Bei dieser Fulfillment-Methode teilt Amazon Sales Kanal keine Mengenaktualisierungen mit zwischen [!DNL Commerce] und Amazon. Daher stehen Ihnen im Amazon Sales Kanal nicht alle in den Mengeneinstellungen beschriebenen Marketingwerkzeuge zur Verfügung.

- **[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - Wenn Ihre Produkte von Ihnen und Amazon erfüllt werden können, können Sie eine [!DNL Commerce] Produktattribut mit Werten für &quot;Fulfillment by Merchant&quot;und &quot;Fulfillment by Amazon&quot;. Wenn dieser Wert pro Produkt festgelegt wird, gibt dies an, wer die Bestellungen erfüllt.

Die Fulfillment-Methode ist ein regionales Attribut und basiert auf **[!UICONTROL Amazon Marketplace Country]** Einstellung definiert während [Speicherintegration](./store-integration.md). Wenn eine Änderung vorgenommen wird, wirkt sich die Änderung auf alle Amazon-Auflistungen aus, die diese Angaben teilen [!DNL Amazon Seller SKU] in Amazon-Geschäften, die in derselben Region verkauft werden (wie in _[!UICONTROL Amazon Marketplace Country]_während [Speicherintegration](./store-integration.md)). Eine Änderung an einer freigegebenen [!DNL Amazon Seller SKU] in den Vereinigten Staaten hat keine Auswirkungen auf Ihre Amazon-Filialen, die für eine andere Region eingerichtet sind (wie bei der Speicherintegration definiert).

>[!NOTE]
>
>Wenn eine Bestellung von Amazon (FBA) ausgeführt wird und die Bestellung importiert wird, können Sie die Dummy-Daten für einige Felder in den Auftragsdetails sehen. Siehe [Amazon-Auftragsdetails](./amazon-order-details.md).

## Konfigurieren Sie [!UICONTROL Fulfilled By] Einstellungen {#configure-fulfilled-by-settings}

1. Klick **[!UICONTROL Listing Settings]** auf dem Dashboard.

1. Erweitern der _[!UICONTROL Fulfilled By]_Abschnitt.

1. für **[!UICONTROL Product Fulfilled By]**, wer die Bestellung erfüllt (Schiffe):

   - `Fulfilled by Merchant` - Der Händler erfüllt die Bestellung.

   - `Fulfilled by Amazon` - Amazon Warehouse erfüllt die Bestellung.

   - `Assign Fulfilled By Using Magento Product Attribute` - A [!DNL Commerce] -Attribut gibt an, wer die Bestellung pro Produkt erfüllt.

      Wählen Sie die [!DNL Commerce] Attribut, dem Sie zuordnen möchten **[!UICONTROL Fulfilled by Attribute]**.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save listing settings]**.

![Erfüllt durch Einstellungen](assets/amazon-fulfilled-by.png)

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Product Fulfilled By] | Optionen:<ul><li>**[!UICONTROL Fulfilled by Merchant]** - (FBM) Wählen Sie aus, ob Sie die Bestellungen erfüllen. Wenn eine Bestellung aufgegeben wird, wird der Lagerbestand von Ihrer Bestellung abgezogen [!DNL Commerce] Katalog. Wenn ein neues Produkt erstellt wird, wird die Fulfillment-Methode von Merchant Fulfillment zugewiesen.</li><li>**[!UICONTROL Fulfilled by Amazon]** - (FBA) Wählen Sie aus, ob Amazon die Bestellungen erfüllt. Bei dieser Fulfillment-Methode wird der Produktbestand nicht von Ihrer [!DNL Commerce] Katalog, wenn eine Bestellung aufgegeben wird. Wenn ein Produkt erstellt wird, wird es erstellt mit _[!UICONTROL Fulfilled by Amazon (FBA)]_als Fulfillment-Typ. Stellen Sie sicher, dass Ihre Produkte innerhalb Ihrer [!DNL Amazon Seller Central] Konto. FBA-Inventar wird auch direkt über Ihre [!DNL Amazon Seller Central] Konto. Bei dieser Fulfillment-Methode werden Quantitätsaktualisierungen nicht in Relation zu Ihrer [!DNL Commerce] Katalog, sodass Sie einige der Marketingwerkzeuge, die unter [Lagerbestand-/Mengeneinstellungen](./stock-quantity.md).</li><li>**[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** - Wählen Sie aus, ob Sie über eine vorhandene [!DNL Commerce] -Attribut, das bestimmt, ob er vom Händler erfüllt oder von Amazon erfüllt wird. Wenn ausgewählt, **[!UICONTROL Fulfilled by Attribute]** aktiviert.</li></ul> |
| [!UICONTROL Fulfilled By Attribute] | Wählen Sie [!DNL Commerce] Attribut, das zur Bestimmung der Fulfillment-Methode verwendet wird.<br><br>Wenn das Attribut z. B. _Erfüllt von_ und wählen Sie den Attributwert aus als _[!UICONTROL Fulfilled By Merchant]_oder_[!UICONTROL Fulfilled By Amazon (FBA)]_ verwendet das System diesen Wert als Fulfillment-Typ für ein neues Produkt. Als Händler sollten Sie sicherstellen, dass Ihre Produkte innerhalb von [!DNL Amazon Seller Central] Konto. Das FBA-Inventar wird auch direkt über Ihr Amazon-Händlerkonto verwaltet.<br><br>Die Optionen hängen von den Attributen ab, die Sie für Ihre Amazon-Produkte festlegen. |

**Schnellzugriff** - [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
