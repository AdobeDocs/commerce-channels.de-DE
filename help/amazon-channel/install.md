---
title: Installieren der Erweiterung
description: Zur Integration Ihrer [!DNL Commerce] Katalog mit [!DNL Amazon Seller Accounts] und über die [!DNL Amazon Marketplace], laden Sie die Amazon Sales Channel-Erweiterung herunter und installieren Sie sie.
exl-id: ebf22e28-b6a2-420b-80ca-2d750839286c
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# Installieren der Erweiterung

>[!IMPORTANT]
>
>Nur [!DNL Amazon Sales Channel] Erweiterungen ab Version 4.0 werden für Adobe Commerce und Magento Open Source 2.4.x unterstützt. Wenn Sie eine Version 2.3.x ausführen, lesen Sie die Dokumentation für [Kompatible Version des Amazon-Vertriebskanals](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html){target="_blank"}. For more information about version compatibility, see the [Availability](https://devdocs.magento.com/release/availability.html){target="_blank"} in der Entwicklerdokumentation.

Die [!UICONTROL Amazon Sales Channel] -Erweiterung installiert und fügt Funktionen hinzu, um Ihren Commerce-Katalog mit [!DNL Amazon Seller Accounts] über [!DNL Amazon Marketplace]. Weitere Informationen finden Sie unter [Amazon Sales Channel](https://marketplace.magento.com/magento-module-amazon.html) Seite in [!DNL Commerce Marketplace] und [Versionshinweise](release-notes.md).

## Voraussetzungen

- **Commerce-Instanz**: Die [!DNL Amazon Sales Channel] -Erweiterung kann auf Instanzen mit Magento Open Source, Adobe Commerce und Adobe Commerce in Cloud-Infrastrukturversionen 2.3.x oder höher installiert werden. Es wird nicht mehr in Version 2.1, 2.2 oder 1.x unterstützt.
- **Commerce-Webkonto**: Sie sollten über ein Commerce-Webkonto verfügen, mit dem ein API-Schlüssel erstellt und verfolgt wird.
- **API-Schlüssel**: Erstellen Sie über Ihr Commerce-Webkonto einen Amazon-API-Schlüssel für den Vertriebskanal. Die folgenden Anweisungen enthalten diese Schritte.

## Installieren

Weitere Informationen zur Verwendung von Composer für diesen Prozess finden Sie unter [Erweiterungsinstallation](https://devdocs.magento.com/extensions/install/){target="_blank"} Anweisungen in der Entwicklerdokumentation.

1. Melden Sie sich bei der [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target="_blank"}.

1. Klicken Sie auf **[!UICONTROL Marketplace]** und klicken Sie auf **[!UICONTROL My Purchases]**.

1. Suchen und Auswählen **[!UICONTROL Amazon Sales Channel]**.

1. Wählen Sie auf der Erweiterungsseite die Version aus.

1. Klicken Sie für den Komponentennamen und die Version auf **[!UICONTROL Technical Details]**.

1. Verwenden Sie den Namen und die Versionsinformationen, um den Service-Connector-Eintrag in Ihrer `composer.json` -Datei.

   - Fügen Sie den Namen und die Version der Erweiterung zu Ihrem `composer.json` -Datei.

   - Navigieren Sie zu Ihrer [!DNL Commerce] Projektverzeichnis und aktualisieren Sie Ihre `composer.json` -Datei.

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - Geben Sie Ihre [Authentifizierungsschlüssel](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target="_blank"}. Ihr öffentlicher Schlüssel ist Ihr Benutzername. Ihr privater Schlüssel ist Ihr Passwort.

   - Warten Sie, bis Composer die Aktualisierung Ihrer Projektabhängigkeiten abgeschlossen hat und sicherstellen Sie, dass keine Fehler auftreten.


1. [Erweiterung überprüfen](https://devdocs.magento.com/extensions/install/#verify-the-extension){target="_blank"}.

## Hinzufügen des Amazon-Vertriebskanal-API-Schlüssels

Geben Sie nach der Installation eine [API-Schlüssel](./amazon-verify-api-key.md) , um die Konfiguration abzuschließen.

## Amazon-Kanalkonfigurationsoptionen festlegen

Sie haben die folgenden Optionen zum Konfigurieren des Amazon-Vertriebskanals. Sie müssen diese Einstellungen nicht ändern, um mit dem Onboarding und Verkaufen in Amazon zu beginnen. Es wird empfohlen, dass erweiterte Administratoren diese Optionen berücksichtigen.

1. Melden Sie sich bei Admin an.

1. Im _Admin_ Seitenleiste, navigieren Sie zu **Stores** > _Einstellungen_ > **Konfiguration**.

1. Klicken **Sales Channel**, dann **Globale Einstellungen**.

1. Für **Protokollverlauf löschen**, legen Sie das Intervall für das Löschen der abgerufenen Protokolle fest.

   Optionen umfassen `Once Daily`, `Once Weekly`und `Once Monthly` (Standard).

1. (Optional) Für **Quelle für Hintergrundaufgaben (CRON)**&#x200B;ändern Sie die Einstellung in `Command Line (CLI) CRON`.

   Diese Einstellung wird für **_Erweiterte Benutzer/Administratoren_**.

1. Klicken **[!UICONTROL Save Config]**.

## Erweiterung aktualisieren

1. Melden Sie sich bei der [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target="_blank"}.

1. Klicken Sie auf **[!UICONTROL Marketplace]** und klicken Sie auf **[!UICONTROL My Purchases]**.

1. Suchen und Auswählen **[!UICONTROL Amazon Sales Channel]**.

1. Wählen Sie auf der Erweiterungsseite die Version aus.

1. Klicken Sie für den Komponentennamen und die Version auf **[!UICONTROL Technical Details]**.

1. Führen Sie die [Anweisungen zum Erweiterungs-Upgrade](https://devdocs.magento.com/extensions/install/#upgrade-an-extension){target="_blank"} in der Entwicklerdokumentation.
