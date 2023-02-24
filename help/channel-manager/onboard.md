---
title: Onboard [!DNL Channel Manager]
description: '''Verbinden Sie Ihre Instanz mit dem [!DNL Channel Manager] Service durch Ausführung einiger Onboarding-Schritte."'
role: User
level: Intermediate
exl-id: 7c4ccd9e-ae32-4511-8d1e-baa690604612
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---


# Onboard [!DNL Channel Manager]

Nachdem Sie das Onboarding-Verfahren für den Kanal-Manager abgeschlossen haben, können Sie über Adobe Commerce auf die Vertriebsvorgänge für den Kanal Walmart Marketplace zugreifen, diese konfigurieren und verwalten. Der Kanal-Manager ist im Menü [!UICONTROL Channel Manager] -Option auf [!UICONTROL Commerce Admin Marketing] Menü.

![[!DNL Channel Manager] Option in der Admin-Ansicht](assets/channel-manager-admin-view.png)

## Voraussetzungen

Überprüfen Sie die Anforderungen für die Verwendung des Kanal-Managers und sammeln Sie die erforderlichen Kontoinformationen und Anmeldeinformationen, um die Erweiterung herunterzuladen, zu installieren und zu konfigurieren.

- **[Anforderungen an Walmart Marketplace](walmart-requirements.md)**-Überprüfen Sie, ob Sie die Anforderungen für die Integration mit dem Kanal-Manager erfüllen, einschließlich [Einrichten Ihres Verkäuferkontos](https://sellerhelp.walmart.com/seller/s/guide?article=000008219) und Generieren des API-Schlüssels zur Aktivierung der Integration.

- **Commerce-Kontoinformationen**- Herunterladen und Installieren [!DNL Channel Manager] erfordert [Commerce-Konto](https://docs.magento.com/user-guide/magento/magento-account.html){target="_blank"}. Sie benötigen eine Konto-ID und Anmeldedaten mit dem Inhaber- oder Administratorzugriff auf die [!DNL Adobe Commerce] oder [!DNL Magento Open Source] -Instanz.

   - **MAGE-ID**-[Anmelden](https://account.magento.com/customer/account/login/) der [!DNL Commerce] -Konto zum Abrufen der ID von **[!UICONTROL My Account - Magento settings]**.

      ![[!DNL MAGEID] on [!DNL Commerce] Kontoeinstellungen](assets/mageid-my-commerce-account.png)

   - **Zugriffsschlüssel -** Abrufen von Authentifizierungsschlüsseln zum Herunterladen [!DNL Commerce] Erweiterungen aus [!DNL Commerce] Composer-Repository `([!DNL repo.magento.com]`).

      ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png)

      Bei Adobe Commerce- und Magento Open Source-Projekten kann der Eigentümer [Freigegebener Zugriff](https://docs.magento.com/user-guide/magento/magento-account-share.html) , damit vertrauenswürdige Mitarbeiter und Dienstleister Erweiterungen mit Anmeldeinformationen aus dem Eigentümer- oder Lizenzinhaberkonto herunterladen können.

      Für [!DNL Adobe Commerce] Bei Cloud-Infrastrukturprojekten müssen Softwareinstallationen folgenden Zugriff auf die [!DNL Commerce] instance:

      - Superbenutzerzugriff auf das Cloud-Projekt
      - Administratorzugriff auf eine bestimmte Umgebung
      - ein [!DNL Adobe Commerce] Konto mit Berechtigungen für den Zugriff auf das Composer-Repository

      Siehe [Benutzerzugriff verwalten](https://devdocs.magento.com/cloud/project/user-admin.html).


- **Erlebnis mit Composer und dem[!DNL Commerce CLI]**-Siehe [Allgemeine CLI-Installation](https://devdocs.magento.com/extensions/install/){target="_blank"} für Informationen zur Verwendung dieser Tools zum Installieren und Verwalten von Erweiterungen in [!DNL Adobe Commerce] oder [!DNL Magento Open Source] Plattformen.

- **[[!DNL Amazon Sales Channel] Version 4.4.2 oder höher](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)**-Wenn aktiviert [!DNL Amazon Sales Channel] für Ihre [!DNL Commerce] Sites, überprüfen Sie, ob Ihre [!DNL Commerce] Die Plattform hat vor der Installation Version 4.4.2 oder höher installiert. [!DNL Channel Manager].

- **[!DNL Inventory Management]Erweiterung für Adobe Commerce und Magento Open Source**

   Wenn Sie planen, den Kanal-Manager für die Bestandsverwaltung und die Lagerbestandsverwaltung zu verwenden, muss die Inventory management-Erweiterung auf Ihrer Adobe Commerce- und Magento Open Source-Instanz installiert und aktiviert sein. In der Regel wird diese Erweiterung in Adobe Commerce installiert und standardmäßig aktiviert und [!DNL Magento Open Source] 2.3.x und höher.

   Wenn Sie Commerce von 2.2.x aktualisiert haben oder Inventory management deaktiviert haben, aktualisieren Sie Ihre Installation, um die erforderlichen Module einzuschließen. Siehe [Installieren von Inventory management](https://devdocs.magento.com/extensions/inventory-management/) in der Adobe Commerce Developer-Dokumentation.

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

## Onboarding-Schritte

1. [Einrichten des Walmart-Verkäuferkontos](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp).

1. [Installieren Sie die [!DNL Channel Manager] Erweiterung](install.md).

1. [Verbindung zu Commerce Services herstellen](connect.md) , um den Kanal-Manager in die Commerce-Instanz und andere unterstützende Dienste zu integrieren.

1. [Verbinden Sie Ihre [!DNL Commerce] speichern in [!DNL Walmart Marketplace]](connect-marketplace.md).

1. [Komplette Store-Einrichtung](complete-sales-channel-store-setup.md).
