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

Listening-Regeln können während des Onboarding definiert, aber auch jederzeit geändert werden. Nach dem Onboarding können Sie auf die [Auflistungsregeln](./listing-rules.md) im Store [Dashboard](./amazon-store-dashboard.md) zugreifen.

## Erstellen einer Listening-Regel während des Onboarding

1. Nachdem Ihr Store verbunden ist, klicken Sie für den hinzugefügten Store auf **[!UICONTROL View Store]** .

   Der Store [Dashboard](./amazon-store-dashboard.md) wird mit der Meldung `No products listed to Amazon` angezeigt.

1. Klicken Sie auf **[!UICONTROL Preview and List Eligible Products]**.

   Die Seite &quot;_[!UICONTROL Listing Rules]_&quot; wird angezeigt.

1. Definieren Sie die gewünschten Bedingungen für die Eignung von Produkten, die in Amazon aufgeführt werden sollen, und klicken Sie auf **[!UICONTROL Preview changes]** oder auf **[!UICONTROL Preview changes]** , um diesen Schritt zu überspringen.

   Siehe [Beispiel: Bedingung definieren](./ob-define-condition-example.md).

1. Überprüfen Sie Ihre Listen in der Listenvorschau:

   ![Listing preview](assets/amazon-ob-listing-preview.png){width="600" zoomable="yes"}

   - **[!UICONTROL Ineligible Listings]** - Auf dieser Registerkarte aufgelistete Produkte können nicht auf der Grundlage Ihrer aktuellen Listenregeleinstellungen in die Amazon-Liste aufgenommen werden.

     Nicht infrage kommende Produkte werden nicht in Amazon veröffentlicht. Wenn ein nicht qualifiziertes Produkt bereits in Amazon aufgeführt ist und Sie die Amazon-Liste mit Ihrem [!DNL Commerce] -Katalogprodukt abgleichen, wird die Menge für die Amazon-Auflistung auf `0` geändert, um den Verkauf des Produkts zu verhindern. Informationen zum manuellen Entfernen einer Liste aus Amazon finden Sie unter [Beenden einer Amazon-Liste](./end-listings-manually.md). Produkte, die nicht für Amazon-Anforderungen infrage kommen, sind hier nicht aufgeführt. Diese Produkte werden auf der Registerkarte [[!UICONTROL Inactive Listings]](./inactive-listings.md) aufgelistet.

     Um eine `Ineligible` -Auflistung in eine `Eligible` -Auflistung zu ändern, wiederholen Sie diesen Vorgang und ändern Sie Ihre Listening-Regeln.

   - **[!UICONTROL Eligible Listings]** - Produkte, die auf dieser Registerkarte aufgeführt sind, können auf Grundlage Ihrer aktuellen Regeleinrichtung für die Auflistung der Amazon-Listen aufgelistet werden und sind für Amazon-Anforderungen geeignet. Diese Registerkarte enthält Ihre vorhandenen Amazon-Listen, die importiert werden (wenn Sie in Ihren [Listening-Einstellungen](./listing-settings.md) den Wert **[!UICONTROL Import Third Party Listings]** auf `Import Listing` festgelegt haben).

   - **[!UICONTROL New Listings]** - Die auf dieser Registerkarte aufgelisteten Produkte umfassen Ihre [!DNL Commerce] -Katalogprodukte, die aufgrund der aktuellen Einrichtung Ihrer Listening-Regeln für die Amazon-Liste neu zugelassen werden können, und erstellen Amazon-Auflistungen.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save and Close]**.

   Der Store [dashboard](./amazon-store-dashboard.md) wird geöffnet.

Nach dem Onboarding eines Stores wird die Informationssynchronisierung zwischen [!DNL Commerce] und Amazon initiiert. Ihre Amazon-Listen werden in [!DNL Commerce] importiert und versuchen, sie mit den Produkten in Ihrem [!DNL Commerce]-Katalog abzugleichen.

Sie können Ihre Amazon-Bestellinformationen im Abschnitt _[!UICONTROL Recent Orders]_des Store-Dashboards anzeigen. Siehe [Dashboard speichern](./amazon-store-dashboard.md) oder [Bestellungen verwalten](./managing-orders.md).

>[!IMPORTANT]
>
>Es gibt einige wichtige Store-Einstellungen (Listen, Preise, Regeln, Erfüllung usw.), die Standardwerte für einen neuen Store haben. Um sicherzustellen, dass Ihr Store für Ihre spezifischen Anforderungen eingerichtet ist, überprüfen Sie Ihre [Speichereinstellungen](./default-store-settings.md) .

![Nächstes Symbol](assets/btn-next.png) [**Weiter zu den standardmäßigen Speichereinstellungen**](./default-store-settings.md)
