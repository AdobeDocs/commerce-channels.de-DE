---
title: Verbindung zu Commerce Services herstellen
description: Verbinden der Kanal-Manager-Instanz mit [!DNL Commerce services] , um die Datensynchronisation und Kommunikation zwischen der Commerce-Instanz, dem Kanal-Manager und anderen unterstützenden Diensten zu aktivieren.
role: User
level: Intermediate
source-git-commit: ec950579a9b2220f9ec106b616779fc3503f3add
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Verbindung zu Commerce Services herstellen

Der Commerce Services Connector integriert den Channel Manager-Dienst in Adobe Commerce- und Magento Open Source-Instanzen. Der Connector ermöglicht die Datensynchronisation und Kommunikation zwischen dem [!DNL Commerce] Instanz, [!DNL Channel Manager]und andere unterstützende Dienste.

Die Einrichtung des Commerce Services Connector ist ein einmaliger Prozess, der für die Verwendung von Adobe erforderlich ist [Commerce SaaS-Dienste](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html){target=&quot;_blank&quot;} wie [!DNL Channel Manager], [!DNL Live Search]und [!DNL Product Recommendations]. Wenn Sie den Connector bereits für einen anderen Dienst konfiguriert haben, können Sie diesen Schritt überspringen.

## Voraussetzungen

- **Commerce-Konto mit [Administratorzugriff](https://docs.magento.com/user-guide/stores/admin.html){target=&quot;_blank&quot;}** zu Ihrer Commerce-Instanz** - Kontoinhaber und Admin-Benutzer können Benutzerkonten über die Commerce-Instanz oder über die Befehlszeile mithilfe der [!DNL Commerce] CLI, Befehl `admin:user:create`.

- **Adobe Commerce [Produktions-API-Schlüssel](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;}**-Aktivieren Sie den API-Zugriff auf Dienste, die für den Kanal-Manager erforderlich sind

   Um die Anmeldedaten bereitzustellen, hat ein Inhaber einer Commerce-Lizenz oder eines Kontos folgende Optionen:
   [Freigeben von Zugriff](https://docs.magento.com/user-guide/magento/magento-account-share.html){target=&quot;_blank&quot;} oder geben Sie die [API-Schlüssel](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;} Anmeldedaten für einen vertrauenswürdigen Entwickler.

## Connector für Commerce Services konfigurieren

1. Öffnen Sie die Konfiguration der Store-Dienste .

   - Wählen Sie im Admin die Option [!UICONTROL Stores].

   - under *Einstellungen* auswählen [!UICONTROL Configuration].

   - Im [!UICONTROL Configuration] Seite, erweitern [!UICONTROL Services] und wählen Sie [!UICONTROL Commerce Services Connector].

1. Fügen Sie Produktions-API-Schlüssel aus Ihrem Adobe Commerce-Konto hinzu.

   ![[!DNL Commerce Service Connector] im [!DNL Admin] Ansicht](assets/commerce-services-connector-admin-service-view.png)


   >[!NOTE]
   >
   > Wenn [!DNL Commerce] Instanz hat andere [!DNL Adobe Commerce] Dienste wie [!DNL Live Search] oder [!DNL Product Recommendations] installiert ist, werden die Anmeldeinformationen in der Benutzeroberfläche angezeigt und es ist keine weitere Konfiguration erforderlich.

1. Konfigurieren Sie das SaaS-Projekt und den Datenraum, damit Commerce Services Daten an den Kanal-Manager-Dienst senden kann.

   ![[!DNL Commerce Service Connector] SaaS-ID-Konfiguration in der [!DNL Admin] Ansicht](assets/commerce-services-connector-saas-config.png)

