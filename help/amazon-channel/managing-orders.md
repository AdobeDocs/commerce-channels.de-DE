---
title: Verwalten von Amazon-Bestellungen
description: Sie können den Bestellimport in Ihren Bestelleinstellungen aktivieren, um Ihre Amazon-Bestellungen einfacher von Ihrem Commerce-Administrator aus zu verwalten.
feature: Sales Channels, Orders
exl-id: 018a8936-2f03-4a2d-b9af-6b72729ca709
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# Verwalten von Amazon-Bestellungen

Sie können Ihre Amazon-Bestellinformationen, wie sie von Amazon erhalten wurden, im _[!UICONTROL Recent Orders]_Abschnitt [Store-Dashboard](./amazon-store-dashboard.md) oder auf_[!UICONTROL Amazon orders]_ Seite (auch als _[!UICONTROL All Orders]_Ansicht).

Wie Sie Ihre Amazon-Bestellungen verwalten, hängt davon ab, ob der Bestellimport in Ihrer [Bestelleinstellungen](./order-settings.md#configure-order-settings).

## Mit aktiviertem Bestellimport

Nachher [Store-Integration](./store-integration.md), die [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) Einstellung ist `Enabled` Standardmäßig. Mit dieser Einstellung entspricht [!DNL Commerce] Bestellungen werden für Ihre Amazon-Bestellungen erstellt und können im [[!DNL Commerce] Bestellungen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) Arbeitsablauf.

>[!NOTE]
>
>Unabhängig von Ihren Einstellungen für den Bestellimport gibt es in Amazon Bestellungen, die in Ihrer [!DNL Amazon Seller Central] -Konto vor [Store-Integration](./store-integration.md) werden nicht importiert.

Importierte Amazon-Bestellungen werden im [[!DNL Commerce] Bestellungen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) Workflow, genau wie Ihre anderen [!DNL Commerce] Stores. Klicken Sie auf die Amazon-Bestellnummer im *[!UICONTROL Order Number]* -Spalte, um die Reihenfolge in der [[!DNL Commerce] Bestellprozess](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#order-view-descriptions). Siehe [Anzeigen von Amazon-Bestellungen](./amazon-orders-all.md).

### Vorgang zum Bestellimport

Wenn eine Bestellung in Amazon aufgegeben wird und [Bestellimport](./order-settings.md) aktiviert ist, beginnt der folgende Prozess.

| Änderung | Aktionen |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Eine Bestellung wird auf Amazon aufgegeben. | <ul><li>Amazon setzt den Bestellstatus auf `Pending`.</li><li>Bestellinformationen werden an [!DNL Commerce].</li><li>Bestellung wird hinzugefügt zu [_Amazon-Bestellungen_ table](./amazon-orders-all.md) mit `Pending` -Status.</li></ul> |
| Amazon ändert den Bestellstatus in `Unshipped`. | <ul><li>Die Statusänderung wird an [!DNL Commerce].</li><li>Im [_Amazon-Bestellungen_ table](./amazon-orders-all.md), ändert sich der Bestellstatus in `Unshipped`.</li><li>Im [[!DNL Commerce] Auftragsworkflow](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html), einer entsprechenden [!DNL Commerce] Die Bestellung wird mit einer `Processing` -Status.</li></ul> |
| In [[!DNL Commerce] Auftragsworkflow](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html), die [!DNL Commerce] Die Bestellung wird verarbeitet und der Status ändert sich in `Shipped`. | <ul><li>Im [_Amazon-Bestellungen_ table](./amazon-orders-all.md), ändert sich der Bestellstatus in `Shipped`.</li><li>Beim nächsten Cron-Auftrag ändert sich der Bestellstatus in `Complete` im [[!DNL Commerce] Auftragsworkflow](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html).</li></ul> |

### Blocker zur Auftragserstellung

Es gibt einige Szenarien, die die Erstellung der entsprechenden [!DNL Commerce] bestellen. [!DNL Commerce] Bestellungen werden nicht für Bestellungen erstellt, die empfangen werden, wenn eines der folgenden Probleme auftritt.

| Szenario | Lösung |
|---------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Das Element ist nicht im [!DNL Commerce] Katalog. | [Produkt erstellen](./creating-assigning-catalog-products.md) in [!DNL Commerce] Katalog und [manuell übereinstimmen](./creating-assigning-catalog-products.md) dem Produkt. |
| Das Element im Katalog ist deaktiviert. | Stellen Sie sicher, dass die Variable [Produktstatus](https://experienceleague.adobe.com/docs/commerce-admin/inventory/configuration/product-options.html) aktiviert ist. |
| Der bestellte Artikel ist nicht vorrätig. | Aktualisieren oder konfigurieren Sie die [Produktoptionen](https://experienceleague.adobe.com/docs/commerce-admin/inventory/configuration/product-options.html) für Menge und Quelle. |

Wenn Bestellungen nicht importiert werden können, wird oben auf dem Bildschirm eine Systemmeldung wie die folgende angezeigt:

`Your Amazon store(s) has orders that cannot be imported into [!DNL Commerce]. See Recent Orders in the store dashboard(s): <store name>`

Wenn das Problem behoben ist, wird die [!DNL Commerce] -Reihenfolge wird bei der nächsten Synchronisierung erstellt.

## Mit deaktiviertem Bestellimport

Wenn Sie Ihre Amazon-Bestellungen nicht in importieren und verwalten möchten [!DNL Commerce], können Sie die [**[!UICONTROL Import Amazon Orders]**](./order-settings.md#configure-order-settings) Einstellung auf `Disabled`. Diese Einstellung bedeutet, dass bei neuen Bestellungen von Amazon die entsprechende [!DNL Commerce] Bestellungen werden nicht erstellt.

Wenn diese Option deaktiviert ist, werden von Amazon empfangene Bestellinformationen im _[!UICONTROL Recent Orders]_im Store-Dashboard und im_[!UICONTROL All Orders]_ anzeigen. Diese Bestellinformationen sind schreibgeschützt und Sie müssen diese Bestellungen in [!DNL Amazon Seller Central]. So öffnen Sie die Bestelldetails in [!DNL Amazon Seller Central]Klicken Sie auf die Amazon-Bestellnummer im _[!UICONTROL Order Number]_Spalte.

Siehe auch [Anzeigen von Amazon-Bestellungen](./amazon-orders-all.md), [Amazon-Bestelldetails anzeigen](./amazon-order-details.md), und [Allgemeine Aufgaben zur Auftragsverarbeitung](./common-order-processing.md).
