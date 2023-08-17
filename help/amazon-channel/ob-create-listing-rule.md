---
title: Erstellen einer Amazon-Listening-Regel
description: Erstellen Sie beim Abschluss des Onboarding-Prozesses für den Amazon-Verkaufskanal die anfänglichen Listening-Regeln zum Generieren von Amazon-Auflistungen für Ihre [!DNL Commerce] Produkte.
role: Admin
feature: Sales Channels, Products, Merchandising, Configuration
exl-id: b318823e-a726-4a59-b117-9838562c7d8b
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Erstellen einer Amazon-Listening-Regel

Listening-Regeln können während des Onboarding definiert, aber auch jederzeit geändert werden. Nach dem Onboarding können Sie auf die [Auflistungsregeln](./listing-rules.md) im Geschäft [Dashboard](./amazon-store-dashboard.md).

## Erstellen einer Listening-Regel während des Onboarding

1. Nachdem Ihr Store verbunden ist, klicken Sie auf **[!UICONTROL View Store]** für den hinzugefügten Store.

   Der Laden [Dashboard](./amazon-store-dashboard.md) mit dem `No products listed to Amazon` Nachricht.

1. Klicken **[!UICONTROL Preview and List Eligible Products]**.

   Die _[!UICONTROL Listing Rules]_angezeigt.

1. Legen Sie die gewünschten Bedingungen für die Aufnahme von Produkten in Amazon fest und klicken Sie auf **[!UICONTROL Preview changes]** oder klicken Sie auf **[!UICONTROL Preview changes]** , um diesen Schritt zu überspringen.

   Siehe [Beispiel: Bedingung definieren](./ob-define-condition-example.md).

1. Überprüfen Sie Ihre Listen in der Listenvorschau:

   ![Listenvorschau](assets/amazon-ob-listing-preview.png){width="600" zoomable="yes"}

   - **[!UICONTROL Ineligible Listings]** - Produkte, die auf dieser Registerkarte aufgelistet sind, können nicht auf der Grundlage Ihrer aktuellen Listenregeleinstellungen in die Amazon-Liste aufgenommen werden.

     Nicht infrage kommende Produkte werden nicht in Amazon veröffentlicht. Wenn ein nicht infrage kommendes Produkt bereits in Amazon aufgeführt ist und Sie die Amazon-Liste mit Ihrer [!DNL Commerce] Katalogprodukt, die Menge für die Amazon, in der Änderungen an `0` um den Verkauf des Erzeugnisses zu verhindern. Informationen zum manuellen Entfernen einer Liste aus Amazon finden Sie unter [Beenden einer Amazon-Auflistung](./end-listings-manually.md). Produkte, die nicht für Amazon-Anforderungen infrage kommen, sind hier nicht aufgeführt. Diese Produkte sind auf der [[!UICONTROL Inactive Listings] tab](./inactive-listings.md).

     So ändern Sie eine `Ineligible` Auflistung von `Eligible` auflisten, diesen Prozess wiederholen und Ihre Listening-Regeln ändern.

   - **[!UICONTROL Eligible Listings]** - Produkte, die auf dieser Registerkarte aufgelistet sind, können auf der Grundlage Ihrer aktuellen Listening-Regel-Einrichtung in die Amazon-Liste aufgenommen werden und sind für Amazon-Anforderungen geeignet. Auf dieser Registerkarte befinden sich die vorhandenen Amazon-Listen, die importiert werden (falls Sie **[!UICONTROL Import Third Party Listings]** auf `Import Listing` in [Listening-Einstellungen](./listing-settings.md)).

   - **[!UICONTROL New Listings]** - Die auf dieser Registerkarte aufgelisteten Produkte umfassen Ihre [!DNL Commerce] Katalogprodukte, die aufgrund der aktuellen Einrichtung Ihrer Listening-Regeln für die Amazon-Auflistung neu zugelassen werden und Amazon-Listen erstellen.

1. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Save and Close]**.

   Der Laden [Dashboard](./amazon-store-dashboard.md) geöffnet.

Nachdem das Onboarding eines Stores abgeschlossen ist, werden die Informationen zwischen [!DNL Commerce] und Amazon initiiert wird. Ihre Amazon-Listen werden in [!DNL Commerce] und versuchen Sie, mit Produkten in Ihrem [!DNL Commerce] Katalog.

Sie können Ihre Amazon-Bestellinformationen im _[!UICONTROL Recent Orders]_des Store-Dashboards. Siehe [Store-Dashboard](./amazon-store-dashboard.md) oder [Bestellungen verwalten](./managing-orders.md).

>[!IMPORTANT]
>
>Es gibt einige wichtige Store-Einstellungen (Listen, Preise, Regeln, Erfüllung usw.), die Standardwerte für einen neuen Store haben. Um sicherzustellen, dass Ihr Store für Ihre spezifischen Anforderungen eingerichtet ist, überprüfen Sie Ihre [Store-Einstellungen](./default-store-settings.md) .

![Nächstes Symbol](assets/btn-next.png) [**Weiter zu den standardmäßigen Speichereinstellungen**](./default-store-settings.md)
