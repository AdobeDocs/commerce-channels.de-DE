---
title: Installieren der Erweiterung
description: Laden Sie die Amazon-Sales Channel-Erweiterung herunter und installieren Sie sie, um [!DNL Commerce] catalog with [!DNL Amazon Seller Accounts] zu integrieren und über  [!DNL Amazon Marketplace] zu verkaufen.
exl-id: ebf22e28-b6a2-420b-80ca-2d750839286c
source-git-commit: 8d12a839bbdf77f27c732507b5b776729e252a9f
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Installieren der Erweiterung

>[!IMPORTANT]
>
>Für Adobe Commerce- und Magento Open Source 2.4.x-Versionen werden nur [!DNL Amazon Sales Channel] -Erweiterungen ab Version 4.0 unterstützt. Wenn Sie eine Version 2.3.x ausführen, lesen Sie die Dokumentation für die [kompatible Amazon-Version des Vertriebskanals](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html){target=&quot;_blank&quot;}. Weitere Informationen zur Versionskompatibilität finden Sie auf der Seite [Verfügbarkeit](https://devdocs.magento.com/release/availability.html){target=&quot;_blank&quot;} in der Entwicklerdokumentation.

Die Erweiterung [!UICONTROL Amazon Sales Channel] installiert und fügt Funktionen hinzu, um Ihren Commerce-Katalog mit [!DNL Amazon Seller Accounts] zu integrieren und über [!DNL Amazon Marketplace] zu verkaufen. Weitere Informationen finden Sie auf der Seite [Amazon Sales Channel](https://marketplace.magento.com/magento-module-amazon.html) unter [!DNL Commerce Marketplace] und den [Versionshinweisen](https://devdocs.magento.com/extensions/amazon-sales/release-notes/) in der Entwicklerdokumentation.

## Voraussetzungen

- **Commerce-Instanz**: Die  [!DNL Amazon Sales Channel] Erweiterung kann auf Instanzen mit Magento Open Source, Adobe Commerce und Adobe Commerce in Cloud-Infrastrukturversionen 2.3.x oder höher installiert werden. Es wird nicht mehr in 2.1-, 2.2- oder 1.x-Versionen unterstützt.
- **Commerce-Webkonto**: Sie sollten über ein Commerce-Webkonto verfügen, mit dem ein API-Schlüssel erstellt und verfolgt wird.
- **API-Schlüssel**: Erstellen Sie über Ihr Commerce-Webkonto einen Amazon-API-Schlüssel für den Vertriebskanal. Die folgenden Anweisungen enthalten diese Schritte.

## Installieren

Weitere Informationen zur Verwendung von Composer für diesen Prozess finden Sie in den Anweisungen [Installation der Erweiterung](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;} in der Entwicklerdokumentation.

1. Melden Sie sich bei [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target=&quot;_blank&quot;} an.

1. Klicken Sie auf die Registerkarte **[!UICONTROL Marketplace]** und dann auf **[!UICONTROL My Purchases]**.

1. Suchen und wählen Sie **[!UICONTROL Amazon Sales Channel]** aus.

1. Wählen Sie auf der Erweiterungsseite die Version aus.

1. Klicken Sie für den Komponentennamen und die Version auf **[!UICONTROL Technical Details]**.

1. Verwenden Sie den Namen und die Versionsinformationen, um den Service-Connector-Eintrag in Ihrer `composer.json`-Datei zu aktualisieren.

   - Fügen Sie den Namen und die Version der Erweiterung Ihrer `composer.json`-Datei hinzu.

   - Navigieren Sie zum Projektverzeichnis [!DNL Commerce] und aktualisieren Sie die Datei `composer.json`.

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - Geben Sie Ihre [Authentifizierungsschlüssel](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target=&quot;_blank&quot;} ein. Ihr öffentlicher Schlüssel ist Ihr Benutzername. Ihr privater Schlüssel ist Ihr Passwort.

   - Warten Sie, bis Composer die Aktualisierung Ihrer Projektabhängigkeiten abgeschlossen hat und sicherstellen Sie, dass keine Fehler auftreten.


1. [Überprüfen Sie die Erweiterung ](https://devdocs.magento.com/extensions/install/#verify-the-extension){target=&quot;_blank&quot;}.

## Hinzufügen des Amazon-Vertriebskanal-API-Schlüssels

Geben Sie nach der Installation einen [API-Schlüssel](./amazon-verify-api-key.md) ein, um die Konfiguration abzuschließen.

## Amazon-Kanalkonfigurationsoptionen festlegen

Sie haben die folgenden Optionen zum Konfigurieren des Amazon-Vertriebskanals. Sie müssen diese Einstellungen nicht ändern, um mit dem Onboarding und Verkaufen in Amazon zu beginnen. Es wird empfohlen, dass erweiterte Administratoren diese Optionen berücksichtigen.

1. Melden Sie sich bei Admin an.

1. Navigieren Sie in der Seitenleiste _Admin_ zu **Stores** > _Einstellungen_ > **Konfiguration**.

1. Klicken Sie auf **Sales Channel** und dann auf **Globale Einstellungen**.

1. Definieren Sie für **Clear Log History** das Intervall zum Löschen der abgerufenen Protokolle.

   Zu den Optionen gehören `Once Daily`, `Once Weekly` und `Once Monthly` (Standard).

1. (Optional) Ändern Sie für **Background Tasks (CRON) Source** die Einstellung in `Command Line (CLI) CRON`.

   Diese Einstellung wird für **_fortgeschrittene Benutzer/Administratoren_** empfohlen.

1. Klicken Sie auf **[!UICONTROL Save Config]**.

## Erweiterung aktualisieren

1. Melden Sie sich bei [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target=&quot;_blank&quot;} an.

1. Klicken Sie auf die Registerkarte **[!UICONTROL Marketplace]** und dann auf **[!UICONTROL My Purchases]**.

1. Suchen und wählen Sie **[!UICONTROL Amazon Sales Channel]** aus.

1. Wählen Sie auf der Erweiterungsseite die Version aus.

1. Klicken Sie für den Komponentennamen und die Version auf **[!UICONTROL Technical Details]**.

1. Füllen Sie die [Anweisungen zum Erweiterungs-Upgrade](https://devdocs.magento.com/extensions/install/#upgrade-an-extension){target=&quot;_blank&quot;} in der Entwicklerdokumentation aus.
