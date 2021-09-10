---
title: Nicht zulässige Listen
description: Der Amazon-Vertriebskanal bietet den Tab [!UICONTROL Ineligible] , mit dem Sie Elemente verwalten können, die basierend auf Ihren aktuellen Listenregeln nicht als Liste gelten.
exl-id: ae63898d-ff5c-43eb-b759-5bc80829d4d4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Nicht infrage kommende Listen

Der Tab _[!UICONTROL Ineligible]_enthält eine Liste aller Produkte, die derzeit in Amazon veröffentlicht sind, aber aufgrund Ihrer aktuellen Listening-Regeln nicht als Liste infrage kommen. Wenn ein früheres Produkt zugelassen war und die Listening-Regeln so geändert wurden, dass es jetzt nicht mehr zugelassen wird, wird die mit einem Produkt verknüpfte Menge auf 0 reduziert und das Produkt wird als_ nicht beihilfefähig _gekennzeichnet. Sie ist jedoch weiterhin auf Ihrem [!DNL Amazon Seller Account] vorhanden.

Um ein Produkt aus dem Tab _[!UICONTROL Ineligible]_zu verschieben, können Sie [Ihre Listening-Regeln](./listing-rules.md) ändern, damit Ihre Produkte zugelassen werden.

Zu den verfügbaren Aktionen auf der Registerkarte _[!UICONTROL Ineligible]_gehören:

Unter _[!UICONTROL Actions]_:

- **[!UICONTROL End Listing(s) on Amazon]**: Wählen Sie aus, um alle ausgewählten Listen aus der  [!DNL Amazon Marketplace]zu entfernen. Siehe [Beenden einer Amazon-Auflistung](./end-listings-manually.md).

- **[!UICONTROL Edit Listing Overrides]**: Wählen Sie aus, die Einstellungen zum Außerkraftsetzen für die Auflistung zu ändern. Siehe [Außerkraftsetzungen](./overrides.md) oder [Bearbeiten oder Entfernen einer Überschreibung](./creating-editing-overrides.md#edit-override-single-listing).

Unter **[!UICONTROL Select]** in der Spalte _[!UICONTROL Action]_:

- **[!UICONTROL View Details]**: Wählen Sie aus, ob Sie Details zur Liste anzeigen möchten, darunter das Protokoll zu den  [Listing-Aktivitäten](./product-listing-details.md#listing-activity-log), die  [Buy Box-Preise für Wettbewerber](./product-listing-details.md#buy-box-competitor-pricing) und die Preise für  [Niedrigste Konkurrenz](./product-listing-details.md#lowest-competitor-pricing). Diese Aktion dient nur der Anzeige. In den Listendetails können keine Änderungen vorgenommen werden. Siehe [Details anzeigen](./product-listing-details.md).

- **[!UICONTROL Create Override]**: Wählen Sie aus, eine Überschreibung zu erstellen und sie auf diese Auflistung anzuwenden. Siehe [Erstellen einer Überschreibung](./creating-editing-overrides.md).

- **[!UICONTROL Edit Assigned ASIN]**: Wählen Sie die Änderung des Ihrem Katalogprodukt zugewiesenen ASIN aus. Diese Aktion wird verwendet, wenn ein Produkt in Ihrem Katalog mit dem falschen ASIN abgeglichen wurde. Siehe [Zugewiesene ASIN bearbeiten](./edit-assigned-asin.md).

- **[!UICONTROL Create Alias Seller SKU]**: Wählen Sie die Erstellung einer Alias-SKU aus, die zum Erstellen einer Amazon-Liste aus demselben Katalogprodukt verwendet werden kann. Siehe [Alias-Verkäufer-SKU erstellen](./create-alias-seller-sku.md).

- **[!UICONTROL Switch to Fulfilled by Amazon/Merchant]**: Wählen Sie aus, ob die mit der Bestellung verknüpfte Ausführungsmethode geändert werden soll. Siehe [Konfiguration von &quot;Erfüllt durch&quot;-Einstellungen](./fulfilled-by.md#configure-fulfilled-by-settings).

- **[!UICONTROL End Listing]**: Wählen Sie aus, um die Liste aus der  [!DNL Amazon Marketplace]zu entfernen. Siehe [Beenden einer Amazon-Auflistung](./end-listings-manually.md).

>[!NOTE]
>Wenn Listen in Bearbeitung sind, wird die Anzahl der Auflistungen in einer Meldung über den Registerkarten angezeigt.

![Nicht infrage kommende Amazon-Listen](assets/amazon-ineligible-listings.png)

Die Startseiten der Amazon-Vertriebskanäle teilen einige gängige [Arbeitsbereichssteuerelemente](./workspace-controls.md), mit denen Sie die angezeigten Daten anpassen können.

## Standardspalten

| Spalte | Beschreibung |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | Die SKU (Stock Keeping Unit, Bestandseinheit), die von Amazon einem Produkt zugewiesen wurde, um das Produkt, die Optionen, den Preis und den Hersteller zu identifizieren. |
| [!UICONTROL ASIN] | Ein eindeutiger Block von 10 Buchstaben und/oder Zahlen zur Identifizierung von Elementen.<br><br>ASIN steht für die  [!DNL Amazon Standard Identification Number]. Ein ASIN ist ein eindeutiger Block von 10 Buchstaben und/oder Zahlen, der Elemente identifiziert. Bei Büchern entspricht das ASIN der ISBN-Nummer, bei allen anderen Produkten wird jedoch beim Hochladen des Artikels in den Katalog ein neues ASIN erstellt. Sie finden einen Artikel-ASIN auf der Produktdetailseite in Amazon sowie weitere Details zum Artikel. |
| [!UICONTROL Product Listing Name] | Der Name des Produkts. |
| [!UICONTROL Condition] | Die [Bedingung](./product-listing-condition.md) des Produkts. |
| [!UICONTROL Landed Price] | Der Börsennotierungspreis für das Produkt zuzüglich des Versandpreises. |
| [!UICONTROL Amazon Quantity] | Die verfügbare Menge, wenn das Produkt aktiv in Amazon aufgeführt wird. |
| [!UICONTROL Action] | Liste der verfügbaren Aktionen, die auf eine bestimmte Liste angewendet werden können. Um eine Aktion anzuwenden, klicken Sie in der Spalte _[!UICONTROL Action]_auf **[!UICONTROL Select]**und wählen Sie eine Option aus:<ul><li>[[!UICONTROL View Details]](./product-listing-details.md)</li><li>[Überschreibung erstellen](./creating-editing-overrides.md)</li><li>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)</li><li>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)</li><li>[[!UICONTROL Switch to Fulfilled By Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings)</li><li>[[!UICONTROL End Listing]](./end-listings-manually.md)</li></ul> |
