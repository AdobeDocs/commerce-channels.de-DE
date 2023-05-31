---
title: Hinzufügen von Produkten zum Kanal-Manager
description: "Erstellen Sie ein Produktsortiment für [!DNL Walmart Marketplace] Vertrieb durch Hinzufügen von Produkten aus dem Katalog zum im Kanal-Manager konfigurierten Vertriebskanal."
exl-id: 00932df7-bdc7-42a1-b269-88dffcc918bc
source-git-commit: a3ae579c0eda0c27bf8eab9d0ac12919eaad494b
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---


# Produkte hinzufügen zu [!DNL Channel Manager]

So fügen Sie Produkte zum [!DNL Walmart Marketplace] Vertriebskanal, wählen Sie sie aus dem [!DNL Commerce] Produktkatalog und importieren Sie sie in [!DNL Channel Manager].
Der Importvorgang kann je nach der Anzahl der ausgewählten Produkte bis zu 30 Minuten oder länger dauern.

## Voraussetzung

**[Katalogattribute zuordnen](map-catalog-attributes.md)**—Im [!DNL Channel Settings] -Konfiguration mindestens ein Attribut aus der [!DNL Commerce] Produktkatalog zu einer der erforderlichen Walmart Product Identifiers --GTIN, ISBN, ISSN, UPC, EAN.

## Listening-Anforderungen

[!DNL Commerce] Produktlisten müssen die folgende erforderliche Attributkonfiguration aufweisen:

- **[!UICONTROL Connect to Channel Manager]** Attribut aktiviert ist

- Geben Sie gültige Werte für die erforderlichen Walmart-Attribute an.

   - Mindestens ein Produktattribut, das mit einem der erforderlichen [!DNL Walmart Marketplace] Produktkennungen - GTIN, ISBN, ISSN, UPC, EAN.

   - Produktpreis, der auf maximal zwei Dezimalstellen festgelegt wird, z. B. `9.99`

   - Produktgewichtung, die auf maximal zwei Dezimalstellen festgelegt wird, z. B. `1.25`

>[!TIP]
>
>Weitere Informationen zur Optimierung von Auflistungen für Ihren Vertriebskanal finden Sie in der [Handbuch zur Qualitätsoptimierung von Walmart Marketplace-Listening](https://marketplace.walmart.com/wp-content/uploads/2020/09/WMP_listing_quality_optimization_guide.pdf).

## Produkte hinzufügen

1. Wählen Sie in einem verbundenen Verkaufskanalspeicher die Option **Produkte hinzufügen** , um den Produktkatalog zu öffnen.

   ![Produkte zum Verkaufskanalspeicher hinzufügen](assets/add-initial-products-to-connected-channel.png){width="600" zoomable="yes"}

   Der Katalog wird in einer neuen Registerkarte geöffnet.

1. Wählen Sie aus der Produktliste des Katalogs Produkte aus, die verkauft werden sollen [!DNL Walmart Marketplace].

   ![Senden von Produkten an den Verkaufskanalspeicher](assets/select-products-from-catalog.png){width="600" zoomable="yes"}

1. Aktivieren Sie die **[!UICONTROL Connect to Channel Manager]** -Attribut für die ausgewählten Elemente.

   - Von **[!UICONTROL Actions]** auswählen **[!UICONTROL Update attributes]**.

   - Scrollen Sie zum **[!UICONTROL Connect to Channel Manager]** -Attribut zuordnen und aktivieren.

   - Stellen Sie sicher, dass die Produktattribute mindestens eines der erforderlichen [!DNL Walmart Product IDs].

   - Auswählen **[!UICONTROL Save]**.

      Eine Bestätigungsmeldung wird angezeigt.

      ![Bestätigungsnachricht zum Produktimport von einem Katalog zu einem Verkaufskanal](assets/product-import-from-catalog-confirmation.png){width="400"}

      Wenn die Meldung anzeigt, dass die Aktualisierung geplant ist, verwenden Sie die [queue:consumers:start](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cli/start-message-queues.html) [!DNL CLI] -Befehl, um die Aktualisierung sofort zu verarbeiten.

      ```bash
      $ bin/magento queue:consumers:start product_action_attribute.update
      ```

1. Überprüfen Sie nach Abschluss des Importvorgangs die hinzugefügten Produkte, indem Sie zu [!DNL Channel Manager] und auswählen **[!UICONTROL Listings]**.

   Zunächst befinden sich die Produkte in *Entwurf* Status. Auswählen **[!UICONTROL Refresh products]** , um die Tabelle zu aktualisieren.

1. Aktualisieren Sie die Ansicht, um die neuen Produkte anzuzeigen, die dem Kanal-Manager hinzugefügt wurden, indem Sie die **[!UICONTROL Draft]** Statuskarte.

   ![Importierte Produkte in verbundene Vertriebskanäle](assets/products-in-marketplace-sales-channel.png){width="400" zoomable="yes"}


