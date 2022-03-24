---
title: Produkte zum Kanalspeicher hinzufügen
description: Erstellen Sie ein Produktsortiment für Marketplace-Verkäufe, indem Sie Produkte aus dem Katalog zum Vertriebskanal hinzufügen.
source-git-commit: 905bedaf1eacdc45b2b7f222e7703e1f7b3dfd9c
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---


# Produkte zum Kanalspeicher hinzufügen

Wählen Sie im Kanal-Manager Produkte aus der [!DNL Commerce] Katalog für Walmart Marketplace-Verkäufe.

Um Produkte mit dem Vertriebskanal zu synchronisieren, müssen die ausgewählten Produkte die folgende Attributkonfiguration aufweisen:

- **[!UICONTROL Publish to Channel Manager]** Attribut aktiviert ist

- Mindestens ein Produktattribut muss mit einem der [erforderliche Walmart Marketplace-Attribute](map-product-attributes-for-matching.md)- GTIN, ISBN, ISSN, UPC, EAN

Nachdem Sie die Auswahl gespeichert haben, importiert der Kanal-Manager die Produktdaten in den Kanal. Dieser Vorgang kann bis zu 30 Minuten dauern.

## Produkte zum Vertriebskanal hinzufügen

1. Öffnen Sie den Produktkatalog, der Ihrem Kanal-Manager-Store zugeordnet ist.

   Wählen Sie in einem verbundenen Verkaufskanalspeicher die Option **Produkte hinzufügen**.

   ![Produkte zum verbundenen Kanal hinzufügen](assets/add-initial-products-to-connected-channel.png)

   Der Katalog wird in einer neuen Registerkarte geöffnet.

1. Wählen Sie aus dem Katalog-Produktraster Produkte aus, die auf dem Walmart Marketplace verkauft werden sollen.

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

   Nachdem der Importvorgang abgeschlossen ist, zeigen Sie Produkte von an **[!UICONTROL Listings]**. Zunächst befinden sich die Produkte in *Entwurf* Status. Auswählen [!UICONTROL Refresh products]**, um die Tabelle zu aktualisieren.

   ![Importierte Produkte in verbundene Vertriebskanäle](assets/products-in-marketplace-sales-channel.png)
