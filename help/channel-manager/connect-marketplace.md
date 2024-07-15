---
title: 'Connect [!DNL Channel Manager] to [!DNL Walmart Marketplace]'
description: "Verbinden Sie eine Commerce Store-Ansicht mit [!DNL Walmart Marketplace] , um den Vertriebskanal zur Verwaltung von Commerce-Produktlisten, -Beständen, -preisen und -Bestellungen für Walmart Marketplace-Verkäufe zu erstellen."
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
role: Admin, Developer
feature: Sales Channels, Install, Integration
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# [!DNL Channel Manager] mit [!DNL Walmart Marketplace] verbinden

Nachdem Sie den Kanal-Manager auf Ihrer [!DNL Commerce] -Instanz installiert haben, erstellen Sie einen Vertriebskanal im Kanal-Manager und konfigurieren Sie die Anmeldeinformationen, um [!DNL Channel Manager] mit [!DNL Walmart Marketplace] zu verbinden.

1. [Erstellen Sie den Verkaufskanal](#create-the-sales-channel), indem Sie den [!DNL Commerce] -Speicher für Produktlisten auswählen.

1. [Verbinden Sie den Kanal mit  [!DNL Walmart Marketplace] durch Hinzufügen von [!UICONTROL Walmart API credentials]](#connect-the-channel-to-walmart-marketplace).

1. [Führen Sie die Einrichtung des Vertriebskanals](#complete-sales-channel-store-setup) durch, um Auflistungen, Inventar, Preise und Bestellungen für Ihr [!DNL Walmart Marketplace] -Produktportfolio zu verwalten.

>[!NOTE]
>
>Der Kanal-Manager erfordert eine Eins-zu-Eins-Verbindung zwischen einem Walmart-Konto und einer [!DNL Commerce] Store-Ansicht. Dieselbe Store-Ansicht kann nicht mit mehreren Walmart-Konten verbunden werden.

## Erstellen des Vertriebskanals

1. Öffnen Sie im Admin [!DNL Channel Manager] durch Auswahl von **[!UICONTROL Marketing** > _Kanäle _> &quot;Kanal-Manager]**&quot;.

1. Wählen Sie im Abschnitt **[!UICONTROL Marketplaces available to connect]** die Option **[!UICONTROL Get Started]** aus.

   ![Verbinden des neuen [!DNL Walmart] Stores mit [!DNL Channel Manager]](assets/channel-manager-home.png){width="700" zoomable="yes"}

1. Richten Sie bei Bedarf Ihr [!DNL Walmart Marketplace Seller] -Konto ein.

1. Konfigurieren Sie den Speicher und die Verbindung:

   - Wählen Sie **[!UICONTROL Add Credentials]** aus.

   - Wählen Sie die Store-Ansicht [!DNL Commerce] aus, die die Produkte anbietet, die Sie auf dem Marketplace verkaufen möchten.

     ![Konfigurieren der Verbindung zwischen [!DNL Commerce] und [!DNL Walmart Marketplace] von [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png){width="500" zoomable="yes"}

   - Geben Sie eine eindeutige **[!UICONTROL store name]** ein.

   - Wählen Sie den Wert **[!UICONTROL Adobe [!DNL Commerce] site]** für Produktlisten und Auftragsverarbeitung aus.

   - Um Benachrichtigungen zu [!DNL Channel Manager] zu erhalten, fügen Sie einen **[!UICONTROL email address]** hinzu.

1. Verbinden Sie den Kanal mit [!DNL Walmart Marketplace].

   - Fügen Sie die Anmeldeinformationen für die [[!DNL Walmart Marketplace Adobe Production API key]](walmart-requirements.md#generate-a-walmart-marketplace-production-api-key) aus Ihrem [!DNL Walmart Marketplace Seller] -Konto hinzu.

   - Wenn Sie nicht über die Anmeldeinformationen verfügen, rufen Sie sie aus dem [!DNL Walmart Marketplace Developer Portal] ab, indem Sie **[!UICONTROL Get API credentials]** auswählen.

     Wählen Sie im Entwicklerportal Ihre Region (USA und Kanada) aus und melden Sie sich dann an.

     ![[!DNL Walmart Marketplace] Kontoanmeldung](assets/walmart-marketplace-login-page.png){width="600"}

   - Kopieren Sie im Formular für den API-Schlüssel die Werte **[!UICONTROL Client ID]** und **[!UICONTROL Client Secret]** für [!UICONTROL Adobe Inc Production API key] und speichern Sie sie an einem sicheren Speicherort.

     ![[!DNL Walmart Marketplace API key] Konfigurationsseite](assets/walmart-api-key-management-form.png){width="600" zoomable="yes"}

     >[!NOTE]
     >
     >Wenn der Schlüssel [!DNL Adobe Inc] nicht im Entwicklerportal aufgeführt ist, wählen Sie **[!UICONTROL Add New Key for a Solution Provider]** aus, um Berechtigungen zu konfigurieren und den Schlüssel zu generieren. Weitere Informationen zur Konfiguration finden Sie unter [Generate a [!DNL Walmart Marketplace API Key]](walmart-requirements.md#generate-a-walmart-marketplace-api-key).

   - Kehren Sie zu [!DNL Channel Manager] zurück, um die Anmeldeinformationen zu den **[!UICONTROL Walmart Connection]** -Informationen hinzuzufügen.

     Wenn Sie Anmeldeinformationen hinzufügen, blendet Adobe das Client-Geheimnis aus und speichert den Wert in einem sicheren Vault.

1. Wählen Sie **[!UICONTROL Save Store]** aus, um die Konfiguration anzuwenden und eine Verbindung zum [!DNL Walmart marketplace] herzustellen.

1. Nachdem Sie die Verbindung erfolgreich hergestellt haben, schließen Sie [die Store-Einrichtung ](complete-sales-channel-store-setup.md) von der **[!UICONTROL Channel Manager]** -Store-Seite ab.

![Einrichten des ersten Stores](assets/channel-manager-setup-first-store.png){width="500" zoomable="yes"}

### Fehlerbehebung bei Verbindungsproblemen

Wenn die Verbindung zu [!DNL Walmart] fehlschlägt, finden Sie Tipps zur Fehlerbehebung in den [Häufig gestellten Fragen zu Walmart Marketplace](https://developer.walmart.com/faq/us/faq-auth/){target="_blank"} .

- Überprüfen Sie anhand der [!DNL Walmart Developer Portal] , ob Sie die richtigen Anmeldeinformationen für den Produktions-API-Schlüssel für [!UICONTROL Adobe Inc.] kopiert haben.

- Stellen Sie sicher, dass die Zugriffskonfiguration für die [!UICONTROL Walmart Adobe API key] über die richtigen Berechtigungen verfügt. Siehe [[!DNL Walmart Requirements]](walmart-requirements.md##generate-a-walmart-marketplace-api-key).

- Vergewissern Sie sich, dass der Dienst [!DNL Walmart API] auf der [Walmart API-Statusseite](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target="_blank"} verfügbar ist.
