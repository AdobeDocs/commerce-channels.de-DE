---
title: Versandunternehmen zuordnen
description: 'Zuordnen von Attributen zum Abgleich [DNL! Commerce-] Produkte in bestehende [!DNL Walmart Marketplace] Auflistungen und Daten synchronisieren zwischen [!DNL Channel Manager] und [!DNL Walmart].'
role: Admin
feature: Sales Channels, Configuration, Shipping/Delivery
exl-id: 98c8d3f6-f129-43c6-920c-d9c36b0e4a40
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---


# Versandunternehmen zuordnen

Vorher [Versand von Prozessbestellungen](process-orders.md#ship-an-order) für [!DNL Walmart Marketplace] Aufträge, die von Walmart bevorzugte Reederei dem entsprechenden Beförderer in [!DNL Commerce] damit die Versanddaten zwischen [!DNL Walmart] und [!DNL Commerce].

Handelsunternehmen, die keinem bevorzugten Netzbetreiber zugeordnet sind, werden als *[!UICONTROL Other Carrier]* on [!DNL Walmart].

**Voraussetzungen**

Führen Sie vor der Zuordnung von Versandunternehmen die folgenden Aufgaben aus:

1. Überprüfen Sie die [Versandmethoden und Best Practices für die On-Time-Bereitstellung](https://sellerhelp.walmart.com/s/guide?article=000009473) für [!DNL Walmart Marketplace].

1. Überprüfen Sie die [[!UICONTROL Shipping Carrier]](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/delivery/shipping-carriers/carriers.html) und [[!UICONTROL Shipping Settings]](https://experienceleague.adobe.com/docs/commerce-admin/config/sales/shipping-settings.html) Konfiguration in Ihrem [!DNL Commerce] speichern, um sicherzustellen, dass Sie die Konfiguration für [!DNL Walmart Marketplace sales].

## Versandunternehmen zuordnen

1. Aus dem **[!UICONTROL Listings]** oder **[!UICONTROL Orders]** Seite, auswählen **[!UICONTROL Channel Settings]**.

1. on **[!UICONTROL Channel Settings]** auswählen **[!UICONTROL Shipping Carriers]**.

   ![Versandunternehmen zuordnen](assets/map-shipping-carriers.png){width="600" zoomable="yes"}

1. Für jeden [!DNL Walmart] Der bevorzugte Anbieter wird aufgelistet, wählen Sie die [!DNL Commerce] Betreibername aus der Dropdown-Liste, wenn der Netzbetreiber verfügbar ist.

1. Auswählen **[!UICONTROL Save]** , um die Konfiguration anzuwenden.

