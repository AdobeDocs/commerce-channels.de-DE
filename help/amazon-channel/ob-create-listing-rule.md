---
title: '"Onboarding: Erstellen einer Listungsregel'''
description: Erstellen Sie beim Abschluss des Onboarding-Prozesses für den Amazon-Verkaufskanal die anfänglichen Listening-Regeln zum Generieren von Amazon-Auflistungen für Ihre  [!DNL Commerce] Produkte.
exl-id: b318823e-a726-4a59-b117-9838562c7d8b
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Onboarding: Erstellen einer Listungsregel

Listening-Regeln können während des Onboarding definiert, aber auch jederzeit geändert werden. Nach dem Onboarding können Sie auf die [Auflistungsregeln](./listing-rules.md) im Store [Dashboard](./amazon-store-dashboard.md) zugreifen.

## Erstellen einer Listening-Regel während des Onboarding

1. Nachdem Ihr Store verbunden ist, klicken Sie für den hinzugefügten Store auf **[!UICONTROL View Store]** .

   Der Speicher [dashboard](./amazon-store-dashboard.md) wird mit der Meldung `No products listed to Amazon` angezeigt.

1. Klicken Sie auf **[!UICONTROL Preview and List Eligible Products]**.

   Die Seite _[!UICONTROL Listing Rules]_wird angezeigt.

1. Definieren Sie die gewünschten Bedingungen für die Eignung von Produkten, die in Amazon aufgeführt werden sollen, und klicken Sie auf **[!UICONTROL Preview changes]** oder klicken Sie auf **[!UICONTROL Preview changes]**, um diesen Schritt zu überspringen.

   Siehe [Beispiel: Definieren Sie eine Bedingung](./ob-define-condition-example.md).

1. Überprüfen Sie Ihre Listen in der Listenvorschau:

   ![Listenvorschau](assets/amazon-ob-listing-preview.png)

   - **[!UICONTROL Ineligible Listings]** - Produkte, die auf dieser Registerkarte aufgelistet sind, können nicht auf der Grundlage Ihrer aktuellen Listenregeleinstellungen in die Amazon-Liste aufgenommen werden.

      Nicht infrage kommende Produkte werden nicht in Amazon veröffentlicht. Wenn ein nicht infrage kommendes Produkt bereits in Amazon aufgeführt ist und Sie die Amazon-Liste mit Ihrem [!DNL Commerce]-Katalogprodukt abgleichen, ändert sich die Menge für die Amazon-Auflistung in `0`, um den Verkauf des Produkts zu verhindern. Informationen zum manuellen Entfernen einer Liste aus Amazon finden Sie unter [Beenden einer Amazon-Liste](./end-listings-manually.md). Produkte, die nicht für Amazon-Anforderungen infrage kommen, sind hier nicht aufgeführt. Diese Produkte sind auf der Registerkarte [[!UICONTROL Inactive Listings]](./inactive-listings.md) aufgeführt.

      Um eine `Ineligible`-Auflistung in eine `Eligible`-Auflistung zu ändern, wiederholen Sie diesen Vorgang und ändern Sie Ihre Listening-Regeln.

   - **[!UICONTROL Eligible Listings]** - Produkte, die auf dieser Registerkarte aufgelistet sind, können auf der Grundlage Ihrer aktuellen Listening-Regel-Einrichtung in die Amazon-Liste aufgenommen werden und sind für Amazon-Anforderungen geeignet. Diese Registerkarte enthält Ihre vorhandenen Amazon-Listen, die importiert werden (wenn Sie **[!UICONTROL Import Third Party Listings]** in [Listeneinstellungen](./listing-settings.md) auf `Import Listing` gesetzt haben).

   - **[!UICONTROL New Listings]** - Die auf dieser Registerkarte aufgelisteten Produkte umfassen Ihre  [!DNL Commerce] Katalogprodukte, die aufgrund Ihrer aktuellen Regeleinrichtung für die Auflistung von Amazon-Produkten neu zugelassen werden können, und erstellen Amazon-Listen.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save and Close]**.

   Der Store [dashboard](./amazon-store-dashboard.md) wird geöffnet.

Nachdem das Onboarding eines Stores abgeschlossen ist, wird die Informationssynchronisierung zwischen [!DNL Commerce] und Amazon initiiert. Ihre Amazon-Listen werden in [!DNL Commerce] importiert und versuchen, sie mit den Produkten im [!DNL Commerce]-Katalog abzugleichen.

Sie können Ihre Amazon-Bestellinformationen im Abschnitt _[!UICONTROL Recent Orders]_des Store-Dashboards anzeigen. Siehe [Dashboard speichern](./amazon-store-dashboard.md) oder [Bestellungen verwalten](./managing-orders.md).

>[!IMPORTANT]
>
>Es gibt einige wichtige Store-Einstellungen (Listen, Preise, Regeln, Erfüllung usw.), die Standardwerte für einen neuen Store haben. Um sicherzustellen, dass Ihr Store für Ihre spezifischen Anforderungen eingerichtet ist, überprüfen Sie Ihre [Store-Einstellungen](./default-store-settings.md) .

![Nächstes ](assets/btn-next.png) [**SymbolWeiter zu Standardspeichereinstellungen**](./default-store-settings.md)
