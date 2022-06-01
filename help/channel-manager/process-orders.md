---
title: Verarbeitungsaufträge
description: Versandanleitung und Stornierung [!DNL Walmart Marketplace] Bestellungen von Adobe Commerce und Magento Open Source.
exl-id: 2fdcb348-5c02-464f-a114-16ec657bed6b
source-git-commit: f1c37111df2f566b9673946bb9b2b282506f990c
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Verarbeitungsaufträge

Nachher [!DNL Walmart Marketplace] Bestellungen wurden bestätigt und erfolgreich an gesendet [!DNL Channel Manager], verwenden Sie [Commerce Order Management](https://docs.magento.com/user-guide/sales/orders-workspace.html) , um die Bestellung zu verarbeiten.

Der Kanal-Manager synchronisiert Aktualisierungen mit [!DNL Walmart Marketplace] , um sicherzustellen, dass der Auftragsstatus und die Versandinformationen aus Commerce mit den in der Variablen [!DNL Walmart Marketplace].

* **Auftragsversand**-Walmart benötigt eine Trackingnummer für alle Sendungen. Wenn einige Artikel nicht vorrätig sind, können Sie Teillieferungen erstellen, um derzeit verfügbare Artikel zu senden. Nach Absendung der Sendung werden die Auftragsaktualisierungen mit [!DNL Walmart Marketplace]. Anschließend informiert Walmart die Kunden über den Bestellstatus und die Versanddetails.

* **Stornierungen von Bestellungen**-Wenn Sie eine [!DNL Walmart Marketplace] Bestellung, Walmart benötigt einen Stornierungsgrund, der in der an den Kunden gesendeten Stornierungsmeldung enthalten ist. Der Stornogrund wird auch im Abschnitt [!DNL Commerce] Bestellzahlinformationen.

>[!NOTE]
>
> Es kann bis zu fünf Minuten dauern, bis Auftragsaktualisierungen mit synchronisiert werden. [!DNL Walmart Marketplace]. Um den Bestellstatus zu überprüfen, kehren Sie zum [!DNL Channel Manager] Bestellseite.

## Auftrag versenden

1. Wählen Sie im Admin die Option **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. Öffnen Sie die Store-Ansicht, indem Sie das Augensymbol für einen Verkaufskanalspeicher auswählen.

1. Zur Ansicht [!DNL Walmart Marketplace] Bestellungen, auswählen *[!UICONTROL *Orders]**.

1. Öffnen Sie in der Tabelle Bestellungen die Versandreihenfolge durch Auswahl der **Commerce-Bestellnummer**.

1. Erstellen und Senden einer Sendung für die gesamte Bestellung oder einen Teil davon durch Auswahl von **[!UICONTROL Ship]**.

   ![Detailansicht einer Commerce-Bestellung für [!DNL Walmart Marketplace] order](assets/order-detail-with-external-order-id.png)

   * Wählen Sie einen Versandunternehmen aus und fügen Sie eine Trackingnummer hinzu, indem Sie **[!UICONTROL Add tracking number]**.

      ![Detailansicht einer Commerce-Bestellung für [!DNL Walmart Marketplace] order](assets/order-shipment-add-tracking-number.png)


   * Füllen Sie nach Bedarf den Rest des Versandformulars aus. Siehe [[!DNL Shipping an Order]](https://docs.magento.com/user-guide/sales/order-ship.html) für detaillierte Anweisungen.

1. Verfolgen Sie nach der Übermittlung der Sendung die [Bestellstatus](manage-orders.md#about-order-status) in [!DNL Channel Manager] , um zu überprüfen, ob Aktualisierungen an [!DNL Walmart Marketplace].

## Abbrechen einer Bestellung

1. Wählen Sie im Admin die Option **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. Öffnen Sie die Store-Ansicht, indem Sie das Augensymbol für einen Verkaufskanalspeicher auswählen.

1. Zur Ansicht [!DNL Walmart Marketplace] Bestellungen, auswählen *[!UICONTROL *Orders]**.

1. Öffnen Sie in der Bestelltabelle die Detailseite der Bestellung, indem Sie die **Commerce-Bestellnummer** für die Bestellung zum Abbrechen.

   ![Detailansicht einer Commerce-Bestellung für[!DNL Walmart Marketplace]order](assets/order-detail-with-external-order-id.png)

1. Abbrechen der Bestellung.

   * Auswählen **Abbrechen** über das Menü Bestelldetails .

   * Im [!UICONTROL Cancel Order] Wählen Sie das **Abbruchsgrund**.
   ![Detailansicht einer Commerce-Bestellung für [!DNL Walmart Marketplace] order](assets/cancel-order-reason-selector.png)

   * Auswählen **Reihenfolge abbrechen**.


1. Verfolgen Sie nach dem Absenden des Abbruchs die [Bestellstatus](manage-orders.md#about-order-status) in [!DNL Channel Manager] , um zu überprüfen, ob Aktualisierungen an [!DNL Walmart Marketplace].
