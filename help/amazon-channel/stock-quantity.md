---
title: Bestand/Menge
description: So steuern Sie die Synchronisierung der Produktmengendetails aus Ihrem Commerce-Store mit Ihrem [!DNL Amazon Seller Central] -Konto, aktualisieren Sie die Einstellungen für Lagerbestand/Menge.
redirect_from: /sales-channels/asc/ob-stock-quantity.html
exl-id: a8b7ab6c-393c-43c6-b5ef-68845177edff
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Bestand/Menge

*[!UICONTROL Stock/Quantity]* -Einstellungen Teil Ihrer Einstellungen für die Ladenliste sind. Auf die Listseinstellungen kann über folgende Optionen zugegriffen werden: [Dashboard speichern](./amazon-store-dashboard.md).

Diese Einstellungen werden verwendet, um die Produktmengendetails von Ihren [!DNL Commerce] speichern Sie die Menge auf [!DNL Amazon Seller Central] Konto. Dieses Tool ist leistungsstark und kann für zusätzliche Werbung verwendet werden, indem es die Dringlichkeit gegenüber dem Käufer zeigt, während Ihr Inventar organisiert bleibt. Einige Händler könnten beispielsweise 150 Artikel einer bestimmten SKU in ihrem Lager vorrätig haben und wollen sicherstellen, dass Amazon-Käufer ihren gesamten Bestand kaufen können. Andere Händler möchten möglicherweise nur ein Element auf einmal Liste haben, um dem Endnutzer ein Gefühl der Knappheit zu vermitteln. In diesem Fall setzen Sie die *[!UICONTROL Maximum Listed Quantity]* nach `1`.

Die Menge ist ein regionales Attribut und basiert auf **[!UICONTROL Amazon Marketplace Country]** Einstellung definieren während [Speicherintegration](./store-integration.md). Wenn eine Änderung der Produktmenge vorgenommen wird, wirkt sich die Änderung auf alle Amazon-Auflistungen aus, die diese Produktmenge teilen [!DNL Amazon Seller SKU] in Ihren Amazon-Geschäften, die im selben Land verkauft werden. Eine Änderung an einer freigegebenen [!DNL Amazon Seller SKU] in den Vereinigten Staaten hat keine Auswirkungen auf Ihre Amazon-Filialen, die für ein anderes Land eingerichtet wurden. Ihr erster Amazon Store, der integriert ist (mit dem ältesten Erstellungsdatum), kontrolliert die Priorität in den Mengeneinstellungen.

>[!NOTE]
>
>Amazon Sales Kanal unterstützt bei Adobe Commerce und Magento Open Source 2.3.x die Verwendung der Lagerbestandsverwaltung ohne zusätzliche Einstellungen. Siehe [Lagerbestand verwalten](https://docs.magento.com/user-guide/v2.3/catalog/inventory-management.html){Zielgruppe=&quot;_blank&quot;}.

## Lager-/Mengeneinstellungen konfigurieren {#configure-stock--quantity-settings}

1. Klick **[!UICONTROL Listing Settings]** auf dem Dashboard.

1. Erweitern der **[!UICONTROL Stock / Quantity]** Abschnitt.

1. für **[!UICONTROL Out-of-Stock Threshold]** (erforderlich) einen numerischen Wert für die niedrigste Menge eines Erzeugnisses eingeben, um das Erzeugnis für die Aufnahme in die Amazon-Liste in Betracht zu ziehen.

   Der Standardwert ist `0`. Wenn [!DNL Commerce] Der Produktbestand liegt unter dieser Zahl, die jeweilige Amazon-Liste ist nicht für den Verkauf über Amazon geeignet.

1. für **[!UICONTROL Maximum Listed Quantity]** (erforderlich), geben Sie einen numerischen Wert für die Menge ein, die Sie in Ihrer Amazon-Liste anzeigen möchten.

   Diese Einstellung Liste alle Ihre Amazon-Auflistungen zum eingegebenen Wert. Beim Verkauf eines Artikels ändert sich die Amazon-Listungsmenge nicht. Die verfügbare Auflistungsmenge verwendet diesen Wert immer, auch wenn die tatsächliche Produktmenge höher oder niedriger ist. Diese Einstellung wird normalerweise verwendet, wenn Sie das Produktinventar nicht verwalten. Sie können z. B. ein Produkt mit einer Menge von 80 in Ihrem [!DNL Commerce] Katalog. Mit Set auf `10`, zeigt die Amazon-Liste immer eine verfügbare Menge an `10` und ändert sich nicht, wenn der Verkauf für das Produkt erfolgt.

1. für **[!UICONTROL "Do Not Manage Stock" Quantity]** (erforderlich), geben Sie einen Mengenwert ein, der für Ihre Amazon-Auflistungen angezeigt werden soll.

   Amazon verlangt, dass Sie eine verfügbare Menge veröffentlichen. für [!DNL Commerce] Produkte, die nicht auf Lager zu verwalten, aber Sie möchten sie auf Amazon, die Liste wird mit der verfügbaren Menge hier eingegeben veröffentlicht.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save listing settings]**.

