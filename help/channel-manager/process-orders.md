---
title: Verarbeitungsaufträge
description: Versandanleitung und Stornierung [!DNL Walmart Marketplace] Bestellungen von Adobe Commerce und Magento Open Source.
source-git-commit: 5670639697550b2d7fee67dd29be9c6278d5782b
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Verarbeitungsaufträge

Wenn Sie Adobe Commerce und die Magento Open Source Order Management verwenden, um Ihre [!DNL Commerce] Verkaufsstellen, verarbeiten Sie [!DNL Walmart Marketplace] Bestellungen aus Commerce mit einem ähnlichen Workflow.

Wenn Sie eine Bestellung in Commerce verarbeiten, synchronisiert der Kanal-Manager Aktualisierungen in [!DNL Walmart Marketplace]. Diese Aktualisierung stellt sicher, dass der Produktbestand und der Bestellstatus aus Commerce mit den in der [!DNL Walmart Marketplace] und benachrichtigt Walmart, den Bestellstatus und Versandinformationen an Kunden zu senden.

>[!NOTE]
>
> Es kann bis zu fünf Minuten dauern, bis die Auftragsaktualisierungen mit synchronisiert werden. [!DNL Walmart Marketplace]. Um den Bestellstatus zu überprüfen, kehren Sie zu [!DNL Channel Manager] Bestellungen.

## Auftrag versenden

Wenn Sie eine Bestellung aus Commerce versenden, verwenden Sie die [[!DNL Commerce Order Management] Versandworkflow](https://docs.magento.com/user-guide/sales/order-ship.html). Nachdem Sie die Bestellung übermittelt haben, werden die Aktualisierungen mit [!DNL Walmart Marketplace]. Anschließend informiert Walmart die Kunden über den Bestellstatus und die Versanddetails.

**Voraussetzung**

Überprüfen Sie vor dem Versand der Bestellungen, ob die [Versandeinstellungen für Kanäle und Betreiberkonfiguration](map-shipping-carriers.md) erfüllen [!DNL Walmart Marketplace requirements].

### Versand erstellen und einreichen

Wenn Sie eine [!DNL Walmart Marketplace] Bestellung von [!DNL Commerce]müssen Sie eine Trackingnummer hinzufügen. Kunden erhalten die Trackingnummer in der Versandbenachrichtigung, von der sie empfangen [!DNL Walmart].

1. Wählen Sie im Admin die Option **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** , um [!UICONTROL Channel Manager Marketplace Stores] Seite.

1. Öffnen Sie die Store-Ansicht, indem Sie das Augensymbol für einen Verkaufskanalspeicher auswählen.

1. Zur Ansicht [!DNL Walmart Marketplace] Bestellungen, auswählen *[!UICONTROL *Orders]**.

1. Öffnen Sie in der Tabelle Bestellungen die Versandreihenfolge durch Auswahl der **Commerce-Bestellnummer**.

1. Erstellen und Senden einer Sendung für die gesamte Bestellung oder einen Teil davon durch Auswahl von **[!UICONTROL Ship]**.

   - Um einen Versandunternehmen auszuwählen und eine Trackingnummer hinzuzufügen, wählen Sie **[!UICONTROL Add tracking number]**.

   - Füllen Sie nach Bedarf den Rest des Versandformulars aus. Siehe [[!DNL Shipping an Order]](https://docs.magento.com/user-guide/sales/order-ship.html) für detaillierte Anweisungen.

1. Verfolgen Sie nach der Übermittlung der Sendung die [Bestellstatus](manage-orders.md#about-order-status) in [!DNL Channel Manager] , um zu überprüfen, ob Aktualisierungen an [!DNL Walmart Marketplace].

## Abbrechen einer Bestellung

Wenn Sie eine [!DNL Walmart Marketplace] Bestellung, Walmart benötigt einen Stornierungsgrund. Wenn die Stornierung der Bestellung auf Walmart aktualisiert wird, ist der Stornierungsgrund in der an den Kunden gesendeten Stornierungsmeldung enthalten.

Der Stornogrund wird auch im Abschnitt [!DNL Commerce] Bestellzahlinformationen.

1. Wählen Sie im Admin die Option **[!UICONTROL Marketing]** > **[!UICONTROL Channel Manager]** , um [!UICONTROL Channel Manager Marketplace Stores] Seite.

1. Öffnen Sie die Store-Ansicht, indem Sie das Augensymbol für einen Verkaufskanalspeicher auswählen.

1. Zur Ansicht [!DNL Walmart Marketplace] Bestellungen, auswählen *[!UICONTROL *Orders]**.

1. Öffnen Sie in der Bestelltabelle die Detailseite der Bestellung, indem Sie die **Commerce-Bestellnummer** für die Bestellung zum Abbrechen.

   ![Commerce Order detail view for a Walmart Marketplace order](assets/order-detail-with-external-order-id.png)

1. Abbrechen der Bestellung.

   - Auswählen **Abbrechen** über das Menü Bestelldetails .

   - Wählen Sie im Formular &quot;Reihenfolge abbrechen&quot;die Option **Abbruchsgrund**.

      ![Commerce Order detail view for a Walmart Marketplace order](assets/order-detail-with-external-order-id.png)

   - Auswählen **Reihenfolge abbrechen**.

1. Überprüfen, ob Aktualisierungen an gesendet wurden [!DNL Walmart Marketplace] durch Überprüfung der [Bestellstatus](manage-orders.md#about-order-status) in [!DNL Channel Manager].
