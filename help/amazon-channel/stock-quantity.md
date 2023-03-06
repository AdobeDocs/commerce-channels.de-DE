---
title: Lager/Menge
description: So steuern Sie die Synchronisierung der Produktmengendetails von Ihrem Commerce-Store mit Ihrem [!DNL Amazon Seller Central] -Konto die Einstellungen für Lager/Menge aktualisieren.
redirect_from: /sales-channels/asc/ob-stock-quantity.html
exl-id: a8b7ab6c-393c-43c6-b5ef-68845177edff
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%

---

# Lager/Menge

*[!UICONTROL Stock/Quantity]* -Einstellungen sind Teil Ihrer Einstellungen für die Store-Auflistung. Auf die Listening-Einstellungen kann über die [Store-Dashboard](./amazon-store-dashboard.md).

Diese Einstellungen werden verwendet, um die Produktmengendetails von Ihren [!DNL Commerce] Storefront zur Menge auf [!DNL Amazon Seller Central] -Konto. Dieses Tool ist leistungsstark und kann für zusätzliche Werbung verwendet werden, indem es die Dringlichkeit für den Käufer zeigt und gleichzeitig Ihr Inventar organisiert. Einige Händler verfügen beispielsweise möglicherweise über 150 Artikel einer bestimmten SKU in ihrem Lager und möchten sicherstellen, dass Amazon-Käufer ihren gesamten Bestand erwerben können. Andere Händler möchten möglicherweise nur ein Element auf einmal auflisten, um dem Endbenutzer ein Gefühl der Verknappung zu erwecken. Legen Sie in diesem Fall die *[!UICONTROL Maximum Listed Quantity]* nach `1`.

&quot;Menge&quot;ist ein regionales Attribut und basiert auf der **[!UICONTROL Amazon Marketplace Country]** festlegen während [Store-Integration](./store-integration.md). Wenn eine Änderung an der Menge eines Produkts vorgenommen wird, wirkt sich die Änderung auf alle Amazon-Listen aus, die diese [!DNL Amazon Seller SKU] in Ihren Amazon-Geschäften, die im selben Land verkauft werden. Änderung an freigegebenen [!DNL Amazon Seller SKU] in den USA betrifft nicht Ihre Amazon-Stores, die für ein anderes Land eingerichtet sind. Ihr erster Amazon-Speicher, der integriert ist (mit dem ältesten Erstellungsdatum), steuert die Priorität in den Mengeneinstellungen.

>[!NOTE]
>
>Für Benutzer von Adobe Commerce und Magento Open Source 2.3.x unterstützt der Amazon-Vertriebskanal die Verwendung der Inventory management-Erweiterung ohne zusätzliche Einrichtung. Siehe [Verwalten des Bestands](https://docs.magento.com/user-guide/v2.3/catalog/inventory-management.html){target="_blank"}.

## Einstellungen für Lager/Menge konfigurieren {#configure-stock--quantity-settings}

1. Klicken **[!UICONTROL Listing Settings]** im Dashboard speichern.

1. Erweitern Sie die **[!UICONTROL Stock / Quantity]** Abschnitt.

1. Für **[!UICONTROL Out-of-Stock Threshold]** (erforderlich) einen numerischen Wert für die niedrigste Menge eines Erzeugnisses eingeben, damit das Erzeugnis für die Amazon-Liste in Frage kommt.

   Der Standardwert ist `0`. Wenn [!DNL Commerce] Der Produktbestand liegt unter dieser Zahl, die entsprechende Amazon-Auflistung ist nicht für den Vertrieb über Amazon geeignet.

1. Für **[!UICONTROL Maximum Listed Quantity]** (erforderlich), geben Sie einen numerischen Wert für die Menge ein, die Sie in Ihrer Amazon-Liste anzeigen möchten.

   Diese Einstellung listet alle Ihre zulässigen Amazon-Auflistungen zum eingegebenen Wert auf. Wenn ein Artikel verkauft wird, ändert sich die Amazon-Listenmenge nicht. Die verfügbare Auflistungsmenge verwendet immer diesen Wert, auch wenn Ihre tatsächliche Produktmenge höher oder niedriger ist. Diese Einstellung wird normalerweise verwendet, wenn Sie kein Produktinventar verwalten. Sie können beispielsweise ein Produkt mit einer Menge von 80 in Ihrer [!DNL Commerce] Katalog. Mit festgelegt auf `10`, zeigt die Amazon-Liste immer eine verfügbare Menge an `10` und ändert sich nicht, wenn der Verkauf für das Produkt erfolgt.

1. Für **[!UICONTROL "Do Not Manage Stock" Quantity]** (erforderlich), geben Sie einen Mengenwert ein, der für Ihre Amazon-Auflistungen angezeigt werden soll.

   Amazon erfordert die Veröffentlichung einer verfügbaren Menge. Für [!DNL Commerce] Produkte, die nicht auf Lager verwalten eingestellt sind, aber sie in Amazon auflisten möchten, wird die Liste mit der hier eingegebenen verfügbaren Menge veröffentlicht.

1. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Save listing settings]**.

