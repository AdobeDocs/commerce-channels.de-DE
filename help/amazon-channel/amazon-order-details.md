---
title: Amazon-Bestelldetails
description: Zeigen Sie Details zu Ihren Amazon Marketplace-Bestellungen in der Adobe Commerce oder Magento Open Source Admin an.
exl-id: a85bb6b3-817d-4859-a815-41777f4b8667
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# Amazon-Bestelldetails

![Amazon-Bestelldetails](assets/amazon-order-details-header.png)

## Amazon-Bestelldetails anzeigen

1. Klicken Sie auf der Store-Karte auf **[!UICONTROL View Store]**.

1. Klicken Sie im Abschnitt _[!UICONTROL Recent Orders]_auf eine Bestellnummer.

   Die Seite _[!UICONTROL Amazon Order Details]_wird geöffnet.

>[!NOTE]
>
>Wenn Sie den Bestellimport in [Bestelleinstellungen](./order-settings.md) aktiviert haben und die Bestellung [von Amazon (FBA)](./fulfilled-by.md) erfüllt wurde, können Sie Platzhalterdaten für einige Felder in den Bestelldetails sehen. Amazon sendet nicht die folgenden Daten für FBA-Bestellungen.
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


### Registerkarte &quot;Bestelldetails und Versanddetails&quot;

Der Tab _[!UICONTROL Order and Shipping Details]_zeigt detaillierte Bestellinformationen an, die von Amazon empfangen wurden.

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
>Vergessen Sie nicht, nach der Bearbeitung auf **Bestellung speichern** zu klicken.

![Bestelldetails und Versanddetails](assets/amazon-order-details.png)

### Registerkarte &quot;Bestellelemente&quot;

Auf der Registerkarte _[!UICONTROL Order Items]_werden alle Elemente angezeigt, die mit der Amazon-Bestellung verknüpft sind, wie von Amazon empfangen.

![Bestellelementdetails](assets/amazon-order-item-details.png)

### Tab Tracking

Der Tab _[!UICONTROL Tracking]_zeigt Tracking-Informationen an, die mit der Amazon-Bestellung verbunden sind.

![Tracking-Details](assets/amazon-order-tracking-details.png)
