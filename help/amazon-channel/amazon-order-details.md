---
title: Amazon-Bestelldetails
description: Zeigen Sie Details zu Ihren Amazon Marketplace-Bestellungen in der Adobe Commerce oder Magento Open Source Admin an.
feature: Sales Channels, Orders
exl-id: a85bb6b3-817d-4859-a815-41777f4b8667
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# Amazon-Bestelldetails

![Amazon-Bestelldetails](assets/amazon-order-details-header.png){width="600" zoomable="yes"}

## Amazon-Bestelldetails anzeigen

1. Klicks **[!UICONTROL View Store]** auf der Speicherkarte.

1. Im _[!UICONTROL Recent Orders]_klicken Sie auf eine Bestellnummer.

   Die _[!UICONTROL Amazon Order Details]_Seite geöffnet.

>[!NOTE]
>
>Wenn Sie den Bestellimport in Ihrem [Bestelleinstellungen](./order-settings.md) und die Reihenfolge lautet [erfüllt von Amazon (FBA)](./fulfilled-by.md), können Sie Platzhalterdaten für einige Felder in den Bestelldetails sehen. Amazon sendet nicht die folgenden Daten für FBA-Bestellungen.
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

### Tab &quot;Bestelldetails&quot;und &quot;Versanddetails&quot;

Die _[!UICONTROL Order and Shipping Details]_-Tab zeigt detaillierte Bestellinformationen an, die von Amazon empfangen wurden.

>[!IMPORTANT]
>
>Amazon akzeptiert nicht standardmäßige Adressinformationen, die nicht in den Amazon-Vertriebskanal importiert werden können, wodurch verhindert wird, dass die Länder-/Ländercodes bei einigen Bestellungen korrekt aktualisiert werden. Um Adressfehler zu korrigieren, können die folgenden Felder in den Bestelldetails bearbeitet werden:
>
>- `Shipping address 1`
>- `Shipping address 2`
>- `Shipping address 3`
>- `Shipping city`
>- `Shipping region`
>- `Shipping postal code`
>- `Shipping country`
>
>Vergessen Sie nicht, auf **Bestellung speichern** nach der Bearbeitung.

![Bestelldetails und Versanddetails](assets/amazon-order-details.png){width="600" zoomable="yes"}

### Registerkarte &quot;Bestellelemente&quot;

Die _[!UICONTROL Order Items]_-Tab zeigt alle mit der Amazon-Bestellung verknüpften Elemente an, wie sie von Amazon empfangen wurden.

![Bestellelementdetails](assets/amazon-order-item-details.png){width="600" zoomable="yes"}

### Tab Tracking

Die _[!UICONTROL Tracking]_zeigt Tracking-Informationen an, die mit der Amazon-Bestellung verbunden sind.

![Tracking-Details](assets/amazon-order-tracking-details.png){width="600" zoomable="yes"}
