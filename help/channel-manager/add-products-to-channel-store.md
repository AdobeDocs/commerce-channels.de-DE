---
title: Hinzufügen von Produkten zum Kanal-Manager
description: "Erstellen Sie ein Produktsortiment für den [!DNL Walmart Marketplace] Verkauf, indem Sie Produkte aus dem Katalog zum im Kanal-Manager konfigurierten Vertriebskanal hinzufügen."
feature: Sales Channels, Merchandising, Products
exl-id: 00932df7-bdc7-42a1-b269-88dffcc918bc
source-git-commit: 0087d60791cf00e4ed2bffe992447ee8e592fd9b
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---


# Produkte zu [!DNL Channel Manager] hinzufügen

Um Produkte zum Absatzkanal [!DNL Walmart Marketplace] hinzuzufügen, wählen Sie sie aus dem Produktkatalog von [!DNL Commerce] aus und importieren Sie sie in [!DNL Channel Manager].
Der Importvorgang kann je nach der Anzahl der ausgewählten Produkte bis zu 30 Minuten oder länger dauern.

## Voraussetzung

**[Katalogattribute zuordnen](map-catalog-attributes.md)** - Ordnen Sie in der [!DNL Channel Settings] -Konfiguration mindestens ein Attribut aus dem [!DNL Commerce] -Produktkatalog einer der erforderlichen Walmart Product Identifiers --GTIN, ISBN, ISSN, UPC, EAN zu.

## Listening-Anforderungen

[!DNL Commerce] -Produktlisten müssen die folgende erforderliche Attributkonfiguration aufweisen:

- **[!UICONTROL Connect to Channel Manager]** Attribut ist aktiviert

- Geben Sie gültige Werte für die erforderlichen Walmart-Attribute an.

   - Mindestens ein Produktattribut, das einer der erforderlichen [!DNL Walmart Marketplace] Produktidentifikatoren-GTIN, ISBN, ISSN, UPC, EAN entspricht.

   - Produktpreis, der auf maximal zwei Dezimalstellen festgelegt wird, z. B. `9.99`

   - Produktgewichtung, die auf maximal zwei Dezimalstellen festgelegt wird, z. B. `1.25`

>[!TIP]
>
>Weitere Informationen zur Optimierung von Auflistungen für Ihren Vertriebskanal finden Sie im [Handbuch zur Qualitätsoptimierung von Walmart Marketplace-Listening-Listen](https://marketplace.walmart.com/wp-content/uploads/2020/09/WMP_listing_quality_optimization_guide.pdf).

## Produkte hinzufügen

1. Wählen Sie in einem verbundenen Verkaufskanalspeicher **Produkte hinzufügen** aus, um den Produktkatalog zu öffnen.

   ![Produkte zum Verkaufskanalspeicher hinzufügen](assets/add-initial-products-to-connected-channel.png){width="600" zoomable="yes"}

   Der Katalog wird in einer neuen Registerkarte geöffnet.

1. Wählen Sie im Katalogproduktraster Produkte aus, die mit [!DNL Walmart Marketplace] verkauft werden sollen.

   ![Produkte an den Verkaufskanalspeicher senden](assets/select-products-from-catalog.png){width="600" zoomable="yes"}

1. Aktivieren Sie das Attribut **[!UICONTROL Connect to Channel Manager]** für die ausgewählten Elemente.

   - Wählen Sie unter **[!UICONTROL Actions]** die Option **[!UICONTROL Update attributes]** aus.

   - Scrollen Sie zum Attribut **[!UICONTROL Connect to Channel Manager]** und aktivieren Sie es.

   - Stellen Sie sicher, dass die Produktattribute mindestens einen der erforderlichen [!DNL Walmart Product IDs] enthalten.

   - Wählen Sie **[!UICONTROL Save]** aus.

     Eine Bestätigungsmeldung wird angezeigt.

     ![Meldung über den Produktimport aus dem Katalog zur Bestätigung des Verkaufskanals](assets/product-import-from-catalog-confirmation.png){width="400"}

     Wenn die Meldung anzeigt, dass die Aktualisierung geplant ist, verwenden Sie den Befehl [`queue:consumers:start`](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cli/start-message-queues.html) [!DNL CLI] , um die Aktualisierung sofort zu verarbeiten.

     ```bash
     $ bin/magento queue:consumers:start product_action_attribute.update
     ```

1. Überprüfen Sie nach Abschluss des Importvorgangs die hinzugefügten Produkte, indem Sie zu [!DNL Channel Manager] zurückkehren und **[!UICONTROL Listings]** auswählen.

   Zunächst befinden sich die Produkte im Status *Entwurf* . Wählen Sie **[!UICONTROL Refresh products]** aus, um die Tabelle zu aktualisieren.

1. Aktualisieren Sie die Ansicht, um die neuen Produkte anzuzeigen, die dem Kanal-Manager hinzugefügt wurden, indem Sie die Statuskarte **[!UICONTROL Draft]** auswählen.

   ![In den verbundenen Vertriebskanal importierte Produkte](assets/products-in-marketplace-sales-channel.png){width="400" zoomable="yes"}


