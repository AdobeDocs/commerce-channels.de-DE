---
title: Onboard [!DNL Channel Manager]
description: Verbinden Sie Ihre Instanz mit dem [!DNL Channel Manager] -Service durch Ausführen einiger Onboarding-Schritte.
role: User
level: Intermediate
exl-id: 7c4ccd9e-ae32-4511-8d1e-baa690604612
source-git-commit: f57c6db4c0314272d10bb5483d2c8a0ae396a9fc
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Onboard [!DNL Channel Manager]

Onboard Channel Manager durch Installation der Channel Manager-Erweiterung auf Ihrem [!DNL Commerce] Instanz und Konfiguration von API-Verbindungen. Diese Verbindungen ermöglichen die Kommunikation und Datensynchronisation zwischen Ihrer Commerce-Instanz und dem Walmart Marketplace.

Nachdem Sie das Onboarding abgeschlossen haben, konfigurieren und verwalten Sie die Vorgänge der Vertriebskanäle über das [!UICONTROL Channel Manager] -Option auf [!UICONTROL Commerce Admin Marketing] Menü.

![[!DNL Channel Manager] Option in der Admin-Ansicht](assets/channel-manager-admin-view.png)

## Onboarding-Übersicht

1. [Installieren Sie die [!DNL Channel Manager] Erweiterung](install.md).

1. [Konfigurieren Sie die [!DNL Commerce Services Connector]](connect.md) , um den Kanal-Manager in die Commerce-Instanz und andere unterstützende Dienste zu integrieren.

1. [Verbinden Sie Ihre [!DNL Commerce] speichern in [!DNL Walmart Marketplace]](connect.md).

1. [Komplette Store-Einrichtung](complete-store-setup.md).

## Voraussetzungen

- Vergewissern Sie sich, dass Sie über die erforderlichen [Voraussetzungen für den Walmart Marketplace](walmart-prerequisites.md) zur Integration mit dem Kanal-Manager.

- **Commerce-Kontoinformationen**- Herunterladen und Installieren [!DNL Channel Manager] erfordert [Commerce-Konto](https://docs.magento.com/user-guide/magento/magento-account.html){target=&quot;_blank&quot;}. Sie benötigen eine Konto-ID und Anmeldedaten mit dem Inhaber- oder Administratorzugriff auf die [!DNL Adobe Commerce] oder [!DNL Magento Open Source] -Instanz.

   - **MAGE-ID**-[Anmelden](https://account.magento.com/customer/account/login/) zum Commerce-Konto, um die ID von zu erhalten **[!UICONTROL My Account - Magento settings]**. Sie benötigen diese ID, um sich für die [!DNL Channel Manager] Service Beta.

      ![[!DNL MAGEID] in den Commerce-Kontoeinstellungen](assets/mageid-my-commerce-account.png)

   - **Zugriffsschlüssel -** Abrufen von Authentifizierungsschlüsseln zum Herunterladen von Commerce-Erweiterungen aus dem Commerce Composer-Repository `([!DNL repo.magento.com]`).

      ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png)

      Bei Adobe Commerce- und Magento Open Source-Projekten kann der Eigentümer [Freigegebener Zugriff](https://docs.magento.com/user-guide/magento/magento-account-share.html) , damit vertrauenswürdige Mitarbeiter und Dienstleister Erweiterungen mit Anmeldeinformationen aus dem Eigentümer- oder Lizenzinhaberkonto herunterladen können.

      on [!DNL Adobe Commerce] Bei Cloud-Infrastrukturprojekten müssen Softwareinstallateure über den folgenden Zugriff verfügen: [!DNL Commerce] instance:

      - Superbenutzerzugriff auf das Cloud-Projekt
      - Administratorzugriff auf eine bestimmte Umgebung
      - ein [!DNL Adobe Commerce] oder [!DNL Magento Open Source] -Konto mit Berechtigungen für den Zugriff auf das Composer-Repository.

      Siehe [Benutzerzugriff verwalten](https://devdocs.magento.com/cloud/project/user-admin.html).


- **Genehmigung zum Herunterladen des Channel Manager Composer-Pakets**- Geben Sie die MAGE-ID aus dem Commerce-Konto, das zur Verwaltung des Dienstes verwendet wird, an den Adobe-Support-Mitarbeiter weiter, der das Beta-Programm für Ihr Unternehmen koordiniert.
- **Erlebnis mit Composer und dem[!DNL Commerce CLI]** -Siehe [Allgemeine CLI-Installation](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;} für Informationen zur Verwendung dieser Tools zum Installieren und Verwalten von Erweiterungen in [!DNL Adobe Commerce] oder [!DNL Magento Open Source] Plattformen.
- **[Amazon Sales Channel Version 4.4.2 oder höher](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)-Wenn Sie Amazon Sales Channel für Ihre Commerce-Sites aktiviert haben, stellen Sie sicher, dass auf Ihrer Commerce-Plattform Version 4.42 installiert ist, bevor Sie Channel Manager installieren.


### Voraussetzungen

- [Adobe Commerce 2.4.x](https://devdocs.magento.com/release/released-versions.html)
- [PHP 7.3 / 7.4](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html)
- [Composer 1.x oder höher](https://devdocs.magento.com/cloud/reference/cloud-composer.html)


### Unterstützte Plattformen

- Adobe Commerce on Cloud (ECE) : 2.4.x
- Adobe Commerce vor Ort (EE): 2.4.x
- Magento Open Source 2.4.x
