---
title: Verwalten von Amazon-Bestellungen
description: Sie können den Bestellimport in Ihren Bestelleinstellungen aktivieren, um Ihre Amazon-Bestellungen einfacher über Ihren Commerce-Administrator zu verwalten.
feature: Sales Channels, Orders
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Verwalten von Amazon-Bestellungen

Sie können Ihre Amazon-Bestellinformationen, wie sie von Amazon erhalten wurden, im Bereich _[!UICONTROL Recent Orders]_des [Dashboard speichern](./amazon-store-dashboard.md) oder auf der Seite_[!UICONTROL Amazon orders]_ (auch als _[!UICONTROL All Orders]_-Ansicht bezeichnet) anzeigen.

Wie Sie Ihre Amazon-Bestellungen verwalten, hängt davon ab, ob der Bestellimport in Ihren [Bestelleinstellungen](./order-settings.md#configure-order-settings) aktiviert oder deaktiviert ist.

## Mit aktiviertem Bestellimport

Nach der [Speicherintegration](./store-integration.md) ist die Einstellung [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) standardmäßig auf `Enabled` eingestellt. Mit dieser Einstellung werden entsprechende [!DNL Commerce] Bestellungen für Ihre Amazon-Bestellungen erstellt und können im Workflow [[!DNL Commerce] Bestellungen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) verwaltet werden.

>[!NOTE]
>
>Unabhängig von Ihren Einstellungen für den Bestellimport werden Amazon-Bestellungen, die in Ihrem [!DNL Amazon Seller Central]-Konto vor Ihrer [Speicherintegration](./store-integration.md) bestanden, nicht importiert.

Importierte Amazon-Bestellungen werden im Workflow [[!DNL Commerce] Bestellungen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) verwaltet, genau wie Ihre anderen [!DNL Commerce] Stores. Klicken Sie in der Spalte *[!UICONTROL Order Number]* auf die Amazon-Bestellnummer, um die Bestellung im [[!DNL Commerce] Bestellprozess](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#order-view-descriptions) zu öffnen. Siehe [Anzeigen von Amazon-Bestellungen](./amazon-orders-all.md).

### Vorgang zum Bestellimport

Wenn eine Bestellung in Amazon aufgegeben und der [Bestellimport](./order-settings.md) aktiviert ist, beginnt der folgende Vorgang.

| Änderung | Aktionen |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Eine Bestellung wird auf Amazon aufgegeben. | <ul><li>Amazon legt den Bestellstatus auf `Pending` fest.</li><li>Bestellinformationen werden an [!DNL Commerce] gesendet.</li><li>Die Bestellung wird der Tabelle [_Amazon-Bestellungen_ mit dem Status `Pending` hinzugefügt.](./amazon-orders-all.md)</li></ul> |
| Amazon ändert den Bestellstatus in `Unshipped`. | <ul><li>Die Statusänderung wird an [!DNL Commerce] gesendet.</li><li>In der Tabelle [_Amazon-Bestellungen_](./amazon-orders-all.md) ändert sich der Bestellstatus in `Unshipped`.</li><li>Im Workflow [[!DNL Commerce] Bestellungen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) wird eine entsprechende [!DNL Commerce] Bestellung mit dem Status `Processing` erstellt.</li></ul> |
| In [[!DNL Commerce] Auftragsworkflow](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) wird die [!DNL Commerce] -Bestellung verarbeitet und der Status ändert sich in `Shipped`. | <ul><li>In der Tabelle [_Amazon-Bestellungen_](./amazon-orders-all.md) ändert sich der Bestellstatus in `Shipped`.</li><li>Beim nächsten Cron-Auftrag ändert sich der Auftragsstatus im [[!DNL Commerce] Auftrags-Workflow](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) in `Complete`.</li></ul> |

### Blocker zur Auftragserstellung

Es gibt einige Szenarien, die die Erstellung der entsprechenden [!DNL Commerce]-Reihenfolge verhindern. [!DNL Commerce] Bestellungen werden nicht für Bestellungen erstellt, die empfangen werden, wenn eines der folgenden Probleme auftritt.

| Szenario | Lösung |
|---------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Das Element ist nicht im [!DNL Commerce] -Katalog enthalten. | [Erstellen Sie das Produkt](./creating-assigning-catalog-products.md) in Ihrem [!DNL Commerce] -Katalog und passen Sie [es manuell mit](./creating-assigning-catalog-products.md) dem Produkt an. |
| Das Element im Katalog ist deaktiviert. | Stellen Sie sicher, dass der [Produktstatus](https://experienceleague.adobe.com/docs/commerce-admin/inventory/configuration/product-options.html) aktiviert ist. |
| Der bestellte Artikel ist nicht vorrätig. | Aktualisieren oder konfigurieren Sie die [Produktoptionen](https://experienceleague.adobe.com/docs/commerce-admin/inventory/configuration/product-options.html) für Menge und Quelle. |

Wenn Bestellungen nicht importiert werden können, wird oben auf dem Bildschirm eine Systemmeldung wie die folgende angezeigt:

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

Wenn das Problem behoben ist, wird die [!DNL Commerce]-Reihenfolge bei der nächsten Synchronisierung erstellt.

## Mit deaktiviertem Bestellimport

Wenn Sie Ihre Amazon-Bestellungen nicht in [!DNL Commerce] importieren und verwalten möchten, können Sie die Einstellung [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) auf `Disabled` ändern. Diese Einstellung bedeutet, dass bei Erhalt neuer Bestellungen von Amazon keine entsprechenden [!DNL Commerce] Bestellungen erstellt werden.

Wenn diese Option deaktiviert ist, werden die von Amazon erhaltenen Bestellinformationen im Abschnitt _[!UICONTROL Recent Orders]_des Store-Dashboards und in der Ansicht_[!UICONTROL All Orders]_ angezeigt. Diese Bestellinformationen sind schreibgeschützt und Sie müssen diese Bestellungen in [!DNL Amazon Seller Central] verwalten. Um die Bestelldetails in [!DNL Amazon Seller Central] zu öffnen, klicken Sie in der Spalte _[!UICONTROL Order Number]_auf die Amazon-Bestellnummer.

Siehe auch [Amazon-Bestellungen anzeigen](./amazon-orders-all.md), [Amazon-Bestelldetails anzeigen](./amazon-order-details.md) und [Allgemeine Auftragsverarbeitungsaufgaben](./common-order-processing.md).
