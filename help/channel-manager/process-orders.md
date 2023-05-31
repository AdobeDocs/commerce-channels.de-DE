---
title: Prozessaufträge
description: "Hinweise für Versand und Stornierung [!DNL Walmart Marketplace] Bestellungen von Adobe Commerce und Magento Open Source."
exl-id: 2fdcb348-5c02-464f-a114-16ec657bed6b
source-git-commit: a3ae579c0eda0c27bf8eab9d0ac12919eaad494b
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Prozessaufträge

Nachher [!DNL Walmart Marketplace] Bestellungen wurden bestätigt und erfolgreich an gesendet [!DNL Channel Manager], verwenden Sie [Commerce Order Management](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#orders-workspace) , um die Bestellung zu verarbeiten.

Der Kanal-Manager synchronisiert Aktualisierungen mit [!DNL Walmart Marketplace] sicherstellen, dass der Auftragsstatus und die Versandinformationen von [!DNL Commerce] entspricht den in der [!DNL Walmart Marketplace].

* **Auftragsversand**-Walmart benötigt eine Trackingnummer für alle Sendungen. Wenn einige Artikel nicht vorrätig sind, können Sie Teillieferungen erstellen, um derzeit verfügbare Artikel zu senden. Nach Absendung der Sendung werden die Auftragsaktualisierungen mit [!DNL Walmart Marketplace]. Anschließend informiert Walmart die Kunden über den Bestellstatus und die Versanddetails.

* **Stornierungen von Bestellungen**-Wenn Sie eine [!DNL Walmart Marketplace] Bestellung, Walmart benötigt einen Stornierungsgrund, der in der an den Kunden gesendeten Stornierungsmeldung enthalten ist. Der Stornogrund wird auch im Abschnitt [!DNL Commerce] Bestellzahlinformationen. Nachdem Sie den Abbruch gesendet haben, werden Bestandsaktualisierungen mit synchronisiert. [!DNL Walmart Marketplace]. Anschließend informiert Walmart die Kunden über den Bestellstatus und die Versanddetails.

   In der Storefront müssen Sie die gesamte Bestellung stornieren. [!DNL Commerce] lässt keine teilweisen Stornierungen zu.

* **Erstattungsantrag**-Wenn eine Walmart Marketplace-Rückgabe für eine versandte Bestellung angefordert wird, wird die [!UICONTROL Status details] enthält einen Link zur Rückkehr. Die Rückgaben und Erstattungen werden über das [Rückgabe](return-refund-orders.md) Dashboard.

Bei der Verarbeitung von Commerce-Bestellungen und [!DNL Channel Manager] Synchronisiert erfolgreich Versand-, Teillieferungs- und Löschaktualisierungen der [!DNL Walmart Marketplace], ist die Auftragsverarbeitung abgeschlossen. Rücksendungsanträge und Erstattungen für versandte Bestellungen werden über das [Rückgabe](return-refund-orders.md) Dashboard.

>[!NOTE]
>
> Es kann bis zu fünf Minuten dauern, bis Auftragsaktualisierungen mit synchronisiert werden. [!DNL Walmart Marketplace]. Um den Bestellstatus zu überprüfen, kehren Sie zum [!DNL Channel Manager] Bestellseite.

## Auftrag versenden

1. Wählen Sie im Admin die Option **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. Öffnen Sie die Store-Ansicht, indem Sie das Augensymbol für einen Verkaufskanalspeicher auswählen.

1. Zur Ansicht [!DNL Walmart Marketplace] Bestellungen, auswählen **[!UICONTROL Orders]**.

1. Öffnen Sie in der Tabelle Bestellungen die Versandreihenfolge durch Auswahl der **[!UICONTROL Commerce Order Number]**.

1. Erstellen und Senden einer Sendung für die gesamte Bestellung oder einen Teil davon durch Auswahl von **[!UICONTROL Ship]**.

   ![Detailansicht einer Commerce-Bestellung für [!DNL Walmart Marketplace] order](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

   * Wählen Sie einen Versandunternehmen aus und fügen Sie eine Trackingnummer hinzu, indem Sie **[!UICONTROL Add tracking number]**.

      ![Detailansicht einer Commerce-Bestellung für [!DNL Walmart Marketplace] order](assets/order-shipment-add-tracking-number.png){width="600" zoomable="yes"}

   * Füllen Sie nach Bedarf den Rest des Versandformulars aus. Siehe [[!DNL Shipping an Order]](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-ship.html) für detaillierte Anweisungen.

1. Verfolgen Sie nach der Übermittlung der Sendung die [Bestellstatus](manage-orders.md#about-order-status) in [!DNL Channel Manager] , um zu überprüfen, ob Aktualisierungen an [!DNL Walmart Marketplace].

Nach dem Versand einer Bestellung können Sie die vollständige oder teilweise Rückerstattung von [!DNL Channel Manager] für Artikel, die in der Bestellung auf der Grundlage von Rückgabeanfragen von [!DNL Walmart Marketplace]. Siehe [Rückgabe- und Erstattungsanordnungen](return-refund-orders.md).

## Abbrechen einer Bestellung

1. Wählen Sie im Admin die Option **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. Öffnen Sie die Store-Ansicht, indem Sie das Augensymbol für einen Verkaufskanalspeicher auswählen.

1. Zur Ansicht [!DNL Walmart Marketplace] Bestellungen, auswählen *[!UICONTROL Orders]**.

1. Öffnen Sie in der Tabelle &quot;Bestellungen&quot;den [Bestelldetailseite](manage-orders.md#view-order-detail) durch Auswahl der **[!UICONTROL Commerce Order Number]** für die Bestellung zum Abbrechen.

   ![Detailansicht einer Commerce-Bestellung für[!DNL Walmart Marketplace]order](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

1. Abbrechen der Bestellung.

   * Auswählen **Abbrechen** über das Menü Bestelldetails .

   * Im [!UICONTROL Cancel Order] Wählen Sie das **[!UICONTROL Cancellation reason]**.
   ![Detailansicht einer Commerce-Bestellung für [!DNL Walmart Marketplace] order](assets/cancel-order-reason-selector.png){width="600" zoomable="yes"}

   * Auswählen **[!UICONTROL Cancel Order]**.


1. Verfolgen Sie nach dem Absenden des Abbruchs die [Bestellstatus](manage-orders.md#about-order-status) in [!DNL Channel Manager] , um zu überprüfen, ob Aktualisierungen an [!DNL Walmart Marketplace].

## Bestellfehler beheben

Fehler können während des Bestellsynchronisierungsprozesses von [!DNL Walmart Marketplace]oder während der Auftragsaktualisierung für Sendungen, Teillieferungen und Stornierungen.

Wenn der Synchronisierungsvorgang für eine Lieferung, eine teilweise Lieferung oder eine Löschung der Aktualisierung fehlschlägt, wird die [!DNL Channel Manager] Auf der Bestellseite wird eine _Fehler_ Status für die Bestellung. Um sicherzustellen, dass Versandinformationen und Auftragsstornierungsinformationen im Walmart Marketplace-Konto korrekt widergespiegelt werden, müssen Sie die Bestellung manuell in Ihrem [!DNL Walmart Marketplace] speichern.