![Lagerungs-/Mengeneinstellungen](assets/amazon-stock-quantity.png)

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Out-of-Stock Threshold] | Geben Sie einen numerischen Wert für die niedrigste Produktmenge ein, damit das Produkt weiterhin für die Amazon-Auflistung in Betracht kommt (Standard: `0`).<br><br>Wenn [!DNL Commerce] Der Produktbestand liegt unter dieser Zahl, die jeweilige Amazon-Liste ist nicht für den Verkauf über Amazon geeignet. |
| [!UICONTROL Maximum Listed Quantity] | Geben Sie einen numerischen Wert für die Menge ein, die Sie in Ihrer Amazon-Liste anzeigen möchten.<br><br>Beim Verkauf eines Artikels wird die Amazon-Liste mit der hier angegebenen Menge erneut veröffentlicht. Diese Einstellung wird normalerweise verwendet, wenn Sie das Produktinventar nicht verwalten.<br><br>Geben Sie z. B. den Wert für die aufgelistete Höchstmenge als `10`. Ihre tatsächliche Menge für ein Produkt ist `80`. weil Sie diesen Wert festgelegt haben auf `10`, zeigt die Amazon-Liste immer eine verfügbare Menge an `10`. Die verfügbare Menge wird immer mit dem definierten Wert angezeigt, auch wenn die Lagermenge niedriger ist. |
| [!UICONTROL "Do Not Manage Stock" Quantity] | Geben Sie einen Wert für die Anzeigemenge Ihrer Amazon-Auflistungen ein.<br><br>Amazon verlangt, dass Sie eine verfügbare Menge veröffentlichen. für [!DNL Commerce] Produkte, die nicht auf Lager zu verwalten, aber Sie möchten sie auf Amazon, die Liste wird mit der verfügbaren Menge des hier eingegebenen Wertes veröffentlicht. |

**Schnellzugriff** - [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)

## Beispiel: Höchstmenge der aufgeführten Menge

Wenn ein Artikel verkauft wird, wird es von der Amazon-Liste in dieser Menge erneut verwendet.

Wenn Sie z. B. *[!UICONTROL Maximum Listed Quantity]* als `12`, zeigt die Amazon-Liste eine Menge von 12, obwohl das Produkt [!DNL Commerce] Menge von 80:

![Beispiel für die angegebene Höchstmenge 1](assets/amazon-max-listed-quantity.png)

Wenn Sie *[!UICONTROL Maximum Listed Quantity]* als `1`werden alle in Betracht kommenden Erzeugnisse mit einer Menge von `1`. Wenn ein Artikel verkauft wird, sucht das System nach [!DNL Commerce] das Produkt und, falls zusätzliche Lagerbestände vorhanden sind, die Ware auf Amazon mit einer Menge `1`.

Diese Option kann bei Produkten nützlich sein, die üblicherweise in einer Menge von 1 bestellt werden. Es erhöht auch die Dringlichkeit für den Käufer, wenn Sie Ihre Amazon-Liste sehen.

![Beispiel für die angegebene Höchstmenge 2](assets/amazon-max-listed-quantity-1.png)
