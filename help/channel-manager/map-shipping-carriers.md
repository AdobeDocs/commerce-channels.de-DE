---
title: Versandunternehmen zuordnen
description: '''Zuordnen von Attributen zum Abgleich [DNL! Commerce]-Produkte in bestehende [!DNL Walmart Marketplace] Auflistungen aufnehmen und Daten zwischen [!DNL Channel Manager] und [!DNL Walmart] synchronisieren.'
role: Admin
feature: Sales Channels, Configuration, Shipping/Delivery
exl-id: 98c8d3f6-f129-43c6-920c-d9c36b0e4a40
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---


# Versandunternehmen zuordnen

Bevor Sie [Bestellaufträge](process-orders.md#ship-an-order) für [!DNL Walmart Marketplace] Bestellungen verarbeiten, ordnen Sie die von Walmart bevorzugten Versandunternehmen dem entsprechenden Beförderer in [!DNL Commerce] zu, damit die Versanddaten zwischen [!DNL Walmart] und [!DNL Commerce] synchronisiert werden können.

Commerce-Träger, die keinem bevorzugten Träger zugeordnet sind, werden unter [!DNL Walmart] als *[!UICONTROL Other Carrier]* gekennzeichnet.

**Voraussetzungen**

Führen Sie vor der Zuordnung von Versandunternehmen die folgenden Aufgaben aus:

1. Überprüfen Sie die [Betreibermethoden und Best Practices für den Versand während der On-Time-Bereitstellung](https://sellerhelp.walmart.com/s/guide?article=000009473) für [!DNL Walmart Marketplace].

1. Überprüfen Sie die Konfigurationen [[!UICONTROL Shipping Carrier]](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/delivery/shipping-carriers/carriers.html) und [[!UICONTROL Shipping Settings]](https://experienceleague.adobe.com/docs/commerce-admin/config/sales/shipping-settings.html) in Ihrem [!DNL Commerce]-Speicher, um sicherzustellen, dass Sie die Konfiguration für [!DNL Walmart Marketplace sales] optimiert haben.

## Versandunternehmen zuordnen

1. Wählen Sie auf der Seite **[!UICONTROL Listings]** oder **[!UICONTROL Orders]** die Option **[!UICONTROL Channel Settings]** aus.

1. Wählen Sie auf **[!UICONTROL Channel Settings]** **[!UICONTROL Shipping Carriers]** aus.

   ![Versandunternehmen zuordnen](assets/map-shipping-carriers.png){width="600" zoomable="yes"}

1. Wählen Sie für jeden aufgelisteten [!DNL Walmart] bevorzugten Netzbetreiber den Namen des [!DNL Commerce] Netzbetreibers aus der Dropdown-Liste aus, wenn der Netzbetreiber verfügbar ist.

1. Wählen Sie **[!UICONTROL Save]** aus, um die Konfiguration anzuwenden.

