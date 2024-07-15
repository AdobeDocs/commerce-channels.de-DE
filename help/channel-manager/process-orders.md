---
title: Prozessaufträge
description: '''Anweisungen zum Versand und zur Stornierung [!DNL Walmart Marketplace] von Bestellungen von Adobe Commerce und Magento Open Source''.'
feature: Sales Channels, Orders, Shipping/Delivery, Customer Service
exl-id: 2fdcb348-5c02-464f-a114-16ec657bed6b
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# Prozessaufträge

Nachdem [!DNL Walmart Marketplace] Bestellungen quittiert und erfolgreich an [!DNL Channel Manager] gesendet wurden, verwenden Sie [Commerce Order Management](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html#orders-workspace), um die Bestellung zu verarbeiten.

Der Kanal-Manager synchronisiert Aktualisierungen auf [!DNL Walmart Marketplace], um sicherzustellen, dass der Bestellstatus und die Versandinformationen von [!DNL Commerce] mit den in der [!DNL Walmart Marketplace] verfolgten Daten übereinstimmen.

* **Bestellen von Sendungen**-Walmart benötigt eine Trackingnummer für alle Sendungen. Wenn einige Artikel nicht vorrätig sind, können Sie Teillieferungen erstellen, um derzeit verfügbare Artikel zu senden. Nach dem Absenden der Sendung werden die Bestellaktualisierungen mit [!DNL Walmart Marketplace] synchronisiert. Anschließend informiert Walmart die Kunden über den Bestellstatus und die Versanddetails.

* **Stornierungen von Bestellungen**-Wenn Sie eine [!DNL Walmart Marketplace] Bestellung stornieren, benötigt Walmart einen Stornierungsgrund, der in der an den Kunden gesendeten Stornierungsmeldung enthalten ist. Der Stornierungsgrund wird auch in den Bestellzahlungsinformationen von [!DNL Commerce] angezeigt. Nachdem Sie den Abbruch gesendet haben, werden Bestandsaktualisierungen mit [!DNL Walmart Marketplace] synchronisiert. Anschließend informiert Walmart die Kunden über den Bestellstatus und die Versanddetails.

  In der Storefront müssen Sie die gesamte Bestellung stornieren. [!DNL Commerce] lässt keine teilweisen Stornierungen zu.

* **Rückerstattungsanfrage** - Wenn eine Rückgabe von Walmart Marketplace für eine versandte Bestellung angefordert wird, enthält die [!UICONTROL Status details] einen Link zur Rückgabe. Die Rückgaben und Erstattungen werden über das Dashboard [Rückgaben](return-refund-orders.md) verwaltet.

Wenn Commerce-Bestellungen verarbeitet werden und [!DNL Channel Manager] Sendungen, Teillieferungen und Stornierungsaktualisierungen erfolgreich mit [!DNL Walmart Marketplace] synchronisiert, ist die Auftragsverarbeitung abgeschlossen. Rücksendungsanfragen und Rückerstattungen für versandte Bestellungen werden über das Dashboard [Rückgaben](return-refund-orders.md) verwaltet.

>[!NOTE]
>
> Es kann bis zu fünf Minuten dauern, bis Auftragsaktualisierungen mit [!DNL Walmart Marketplace] synchronisiert werden. Um den Bestellstatus zu überprüfen, kehren Sie zur Seite [!DNL Channel Manager] Bestellungen zurück.

## Auftrag versenden

1. Wählen Sie im Admin **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** aus.

1. Öffnen Sie die Store-Ansicht, indem Sie das Augensymbol für einen Verkaufskanalspeicher auswählen.

1. Um [!DNL Walmart Marketplace] Bestellungen anzuzeigen, wählen Sie **[!UICONTROL Orders]** aus.

1. Öffnen Sie in der Tabelle Bestellungen die auszustellende Reihenfolge durch Auswahl von **[!UICONTROL Commerce Order Number]**.

1. Erstellen und senden Sie eine Sendung für alle oder einen Teil einer Bestellung, indem Sie **[!UICONTROL Ship]** auswählen.

   ![Commerce Bestelldetailansicht für eine [!DNL Walmart Marketplace] Bestellung](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

   * Wählen Sie einen Versandunternehmen aus und fügen Sie eine Trackingnummer hinzu, indem Sie **[!UICONTROL Add tracking number]** auswählen.

     ![Commerce Bestelldetailansicht für eine [!DNL Walmart Marketplace] Bestellung](assets/order-shipment-add-tracking-number.png){width="600" zoomable="yes"}

   * Füllen Sie nach Bedarf den Rest des Versandformulars aus. Detaillierte Anweisungen finden Sie unter [[!DNL Shipping an Order]](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/order-ship.html) .

1. Verfolgen Sie nach dem Senden der Sendung den [Bestellstatus](manage-orders.md#about-order-status) in [!DNL Channel Manager], um zu überprüfen, ob Aktualisierungen an [!DNL Walmart Marketplace] gesendet wurden.

Nachdem eine Bestellung versandt wurde, können Sie die vollständigen oder teilweisen Rückerstattungen von [!DNL Channel Manager] für Artikel, die in der Bestellung enthalten sind, auf der Grundlage der von [!DNL Walmart Marketplace] empfangenen Rückgabeanfragen verarbeiten. Siehe [Rückgabe und Rückerstattung von Bestellungen](return-refund-orders.md).

## Abbrechen einer Bestellung

1. Wählen Sie im Admin **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** aus.

1. Öffnen Sie die Store-Ansicht, indem Sie das Augensymbol für einen Verkaufskanalspeicher auswählen.

1. Um [!DNL Walmart Marketplace] Bestellungen anzuzeigen, wählen Sie *[!UICONTROL Orders]**.

1. Öffnen Sie in der Tabelle &quot;Bestellungen&quot;die Detailseite [Bestellung](manage-orders.md#view-order-detail), indem Sie die Option **[!UICONTROL Commerce Order Number]** auswählen, damit die Bestellung abgebrochen werden kann.

   ![Commerce Bestelldetailansicht für eine [!DNL Walmart Marketplace]Bestellung](assets/order-detail-with-external-order-id.png){width="600" zoomable="yes"}

1. Abbrechen der Bestellung.

   * Wählen Sie **Abbrechen** aus dem Menü &quot;Bestelldetails&quot;.

   * Wählen Sie im Formular [!UICONTROL Cancel Order] den Wert **[!UICONTROL Cancellation reason]** aus.

   ![Commerce Bestelldetailansicht für eine [!DNL Walmart Marketplace] Bestellung](assets/cancel-order-reason-selector.png){width="600" zoomable="yes"}

   * Wählen Sie **[!UICONTROL Cancel Order]** aus.

1. Verfolgen Sie nach dem Absenden der Stornierung den [Bestellstatus](manage-orders.md#about-order-status) in [!DNL Channel Manager], um sicherzustellen, dass Aktualisierungen an [!DNL Walmart Marketplace] gesendet wurden.

## Bestellfehler beheben

Fehler können während des Synchronisierungsprozesses der Bestellung von [!DNL Walmart Marketplace] oder während der Bestellaktualisierung für Sendungen, Teillieferungen und Stornierungen auftreten.

Wenn der Synchronisierungsvorgang für eine Sendung, einen Teil der Sendung oder eine Aktualisierung der Löschung fehlschlägt, zeigt die Seite [!DNL Channel Manager] Bestellungen den Status _Fehler_ für die Bestellung an. Um sicherzustellen, dass Versandinformationen und Informationen zur Stornierung von Bestellungen im Walmart Marketplace -Konto korrekt widergespiegelt werden, aktualisieren Sie die Bestellung manuell in Ihrem [!DNL Walmart Marketplace] -Store.


