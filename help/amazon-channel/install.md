---
title: Installieren der [!DNL Amazon Sales Channel] Erweiterung
description: Laden Sie die Amazon-Sales Channel-Erweiterung herunter und installieren Sie sie, um Ihren [!DNL Commerce] Katalog in [!DNL Amazon Seller Accounts] zu integrieren und über den [!DNL Amazon Marketplace] zu verkaufen.
role: Admin, Developer
feature: Sales Channels, Install, Integration, Tools and External Services
exl-id: ebf22e28-b6a2-420b-80ca-2d750839286c
source-git-commit: 010a95d7be29354515cf4dcbf5d557eebaa40ed6
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# Installieren der Erweiterung [!DNL Amazon Sales Channel]

>[!IMPORTANT]
>
>Für Adobe Commerce und Magento Open Source 2.4.x werden nur [!DNL Amazon Sales Channel] Erweiterungen ab Version 4.0 unterstützt. Wenn Sie eine Version 2.3.x ausführen, lesen Sie die Dokumentation für die [kompatible Version des Amazon-Verkaufskanals](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html). Weitere Informationen zur Versionskompatibilität finden Sie auf der Seite [Verfügbarkeit](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html) in der Entwicklerdokumentation.

Die Erweiterung [!UICONTROL Amazon Sales Channel] installiert und fügt Funktionen hinzu, um Ihren Commerce-Katalog mit [!DNL Amazon Seller Accounts] zu integrieren und über die [!DNL Amazon Marketplace] zu verkaufen. Weitere Informationen finden Sie auf der Seite [Amazon Sales Channel](https://marketplace.magento.com/magento-module-amazon.html) in [!DNL Commerce Marketplace] und in den [Versionshinweisen](release-notes.md).

## Voraussetzungen

- **Commerce-Instanz**: Die [!DNL Amazon Sales Channel] -Erweiterung kann auf Instanzen mit Magento Open Source, Adobe Commerce und Adobe Commerce in Cloud-Infrastrukturversionen 2.3.x oder höher installiert werden. Es wird nicht mehr in Version 2.1, 2.2 oder 1.x unterstützt.
- **Commerce-Webkonto**: Sie sollten über ein Commerce-Webkonto verfügen, mit dem ein API-Schlüssel erstellt und verfolgt wird.
- **API-Schlüssel**: Erstellen Sie einen Amazon Sales Channel-API-Schlüssel über Ihr Commerce-Webkonto. Die folgenden Anweisungen enthalten diese Schritte.

## Installieren

Ausführlichere Informationen zur Verwendung von Composer für diesen Prozess finden Sie in den Anweisungen zur Installation der [Erweiterung](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html) in der Entwicklerdokumentation.

1. Melden Sie sich bei [Commerce Marketplace](https://marketplace.magento.com/customer/account/) an.

1. Klicken Sie auf die Registerkarte **[!UICONTROL Marketplace]** und dann auf **[!UICONTROL My Purchases]**.

1. Suchen und wählen Sie **[!UICONTROL Amazon Sales Channel]** aus.

1. Wählen Sie auf der Erweiterungsseite die Version aus.

1. Klicken Sie für den Komponentennamen und die Version auf **[!UICONTROL Technical Details]**.

1. Verwenden Sie den Namen und die Versionsinformationen, um den Service-Connector-Eintrag in Ihrer `composer.json` -Datei zu aktualisieren.

   - Fügen Sie den Erweiterungsnamen und die Version zu Ihrer `composer.json` -Datei hinzu.

   - Navigieren Sie zu Ihrem &quot;[!DNL Commerce]&quot;-Projektverzeichnis und aktualisieren Sie Ihre &quot;`composer.json`&quot;-Datei.

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - Geben Sie Ihre [Authentifizierungsschlüssel](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html) ein. Ihr öffentlicher Schlüssel ist Ihr Benutzername, Ihr privater Schlüssel ist Ihr Passwort.

   - Warten Sie, bis Composer die Aktualisierung Ihrer Projektabhängigkeiten abgeschlossen hat und sicherstellen Sie, dass keine Fehler auftreten.

1. [Überprüfen Sie die Erweiterung](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html).

## Hinzufügen des Amazon Sales Channel-API-Schlüssels

Geben Sie nach der Installation einen [API-Schlüssel](./amazon-verify-api-key.md) ein, um die Konfiguration abzuschließen.

## Amazon-Kanalkonfigurationsoptionen festlegen

Sie haben die folgenden Optionen zum Konfigurieren des Amazon-Vertriebskanals. Sie müssen diese Einstellungen nicht ändern, um mit dem Onboarding und Verkaufen in Amazon zu beginnen. Es wird empfohlen, dass erweiterte Administratoren diese Optionen berücksichtigen.

1. Melden Sie sich bei Admin an.

1. Wechseln Sie in der Seitenleiste _Admin_ zu **Stores** > _Einstellungen_ > **Konfiguration**.

1. Klicken Sie auf **Sales Channel** und dann auf **Globale Einstellungen**.

1. Definieren Sie für **Protokollverlauf löschen** das Intervall zum Löschen der erfassten Protokolle.

   Zu den Optionen gehören `Once Daily`, `Once Weekly` und `Once Monthly` (Standard).

1. (Optional) Ändern Sie für **Hintergrundaufgaben (CRON) Source** die Einstellung auf `Command Line (CLI) CRON`.

   Diese Einstellung wird für **_fortgeschrittene Benutzer/Administratoren_** empfohlen.

1. Klicken Sie auf **[!UICONTROL Save Config]**.

## Erweiterung aktualisieren

1. Melden Sie sich bei [Commerce Marketplace](https://marketplace.magento.com/customer/account/) an.

1. Klicken Sie auf die Registerkarte **[!UICONTROL Marketplace]** und dann auf **[!UICONTROL My Purchases]**.

1. Suchen und wählen Sie **[!UICONTROL Amazon Sales Channel]** aus.

1. Wählen Sie auf der Erweiterungsseite die Version aus.

1. Klicken Sie für den Komponentennamen und die Version auf **[!UICONTROL Technical Details]**.

1. Führen Sie die [Anweisungen für das Erweiterungs-Upgrade](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html) im _Installationshandbuch_ aus.
