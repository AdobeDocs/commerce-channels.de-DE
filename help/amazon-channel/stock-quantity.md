---
title: Lager/Menge
description: 'Um die Synchronisierung der Produktmengendetails von Ihrem Commerce-Store mit Ihrem [!DNL Amazon Seller Central] Konto zu steuern, aktualisieren Sie die Einstellungen für Lager/Menge .'
redirect_from: /sales-channels/asc/ob-stock-quantity.html: 
exl-id: a8b7ab6c-393c-43c6-b5ef-68845177edff
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: 771
ht-degree: 0%

---

# Lager/Menge

*[!UICONTROL Stock/Quantity]* -Einstellungen sind Teil Ihrer Einstellungen für die Store-Auflistung. Auf die Listening-Einstellungen kann über das [Store-Dashboard](./amazon-store-dashboard.md) zugegriffen werden.

Diese Einstellungen werden verwendet, um die Produktmengendetails von Ihrer [!DNL Commerce] Storefront mit der Menge in Ihrem [!DNL Amazon Seller Central]-Konto zu synchronisieren. Dieses Tool ist leistungsstark und kann für zusätzliche Werbung verwendet werden, indem es die Dringlichkeit für den Käufer zeigt und gleichzeitig Ihr Inventar organisiert. Einige Händler verfügen beispielsweise möglicherweise über 150 Artikel einer bestimmten SKU in ihrem Lager und möchten sicherstellen, dass Amazon-Käufer ihren gesamten Bestand erwerben können. Andere Händler möchten möglicherweise nur ein Element auf einmal auflisten, um dem Endbenutzer ein Gefühl der Verknappung zu erwecken. Setzen Sie in diesem Fall *[!UICONTROL Maximum Listed Quantity]* auf `1`.

&quot;Quantity&quot;ist ein regionales Attribut und basiert auf der Einstellung **[!UICONTROL Amazon Marketplace Country]** , die während der [Store-Integration](./store-integration.md) definiert wird. Wenn die Produktmenge geändert wird, wirkt sich die Änderung auf alle Amazon-Listen aus, die [!DNL Amazon Seller SKU] in Ihren Amazon-Stores verwenden, die im selben Land verkauft werden. Eine Änderung an einem freigegebenen [!DNL Amazon Seller SKU] in den USA wirkt sich nicht auf Ihre Amazon Stores aus, die für ein anderes Land eingerichtet sind. Ihr erster Amazon-Speicher, der integriert ist (mit dem ältesten Erstellungsdatum), steuert die Priorität in den Mengeneinstellungen.

>[!NOTE]
>
>Für Adobe Commerce- und Magento Open Source 2.3.x-Benutzer unterstützt der Amazon-Vertriebskanal die Verwendung der Erweiterung &quot;Lagerbestandsverwaltung&quot;ohne zusätzliche Einrichtung. Siehe [Verwalten des Bestands](https://docs.magento.com/user-guide/v2.3/catalog/inventory-management.html){:target=&quot;_blank&quot;}.

## Einstellungen für Lager/Menge konfigurieren {#configure-stock--quantity-settings}

1. Klicken Sie im Store-Dashboard auf **[!UICONTROL Listing Settings]** .

1. Erweitern Sie den Abschnitt **[!UICONTROL Stock / Quantity]** .

1. Geben Sie für **[!UICONTROL Out-of-Stock Threshold]** (erforderlich) einen numerischen Wert für die niedrigste Produktmenge ein, damit das Produkt für die Amazon-Liste infrage kommt.

   Der Standardwert ist `0`. Wenn Ihr [!DNL Commerce]-Produktbestand unter dieser Zahl liegt, kann die entsprechende Amazon-Auflistung über Amazon nicht verkauft werden.

1. Geben Sie für **[!UICONTROL Maximum Listed Quantity]** (erforderlich) einen numerischen Wert für die Menge ein, die Sie in Ihrer Amazon-Liste anzeigen möchten.

   Diese Einstellung listet alle Ihre zulässigen Amazon-Auflistungen zum eingegebenen Wert auf. Wenn ein Artikel verkauft wird, ändert sich die Amazon-Listenmenge nicht. Die verfügbare Auflistungsmenge verwendet immer diesen Wert, auch wenn Ihre tatsächliche Produktmenge höher oder niedriger ist. Diese Einstellung wird normalerweise verwendet, wenn Sie kein Produktinventar verwalten. Beispielsweise könnte ein Produkt mit einer Menge von 80 in Ihrem [!DNL Commerce] -Katalog enthalten sein. Mit dem Wert `10` zeigt die Amazon-Liste immer die verfügbare Menge `10` an und ändert sich nicht, wenn das Produkt verkauft wird.

1. Geben Sie für **[!UICONTROL "Do Not Manage Stock" Quantity]** (erforderlich) einen Mengenwert ein, der für Ihre Amazon-Auflistungen angezeigt werden soll.

   Amazon erfordert die Veröffentlichung einer verfügbaren Menge. Für [!DNL Commerce] -Produkte, die nicht für die Verwaltung von Lagern festgelegt sind, aber sie in Amazon auflisten möchten, wird die Liste mit der hier eingegebenen verfügbaren Menge veröffentlicht.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save listing settings]**.