![Einstellungen für Lager/Menge](assets/amazon-stock-quantity.png)

| Feld | Beschreibung |
|---|---|
| [!UICONTROL Out-of-Stock Threshold] | Geben Sie einen numerischen Wert für die niedrigste Produktmenge ein, um das Produkt für die Amazon-Auflistung in Frage zu stellen (Standard ist `0`).<br><br>Wenn [!DNL Commerce] Der Produktbestand liegt unter dieser Zahl, die entsprechende Amazon-Auflistung ist nicht für den Vertrieb über Amazon geeignet. |
| [!UICONTROL Maximum Listed Quantity] | Geben Sie einen numerischen Wert für die Menge ein, die in Ihrer Amazon-Liste angezeigt werden soll.<br><br>Wenn ein Artikel verkauft wird, wird die Amazon-Liste mit der hier eingegebenen Menge erneut veröffentlicht. Diese Einstellung wird normalerweise verwendet, wenn Sie kein Produktinventar verwalten.<br><br>Geben Sie beispielsweise den Wert für die maximal aufgeführte Menge als `10`. Ihre tatsächliche Menge für ein Produkt ist `80`. Da Sie diesen Wert auf `10`, zeigt die Amazon-Liste immer eine verfügbare Menge an `10`. Die verfügbare Menge wird immer mit dem definierten Wert angezeigt, auch wenn die Lagermenge niedriger ist. |
| [!UICONTROL "Do Not Manage Stock" Quantity] | Geben Sie einen Wert für Ihre Anzeigemenge für Ihre Amazon-Auflistungen ein.<br><br>Amazon erfordert die Veröffentlichung einer verfügbaren Menge. Für [!DNL Commerce] Produkte, die nicht für die Verwaltung von Lagern festgelegt sind, aber Sie sie in Amazon auflisten möchten, wird die Liste mit der verfügbaren Menge des hier eingegebenen Werts veröffentlicht. |

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

Wenn Sie beispielsweise *[!UICONTROL Maximum Listed Quantity]* as `12`, zeigt die Amazon-Liste eine Menge von 12 an, obwohl das Produkt über eine [!DNL Commerce] Menge 80:

![Beispiel für die angegebene Höchstmenge 1](assets/amazon-max-listed-quantity.png)

Wenn Sie *[!UICONTROL Maximum Listed Quantity]* as `1`alle in Betracht kommenden Erzeugnisse mit einer Menge von `1`. Wenn ein Artikel verkauft wird, prüft das System Ihre [!DNL Commerce] -Produkt und, falls ein zusätzliches Lager vorhanden ist, benötigt das Element auf Amazon eine Menge von `1`.

Diese Option kann für Produkte nützlich sein, die normalerweise mit einer Menge von 1 bestellt werden. Darüber hinaus erhöht sich die Dringlichkeit für den Käufer, wenn er Ihre Amazon-Liste anzeigt.

![Beispiel für die angegebene Höchstmenge 2](assets/amazon-max-listed-quantity-1.png)
