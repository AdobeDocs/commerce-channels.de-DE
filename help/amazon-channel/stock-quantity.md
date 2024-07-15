---
title: Amazon Sales Channel - [!UICONTROL Stock/Quantity]
description: Um die Synchronisierung der Produktmengendetails von Ihrem Commerce-Store mit Ihrem [!DNL Amazon Seller Central] Konto zu steuern, aktualisieren Sie die Einstellungen für Lager/Menge .
feature: Sales Channels, Inventory
exl-id: a8b7ab6c-393c-43c6-b5ef-68845177edff
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%

---

# [!UICONTROL Stock/Quantity]

*[!UICONTROL Stock/Quantity]* -Einstellungen sind Teil Ihrer Einstellungen für die Store-Auflistung. Auf die Listening-Einstellungen kann über das [Dashboard speichern](./amazon-store-dashboard.md) zugegriffen werden.

Diese Einstellungen werden verwendet, um die Details zur Produktmenge von Ihrer [!DNL Commerce] -Storefront mit der Menge in Ihrem [!DNL Amazon Seller Central] -Konto zu synchronisieren. Dieses Tool ist leistungsstark und kann für zusätzliche Werbung verwendet werden, indem es die Dringlichkeit für den Käufer zeigt und gleichzeitig Ihr Inventar organisiert. Einige Händler verfügen beispielsweise möglicherweise über 150 Artikel einer bestimmten SKU in ihrem Lager und möchten sicherstellen, dass Amazon-Käufer ihren gesamten Bestand erwerben können. Andere Händler möchten möglicherweise nur ein Element auf einmal auflisten, um dem Endbenutzer ein Gefühl der Verknappung zu erwecken. Setzen Sie in diesem Fall die *[!UICONTROL Maximum Listed Quantity]* auf `1`.

&quot;Quantity&quot;ist ein regionales Attribut und basiert auf der Einstellung **[!UICONTROL Amazon Marketplace Country]** , die während der [Store-Integration](./store-integration.md) definiert wird. Wenn die Menge eines Produkts geändert wird, wirkt sich die Änderung auf alle Amazon-Listen aus, die den Wert &quot;[!DNL Amazon Seller SKU]&quot;in Ihren Amazon-Stores verwenden, die im selben Land verkauft werden. Eine Änderung an einer freigegebenen [!DNL Amazon Seller SKU] in den USA wirkt sich nicht auf Ihre Amazon Stores aus, die für ein anderes Land eingerichtet sind. Ihr erster Amazon-Speicher, der integriert ist (mit dem ältesten Erstellungsdatum), steuert die Priorität in den Mengeneinstellungen.

>[!NOTE]
>
>Für Benutzer von Adobe Commerce und Magento Open Source 2.3.x unterstützt der Amazon-Vertriebskanal die Verwendung der Inventory management-Erweiterung ohne zusätzliche Einrichtung. Siehe [Verwalten des Bestands](https://docs.magento.com/user-guide/v2.3/catalog/inventory-management.html){target="_blank"}.

## Einstellungen für Lager/Menge konfigurieren {#configure-stock--quantity-settings}

1. Klicken Sie im Store-Dashboard auf **[!UICONTROL Listing Settings]** .

1. Erweitern Sie den Abschnitt **[!UICONTROL Stock / Quantity]** .

1. Geben Sie für &quot;**[!UICONTROL Out-of-Stock Threshold]**&quot;(erforderlich) einen numerischen Wert für die niedrigste Produktmenge ein, damit das Produkt für die Amazon-Liste infrage kommt.

   Der Standardwert ist `0`. Wenn Ihr [!DNL Commerce] -Produktbestand unter dieser Zahl liegt, ist die entsprechende Amazon-Auflistung nicht für den Vertrieb über Amazon geeignet.

1. Geben Sie für &quot;**[!UICONTROL Maximum Listed Quantity]**&quot;(erforderlich) einen numerischen Wert für die Menge ein, die Sie in Ihrer Amazon-Liste anzeigen möchten.

   Diese Einstellung listet alle Ihre zulässigen Amazon-Auflistungen zum eingegebenen Wert auf. Wenn ein Artikel verkauft wird, ändert sich die Amazon-Listenmenge nicht. Die verfügbare Auflistungsmenge verwendet immer diesen Wert, auch wenn Ihre tatsächliche Produktmenge höher oder niedriger ist. Diese Einstellung wird normalerweise verwendet, wenn Sie kein Produktinventar verwalten. Beispielsweise könnte ein Produkt mit einer Menge von 80 in Ihrem [!DNL Commerce] -Katalog enthalten sein. Mit dem Wert &quot;`10`&quot;zeigt die Amazon-Liste immer eine verfügbare Menge von &quot;`10`&quot;an und ändert sich nicht, wenn das Produkt verkauft wird.

1. Geben Sie für &quot;**[!UICONTROL "Do Not Manage Stock" Quantity]**&quot;(erforderlich) einen Mengenwert ein, der für Ihre Amazon-Auflistungen angezeigt werden soll.

   Amazon erfordert die Veröffentlichung einer verfügbaren Menge. Für [!DNL Commerce] -Produkte, die nicht für die Verwaltung von Lagern festgelegt sind, diese aber in Amazon auflisten möchten, wird die Liste mit der hier eingegebenen verfügbaren Menge veröffentlicht.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save listing settings]**.