![Einstellungen für Lager/Menge](assets/amazon-stock-quantity.png)

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Out-of-Stock Threshold] | Geben Sie einen numerischen Wert für die niedrigste Produktmenge ein, damit das Produkt für die Amazon-Liste infrage kommt (Standard ist `0`).<br><br>Wenn Ihr  [!DNL Commerce] Produktbestand unter dieser Zahl liegt, kann die entsprechende Amazon-Auflistung über Amazon nicht verkauft werden. |
| [!UICONTROL Maximum Listed Quantity] | Geben Sie einen numerischen Wert für die Menge ein, die in Ihrer Amazon-Liste angezeigt werden soll.<br><br>Wenn ein Artikel verkauft wird, wird die Amazon-Liste mit der hier eingegebenen Menge erneut veröffentlicht. Diese Einstellung wird normalerweise verwendet, wenn Sie kein Produktinventar verwalten.<br><br>Geben Sie beispielsweise den Wert &quot;Maximal aufgelistete Menge&quot;als  `10` ein. Ihre tatsächliche Menge für ein Produkt ist `80`. Da Sie diesen Wert auf `10` festgelegt haben, zeigt die Amazon-Liste immer die verfügbare Menge `10` an. Die verfügbare Menge wird immer mit dem definierten Wert angezeigt, auch wenn die Lagermenge niedriger ist. |
| [!UICONTROL "Do Not Manage Stock" Quantity] | Geben Sie einen Wert für Ihre Anzeigemenge für Ihre Amazon-Auflistungen ein.<br><br>Amazon erfordert die Veröffentlichung einer verfügbaren Menge. Für [!DNL Commerce] -Produkte, die nicht für die Verwaltung von Lagern festgelegt sind, aber sie in Amazon auflisten möchten, wird die Liste mit der verfügbaren Menge des hier eingegebenen Werts veröffentlicht. |

**Schnellzugriff**  -  [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)

## Beispiel: Maximale angegebene Menge

Wenn ein Artikel verkauft wird, wird er von der Amazon-Auflistung auf diese Menge angewiesen.

Wenn Sie beispielsweise *[!UICONTROL Maximum Listed Quantity]* auf `12` setzen, zeigt die Amazon-Liste eine Menge von 12 an, obwohl das Produkt eine Menge von [!DNL Commerce] von 80 aufweist:

![Beispiel für die angegebene Höchstmenge 1](assets/amazon-max-listed-quantity.png)

Wenn Sie *[!UICONTROL Maximum Listed Quantity]* auf `1` setzen, werden alle infrage kommenden Produkte mit einer Menge `1` aufgelistet. Wenn ein Artikel verkauft wird, sucht das System nach Ihrem [!DNL Commerce]-Produkt und setzt, falls ein zusätzliches Lager vorhanden ist, den Artikel auf Amazon mit einer Menge von `1` erneut.

Diese Option kann für Produkte nützlich sein, die normalerweise mit einer Menge von 1 bestellt werden. Darüber hinaus erhöht sich die Dringlichkeit für den Käufer, wenn er Ihre Amazon-Liste anzeigt.

![Beispiel für die angegebene Höchstmenge 2](assets/amazon-max-listed-quantity-1.png)
