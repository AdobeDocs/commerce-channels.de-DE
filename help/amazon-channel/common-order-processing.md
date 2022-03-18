---
title: Allgemeine Aufgaben zur Auftragsverarbeitung
description: Verwenden Sie die entsprechende [!DNL Commerce] Bestellungen, die für Amazon-Bestellungen erstellt wurden, um die Bestellaktivität und -verarbeitung im [!UICONTROL Commerce] Admin.
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Allgemeine Aufgaben zur Bestellverarbeitung

[[!DNL Commerce] Bestellverarbeitung](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} kann Ihre Amazon-Bestellungen verwalten, einschließlich der E-Mail-Versendung an den Käufer, der Erfüllung der Bestellung (Versand), der Ausstellung von Gutschriften/Erstattungen, der Hinzufügung von Kommentaren und mehr. Um Ihre Amazon-Bestellungen zu verwalten, benötigen Sie [**Importieren von Amazon-Bestellungen**](./order-settings.md) muss auf `Enabled` so, dass [!DNL Commerce] Bestellungen werden erstellt, wenn Amazon-Bestellungen empfangen werden. Amazon-Bestellinformationen werden im *[!UICONTROL Recent Orders]* des Store-Dashboards.

Wenn aktiviert, entspricht [!DNL Commerce] Bestellungen werden für Amazon-Bestellungen erstellt und die Amazon-Bestellnummer wird im _[!UICONTROL Order Number]_Spalte. Wenn eine [!DNL Commerce] -Bestellung erstellt wird, klicken Sie auf die Bestellnummer, um die Bestellung im [!DNL Commerce] [Bestellverarbeitung](https://docs.magento.com/user-guide/sales/order-processing.html)Seite {target=&quot;_blank&quot;}. Sie können die Bestellung so verwalten, wie Sie sie bei Ihren anderen [[!DNL Commerce] Bestellverarbeitung](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}.

Die [!DNL Commerce] Die Bestellnummer wird nicht mit der _[!UICONTROL Recent Orders]_Informationen. Die [!DNL Commerce] Die Bestellnummer wird nur angezeigt, wenn Sie auf die Bestellnummer im Store-Dashboard klicken und die Bestellung in [[!DNL Commerce] Bestellverarbeitung](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}. Beim Anzeigen der [!DNL Commerce] -Reihenfolge, wird die Amazon-Bestellnummer in der *[!UICONTROL Payment & Shipping Method]*Abschnitt. Es enthält auch Optionen für *[!UICONTROL View or Cancel Amazon Order]*und *[!UICONTROL View all Amazon Orders]*, abhängig vom Versandstatus der Bestellung.

Siehe [unversandte Bestellung stornieren](./cancel-unshipped-order.md).

![Amazon-Bestellinformationen in Commerce-Reihenfolge](assets/amazon-order-number-payment-info.png)

Bei der Verarbeitung einer Amazon-Bestellung aktualisiert und synchronisiert der Amazon-Vertriebskanal die Bestellinformationen mit Ihrem [!DNL Amazon Seller Central] -Konto. Ihre Cron-Einstellungen bestimmen, wie oft Bestellinformationen zwischen dem Amazon- und Amazon-Vertriebskanal synchronisiert werden.

Häufig [!DNL Commerce] [Bestellverarbeitung](https://docs.magento.com/user-guide/sales/order-processing.html)Zu den Aufgaben {target=&quot;_blank&quot;} gehören:

- [Bestellaktionen](https://docs.magento.com/user-guide/sales/order-actions.html){target=&quot;_blank&quot;}
- [Bestellsuche](https://docs.magento.com/user-guide/sales/orders-search.html){target=&quot;_blank&quot;}
- [Auftrag verarbeiten](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}
   - [Bestellung anzeigen](https://docs.magento.com/user-guide/sales/order-processing.html#view-an-order){target=&quot;_blank&quot;}
   - [Auftrag verarbeiten](https://docs.magento.com/user-guide/sales/order-processing.html#process-an-order){target=&quot;_blank&quot;}
   - [Bestellungen und Kontoinformationen](https://docs.magento.com/user-guide/sales/order-processing.html#order-and-account-information){target=&quot;_blank&quot;}
   - [Adressinformationen](https://docs.magento.com/user-guide/sales/order-processing.html#address-information){target=&quot;_blank&quot;}
   - [Zahlungs- und Versandmethode](https://docs.magento.com/user-guide/sales/order-processing.html#payment--shipping-method){target=&quot;_blank&quot;}
   - [Bestellte Elemente überprüfen](https://docs.magento.com/user-guide/sales/order-processing.html#review-items-ordered){target=&quot;_blank&quot;}
- [Gutschrift/Rückerstattung](https://docs.magento.com/user-guide/sales/credit-memo-create.html){target=&quot;_blank&quot;}
- [Auftrag ausführen/versenden](https://docs.magento.com/user-guide/sales/shipments-create.html){target=&quot;_blank&quot;}
- [Rechnung erstellen](https://docs.magento.com/user-guide/sales/invoice-create.html){target=&quot;_blank&quot;}
- [Abbrechen einer nicht versandten Bestellung](./cancel-unshipped-order.md)

>[!NOTE]
>
>Wenn eine Bestellung in `Unshipped` Status, können Sie [Abbrechen einer Amazon-Bestellung](./cancel-unshipped-order.md) auf [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) Seite. Wenn eine Bestellung versandt wurde, kann sie nicht storniert werden.

Siehe [Commerce Order Management](https://docs.magento.com/user-guide/sales/order-management.html){target=&quot;_blank&quot;}.
