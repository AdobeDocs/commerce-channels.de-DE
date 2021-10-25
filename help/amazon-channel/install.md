---
title: Erweiterung installieren
description: To integrate your [!DNL Commerce] catalog with [!DNL Amazon Seller Accounts] and sell through the [!DNL Amazon Marketplace], download and install the Amazon Sales Channel extension.
exl-id: ebf22e28-b6a2-420b-80ca-2d750839286c
source-git-commit: 8d12a839bbdf77f27c732507b5b776729e252a9f
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Erweiterung installieren

>[!IMPORTANT]
>
>Nur [!DNL Amazon Sales Channel] Erweiterungsversionen ab Version 4.0 werden für Adobe Commerce und Magento Open Source 2.4.x unterstützt. Wenn Sie eine 2.3.x-Version ausführen, lesen Sie die Dokumentation für [Amazon Sales Kanal Release](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html){Zielgruppe=&quot;_blank&quot;}. For more information about version compatibility, see the [Availability](https://devdocs.magento.com/release/availability.html){target=&quot;_blank&quot;} page in the developer documentation.

Die [!UICONTROL Amazon Sales Channel] Erweiterung installiert und fügt Funktionen zur Integration Ihres Commerce-Katalogs hinzu mit [!DNL Amazon Seller Accounts] über [!DNL Amazon Marketplace]. To review additional information, see the [Amazon Sales Channel](https://marketplace.magento.com/magento-module-amazon.html) page in [!DNL Commerce Marketplace] and the [release notes](https://devdocs.magento.com/extensions/amazon-sales/release-notes/) in the developer documentation.

## Anforderungen

- **Commerce-Instanz**: Die [!DNL Amazon Sales Channel] -Erweiterung kann auf Instanzen mit Magento Open Source, Adobe Commerce und Adobe Commerce auf Cloud-Infrastrukturversionen 2.3.x oder höher installiert werden. Es wird nicht mehr auf 2.1, 2.2 oder 1.x Versionen unterstützt.
- **Commerce web account**: You should have a Commerce web account, which is used to create and track an API key.
- **API-Schlüssel**: Erstellen Sie über Ihr Commerce-Webkonto einen Amazon Sales Kanal-API-Schlüssel. Die folgenden Anweisungen enthalten diese Schritte.

## Installieren

Weitere Informationen zur Verwendung des Composer für diesen Prozess finden Sie im [Erweiterungsinstallation](https://devdocs.magento.com/extensions/install/){Zielgruppe=&quot;_blank&quot;} Anweisungen in der Entwicklerdokumentation.

1. Anmelden bei [Commerce Marketplace](https://marketplace.magento.com/customer/account/){Zielgruppe=&quot;_blank&quot;}.

1. Click the **[!UICONTROL Marketplace]** tab, and then click **[!UICONTROL My Purchases]**.

1. Suchen und auswählen **[!UICONTROL Amazon Sales Channel]**.

1. Wählen Sie auf der Erweiterungsseite die Version aus.

1. For the component name and version, click **[!UICONTROL Technical Details]**.

1. Verwenden Sie den Namen und die Versionsinformationen, um den Dienstschnittstelleneintrag in Ihrer `composer.json` Datei.

   - Namen und Version der Erweiterung Hinzufügen auf Ihren `composer.json` Datei.

   - Zu Ihrer [!DNL Commerce] Projektverzeichnis und aktualisieren Sie Ihre `composer.json` Datei.

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - Geben Sie Ihren [Authentifizierungsschlüssel](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){Zielgruppe=&quot;_blank&quot;}. Ihr öffentlicher Schlüssel ist Ihr Benutzername. Ihr privater Schlüssel ist Ihr Kennwort.

   - Wait for Composer to finish updating your project dependencies and ensure that there are no errors.


1. [Erweiterung überprüfen](https://devdocs.magento.com/extensions/install/#verify-the-extension){Zielgruppe=&quot;_blank&quot;}.

## Add the Amazon sales channel API key

Geben Sie nach der Installation eine [API-Schlüssel](./amazon-verify-api-key.md) , um die Konfiguration abzuschließen.

## Amazon Kanal-Konfigurationsoptionen festlegen

Sie haben die folgenden Optionen zur Konfiguration des Amazon Sales Kanals. You do not need to modify these settings to begin onboarding and selling on Amazon. It is recommended that advanced administrators consider these options.

1. Log into the Admin.

1. Auf _Admin_ Sidebar, Gehe zu **Geschäfte** > _Einstellungen_ > **Konfiguration**.

1. Klick **Sales Channel**, dann **Globale Einstellungen**.

1. für **Protokollverlauf löschen**, legen Sie das Intervall für das Löschen der gesammelten Protokolle fest.

   Options include `Once Daily`, `Once Weekly`, and `Once Monthly` (default).

1. (Optional) für **Quelle für Hintergrund-Aufgaben (CRON)**, ändern Sie die Einstellung in `Command Line (CLI) CRON`.

   Diese Einstellung wird empfohlen für **_Erweiterte Benutzer/Administratoren_**.

1. Click **[!UICONTROL Save Config]**.

## Update the extension

1. Anmelden bei [Commerce Marketplace](https://marketplace.magento.com/customer/account/){Zielgruppe=&quot;_blank&quot;}.

1. Klicken Sie auf **[!UICONTROL Marketplace]** und klicken Sie anschließend auf **[!UICONTROL My Purchases]**.

1. Suchen und auswählen **[!UICONTROL Amazon Sales Channel]**.

1. On the extension page, select the version.

1. Für den Komponentennamen und die Version klicken Sie auf **[!UICONTROL Technical Details]**.

1. Complete the [extension upgrade instructions](https://devdocs.magento.com/extensions/install/#upgrade-an-extension){target=&quot;_blank&quot;} in the developer documentation.