![Einstellungen für Lager/Menge](assets/amazon-stock-quantity.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|---------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Out-of-Stock Threshold] | Geben Sie einen numerischen Wert für die niedrigste Produktmenge ein, damit das Produkt für die Amazon-Liste infrage kommt (der Standardwert ist `0`).<br><br>Wenn Ihr [!DNL Commerce] -Produktbestand unter dieser Zahl liegt, ist die entsprechende Amazon-Liste nicht für den Vertrieb über Amazon geeignet. |
| [!UICONTROL Maximum Listed Quantity] | Geben Sie einen numerischen Wert für die Menge ein, die in Ihrer Amazon-Liste angezeigt werden soll.<br><br>Wenn ein Artikel verkauft wird, wird die Amazon-Liste mit der hier eingegebenen Menge erneut veröffentlicht. Diese Einstellung wird normalerweise verwendet, wenn Sie kein Produktinventar verwalten.<br><br>Sie geben beispielsweise den Wert für die maximal aufgeführte Menge als `10` ein. Ihre tatsächliche Menge für ein Produkt ist `80`. Da Sie diesen Wert auf `10` festgelegt haben, zeigt die Amazon-Liste immer die verfügbare Menge `10` an. Die verfügbare Menge wird immer mit dem definierten Wert angezeigt, auch wenn die Lagermenge niedriger ist. |
| [!UICONTROL "Do Not Manage Stock" Quantity] | Geben Sie einen Wert für Ihre Anzeigemenge für Ihre Amazon-Auflistungen ein.<br><br>Amazon erfordert die Veröffentlichung einer verfügbaren Menge. Für [!DNL Commerce] -Produkte, die nicht für die Verwaltung von Lagern festgelegt sind, diese aber in Amazon auflisten möchten, wird die Liste mit der verfügbaren Menge des hier eingegebenen Werts veröffentlicht. |

**Schnellzugriff** - [!UICONTROL Listing Settings] Abschnitte

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

Wenn Sie beispielsweise &quot;*[!UICONTROL Maximum Listed Quantity]*&quot;auf &quot;`12`&quot;setzen, zeigt die Amazon-Liste eine Menge von 12 an, auch wenn das Produkt eine [!DNL Commerce] -Menge von 80 aufweist:

![Maximale aufgelistete Menge, Beispiel 1](assets/amazon-max-listed-quantity.png){width="300"}

Wenn Sie Ihren *[!UICONTROL Maximum Listed Quantity]* auf `1` setzen, werden alle infrage kommenden Produkte mit einer Menge von `1` aufgelistet. Wenn ein Artikel verkauft wird, sucht das System nach Ihrem [!DNL Commerce] -Produkt und setzt, falls ein zusätzliches Lager vorhanden ist, den Artikel auf Amazon mit einer Menge von `1` zurück.

Diese Option kann für Produkte nützlich sein, die normalerweise mit einer Menge von 1 bestellt werden. Darüber hinaus erhöht sich die Dringlichkeit für den Käufer, wenn er Ihre Amazon-Liste anzeigt.

![Beispiel für die maximal aufgelistete Menge 2](assets/amazon-max-listed-quantity-1.png){width="300"}
