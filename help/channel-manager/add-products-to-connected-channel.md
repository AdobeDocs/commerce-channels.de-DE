---
title: Produkte zum verbundenen Kanal hinzufügen
description: Erstellen Sie ein Produktsortiment für Marketplace-Verkäufe, indem Sie Produkte aus dem Katalog zum Vertriebskanal hinzufügen.
exl-id: 00932df7-bdc7-42a1-b269-88dffcc918bc
source-git-commit: e6368d30e16ccffcb1dfc64bdd56561116934b54
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Produkte zum verbundenen Kanal hinzufügen

Um Produkte mit dem Walmart Marketplace Vertriebskanal zu synchronisieren, wählen Sie Produkte aus dem [!DNL Commerce] Produktkatalog erstellen und in den Kanal-Manager importieren. Die ausgewählten Produkte müssen die folgende Attributkonfiguration aufweisen:

- **[!UICONTROL Publish to Channel Manager]** Attribut aktiviert ist

- Mindestens ein Produktattribut muss mit einem der [erforderliche Walmart Marketplace-Attribute](map-product-attributes-for-matching.md)- GTIN, ISBN, ISSN, UPC, EAN

Das Verfahren zum Importieren von Produkten aus [!DNL Commerce] Je nach der Anzahl der ausgewählten Produkte kann es bis zu 30 Minuten oder länger dauern.

## Produkte zum Vertriebskanal hinzufügen

1. Wählen Sie in einem verbundenen Verkaufskanalspeicher die Option **Produkte hinzufügen** , um den Produktkatalog zu öffnen.

   ![Produkte zum verbundenen Kanal hinzufügen](assets/add-initial-products-to-connected-channel.png)

   Der Katalog wird in einer neuen Registerkarte geöffnet.

1. Wählen Sie aus der Produktliste des Katalogs Produkte aus, die verkauft werden sollen [!DNL Walmart Marketplace].

   ![Produkte an den verbundenen Kanal senden](assets/select-products-from-catalog.png)

1. Aktivieren Sie die **[!UICONTROL Publish to Channel Manager]** -Attribut für die ausgewählten Elemente.

   - Von **[!UICONTROL Actions]** auswählen **[!UICONTROL Update attributes]**.

   - Scrollen Sie zum **[!UICONTROL Publish to Channel Manager]** -Attribut zuordnen und aktivieren.

   - Stellen Sie sicher, dass die Produktattribute mindestens eine der erforderlichen Walmart-Produkt-IDs enthalten.

   - Auswählen **[!UICONTROL Save]**.

   Eine Bestätigungsmeldung wird angezeigt.

   ![Bestätigungsnachricht zum Produktimport von einem Katalog zu einem Verkaufskanal](assets/product-import-from-catalog-confirmation.png)

   Wenn die Meldung anzeigt, dass die Aktualisierung geplant ist, verwenden Sie die [queue:consumers:start](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-queue.html) [!DNL CLI] -Befehl, um die Aktualisierung sofort zu verarbeiten.

   ```bash
   $ bin/magento queue:consumers:start product_action_attribute.update
   ```

1. Kehren Sie zum verbundenen Vertriebskanal in zurück. [!DNL Channel Manager].

1. Nachdem der Importvorgang abgeschlossen ist, zeigen Sie Produkte von an **[!UICONTROL Listings]**.

   ![Importierte Produkte in verbundene Vertriebskanäle](assets/products-in-marketplace-sales-channel.png)

   Zunächst befinden sich die Produkte in *Entwurf* Status. Auswählen **[!UICONTROL Refresh products]** , um die Tabelle zu aktualisieren.

