---
title: Allgemeine Aufgaben zur Auftragsverarbeitung
description: Verwenden Sie die entsprechende [!DNL Commerce] Bestellungen, die für Amazon-Bestellungen erstellt wurden, um die Bestellaktivität und -verarbeitung im [!UICONTROL Commerce] Admin.
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Allgemeine Aufgaben zur Auftragsverarbeitung

[[!DNL Commerce] Bestellverarbeitung](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"} Sie können Ihre Amazon-Bestellungen verwalten, einschließlich E-Mail an den Käufer, Erfüllung der Bestellung (Versand), Ausstellung von Gutschriften/Erstattungen, Hinzufügen von Kommentaren und mehr. Um Ihre Amazon-Bestellungen zu verwalten, benötigen Sie [**Importieren von Amazon-Bestellungen**](./order-settings.md) muss auf `Enabled` so, dass [!DNL Commerce] Bestellungen werden erstellt, wenn Amazon-Bestellungen empfangen werden. Amazon-Bestellinformationen werden im *[!UICONTROL Recent Orders]* des Store-Dashboards.

Wenn aktiviert, entspricht [!DNL Commerce] Bestellungen werden für Amazon-Bestellungen erstellt und die Amazon-Bestellnummer wird im _[!UICONTROL Order Number]_Spalte. Wenn eine [!DNL Commerce] -Bestellung erstellt wird, klicken Sie auf die Bestellnummer, um die Bestellung im [!DNL Commerce] [Bestellverarbeitung](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"} page. You can manage the order as you do your other [[!DNL Commerce] order processing](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"}.

Die [!DNL Commerce] Die Bestellnummer wird nicht mit der _[!UICONTROL Recent Orders]_Informationen. Die [!DNL Commerce] Die Bestellnummer wird nur angezeigt, wenn Sie auf die Bestellnummer im Store-Dashboard klicken und die Bestellung in [[!DNL Commerce] Bestellverarbeitung](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"}. Beim Anzeigen der [!DNL Commerce] -Reihenfolge, wird die Amazon-Bestellnummer in der *[!UICONTROL Payment & Shipping Method]*Abschnitt. Es enthält auch Optionen für *[!UICONTROL View or Cancel Amazon Order]*und *[!UICONTROL View all Amazon Orders]*, abhängig vom Versandstatus der Bestellung.

Siehe [unversandte Bestellung stornieren](./cancel-unshipped-order.md).

![Amazon-Bestellinformationen in Commerce-Reihenfolge](assets/amazon-order-number-payment-info.png)

Bei der Verarbeitung einer Amazon-Bestellung aktualisiert und synchronisiert der Amazon-Vertriebskanal die Bestellinformationen mit Ihrem [!DNL Amazon Seller Central] -Konto. Ihre Cron-Einstellungen bestimmen, wie oft Bestellinformationen zwischen dem Amazon- und Amazon-Vertriebskanal synchronisiert werden.

Häufig [!DNL Commerce] [Bestellverarbeitung](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"} Zu den Aufgaben gehören:

- [Bestellaktionen](https://docs.magento.com/user-guide/sales/order-actions.html){target="_blank"}
- [Bestellsuche](https://docs.magento.com/user-guide/sales/orders-search.html){target="_blank"}
- [Auftrag verarbeiten](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"}
   - [Bestellung anzeigen](https://docs.magento.com/user-guide/sales/order-processing.html#view-an-order){target="_blank"}
   - [Auftrag verarbeiten](https://docs.magento.com/user-guide/sales/order-processing.html#process-an-order){target="_blank"}
   - [Bestellungen und Kontoinformationen](https://docs.magento.com/user-guide/sales/order-processing.html#order-and-account-information){target="_blank"}
   - [Adressinformationen](https://docs.magento.com/user-guide/sales/order-processing.html#address-information){target="_blank"}
   - [Zahlungs- und Versandmethode](https://docs.magento.com/user-guide/sales/order-processing.html#payment--shipping-method){target="_blank"}
   - [Bestellte Elemente überprüfen](https://docs.magento.com/user-guide/sales/order-processing.html#review-items-ordered){target="_blank"}
- [Gutschrift/Rückerstattung](https://docs.magento.com/user-guide/sales/credit-memo-create.html){target="_blank"}
- [Auftrag ausführen/versenden](https://docs.magento.com/user-guide/sales/shipments-create.html){target="_blank"}
- [Rechnung erstellen](https://docs.magento.com/user-guide/sales/invoice-create.html){target="_blank"}
- [Abbrechen einer nicht versandten Bestellung](./cancel-unshipped-order.md)

>[!NOTE]
>
>Wenn eine Bestellung in `Unshipped` Status, können Sie [Abbrechen einer Amazon-Bestellung](./cancel-unshipped-order.md) auf [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) Seite. Wenn eine Bestellung versandt wurde, kann sie nicht storniert werden.

Siehe [Commerce Order Management](https://docs.magento.com/user-guide/sales/order-management.html){target="_blank"}.
