---
title: Verkaufskanal verbinden mit [!DNL Walmart Marketplace]
description: Konfigurieren Sie den Vertriebskanal und verbinden Sie sich mit dem Walmart Marketplace.
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
source-git-commit: aaab7aa7feb05264c24386e62193564dc5ae8fe3
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Verkaufskanal verbinden mit [!DNL Walmart Marketplace]

Nach der Installation von Channel Manager auf Ihrer [!DNL Commerce] Instanz, eine [!DNL Commerce] speichern in [!DNL Walmart Marketplace].

1. [Erstellen des Vertriebskanals](#create-the-sales-channel) durch Auswahl des Commerce-Stores für Produktlisten.

1. [Verbinden Sie den Kanal mit [!DNL Walmart Marketplace] durch Hinzufügen von [!UICONTROL Walmart API credentials]](#connect-the-channel-to-walmart-marketplace).

1. [Vollständige Einrichtung des Vertriebskanals](#complete-store-setup) zur Verwaltung von Listen, Beständen, Preisen und Bestellungen für Ihre [!DNL Walmart Marketplace] Produktsortiment.

## Erstellen des Vertriebskanals

1. Öffnen Sie über den Administrator [!DNL Channel Manager] durch Auswahl **[!UICONTROL Marketing** > _Kanäle _> **Kanal-Manager]**.

1. Im **[!UICONTROL Marketplaces available to connect]** Bereich, wählen Sie **[!UICONTROL Get Started]**.

   ![Neu verbinden [!DNL Walmart] speichern in [!DNL Channel Manager]](assets/channel-manager-home.png)

1. Richten Sie bei Bedarf Ihre [!DNL Walmart Marketplace Seller] -Konto.

1. Konfigurieren Sie den Speicher und die Verbindung:

   - Auswählen **[!UICONTROL Add Credentials]**.

   - Wählen Sie die [!DNL Commerce] Store-Ansicht, um eine Verbindung zum Marketplace herzustellen.

      ![Verbindung zwischen Commerce und konfigurieren [!DNL Walmart Marketplace] von [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png)

   - Eindeutige Eingabe **[!UICONTROL store name]**.

   - Wählen Sie die **[!UICONTROL Adobe Commerce site]** für Produktlisten.

   - Hinzufügen einer **[!UICONTROL email address]** zum Empfang von Dienstbenachrichtigungen im Zusammenhang mit [!DNL Channel Manager].

1. Verbinden Sie den Kanal mit [!DNL Walmart Marketplace].

   - Fügen Sie die Anmeldeinformationen für die [[!DNL Walmart Marketplace Adobe Production API key]](walmart-requirements.md#generate-a-walmart-marketplace-production-api-key) von [!DNL Walmart Marketplace Seller] -Konto.

   - Wenn Sie nicht über die Anmeldeinformationen verfügen, rufen Sie sie aus dem [!DNL Walmart Marketplace Developer Portal] durch Auswahl **[!UICONTROL Get API credentials]**.

      Wählen Sie im Entwicklerportal Ihre Region (USA und Kanada) aus und melden Sie sich dann an.

      ![[!DNL Walmart Marketplace] Kontoanmeldung](assets/walmart-marketplace-login-page.png)

   - Kopieren Sie im Formular für den API-Schlüssel das **[!UICONTROL Client ID]** und **[!UICONTROL Client Secret]** -Werte für [!UICONTROL Adobe Inc Production API key] an einen sicheren Ort.

      ![[!DNL Walmart Marketplace API key] Konfigurationsseite](assets/walmart-api-key-management-form.png)

      >[!NOTE]
      >
      >Wenn die Variable [!DNL Adobe Inc] nicht im Entwicklerportal aufgeführt ist, wählen Sie **[!UICONTROL Add New Key for a Solution Provider]** um Berechtigungen zu konfigurieren und den Schlüssel zu generieren. Weitere Informationen zur Konfiguration finden Sie unter [Generieren Sie eine [!DNL Walmart Marketplace API Key]](walmart-requirements.md#generate-a-walmart-marketplace-api-key).

   - Zurück zu [!DNL Channel Manager] , um die Anmeldeinformationen zum **[!UICONTROL Walmart Connection]** Informationen.

      Wenn Sie Anmeldeinformationen hinzufügen, blendet Adobe das Client-Geheimnis aus und speichert den Wert in einem sicheren Vault.

1. Auswählen **[!UICONTROL Save Store]** , um die Konfiguration anzuwenden und eine Verbindung zum [!DNL Walmart marketplace].

1. Nach erfolgreicher Verbindung [Komplette Store-Einrichtung](complete-store-setup.md) von **[!UICONTROL Channel Manager]** Store-Seite.

![Einrichten des ersten Stores](assets/channel-manager-setup-first-store.png)

### Beheben von Verbindungsproblemen

Wenn die Verbindung zu [!DNL Walmart] schlägt fehl, siehe [Häufig gestellte Fragen zu Walmart Marketplace](https://developer.walmart.com/faq/us/faq-auth/){target=&quot;_blank&quot;} für Tipps zur Fehlerbehebung.

- Aus dem [!DNL Walmart Developer Portal], überprüfen Sie, ob Sie die richtigen Anmeldeinformationen für den Produktions-API-Schlüssel für [!UICONTROL Adobe Inc.]

- Überprüfen Sie, ob die Zugriffskonfiguration für die [!UICONTROL Walmart Adobe API key] verfügt über die richtigen Berechtigungen. Siehe [[!DNL Walmart Requirements]](walmart-requirements.md##generate-a-walmart-marketplace-api-key).

- Vergewissern Sie sich, dass die [!DNL Walmart API] -Dienst ist im [Walmart-API-Statusseite](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target=&quot;_blank&quot;}.
