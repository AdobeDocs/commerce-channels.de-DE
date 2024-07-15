---
title: Verwalten der Walmart Marketplace-Verbindung
description: '''Aktualisieren Sie die API-Anmeldeinformationen, um die Verbindung zwischen einem [DNL! Commerce] Store-Ansicht und die [!DNL Walmart Marketplace]. The connection is required to connect [!DNL Commerce] Produktlisten sowie Bestands-, Preis-, Bestell- und Versanddaten zwischen [!DNL Commerce]  und Walmart synchronisieren.'
role: Admin, Developer
feature: Sales Channels, Configuration, Shipping/Delivery, Integration
exl-id: 817b1b58-a57e-4c8d-b08f-1ce3bec15bc3
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# Versandunternehmen zuordnen

Bevor Sie [Bestellaufträge](process-orders.md#ship-an-order) für [!DNL Walmart Marketplace] Bestellungen verarbeiten, ordnen Sie die von Walmart bevorzugten Versandunternehmen dem entsprechenden Beförderer in [!DNL Commerce] zu, damit die Versanddaten zwischen [!DNL Walmart] und [!DNL Commerce] synchronisiert werden können.

Commerce-Träger, die keinem bevorzugten Träger zugeordnet sind, werden unter [!DNL Walmart] als *[!UICONTROL Other Carrier]* gekennzeichnet.

**Voraussetzungen**

Überprüfen Sie die [Walmart-Anforderungen](walmart-requirements.md) für die [!DNL Marketplace Seller account].

## Verbindungsberechtigungen aktualisieren

1. Wählen Sie auf der Seite [!UICONTROL Listings] für den Verkaufskanalspeicher **[!UICONTROL Channel Settings]** aus.

1. Wählen Sie auf **[!UICONTROL Channel Settings]** **[!UICONTROL Walmart Connection]** aus.

1. Um die Anmeldeinformationen zu ändern, wählen Sie **[!UICONTROL Change Credentials]** aus.

   ![Aktualisieren Sie die Anmeldeinformationen der Walmart-API, um die Verbindung zu autorisieren](assets/update-connection-credentials.png){width="700" zoomable="yes"}

1. Geben Sie die Werte **[!UICONTROL Walmart Client ID]** und **[!UICONTROL Walmart Client Secret]** ein.

1. Wählen Sie **[!UICONTROL Save]** aus, um die Konfiguration anzuwenden.
