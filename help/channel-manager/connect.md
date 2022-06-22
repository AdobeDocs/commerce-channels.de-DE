---
title: '"Verbinden mit [!DNL Commerce] Dienste'''
description: '"Verbinden Sie den Kanal-Manager mit [!DNL Commerce] Dienste, die die Datensynchronisation und Kommunikation zwischen [!DNL Commerce] -Instanz, Kanal-Manager und anderen unterstützenden Diensten."'
role: User
level: Intermediate
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: 7e7a3e854bbc6062e2d15c1962ddf787451e7275
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# Verbinden mit [!DNL Commerce] Dienstleistungen

Die [!DNL Commerce Services Connector] integriert den Kanal-Manager-Dienst in Adobe Commerce- und Magento Open Source-Instanzen. Der Connector ermöglicht die Datensynchronisation und Kommunikation zwischen dem [!DNL Commerce] Instanz, [!DNL Channel Manager]und andere unterstützende Dienste.

[!DNL Commerce Services Connector] Einrichtung ist ein einmaliger Prozess, der verwendet werden muss [Adobe Commerce SaaS-Dienste](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html){target=&quot;_blank&quot;}, z. B. [!DNL Channel Manager], [!DNL Live Search]und [!DNL Product Recommendations]. Wenn Sie den Connector bereits für einen anderen Dienst konfiguriert haben, überspringen Sie diesen Schritt.

## Voraussetzungen

- **Commerce-Konto**-Installieren der Software auf [!DNL Commerce] -Instanzen müssen Sie über ein Konto mit dem Inhaber- oder Administratorzugriff auf die [!DNL Commerce] Plattform.

   Kontoinhaber und Superbenutzer können über die [!DNL Commerce] -Instanz oder über die Befehlszeile mit der [!DNL Commerce] CLI, Befehl `admin:user:create`.

- **Adobe Commerce Production API-Schlüssel**-this [key](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;} ermöglicht API-Zugriff auf Dienste, die für den Kanal-Manager erforderlich sind. Sie benötigen die öffentlichen und privaten Anmeldeinformationen für diesen Schlüssel.

>[!TIP]
>
>Um die Anmeldeinformationen anzugeben, muss ein [!DNL Commerce] Lizenzinhaber oder Kontoinhaber hat Optionen [Freigeben von Zugriff](https://docs.magento.com/user-guide/magento/magento-account-share.html){target=&quot;_blank&quot;} oder geben Sie die [API-Schlüssel](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;} Anmeldedaten für einen vertrauenswürdigen Entwickler.

## Konfigurieren Sie die [!DNL Commerce Services Connector]

1. Öffnen Sie die Konfiguration der Store-Dienste .

   - Wählen Sie im Admin die Option **[!UICONTROL Stores]**.

   - under *[!UICONTROL Settings]* auswählen **[!UICONTROL Configuration]**.

   - Erweitern **[!UICONTROL Services]** und wählen Sie **[!UICONTROL Commerce Services Connector]**.

1. Fügen Sie Anmeldedaten für den Produktions-API-Schlüssel aus Ihrem Adobe Commerce-Konto hinzu.

   ![[!DNL Commerce Services Connector] im [!DNL Admin] Ansicht](assets/commerce-services-connector-admin-service-view.png)


   >[!NOTE]
   >
   > Wenn [!DNL Commerce] Instanz hat andere [!DNL Adobe Commerce] Dienste wie [!DNL Live Search] oder [!DNL Product Recommendations] installiert ist, werden die Anmeldeinformationen in der Benutzeroberfläche angezeigt und es ist keine weitere Konfiguration erforderlich.

1. Konfigurieren Sie das SaaS-Projekt und den Datenraum, damit Commerce Services Daten an den Kanal-Manager-Dienst senden kann.

   ![[!DNL Commerce Services Connector] SaaS-ID-Konfiguration in der [!DNL Admin] Ansicht](assets/commerce-services-connector-saas-config.png)

