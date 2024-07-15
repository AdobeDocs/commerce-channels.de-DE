---
title: "Mit [!DNL Commerce] Diensten verbinden"
description: "Verbinden Sie den Kanal-Manager mit den [!DNL Commerce] Diensten, um die Datensynchronisation und Kommunikation zwischen der [!DNL Commerce] Instanz, dem Kanal-Manager und anderen unterstützenden Diensten zu ermöglichen."
role: Admin, Developer
level: Intermediate
feature: Sales Channels, Install, Integration
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# Mit [!DNL Commerce] Diensten verbinden

Der Dienst &quot;[!DNL Commerce Services Connector]&quot; integriert den Kanal-Manager-Dienst in Adobe Commerce- und Magento Open Source-Instanzen. Der Connector ermöglicht die Datensynchronisation und Kommunikation zwischen der [!DNL Commerce]-Instanz, [!DNL Channel Manager] und anderen unterstützenden Diensten.

Das Setup von [!DNL Commerce Services Connector] ist ein einmaliger Prozess, der zur Verwendung von [Adobe Commerce SaaS-Diensten](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html) wie [!DNL Channel Manager], [!DNL Live Search] und [!DNL Product Recommendations] erforderlich ist. Wenn Sie den Connector bereits für einen anderen Dienst konfiguriert haben, überspringen Sie diesen Schritt.

## Voraussetzungen

- **Commerce-Konto**-Um die Software auf [!DNL Commerce] -Instanzen zu installieren, müssen Sie über ein Konto mit Eigentümer- oder Administratorzugriff auf die [!DNL Commerce] -Plattform verfügen.

  Kontoinhaber und Superbenutzer können über die [!DNL Commerce] -Instanz oder über die Befehlszeile Admin-Konten mit dem Befehl [!DNL Commerce] CLI command `admin:user:create` erstellen.

- **Adobe Commerce Production API-Schlüssel** - Dieser 2}Schlüssel](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/integration-services/saas.html#genapikey) ermöglicht den API-Zugriff auf Dienste, die für den Kanal-Manager erforderlich sind. [ Sie benötigen die öffentlichen und privaten Anmeldeinformationen für diesen Schlüssel.

>[!TIP]
>
>Um die Anmeldedaten bereitzustellen, hat ein [!DNL Commerce] Lizenzinhaber oder Kontoinhaber Optionen zum [Freigeben des Zugriffs](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-share.html) oder zum Übergeben der [API-Schlüssel](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/integration-services/saas.html)-Anmeldeinformationen an einen vertrauenswürdigen Entwickler.

## Konfigurieren des [!DNL Commerce Services Connector]

1. Öffnen Sie die Konfiguration der Store-Dienste .

   - Wählen Sie im Admin **[!UICONTROL Stores]** aus.

   - Wählen Sie unter &quot;*[!UICONTROL Settings]*&quot;die Option &quot;**[!UICONTROL Configuration]**&quot;.

   - Erweitern Sie **[!UICONTROL Services]** und wählen Sie **[!UICONTROL Commerce Services Connector]** aus.

1. Fügen Sie Anmeldedaten für den Produktions-API-Schlüssel aus Ihrem Adobe Commerce-Konto hinzu.

   ![[!DNL Commerce Services Connector] Dienst in der [!DNL Admin] Ansicht](assets/commerce-services-connector-admin-service-view.png){width="600" zoomable="yes"}


   >[!NOTE]
   >
   > Wenn für Ihre [!DNL Commerce] -Instanz andere [!DNL Adobe Commerce] -Dienste wie [!DNL Live Search] oder [!DNL Product Recommendations] installiert sind, werden die Anmeldeinformationen in der Benutzeroberfläche angezeigt und es ist keine weitere Konfiguration erforderlich.

1. Konfigurieren Sie das SaaS-Projekt und den Datenraum, damit Commerce Services Daten an den Channel Manager-Dienst senden kann.

   ![[!DNL Commerce Services Connector] Konfiguration der SaaS-Kennung in der [!DNL Admin] Ansicht](assets/commerce-services-connector-saas-config.png){width="600" zoomable="yes"}

