---
title: Allgemeine Amazon-Auftragsverarbeitungsaufgaben
description: Verwenden Sie die entsprechenden [!DNL Commerce] Bestellungen, die für Amazon-Bestellungen erstellt wurden, um die Bestellaktivität und -verarbeitung im [!UICONTROL Commerce] -Admin zu verwalten.
feature: Sales Channels, Orders
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Allgemeine Amazon-Auftragsverarbeitungsaufgaben

[Commerce-Auftragsverarbeitung](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) kann Ihre Amazon-Bestellungen verwalten, einschließlich der E-Mail-Versendung an den Käufer, der Erfüllung der Bestellung (Versand), der Ausstellung von Gutschriften/Erstattungen, der Hinzufügung von Kommentaren und mehr. Um Ihre Amazon-Bestellungen zu verwalten, muss die Einstellung [**Amazon-Bestellungen importieren**](./order-settings.md) auf `Enabled` gesetzt werden, damit die entsprechenden [!DNL Commerce] Bestellungen erstellt werden, wenn Amazon-Bestellungen empfangen werden. Amazon-Bestellinformationen werden im Abschnitt *[!UICONTROL Recent Orders]* des Store-Dashboards angezeigt.

Wenn diese Option aktiviert ist, werden entsprechende [!DNL Commerce] Bestellungen für Amazon-Bestellungen erstellt und die Amazon-Bestellnummer wird in der Spalte _[!UICONTROL Order Number]_angezeigt. Wenn eine entsprechende [!DNL Commerce] -Bestellung erstellt wird, klicken Sie auf die Bestellnummer, um die Bestellung auf der Seite [Commerce order processing](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) zu öffnen. Sie können die Reihenfolge so verwalten wie Ihre anderen [[!DNL Commerce] Bestellvorgänge](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order).

Die [!DNL Commerce] Bestellnummer wird nicht mit den _[!UICONTROL Recent Orders]_-Informationen angezeigt. Die Commerce-Bestellnummer wird nur angezeigt, wenn Sie auf die Bestellnummer im Store-Dashboard klicken und die Bestellung in [Commerce order processing](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) öffnen. Bei Ansicht der Bestellung [!DNL Commerce] wird die Amazon-Bestellnummer im Abschnitt *[!UICONTROL Payment & Shipping Method]*angezeigt. Je nach Versandstatus der Bestellung enthält es auch Optionen für *[!UICONTROL View or Cancel Amazon Order]*und *[!UICONTROL View all Amazon Orders]*.

Siehe [Abbrechen einer nicht versandten Bestellung](./cancel-unshipped-order.md).

![Amazon-Bestellinformationen in Commerce-Reihenfolge](assets/amazon-order-number-payment-info.png){width="500"}

Bei der Verarbeitung einer Amazon-Bestellung aktualisiert und synchronisiert der Amazon-Vertriebskanal die Bestellinformationen mit Ihrem [!DNL Amazon Seller Central] -Konto. Ihre Cron-Einstellungen bestimmen, wie oft Bestellinformationen zwischen dem Amazon- und Amazon-Vertriebskanal synchronisiert werden.

Zu den gängigen Aufgaben für die Commerce [Bestellverarbeitung](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order) gehören:

- [Bestellaktionen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#actions)
- [Bestellsuche](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#order-search)
- [Verarbeiten einer Bestellung](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order)
   - [Eine Bestellung anzeigen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#view-an-order)
   - [Verarbeiten einer Bestellung](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#process-an-order)
   - [Bestellungen und Kontoinformationen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#order-and-account-information)
   - [Adressinformationen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#address-information)
   - [Zahlungs- und Versandmethode](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#payment--shipping-method)
   - [Überprüfen der bestellten Elemente](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-processing.html#process-an-order#review-items-ordered)
- [Gutschrift/Rückerstattung vornehmen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memo-create.html)
- [Erfüllen/Versenden einer Bestellung](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/shipments.html#create-a-shipment)
- [Erstellen einer Rechnung](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/invoices.html#create-an-invoice)
- [Abbrechen einer nicht versandten Bestellung](./cancel-unshipped-order.md)

>[!NOTE]
>
>Wenn eine Bestellung den Status `Unshipped` aufweist, können Sie [eine Amazon-Bestellung abbrechen](./cancel-unshipped-order.md) auf der Seite [[!UICONTROL Amazon Order Details]](./amazon-order-details.md). Wenn eine Bestellung versandt wurde, kann sie nicht storniert werden.

Siehe [Commerce Order Management](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/introduction.html#order-management-and-operations).
