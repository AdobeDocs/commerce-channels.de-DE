---
title: Allgemeine Aufgaben zur Auftragsverarbeitung
description: Verwenden Sie den entsprechenden  [!DNL Commerce] orders created for Amazon orders to manage order activity and processing in the [!UICONTROL Commerce] Admin.
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# Allgemeine Aufgaben zur Bestellverarbeitung

[[!DNL Commerce] Die Auftragsverarbeitung](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} kann Ihre Amazon-Bestellungen verwalten, einschließlich der E-Mail-Versendung an den Käufer, der Erfüllung der Bestellung (Versand), der Ausstellung von Gutschriften/Erstattungen, der Hinzufügung von Kommentaren und mehr. Um Ihre Amazon-Bestellungen zu verwalten, muss Ihre Einstellung [**Amazon-Bestellungen importieren**](./order-settings.md) auf `Enabled` gesetzt werden, damit die entsprechenden [!DNL Commerce]-Bestellungen erstellt werden, wenn Amazon-Bestellungen empfangen werden. Amazon-Bestellinformationen werden im Abschnitt *[!UICONTROL Recent Orders]* des Store-Dashboards angezeigt.

Wenn diese Option aktiviert ist, werden entsprechende [!DNL Commerce]-Bestellungen für Amazon-Bestellungen erstellt und die Amazon-Bestellnummer wird in der Spalte _[!UICONTROL Order Number]_angezeigt. Wenn eine entsprechende [!DNL Commerce]-Bestellung erstellt wird, klicken Sie auf die Bestellnummer, um die Bestellung auf der Seite [!DNL Commerce] [Bestellverarbeitung](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} zu öffnen. Sie können die Bestellung so verwalten, wie Sie Ihre anderen [[!DNL Commerce] Bestellvorgänge](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} durchführen.

Die [!DNL Commerce]-Bestellnummer wird nicht mit den _[!UICONTROL Recent Orders]_-Informationen angezeigt. Die Bestellnummer [!DNL Commerce] wird nur angezeigt, wenn Sie im Store-Dashboard auf die Bestellnummer klicken und die Bestellung in [[!DNL Commerce] Auftragsverarbeitung](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} öffnen. Bei Ansicht der Bestellung [!DNL Commerce] wird die Amazon-Bestellnummer im Abschnitt *[!UICONTROL Payment & Shipping Method]*angezeigt. Es enthält auch Optionen zu *[!UICONTROL View or Cancel Amazon Order]*und *[!UICONTROL View all Amazon Orders]*, je nach Versandstatus der Bestellung.

Siehe [Abbrechen einer nicht versandten Bestellung](./cancel-unshipped-order.md).

![Amazon-Bestellinformationen in Commerce-Reihenfolge](assets/amazon-order-number-payment-info.png)

Bei der Verarbeitung einer Amazon-Bestellung aktualisiert und synchronisiert der Amazon-Vertriebskanal die Bestellinformationen mit Ihrem [!DNL Amazon Seller Central]-Konto. Ihre Cron-Einstellungen bestimmen, wie oft Bestellinformationen zwischen dem Amazon- und Amazon-Vertriebskanal synchronisiert werden.

Zu den gängigen Aufgaben [!DNL Commerce] [Bestellverarbeitung](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;} gehören:

- [Bestellaktionen](https://docs.magento.com/user-guide/sales/order-actions.html){target=&quot;_blank&quot;}
- [Bestellsuche](https://docs.magento.com/user-guide/sales/orders-search.html){target=&quot;_blank&quot;}
- [Verarbeiten einer Bestellung](https://docs.magento.com/user-guide/sales/order-processing.html){target=&quot;_blank&quot;}
   - [Anzeigen einer Bestellung](https://docs.magento.com/user-guide/sales/order-processing.html#view-an-order){target=&quot;_blank&quot;}
   - [Verarbeiten einer Bestellung](https://docs.magento.com/user-guide/sales/order-processing.html#process-an-order){target=&quot;_blank&quot;}
   - [Reihenfolge und Kontoinformationen](https://docs.magento.com/user-guide/sales/order-processing.html#order-and-account-information){target=&quot;_blank&quot;}
   - [Adressinformationen](https://docs.magento.com/user-guide/sales/order-processing.html#address-information){target=&quot;_blank&quot;}
   - [Zahlungs- und Versandmethode](https://docs.magento.com/user-guide/sales/order-processing.html#payment--shipping-method){target=&quot;_blank&quot;}
   - [Überprüfen Sie die bestellten Elemente ](https://docs.magento.com/user-guide/sales/order-processing.html#review-items-ordered){target=&quot;_blank&quot;}
- [Gutschrift/Rückerstattung ausgeben](https://docs.magento.com/user-guide/sales/credit-memo-create.html){target=&quot;_blank&quot;}
- [Auftrag ausfüllen/versenden](https://docs.magento.com/user-guide/sales/shipments-create.html){target=&quot;_blank&quot;}
- [Rechnung erstellen](https://docs.magento.com/user-guide/sales/invoice-create.html){target=&quot;_blank&quot;}
- [Abbrechen einer nicht versandten Bestellung](./cancel-unshipped-order.md)

>[!NOTE]
>
>Wenn eine Bestellung den Status `Unshipped` aufweist, können Sie [eine Amazon-Bestellung](./cancel-unshipped-order.md) auf der Seite [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) abbrechen. Wenn eine Bestellung versandt wurde, kann sie nicht storniert werden.

Siehe [Commerce Order Management](https://docs.magento.com/user-guide/sales/order-management.html){target=&quot;_blank&quot;}.
