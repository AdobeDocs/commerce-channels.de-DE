---
title: Amazon-Auftragsdetails
description: Ansicht für Ihre Amazon Marketplace-Bestellungen im Adobe Commerce oder Magento Open Source Admin.
exl-id: a85bb6b3-817d-4859-a815-41777f4b8667
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# Amazon-Auftragsdetails

![Amazon-Auftragsdetails](assets/amazon-order-details-header.png)

## Ansicht Amazon Auftragsdetails

1. Klick **[!UICONTROL View Store]** auf der Ladenkarte.

1. In _[!UICONTROL Recent Orders]_klicken Sie auf eine Bestellnummer.

   Die _[!UICONTROL Amazon Order Details]_Seite wird geöffnet.

>[!NOTE]
>
>Wenn der Auftragsimport in Ihrem [Auftragseinstellungen](./order-settings.md) und die Bestellung [erfüllt von Amazon (FBA)](./fulfilled-by.md), können Sie die Dummy-Daten für einige Felder in den Auftragsdetails sehen. Amazon sendet folgende Daten für FBA-Bestellungen nicht.
>
> - `AddressType`
> - `AddressLine1`
> - `AddressLine2`
> - `AddressLine3`
> - `BuyerName`
> - `Phone`
> - `PurchaseOrderNumber`
> - `RecipientName`
> - `CustomizedURL`
> - `GiftMessageText`


### Registerkarte &quot;Order and Shipping Details&quot;

Die _[!UICONTROL Order and Shipping Details]_auf der Registerkarte erhalten Sie detaillierte Bestellinformationen von Amazon.

>[!IMPORTANT]
>
>Amazon akzeptiert nicht standardmäßige Adressinformationen, die nicht in den Amazon Sales Kanal importiert werden können, wodurch verhindert wird, dass die Staaten-/Ländercodes bei einigen Bestellungen korrekt aktualisiert werden. Die folgenden Felder können in den Auftragsdetails bearbeitet werden, um Adressfehler zu beheben:
>
>- `Shipping address 1`
>- `Shipping address 2`
>- `Shipping address 3`
>- `Shipping city`
>- `Shipping region`
>- `Shipping postal code`
>- `Shipping country`

>
>Klicken Sie auf **Bestellung speichern** nach Bearbeitung.

![Bestellungs- und Versanddetails](assets/amazon-order-details.png)

### Registerkarte &quot;Elemente&quot;

Die _[!UICONTROL Order Items]_-Tab zeigt alle mit der Amazon-Bestellung verknüpften Elemente an, wie sie von Amazon empfangen wurden.

![Auftragselementdetails](assets/amazon-order-item-details.png)

### Registerkarte Laufweite

Die _[!UICONTROL Tracking]_auf dieser Registerkarte werden Verfolgungsinformationen angezeigt, die mit der Amazon-Bestellung verbunden sind.

![Trackingdetails](assets/amazon-order-tracking-details.png)
