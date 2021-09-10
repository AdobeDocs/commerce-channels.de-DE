---
title: Bestellungen verwalten
description: Sie können den Bestellimport in Ihren Bestelleinstellungen aktivieren, um Ihre Amazon-Bestellungen einfacher von Ihrem Commerce-Administrator aus zu verwalten.
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# Bestellungen verwalten

Sie können Ihre Amazon-Bestellinformationen, wie sie von Amazon erhalten wurden, im Abschnitt _[!UICONTROL Recent Orders]_des [Dashboard speichern](./amazon-store-dashboard.md) oder auf der Seite_[!UICONTROL Amazon orders]_ (auch _[!UICONTROL All Orders]_-Ansicht genannt) anzeigen.

Wie Sie Ihre Amazon-Bestellungen verwalten, hängt davon ab, ob der Bestellimport in [Bestelleinstellungen](./order-settings.md#configure-order-settings) aktiviert oder deaktiviert ist.

## Mit aktiviertem Bestellimport

Nach [Store-Integration](./store-integration.md) ist die Einstellung [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) standardmäßig `Enabled`. Mit dieser Einstellung werden die entsprechenden [!DNL Commerce]-Bestellungen für Ihre Amazon-Bestellungen erstellt und können im Workflow [[!DNL Commerce] Bestellungen](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;} verwaltet werden.

>[!NOTE]
>
>Unabhängig von Ihren Einstellungen für den Bestellimport werden Amazon-Bestellungen, die in Ihrem [!DNL Amazon Seller Central]-Konto vor der [Store-Integration](./store-integration.md) vorhanden waren, nicht importiert.

Importierte Amazon-Bestellungen werden im Workflow [[!DNL Commerce] Bestellungen](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;} verwaltet, genau wie Ihre anderen [!DNL Commerce] Stores. Klicken Sie in der Spalte *[!UICONTROL Order Number]* auf die Amazon-Bestellnummer, um die Bestellung im Ordner [[!DNL Commerce] Bestellprozess](https://docs.magento.com/user-guide/sales/order-processing.html#order-view-descriptions){target=&quot;_blank&quot;} zu öffnen. Siehe [Amazon-Bestellungen anzeigen](./amazon-orders-all.md).

### Vorgang zum Bestellimport

Wenn eine Bestellung in Amazon aufgegeben und [Bestellimport](./order-settings.md) aktiviert ist, beginnt der folgende Vorgang.

| Änderung | Aktionen |
|---|---|
| Eine Bestellung wird auf Amazon aufgegeben. | <ul><li>Amazon legt den Bestellstatus auf `Pending` fest.</li><li>Bestellinformationen werden an [!DNL Commerce] gesendet.</li><li>Die Bestellung wird der Tabelle [_Amazon-Bestellungen_](./amazon-orders-all.md) mit dem Status `Pending` hinzugefügt.</li></ul> |
| Amazon ändert den Bestellstatus in `Unshipped`. | <ul><li>Die Statusänderung wird an [!DNL Commerce] gesendet.</li><li>In der Tabelle [_Amazon-Bestellungen_](./amazon-orders-all.md) ändert sich der Auftragsstatus in `Unshipped`.</li><li>Im [[!DNL Commerce] Auftrags-Workflow](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;} wird eine entsprechende [!DNL Commerce]-Bestellung mit dem Status `Processing` erstellt.</li></ul> |
| In [[!DNL Commerce] order workflow](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;} wird die [!DNL Commerce]-Bestellung verarbeitet und der Status ändert sich in `Shipped`. | <ul><li>In der Tabelle [_Amazon-Bestellungen_](./amazon-orders-all.md) ändert sich der Auftragsstatus in `Shipped`.</li><li>Beim nächsten Cron-Auftrag ändert sich der Auftragsstatus in `Complete` im [[!DNL Commerce] Auftrags-Workflow](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}.</li></ul> |

### Blocker zur Auftragserstellung

Es gibt einige Szenarien, die die Erstellung der entsprechenden [!DNL Commerce]-Bestellung verhindern. [!DNL Commerce] Bestellungen werden nicht für Bestellungen erstellt, die empfangen werden, wenn eines der folgenden Probleme auftritt.

| Szenario | Lösung |
|---|---|
| Das Element ist im Katalog [!DNL Commerce] nicht vorhanden. | [Erstellen Sie die ](./creating-assigning-catalog-products.md) Produktion in Ihrem  [!DNL Commerce] Katalog und passen Sie sie  [manuell ](./creating-assigning-catalog-products.md) an das Produkt an. |
| Das Element im Katalog ist deaktiviert. | Stellen Sie sicher, dass der [Produktstatus](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){:target=&quot;_blank&quot;} aktiviert ist. |
| Der bestellte Artikel ist nicht vorrätig. | Aktualisieren oder konfigurieren Sie die [Produktoptionen](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){:target=&quot;_blank&quot;} für Menge und Quelle. |

Wenn Bestellungen nicht importiert werden können, wird oben auf dem Bildschirm eine Systemmeldung wie die folgende angezeigt:

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

Wenn das Problem behoben ist, wird die [!DNL Commerce]-Reihenfolge bei der nächsten Synchronisierung erstellt.

## Mit deaktiviertem Bestellimport

Wenn Sie Ihre Amazon-Bestellungen nicht in [!DNL Commerce] importieren und verwalten möchten, können Sie die Einstellung [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) in `Disabled` ändern. Diese Einstellung bedeutet, dass bei Erhalt neuer Bestellungen von Amazon keine entsprechenden [!DNL Commerce] Bestellungen erstellt werden.

Wenn diese Option deaktiviert ist, werden die von Amazon erhaltenen Bestellinformationen im Abschnitt _[!UICONTROL Recent Orders]_des Store-Dashboards und in der Ansicht_[!UICONTROL All Orders]_ angezeigt. Diese Bestellinformationen sind schreibgeschützt und Sie müssen diese Bestellungen in [!DNL Amazon Seller Central] verwalten. Um die Bestelldetails in [!DNL Amazon Seller Central] zu öffnen, klicken Sie in der Spalte _[!UICONTROL Order Number]_auf die Amazon-Bestellnummer.

Siehe auch [Amazon-Bestellungen anzeigen](./amazon-orders-all.md), [Amazon-Bestelldetails anzeigen](./amazon-order-details.md) und [Allgemeine Auftragsverarbeitungsaufgaben](./common-order-processing.md).
