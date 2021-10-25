---
title: '''Einstieg: Listungsregel erstellen"'
description: Erstellen Sie während des Einboarding-Prozesses des Amazon Sales Kanal die anfänglichen Regeln für die Erstellung von Amazon-Listen für Ihre [!DNL Commerce] Produkte.
exl-id: b318823e-a726-4a59-b117-9838562c7d8b
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Einstieg: Listungsregel erstellen

Listing-Regeln können während des Einbodens definiert, aber auch jederzeit geändert werden. Nach dem Einsteigen können Sie auf die [Listungsregeln](./listing-rules.md) im Geschäft [Dashboard](./amazon-store-dashboard.md).

## Listungsregel während des Einstiegs erstellen

1. Klicken Sie nach der Verbindung mit dem Store auf **[!UICONTROL View Store]** für den hinzugefügten Store.

   Der Laden [Dashboard](./amazon-store-dashboard.md) wird mit `No products listed to Amazon` Nachricht.

1. Klick **[!UICONTROL Preview and List Eligible Products]**.

   Die _[!UICONTROL Listing Rules]_angezeigt.

1. Legen Sie die Bedingungen fest, unter denen Produkte unter Amazon zugelassen werden sollen, und klicken Sie auf **[!UICONTROL Preview changes]** oder klicken Sie auf **[!UICONTROL Preview changes]** um diesen Schritt zu überspringen.

   Siehe [Beispiel: Bedingung definieren](./ob-define-condition-example.md).

1. Überprüfen Sie Ihre Einträge in der Listing-Vorschau:

   ![Listing-Vorschau](assets/amazon-ob-listing-preview.png)

   - **[!UICONTROL Ineligible Listings]** - Produkte, die auf dieser Registerkarte aufgelistet sind, sind aufgrund Ihrer aktuellen Listenregeleinstellungen nicht für eine Amazon-Auflistung zugelassen.

      Nicht förderfähige Produkte werden nicht auf Amazon veröffentlicht. Wenn ein nicht zugelassenes Produkt bereits auf Amazon aufgeführt ist und Sie die Amazon-Liste Ihrem [!DNL Commerce] Katalogprodukt, die Menge für die Amazon-Auflistung ändert sich in `0` um den Verkauf der Ware zu verhindern. Informationen zum manuellen Entfernen einer Auflistung aus Amazon finden Sie unter [Beenden einer Amazon-Liste](./end-listings-manually.md). Produkte, die nicht unter die Amazon-Anforderungen fallen, sind hier nicht aufgeführt. Diese Erzeugnisse sind im [[!UICONTROL Inactive Listings] Tab](./inactive-listings.md).

      So ändern Sie `Ineligible` Auflistung in einer `Eligible` auflisten, diesen Prozess wiederholen und Ihre Listingregeln ändern.

   - **[!UICONTROL Eligible Listings]** - Produkte, die auf dieser Registerkarte aufgeführt sind, sind für eine Amazon-Auflistung entsprechend Ihrer aktuellen Listing-Regel zugelassen und können nach den Amazon-Anforderungen aufgelistet werden. Auf dieser Registerkarte sind die bereits vorhandenen Amazon-Einträge enthalten, die importiert werden (falls Sie **[!UICONTROL Import Third Party Listings]** einstellen auf `Import Listing` in [Listingeinstellungen](./listing-settings.md)).

   - **[!UICONTROL New Listings]** - Zu den auf dieser Registerkarte aufgelisteten Produkten gehören [!DNL Commerce] Katalogprodukte, die aufgrund Ihrer aktuellen Listungsregel-Einrichtung für die Amazon-Auflistung zugelassen wurden, und erstellen Sie Amazon-Listen.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save and Close]**.

   Der Laden [Dashboard](./amazon-store-dashboard.md) öffnet.

Nach Abschluss des Einstiegs in einen Store werden die Informationen synchronisiert zwischen [!DNL Commerce] und Amazon initiiert wird. Ihre Amazon-Listen werden in importiert [!DNL Commerce] und versuchen Sie, mit den Produkten in Ihrer [!DNL Commerce] Katalog.

Sie können Ihre Amazon-Bestellinformationen in der Ansicht _[!UICONTROL Recent Orders]_des Dashboards. Siehe [Dashboard speichern](./amazon-store-dashboard.md) oder [Bestellungen verwalten](./managing-orders.md).

>[!IMPORTANT]
>
>Es gibt einige wichtige Store-Einstellungen (Listen, Preise, Regeln, Fulfillment, etc.), die Standardwerte für einen neuen Store haben. Überprüfen Sie Ihre [Speichereinstellungen](./default-store-settings.md) .

![Nächstes Symbol](assets/btn-next.png) [**Weiter zu den Standard-Store-Einstellungen**](./default-store-settings.md)
