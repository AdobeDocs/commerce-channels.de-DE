---
title: Onboard [!DNL Channel Manager]
description: 'Verbinden Sie Ihre Instanz mit dem [!DNL Channel Manager] Dienst, indem Sie einige Onboarding-Schritte ausführen.'
level: Intermediate
role: Leader, Admin, Developer
feature: Sales Channels, Install
exl-id: 7c4ccd9e-ae32-4511-8d1e-baa690604612
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---


# Onboard [!DNL Channel Manager]

Nachdem Sie das Onboarding-Verfahren für den Kanal-Manager abgeschlossen haben, können Sie über Adobe Commerce auf die Vertriebsvorgänge für den Kanal Walmart Marketplace zugreifen, diese konfigurieren und verwalten. Der Kanal-Manager ist über die Option [!UICONTROL Channel Manager] im Menü [!UICONTROL Commerce Admin Marketing] verfügbar.

![[!DNL Channel Manager] -Option in der Admin-Ansicht](assets/channel-manager-admin-view.png){width="500"}

## Voraussetzungen

Überprüfen Sie die Anforderungen für die Verwendung des Kanal-Managers und sammeln Sie die erforderlichen Kontoinformationen und Anmeldeinformationen, um die Erweiterung herunterzuladen, zu installieren und zu konfigurieren.

- **[Walmart Marketplace-Anforderungen](walmart-requirements.md)** - Überprüfen Sie, ob Sie die Anforderungen für die Integration mit dem Kanal-Manager erfüllen, einschließlich der [ Einrichtung Ihres Verkäuferkontos](https://sellerhelp.walmart.com/seller/s/guide?article=000008219) und Generierung des API-Schlüssels zur Aktivierung der Integration.

- **Commerce-Kontoinformationen** - Für das Herunterladen und Installieren von [!DNL Channel Manager] ist ein [Commerce-Konto](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-create.html) erforderlich. Sie benötigen eine Konto-ID und Anmeldeinformationen mit dem Inhaber- oder Administratorzugriff auf die Instanz [!DNL Adobe Commerce] oder [!DNL Magento Open Source].

   - **MAGE ID**-[Melden Sie sich ](https://account.magento.com/customer/account/login/) beim [!DNL Commerce] -Konto an, um die ID von **[!UICONTROL My Account - Magento settings]** zu erhalten.

     ![[!DNL MAGEID] in den [!DNL Commerce] Kontoeinstellungen](assets/mageid-my-commerce-account.png){width="250"}

   - **Zugriffsschlüssel -** Abrufen von Authentifizierungsschlüsseln zum Herunterladen von [!DNL Commerce] Erweiterungen aus dem [!DNL Commerce] Composer-Repository `([!DNL repo.magento.com]`).

     ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png){width="400"}

     Bei Adobe Commerce- und Magento Open Source-Projekten kann der Inhaber den [Freigegebenen Zugriff](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-share.html) einrichten, damit vertrauenswürdige Mitarbeiter und Dienstanbieter Erweiterungen mit Berechtigungen aus dem Inhaber- oder Lizenzinhaberkonto herunterladen können.

     Für [!DNL Adobe Commerce] bei Cloud-Infrastrukturprojekten müssen Softwareinstallateure den folgenden Zugriff auf die [!DNL Commerce] -Instanz haben:

      - Superbenutzerzugriff auf das Cloud-Projekt
      - Administratorzugriff auf eine bestimmte Umgebung
      - ein [!DNL Adobe Commerce] -Konto mit Berechtigungen für den Zugriff auf das Composer-Repository

     Siehe [Verwalten des Benutzerzugriffs](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/project/user-access.html) im *Commerce on Cloud Infrastructure Guide*.

- **Erlebnis mit Composer und[!DNL Commerce CLI]** - Siehe [Installieren einer Erweiterung](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html) im *Installationshandbuch* für Informationen zur Verwendung dieser Tools zum Installieren und Verwalten von Erweiterungen auf [!DNL Adobe Commerce] - oder [!DNL Magento Open Source] -Plattformen.

- **[[!DNL Amazon Sales Channel] Version 4.4.2 oder höher](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)**-Wenn Sie [!DNL Amazon Sales Channel] für Ihre [!DNL Commerce]-Sites aktiviert haben, stellen Sie sicher, dass auf Ihrer [!DNL Commerce]-Plattform Version 4.4.2 oder höher installiert ist, bevor Sie [!DNL Channel Manager] installieren.

- **[!DNL Inventory Management]Erweiterung für Adobe Commerce und Magento Open Source**

  Wenn Sie planen, den Kanal-Manager für die Bestandsverwaltung und die Lagerbestandsverwaltung zu verwenden, muss die Inventory management-Erweiterung auf Ihrer Adobe Commerce- und Magento Open Source-Instanz installiert und aktiviert sein. In der Regel wird diese Erweiterung unter Adobe Commerce und [!DNL Magento Open Source] 2.3.x und höher standardmäßig installiert und aktiviert.

  Wenn Sie Commerce von 2.2.x aktualisiert haben oder Inventory management deaktiviert haben, aktualisieren Sie Ihre Installation, um die erforderlichen Module einzuschließen. Siehe [Installieren von Inventory management](https://experienceleague.adobe.com/docs/commerce-admin/inventory/get-started/install-update.html) im *Inventory management-Handbuch*.

### Systemanforderungen

- [Adobe Commerce 2.4.x](https://experienceleague.adobe.com/docs/commerce-operations/release/versions.html)
- [PHP 7.3 / 7.4](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/php-settings.html)
- [Composer 1.x oder höher](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/overview.html)
- [[!DNL Amazon Sales Channel] Version 4.4.2 oder höher](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)-Wenn Sie [!DNL Amazon Sales Channel] für Ihre [!DNL Commerce]-Sites aktiviert haben, stellen Sie sicher, dass auf Ihrer [!DNL Commerce]-Plattform Version 4.4.2 installiert ist, bevor Sie [!DNL Channel Manager] installieren.
- [[!DNL Inventory Management]](https://experienceleague.adobe.com/docs/commerce-admin/inventory/get-started/install-update.html)

### Unterstützte Plattformen

- Adobe Commerce on Cloud (ECE) : 2.4.x
- Adobe Commerce vor Ort (EE): 2.4.x
- Magento Open Source 2.4.x

## Onboarding-Schritte

1. [Richten Sie Ihr Walmart-Verkaufskonto ein](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp).

1. [Installieren Sie die  [!DNL Channel Manager] Erweiterung](install.md).

1. [Stellen Sie eine Verbindung zu Commerce Services her](connect.md) , um den Kanal-Manager mit der Commerce-Instanz und anderen unterstützenden Diensten zu integrieren.

1. [Verbinden Sie Ihren [!DNL Commerce] Speicher mit [!DNL Walmart Marketplace]](connect-marketplace.md).

1. [Schließen Sie die Einrichtung des Stores ab](complete-sales-channel-store-setup.md).
