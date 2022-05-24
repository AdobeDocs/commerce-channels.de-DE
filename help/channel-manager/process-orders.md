---
title: Verarbeitungsaufträge
description: Versandanleitung und Stornierung [!DNL Walmart Marketplace] Bestellungen von Adobe Commerce und Magento Open Source.
source-git-commit: 90ccbecd6d1433ae1312d79f7ae2d34c8f381b97
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# Verarbeitungsaufträge

Wenn Sie Adobe Commerce und die Magento Open Source Order Management verwenden, um Ihre [!DNL Commerce] Storeverkäufe, Prozesse [!DNL Walmart Marketplace] Bestellungen aus Commerce mit einem ähnlichen Workflow.

Wenn Sie eine Bestellung in Commerce verarbeiten, synchronisiert der Kanal-Manager Aktualisierungen in [!DNL Walmart Marketplace]. Durch diese Aktualisierung wird sichergestellt, dass der Auftragsstatus und die Versandinformationen aus Commerce mit den in der Variablen [!DNL Walmart Marketplace].

* **Auftragsversand**-Walmart benötigt eine Trackingnummer für alle Sendungen. Wenn die Lagermenge nicht ausreicht, um eine ganze Bestellung zu bestellen, erstellen Sie eine Teillieferung. Nach Absendung der Sendung werden die Auftragsaktualisierungen mit [!DNL Walmart Marketplace]. Anschließend informiert Walmart die Kunden über den Bestellstatus und die Versanddetails.

* **Stornierungen von Bestellungen**-Wenn Sie eine [!DNL Walmart Marketplace] Bestellung, Walmart benötigt einen Stornierungsgrund. Der Stornierungsgrund ist in der an den Kunden gesendeten Stornierungsmeldung enthalten. Der Stornogrund wird auch im Abschnitt [!DNL Commerce] Bestellzahlinformationen.

>[!NOTE]
>
> Es kann bis zu fünf Minuten dauern, bis Auftragsaktualisierungen mit synchronisiert werden. [!DNL Walmart Marketplace]. Um den Bestellstatus zu überprüfen, kehren Sie zum [!DNL Channel Manager] Bestellseite.

## Auftrag versenden

1. Wählen Sie im Admin die Option **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. Öffnen Sie die Store-Ansicht, indem Sie das Augensymbol für einen Verkaufskanalspeicher auswählen.

1. Zur Ansicht [!DNL Walmart Marketplace] Bestellungen, auswählen *[!UICONTROL *Orders]**.

1. Öffnen Sie in der Tabelle Bestellungen die Versandreihenfolge durch Auswahl der **Commerce-Bestellnummer**.

1. Erstellen und Senden einer Sendung für die gesamte Bestellung oder einen Teil davon durch Auswahl von **[!UICONTROL Ship]**.

   ![Commerce Order detail view for a Walmart Marketplace order](assets/order-detail-with-external-order-id.png)

   * Um einen Versandunternehmen auszuwählen und eine Trackingnummer hinzuzufügen, wählen Sie **[!UICONTROL Add tracking number]**.

   * Füllen Sie nach Bedarf den Rest des Versandformulars aus. Siehe [[!DNL Shipping an Order]](https://docs.magento.com/user-guide/sales/order-ship.html) für detaillierte Anweisungen.

1. Verfolgen Sie nach der Übermittlung der Sendung die [Bestellstatus](manage-orders.md#about-order-status) in [!DNL Channel Manager] , um zu überprüfen, ob Aktualisierungen an [!DNL Walmart Marketplace].

## Abbrechen einer Bestellung

1. Wählen Sie im Admin die Option **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]**.

1. Öffnen Sie die Store-Ansicht, indem Sie das Augensymbol für einen Verkaufskanalspeicher auswählen.

1. Zur Ansicht [!DNL Walmart Marketplace] Bestellungen, auswählen *[!UICONTROL *Orders]**.

1. Öffnen Sie in der Bestelltabelle die Detailseite der Bestellung, indem Sie die **Commerce-Bestellnummer** für die Bestellung zum Abbrechen.

![Commerce Order detail view for a Walmart Marketplace order](assets/order-detail-with-external-order-id.png)

1. Abbrechen der Bestellung.

   * Auswählen **Abbrechen** über das Menü Bestelldetails .

   * Im [!UICONTROL Cancel Order] Wählen Sie das **Abbruchsgrund**.

   ![Commerce Order detail view for a Walmart Marketplace order](assets/cancel-order-reason-selector.png)

   * Auswählen **Reihenfolge abbrechen**.


1. Überprüfen, ob Aktualisierungen an gesendet wurden [!DNL Walmart Marketplace] durch Überprüfung der [Bestellstatus](manage-orders.md#about-order-status) in [!DNL Channel Manager].
