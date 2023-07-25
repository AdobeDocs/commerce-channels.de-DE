---
title: Allgemeine Amazon-Auftragsverarbeitungsaufgaben
description: Verwenden Sie die entsprechende [!DNL Commerce] Bestellungen, die für Amazon-Bestellungen erstellt wurden, um die Bestellaktivität und -verarbeitung im [!UICONTROL Commerce] Admin.
feature: Sales Channels, Orders
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Allgemeine Amazon-Auftragsverarbeitungsaufgaben

[Verarbeitung von Commerce-Aufträgen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) Sie können Ihre Amazon-Bestellungen verwalten, einschließlich E-Mail an den Käufer, Erfüllung der Bestellung (Versand), Ausstellung von Gutschriften/Erstattungen, Hinzufügen von Kommentaren und mehr. Um Ihre Amazon-Bestellungen zu verwalten, benötigen Sie [**Importieren von Amazon-Bestellungen**](./order-settings.md) muss auf `Enabled` so, dass [!DNL Commerce] Bestellungen werden erstellt, wenn Amazon-Bestellungen empfangen werden. Amazon-Bestellinformationen werden im *[!UICONTROL Recent Orders]* des Store-Dashboards.

Wenn aktiviert, entspricht [!DNL Commerce] Bestellungen werden für Amazon-Bestellungen erstellt und die Amazon-Bestellnummer wird im _[!UICONTROL Order Number]_Spalte. Wenn eine [!DNL Commerce] -Bestellung erstellt wird, klicken Sie auf die Bestellnummer, um die Bestellung im [Verarbeitung von Commerce-Aufträgen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) Seite. Sie können die Bestellung so verwalten, wie Sie sie bei Ihren anderen [[!DNL Commerce] Bestellverarbeitung](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order).

Die [!DNL Commerce] Die Bestellnummer wird nicht mit der _[!UICONTROL Recent Orders]_Informationen. Die Commerce-Bestellnummer wird nur angezeigt, wenn Sie auf die Bestellnummer im Store-Dashboard klicken und die Bestellung in [Verarbeitung von Commerce-Aufträgen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order). Beim Anzeigen der [!DNL Commerce] -Reihenfolge, wird die Amazon-Bestellnummer in der *[!UICONTROL Payment & Shipping Method]*Abschnitt. Es enthält auch Optionen für *[!UICONTROL View or Cancel Amazon Order]*und *[!UICONTROL View all Amazon Orders]*, abhängig vom Versandstatus der Bestellung.

Siehe [unversandte Bestellung stornieren](./cancel-unshipped-order.md).

![Amazon-Bestellinformationen in Commerce-Reihenfolge](assets/amazon-order-number-payment-info.png){width="500"}

Bei der Verarbeitung einer Amazon-Bestellung aktualisiert und synchronisiert der Amazon-Vertriebskanal die Bestellinformationen mit Ihrem [!DNL Amazon Seller Central] -Konto. Ihre Cron-Einstellungen bestimmen, wie oft Bestellinformationen zwischen dem Amazon- und Amazon-Vertriebskanal synchronisiert werden.

Allgemeiner Handel [Bestellverarbeitung](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) Zu den Aufgaben gehören:

- [Bestellaktionen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#actions)
- [Bestellsuche](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#order-search)
- [Auftrag verarbeiten](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)
   - [Bestellung anzeigen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#view-an-order)
   - [Auftrag verarbeiten](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#process-an-order)
   - [Bestellungen und Kontoinformationen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#order-and-account-information)
   - [Adressinformationen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#address-information)
   - [Zahlungs- und Versandmethode](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#payment--shipping-method)
   - [Bestellte Elemente überprüfen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#review-items-ordered)
- [Gutschrift/Rückerstattung](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memo-create.html)
- [Auftrag ausführen/versenden](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/shipments.html#create-a-shipment)
- [Rechnung erstellen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/invoices.html#create-an-invoice)
- [Abbrechen einer nicht versandten Bestellung](./cancel-unshipped-order.md)

>[!NOTE]
>
>Wenn eine Bestellung in `Unshipped` Status, können Sie [Abbrechen einer Amazon-Bestellung](./cancel-unshipped-order.md) auf [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) Seite. Wenn eine Bestellung versandt wurde, kann sie nicht storniert werden.

Siehe [Commerce Order Management](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/introduction.html#order-management-and-operations).
