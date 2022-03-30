---
title: Sales Channel verbinden mit [!DNL Walmart Marketplace]
description: Konfigurieren Sie den Vertriebskanal und verbinden Sie sich mit dem Walmart Marketplace.
exl-id: 8c78c582-7b57-4f73-894e-134ba0ba3640
source-git-commit: 8f07b215c20cc28aa9a6862bcb2b00da30a1ed84
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---


# Verbinden mit [!DNL Walmart Marketplace]

Nach der Installation von Channel Manager auf Ihrer [!DNL Commerce] z. B. einen Commerce-Store mit dem Walmart Marketplace verbinden.

1. Erstellen Sie den Vertriebskanal nach [Auswählen des Commerce-Stores für Produktlisten](#select-the-commerce-store-for-the-sales-channel).

1. [Verbinden Sie den Kanal mit [!DNL Walmart Marketplace] durch Hinzufügen von Walmart API-Anmeldeinformationen](#connect-the-channel-to-walmart-marketplace).

1. [Vollständige Einrichtung des Vertriebskanals](#complete-store-setup) damit Sie Auflistungen, Inventar, Preise und Verkäufe vom Channel Manager verwalten können.

## Erstellen des Vertriebskanals

1. Öffnen Sie den Kanal-Manager.

   - Wählen Sie im Admin die Option **[!UICONTROL Marketing** > _Kanäle _> **Kanal-Manager]**.

   - Auswählen **[!UICONTROL Connect New Store]**.

      ![Verbinden Sie den Commerce Store mit [!DNL Walmart Marketplace] von [!DNL Channel Manager]](assets/connect-commerce-store-to-marketplace.png)


1. Konfigurieren Sie den Speicher und die Verbindung:

   - Eindeutige Eingabe **[!UICONTROL store name]**.

   - Wählen Sie die **[!UICONTROL Adobe Commerce site]** für Produktlisten.

   - Hinzufügen einer **[!UICONTROL email address]** zum Empfang von Dienstbenachrichtigungen im Zusammenhang mit [!DNL Channel Manager].

      ![Verbindung zwischen Commerce und konfigurieren [!DNL Walmart Marketplace] von [!DNL Channel Manager]](assets/configure-commerce-to-marketplace-connection.png)


## Verbinden des Kanals mit dem Walmart Marketplace

1. Fügen Sie die Anmeldeinformationen für die [!DNL Walmart Marketplace Adobe Production API key] von [!DNL Walmart Marketplace Seller] -Konto.

   - Wenn Sie nicht über die Anmeldeinformationen verfügen, wählen Sie **[!UICONTROL Get API credentials]** um sie aus dem [!DNL Walmart Marketplace Developer Portal].

      Wählen Sie bei entsprechender Aufforderung Ihre Region (USA und Kanada) aus und melden Sie sich dann an.

      ![[!DNL Walmart Marketplace] Kontoanmeldung](assets/walmart-marketplace-login-page.png)

   - Kopieren Sie im Formular für den API-Schlüssel das **[!UICONTROL Client ID]** und **[!UICONTROL Client Secret]** -Werte für [!UICONTROL Adobe Inc Production API key] an einen sicheren Ort.

      ![[!DNL Walmart Marketplace API key] Konfigurationsseite](assets/walmart-api-key-management-form.png)

      >[!NOTE]
      >
      >Wenn die Variable [!DNL Adobe Inc] nicht im Entwicklerportal aufgeführt ist, wählen Sie **[!UICONTROL Add New Key for a Solution Provider]** um Berechtigungen zu konfigurieren und den Schlüssel zu generieren. Weitere Informationen zur Konfiguration finden Sie unter [Generieren Sie eine [!DNL Walmart Marketplace API Key]](walmart-prerequisites.md#generate-a-walmart-marketplace-api-key).

   - Zurück zu [!DNL Channel Manager] , um die Anmeldeinformationen zum **[!UICONTROL Walmart Connection]** Informationen.

      Wenn Sie Anmeldeinformationen zu [!DNL Channel Manager], blendet Adobe das Client-Geheimnis aus und speichert den Wert in einem sicheren Vault.

1. [!UICONTROL Save] die Konfiguration, um die Verbindung herzustellen.

   Nachdem Sie die Verbindung erfolgreich hergestellt haben, verwalten Sie den Kanal über **[!UICONTROL Channel Manager > Marketplace Stores]**.

   ![[!DNL Walmart Marketplace API key] Konfigurationsseite](assets/manage-connected-stores.png)


### Beheben von Verbindungsproblemen

Wenn die Verbindung zu Walmart fehlschlägt, lesen Sie den Abschnitt [Häufig gestellte Fragen zu Walmart Marketplace](https://developer.walmart.com/faq/us/faq-auth/){target=&quot;_blank&quot;} für Tipps zur Fehlerbehebung.

- Aus dem [!DNL Walmart Developer Portal], überprüfen Sie, ob Sie die richtigen Anmeldeinformationen für den Produktions-API-Schlüssel für [!UICONTROL Adobe Inc.]

- Stellen Sie sicher, dass die Zugriffskonfiguration für den API-Schlüssel der Walmart-Adobe über die richtigen Berechtigungen verfügt. Siehe [Walmart-Voraussetzungen](walmart-prerequisites.md##generate-a-walmart-marketplace-api-key).

- Vergewissern Sie sich, dass der Walmart-API-Dienst im [Walmart-API-Statusseite](https://developer.walmart.com/us/whats-new/new-api-status-information-now-available/){target=&quot;_blank&quot;}.