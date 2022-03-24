---
title: Verbindung zu Commerce Services herstellen
description: Verbinden der Kanal-Manager-Instanz mit [!DNL Commerce services] , um die Datensynchronisation und Kommunikation zwischen der Commerce-Instanz, dem Kanal-Manager und anderen unterstützenden Diensten zu aktivieren.
role: User
level: Intermediate
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: 8f07b215c20cc28aa9a6862bcb2b00da30a1ed84
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Verbindung zu Commerce Services herstellen

Der Commerce Services Connector integriert den Channel Manager-Dienst in Adobe Commerce- und Magento Open Source-Instanzen. Der Connector ermöglicht die Datensynchronisation und Kommunikation zwischen dem [!DNL Commerce] Instanz, [!DNL Channel Manager]und andere unterstützende Dienste.

Die Einrichtung des Commerce Services Connector ist ein einmaliger Prozess, der für die Verwendung von Adobe erforderlich ist [Commerce SaaS-Dienste](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html){target=&quot;_blank&quot;} wie [!DNL Channel Manager], [!DNL Live Search]und [!DNL Product Recommendations]. Wenn Sie den Connector bereits für einen anderen Dienst konfiguriert haben, überspringen Sie diesen Schritt.

## Voraussetzungen

- **Commerce-Konto**-Um Software auf Commerce-Instanzen zu installieren, müssen Sie über ein Konto mit dem Eigentümer oder Administrator Zugriff auf die Commerce-Plattform verfügen.

   Kontoinhaber und Admin-Benutzer können neue Admin-Konten aus der Commerce-Instanz oder über die Befehlszeile erstellen, die die [!DNL Commerce] CLI, Befehl `admin:user:create`.

- **Adobe Commerce Production API-Schlüssel**-this [key](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;} ermöglicht API-Zugriff auf Dienste, die für den Kanal-Manager erforderlich sind. Sie benötigen die öffentlichen und privaten Anmeldeinformationen für diesen Schlüssel.

   Um die Anmeldedaten bereitzustellen, hat ein Inhaber einer Commerce-Lizenz oder eines Kontos folgende Optionen:
   [Freigeben von Zugriff](https://docs.magento.com/user-guide/magento/magento-account-share.html){target=&quot;_blank&quot;} oder geben Sie die [API-Schlüssel](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;} Anmeldedaten für einen vertrauenswürdigen Entwickler.

## Connector für Commerce Services konfigurieren

1. Öffnen Sie die Konfiguration der Store-Dienste .

   - Wählen Sie im Admin die Option **[!UICONTROL Stores]**.

   - under *Einstellungen* auswählen **[!UICONTROL Configuration]**.

   - Erweitern **[!UICONTROL Services]** und wählen Sie **[!UICONTROL Commerce Services Connector]**.

1. Fügen Sie Anmeldedaten für den Produktions-API-Schlüssel aus Ihrem Adobe Commerce-Konto hinzu.

   ![[!DNL Commerce Service Connector] im [!DNL Admin] Ansicht](assets/commerce-services-connector-admin-service-view.png)


   >[!NOTE]
   >
   > Wenn [!DNL Commerce] Instanz hat andere [!DNL Adobe Commerce] Dienste wie [!DNL Live Search] oder [!DNL Product Recommendations] installiert ist, werden die Anmeldeinformationen in der Benutzeroberfläche angezeigt und es ist keine weitere Konfiguration erforderlich.

1. Konfigurieren Sie das SaaS-Projekt und den Datenraum, damit Commerce Services Daten an den Kanal-Manager-Dienst senden kann.

   ![[!DNL Commerce Service Connector] SaaS-ID-Konfiguration in der [!DNL Admin] Ansicht](assets/commerce-services-connector-saas-config.png)

