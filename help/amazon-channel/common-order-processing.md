---
title: Allgemeine Aufgaben zur Auftragsverarbeitung
description: Entsprechende verwenden [!DNL Commerce] orders created for Amazon orders to manage order activity and processing in the [!UICONTROL Commerce] Admin.
exl-id: a44f36f0-db18-4de5-9c5b-cc68f4793008
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# Aufgaben zur Verarbeitung gemeinsamer Bestellungen

[[!DNL Commerce] Auftragsverarbeitung](https://docs.magento.com/user-guide/sales/order-processing.html){Zielgruppe=&quot;_blank&quot;} kann Ihre Amazon-Bestellungen verwalten, z. B. per E-Mail an den Käufer senden, die Bestellung ausfüllen, Gutschriften/Erstattungen ausgeben, Kommentare hinzufügen und vieles mehr. Um Ihre Amazon-Aufträge zu verwalten, [**Amazon-Bestellungen importieren**](./order-settings.md) Einstellung muss auf `Enabled` so, dass [!DNL Commerce] Bestellungen werden erstellt, wenn Amazon Bestellungen entgegengenommen werden. Amazon-Bestellinformationen im *[!UICONTROL Recent Orders]* des Dashboards.

Wenn aktiviert, entsprechende [!DNL Commerce] Bestellungen werden für Amazon-Bestellungen erstellt und die Amazon-Bestellnummer wird angezeigt im _[!UICONTROL Order Number]_Spalte. Wenn [!DNL Commerce] Auftrag erstellt wurde, klicken Sie auf die Bestellnummer, um die Bestellung in der [!DNL Commerce] [Auftragsverarbeitung](https://docs.magento.com/user-guide/sales/order-processing.html){Zielgruppe=&quot;_blank&quot;} Seite. Sie können die Bestellung so verwalten, wie Sie es bei Ihren anderen tun [[!DNL Commerce] Auftragsverarbeitung](https://docs.magento.com/user-guide/sales/order-processing.html){Zielgruppe=&quot;_blank&quot;}.

Die [!DNL Commerce] Bestellnummer wird nicht angezeigt mit _[!UICONTROL Recent Orders]_Informationen. Die [!DNL Commerce] Die Bestellnummer wird nur angezeigt, wenn Sie auf die Bestellnummer auf dem Store-Dashboard klicken und die Bestellung in [[!DNL Commerce] Auftragsverarbeitung](https://docs.magento.com/user-guide/sales/order-processing.html){Zielgruppe=&quot;_blank&quot;}. Bei Ansicht des [!DNL Commerce] die Amazon-Bestellnummer wird im *[!UICONTROL Payment & Shipping Method]*Abschnitt. Es enthält auch Optionen für *[!UICONTROL View or Cancel Amazon Order]*und *[!UICONTROL View all Amazon Orders]*, je nach Versandstatus der Bestellung.

Siehe [Nicht versandte Bestellung stornieren](./cancel-unshipped-order.md).

![Amazon-Bestellinformationen in Commerce-Bestellung](assets/amazon-order-number-payment-info.png)

Bei der Verarbeitung einer Amazon-Bestellung aktualisiert und synchronisiert Amazon Sales Kanal die Bestellinformationen mit Ihren [!DNL Amazon Seller Central] Konto. Ihre cron-Einstellungen bestimmen, wie oft Bestellinformationen zwischen Amazon und Amazon Sales Kanal synchronisiert werden.

Häufig [!DNL Commerce] [Auftragsverarbeitung](https://docs.magento.com/user-guide/sales/order-processing.html){Zielgruppe=&quot;_blank&quot;} Aufgaben umfassen:

- [Aktionen bestellen](https://docs.magento.com/user-guide/sales/order-actions.html){Zielgruppe=&quot;_blank&quot;}
- [Auftragssuche](https://docs.magento.com/user-guide/sales/orders-search.html){Zielgruppe=&quot;_blank&quot;}
- [Auftrag verarbeiten](https://docs.magento.com/user-guide/sales/order-processing.html){Zielgruppe=&quot;_blank&quot;}
   - [Ansicht und Bestellung](https://docs.magento.com/user-guide/sales/order-processing.html#view-an-order){Zielgruppe=&quot;_blank&quot;}
   - [Auftrag verarbeiten](https://docs.magento.com/user-guide/sales/order-processing.html#process-an-order){Zielgruppe=&quot;_blank&quot;}
   - [Auftrags- und Kontoinformationen](https://docs.magento.com/user-guide/sales/order-processing.html#order-and-account-information){Zielgruppe=&quot;_blank&quot;}
   - [Adressinformationen](https://docs.magento.com/user-guide/sales/order-processing.html#address-information){Zielgruppe=&quot;_blank&quot;}
   - [Zahlungs- und Versandmethode](https://docs.magento.com/user-guide/sales/order-processing.html#payment--shipping-method){Zielgruppe=&quot;_blank&quot;}
   - [Bestellte Elemente überprüfen](https://docs.magento.com/user-guide/sales/order-processing.html#review-items-ordered){Zielgruppe=&quot;_blank&quot;}
- [Ausgabe eines Kredits/einer Rückerstattung](https://docs.magento.com/user-guide/sales/credit-memo-create.html){Zielgruppe=&quot;_blank&quot;}
- [Auftrag wird ausgeführt/versendet](https://docs.magento.com/user-guide/sales/shipments-create.html){Zielgruppe=&quot;_blank&quot;}
- [Rechnung erstellen](https://docs.magento.com/user-guide/sales/invoice-create.html){Zielgruppe=&quot;_blank&quot;}
- [Nicht versandte Bestellung abbrechen](./cancel-unshipped-order.md)

>[!NOTE]
>
>Wenn eine Bestellung in `Unshipped` Status, können Sie [Amazon-Bestellung stornieren](./cancel-unshipped-order.md) zu [[!UICONTROL Amazon Order Details]](./amazon-order-details.md) Seite. Wenn eine Bestellung versendet wurde, kann sie nicht storniert werden.

Siehe [Commerce-Auftragsverwaltung](https://docs.magento.com/user-guide/sales/order-management.html){Zielgruppe=&quot;_blank&quot;}.
