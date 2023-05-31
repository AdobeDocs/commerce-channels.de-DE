---
title: '"Verbinden mit [!DNL Commerce] Dienste'''
description: "Verbinden Sie den Kanal-Manager mit [!DNL Commerce] Dienste, die die Datensynchronisation und Kommunikation zwischen [!DNL Commerce] -Instanz, Kanal-Manager und anderen unterstützenden Diensten."
role: User
level: Intermediate
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: a3ae579c0eda0c27bf8eab9d0ac12919eaad494b
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---


# Verbinden mit [!DNL Commerce] Dienste

Die [!DNL Commerce Services Connector] integriert den Kanal-Manager-Dienst in Adobe Commerce- und Magento Open Source-Instanzen. Der Connector ermöglicht die Datensynchronisation und Kommunikation zwischen dem [!DNL Commerce] Instanz, [!DNL Channel Manager]und andere unterstützende Dienste.

[!DNL Commerce Services Connector] Einrichtung ist ein einmaliger Prozess, der verwendet werden muss [Adobe Commerce SaaS-Dienste](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html) wie [!DNL Channel Manager], [!DNL Live Search]und [!DNL Product Recommendations]. Wenn Sie den Connector bereits für einen anderen Dienst konfiguriert haben, überspringen Sie diesen Schritt.

## Voraussetzungen

- **Commerce-Konto**-Installieren der Software auf [!DNL Commerce] -Instanzen müssen Sie über ein Konto mit dem Inhaber- oder Administratorzugriff auf die [!DNL Commerce] Plattform.

   Kontoinhaber und Superbenutzer können über die [!DNL Commerce] -Instanz oder über die Befehlszeile mit der [!DNL Commerce] CLI, Befehl `admin:user:create`.

- **Adobe Commerce Production API-Schlüssel**-this [key](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/integration-services/saas.html#genapikey) ermöglicht API-Zugriff auf Dienste, die für den Kanal-Manager erforderlich sind. Sie benötigen die öffentlichen und privaten Anmeldeinformationen für diesen Schlüssel.

>[!TIP]
>
>Um die Anmeldeinformationen anzugeben, muss ein [!DNL Commerce] Lizenzinhaber oder Kontoinhaber hat Optionen [Freigeben von Zugriff](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-share.html)oder geben Sie die [API-Schlüssel](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/integration-services/saas.html) -Anmeldedaten für einen vertrauenswürdigen Entwickler.

## Konfigurieren Sie die [!DNL Commerce Services Connector]

1. Öffnen Sie die Konfiguration der Store-Dienste .

   - Wählen Sie im Admin die Option **[!UICONTROL Stores]**.

   - under *[!UICONTROL Settings]* auswählen **[!UICONTROL Configuration]**.

   - Erweitern **[!UICONTROL Services]** und wählen Sie **[!UICONTROL Commerce Services Connector]**.

1. Fügen Sie Anmeldedaten für den Produktions-API-Schlüssel aus Ihrem Adobe Commerce-Konto hinzu.

   ![[!DNL Commerce Services Connector] im [!DNL Admin] Ansicht](assets/commerce-services-connector-admin-service-view.png){width="600" zoomable="yes"}


   >[!NOTE]
   >
   > Wenn [!DNL Commerce] Instanz hat andere [!DNL Adobe Commerce] Dienste wie [!DNL Live Search] oder [!DNL Product Recommendations] installiert ist, werden die Anmeldeinformationen in der Benutzeroberfläche angezeigt und es ist keine weitere Konfiguration erforderlich.

1. Konfigurieren Sie das SaaS-Projekt und den Datenraum, damit Commerce Services Daten an den Kanal-Manager-Dienst senden kann.

   ![[!DNL Commerce Services Connector] SaaS-ID-Konfiguration in der [!DNL Admin] Ansicht](assets/commerce-services-connector-saas-config.png){width="600" zoomable="yes"}

