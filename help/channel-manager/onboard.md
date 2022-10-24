---
title: Onboard [!DNL Channel Manager]
description: '''Verbinden Sie Ihre Instanz mit dem [!DNL Channel Manager] Service durch Ausführung einiger Onboarding-Schritte."'
role: User
level: Intermediate
exl-id: 7c4ccd9e-ae32-4511-8d1e-baa690604612
source-git-commit: 3f6039ad78ff500c31129bee12d65e291e226567
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---


# Onboard [!DNL Channel Manager]

Nachdem Sie das Onboarding abgeschlossen haben, konfigurieren und verwalten Sie die Vorgänge der Vertriebskanäle über das [!UICONTROL Channel Manager] -Option auf [!UICONTROL Commerce Admin Marketing] Menü.

![[!DNL Channel Manager] Option in der Admin-Ansicht](assets/channel-manager-admin-view.png)

## Onboarding-Übersicht

1. [Installieren Sie die [!DNL Channel Manager] Erweiterung](install.md).

1. [Konfigurieren Sie die [!DNL Commerce Services Connector]](connect.md) , um den Kanal-Manager in die Commerce-Instanz und andere unterstützende Dienste zu integrieren.

1. [Verbinden Sie Ihre [!DNL Commerce] speichern in [!DNL Walmart Marketplace]](connect.md).

1. [Komplette Store-Einrichtung](complete-sales-channel-store-setup.md).

## Voraussetzungen

- Vergewissern Sie sich, dass Sie die [Anforderungen an Walmart Marketplace](walmart-requirements.md) zur Integration mit dem Kanal-Manager.

- **Commerce-Kontoinformationen**- Herunterladen und Installieren [!DNL Channel Manager] erfordert [Commerce-Konto](https://docs.magento.com/user-guide/magento/magento-account.html){target=&quot;_blank&quot;}. Sie benötigen eine Konto-ID und Anmeldedaten mit dem Inhaber- oder Administratorzugriff auf die [!DNL Adobe Commerce] oder [!DNL Magento Open Source] -Instanz.

   - **MAGE-ID**-[Anmelden](https://account.magento.com/customer/account/login/) der [!DNL Commerce] -Konto zum Abrufen der ID von **[!UICONTROL My Account - Magento settings]**.

      ![[!DNL MAGEID] on [!DNL Commerce] Kontoeinstellungen](assets/mageid-my-commerce-account.png)

   - **Zugriffsschlüssel -** Abrufen von Authentifizierungsschlüsseln zum Herunterladen [!DNL Commerce] Erweiterungen aus [!DNL Commerce] Composer-Repository `([!DNL repo.magento.com]`).

      ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png)

      Bei Adobe Commerce- und Magento Open Source-Projekten kann der Eigentümer [Freigegebener Zugriff](https://docs.magento.com/user-guide/magento/magento-account-share.html) , damit vertrauenswürdige Mitarbeiter und Dienstleister Erweiterungen mit Anmeldeinformationen aus dem Eigentümer- oder Lizenzinhaberkonto herunterladen können.

      Für [!DNL Adobe Commerce] Bei Cloud-Infrastrukturprojekten müssen Softwareinstallationen folgenden Zugriff auf die [!DNL Commerce] instance:

      - Superbenutzerzugriff auf das Cloud-Projekt
      - Administratorzugriff auf eine bestimmte Umgebung
      - ein [!DNL Adobe Commerce] oder [!DNL Magento Open Source] Konto mit Berechtigungen für den Zugriff auf das Composer-Repository

      Siehe [Benutzerzugriff verwalten](https://devdocs.magento.com/cloud/project/user-admin.html).


- **Erlebnis mit Composer und dem[!DNL Commerce CLI]** -Siehe [Allgemeine CLI-Installation](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;} für Informationen zur Verwendung dieser Tools zum Installieren und Verwalten von Erweiterungen in [!DNL Adobe Commerce] oder [!DNL Magento Open Source] Plattformen.

- [[!DNL Amazon Sales Channel] Version 4.4.2 oder höher](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)-Wenn Sie aktiviert haben [!DNL Amazon Sales Channel] für Ihre [!DNL Commerce] Sites, überprüfen Sie, ob Ihre [!DNL Commerce] Auf der Plattform ist vor der Installation Version 4.4.2 installiert. [!DNL Channel Manager].

- [!DNL Inventory Management] Erweiterung für Adobe Commerce und Magento Open Source

   Wenn Sie planen, den Kanal-Manager für die Bestandsverwaltung und Auftragsverwaltung zu verwenden, muss die Inventory management-Erweiterung auf Ihrer Adobe Commerce- und Magento Open Source-Instanz installiert und aktiviert sein. In der Regel wird diese Erweiterung unter Adobe Commerce und Magento Open Source 2.3.x und höher standardmäßig installiert und aktiviert.

   Wenn Sie Commerce von 2.2.x aktualisiert haben oder Inventory management deaktiviert haben, müssen Sie Ihre Installation aktualisieren, um die erforderlichen Module einzuschließen. Weitere Informationen finden Sie unter [Installieren von Inventory management](https://devdocs.magento.com/extensions/inventory-management/) in der Adobe Commerce Developer-Dokumentation.

### Systemanforderungen

- [Adobe Commerce 2.4.x](https://devdocs.magento.com/release/released-versions.html)
- [PHP 7.3 / 7.4](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html)
- [Composer 1.x oder höher](https://devdocs.magento.com/cloud/reference/cloud-composer.html)
- [[!DNL Amazon Sales Channel] Version 4.4.2 oder höher](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)-Wenn Sie aktiviert haben [!DNL Amazon Sales Channel] für Ihre [!DNL Commerce] Sites, überprüfen Sie, ob Ihre [!DNL Commerce] Auf der Plattform ist vor der Installation Version 4.4.2 installiert. [!DNL Channel Manager].
- [[!DNL Inventory Management]](https://devdocs.magento.com/extensions/inventory-management/)

### Unterstützte Plattformen

- Adobe Commerce on Cloud (ECE) : 2.4.x
- Adobe Commerce vor Ort (EE): 2.4.x
- Magento Open Source 2.4.x
