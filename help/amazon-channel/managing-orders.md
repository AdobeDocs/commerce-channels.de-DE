---
title: Bestellungen verwalten
description: You can enable order import in your Order Settings to more easily manage your Amazon orders from your Commerce Admin.
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: 1d1b888db4de4f6e3658af768cd6f5cf30828788
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# Bestellungen verwalten

Sie können Ihre Amazon-Bestellinformationen, die Sie von Amazon erhalten haben, in der Ansicht _[!UICONTROL Recent Orders]_Abschnitt [Dashboard speichern](./amazon-store-dashboard.md) oder auf_[!UICONTROL Amazon orders]_ Seite (auch als _[!UICONTROL All Orders]_Ansicht).

Wie Sie Ihre Amazon-Bestellungen verwalten, hängt davon ab, ob der Auftragsimport in Ihrem [Auftragseinstellungen](./order-settings.md#configure-order-settings).

## Mit Bestellimport aktiviert

Nach [Speicherintegration](./store-integration.md), [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) Einstellung ist `Enabled` in der Standardeinstellung. Mit dieser Einstellung entspricht [!DNL Commerce] Bestellungen werden für Ihre Amazon-Bestellungen erstellt und können verwaltet werden im [[!DNL Commerce] Bestellungen](https://docs.magento.com/user-guide/sales/orders.html)Workflow für {Zielgruppe=&quot;_blank&quot;}.

>[!NOTE]
>
>Unabhängig von den Einstellungen für den Auftragsimport wurden Amazon-Bestellungen in Ihren [!DNL Amazon Seller Central] Konto vor [Speicherintegration](./store-integration.md) nicht importiert werden.

Imported Amazon orders are managed in the [[!DNL Commerce] Orders](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;} workflow, just like your other [!DNL Commerce] stores. Klicken Sie auf die Amazon-Bestellnummer im *[!UICONTROL Order Number]* -Spalte, um die Reihenfolge in [[!DNL Commerce] Bestellvorgang](https://docs.magento.com/user-guide/sales/order-processing.html#order-view-descriptions){Zielgruppe=&quot;_blank&quot;}. Siehe [Ansicht Amazon Bestellungen](./amazon-orders-all.md).

### Prozess für Auftragsimport

Wenn eine Bestellung auf Amazon und [Import bestellen](./order-settings.md) aktiviert ist, beginnt der folgende Prozess.

| Ändern | Aktionen |
|---|---|
| Eine Bestellung wird auf Amazon aufgegeben. | <ul><li>Amazon legt den Bestellstatus fest auf `Pending`.</li><li>Bestellinformationen werden gesendet an [!DNL Commerce].</li><li>Auftrag wird hinzugefügt zu [_Amazon-Aufträge_ Tabelle](./amazon-orders-all.md) mit `Pending` Status.</li></ul> |
| Amazon ändert den Bestellstatus in `Unshipped`. | <ul><li>The status change is sent to [!DNL Commerce].</li><li>In [_Amazon-Aufträge_ Tabelle](./amazon-orders-all.md), ändert sich der Bestellstatus in `Unshipped`.</li><li>In [[!DNL Commerce] Auftragsarbeitsablauf](https://docs.magento.com/user-guide/sales/orders.html){Zielgruppe=&quot;_blank&quot;}, entsprechende [!DNL Commerce] Auftrag wurde mit einem `Processing` Status.</li></ul> |
| In [[!DNL Commerce] Auftragsarbeitsablauf](https://docs.magento.com/user-guide/sales/orders.html){Zielgruppe=&quot;_blank&quot;}, die [!DNL Commerce] Auftrag wird verarbeitet und der Status ändert sich in `Shipped`. | <ul><li>In [_Amazon-Aufträge_ Tabelle](./amazon-orders-all.md), ändert sich der Bestellstatus in `Shipped`.</li><li>Beim nächsten Cron-Auftrag ändert sich der Auftragsstatus in `Complete` in [[!DNL Commerce] Auftragsarbeitsablauf](https://docs.magento.com/user-guide/sales/orders.html){Zielgruppe=&quot;_blank&quot;}.</li></ul> |

### Blocker für Auftragserstellung

Es gibt einige Szenarios, die die Erstellung der entsprechenden [!DNL Commerce] bestellen. [!DNL Commerce] Bestellungen werden nicht für Bestellungen erstellt, die empfangen werden, wenn eines der folgenden Probleme auftritt.

| Szenario | Lösung |
|---|---|
| Das Element ist nicht im [!DNL Commerce] Katalog. | [Produkt erstellen](./creating-assigning-catalog-products.md) in [!DNL Commerce] Katalog und [Manuell übereinstimmen](./creating-assigning-catalog-products.md) dem Produkt. |
| Das Element im Katalog ist deaktiviert. | Vergewissern Sie sich, dass [Produktstatus](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){Zielgruppe=&quot;_blank&quot;} ist aktiviert. |
| The ordered item is out of stock. | Aktualisieren oder konfigurieren Sie [Produktoptionen](https://docs.magento.com/user-guide/catalog/inventory-product-stock-options.html){Zielgruppe=&quot;_blank&quot;} für Menge und Quelle. |

Wenn Bestellungen nicht importiert werden können, wird oben auf dem Bildschirm eine Systemnachricht ähnlich der folgenden angezeigt:

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

Wenn das Problem behoben ist, [!DNL Commerce] Reihenfolge wird bei der nächsten Synchronisierung erstellt.

## Mit Bestellimport deaktiviert

Wenn Sie Ihre Amazon-Bestellungen nicht importieren und verwalten möchten [!DNL Commerce], können Sie [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) Einstellung auf `Disabled`. Diese Einstellung bedeutet, dass bei neuen Bestellungen von Amazon entsprechende [!DNL Commerce] Bestellungen werden nicht erstellt.

Wenn deaktiviert, werden die von Amazon erhaltenen Bestellinformationen im _[!UICONTROL Recent Orders]_des Dashboards und_[!UICONTROL All Orders]_ Ansicht. Diese Bestellinformationen sind nur für Ansichten verfügbar. Sie müssen diese Bestellungen verwalten in [!DNL Amazon Seller Central]. So öffnen Sie die Auftragsdetails unter [!DNL Amazon Seller Central]Klicken Sie auf die Amazon-Bestellnummer in der _[!UICONTROL Order Number]_Spalte.

Siehe auch [Ansicht Amazon Bestellungen](./amazon-orders-all.md), [Ansicht Amazon Auftragsdetails](./amazon-order-details.md)und [Allgemeine Aufgaben zur Auftragsverarbeitung](./common-order-processing.md).
