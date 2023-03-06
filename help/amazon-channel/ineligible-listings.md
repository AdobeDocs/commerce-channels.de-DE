---
title: Nicht zulässige Listen
description: Der Amazon-Vertriebskanal stellt die [!UICONTROL Ineligible] -Registerkarte, um Sie bei der Verwaltung von Elementen zu unterstützen, sind nicht als Liste auf der Grundlage Ihrer aktuellen Listening-Regeln qualifiziert.
exl-id: ae63898d-ff5c-43eb-b759-5bc80829d4d4
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Nicht zulässige Listen

Die _[!UICONTROL Ineligible]_zeigt eine Liste aller Produkte an, die derzeit in Amazon veröffentlicht sind, aber aufgrund Ihrer aktuellen Listening-Regeln nicht als Liste infrage kommen. Wenn ein früheres Produkt in Frage kam und die Listening-Regeln so geändert werden, dass es jetzt nicht mehr zugelassen wird, wird die mit einem Produkt verbundene Menge auf 0 gesetzt und das Produkt wird als_ nicht förderfähig _. Es ist jedoch weiterhin in Ihrer [!DNL Amazon Seller Account].

So verschieben Sie ein Produkt aus der _[!UICONTROL Ineligible]_Registerkarte [Ändern von Listening-Regeln](./listing-rules.md) , damit Ihre Produkte zugelassen werden können.

Die verfügbaren Aktionen für die _[!UICONTROL Ineligible]_einschließen:

under _[!UICONTROL Actions]_:

- **[!UICONTROL End Listing(s) on Amazon]**: Wählen Sie aus, ob alle ausgewählten Listen aus dem [!DNL Amazon Marketplace]. Siehe [Beenden einer Amazon-Auflistung](./end-listings-manually.md).

- **[!UICONTROL Edit Listing Overrides]**: Wählen Sie aus, die Einstellungen zum Außerkraftsetzen für die Auflistung zu ändern. Siehe [Überschreibungen](./overrides.md) oder [Bearbeiten oder Entfernen einer Überschreibung](./creating-editing-overrides.md#edit-override-single-listing).

under **[!UICONTROL Select]** im _[!UICONTROL Action]_column:

- **[!UICONTROL View Details]**: Wählen Sie aus, um Details zur Auflistung anzuzeigen, einschließlich der [Auflisten des Aktivitätsprotokolls](./product-listing-details.md#listing-activity-log), [Buy Box Konkurrentenpreise](./product-listing-details.md#buy-box-competitor-pricing)und [Niedrigste Preise für Wettbewerber](./product-listing-details.md#lowest-competitor-pricing). Diese Aktion dient nur der Anzeige. In den Listendetails können keine Änderungen vorgenommen werden. Siehe [Details anzeigen](./product-listing-details.md).

- **[!UICONTROL Create Override]**: Wählen Sie aus, eine Überschreibung zu erstellen und sie auf diese Auflistung anzuwenden. Siehe [Erstellen einer Überschreibung](./creating-editing-overrides.md).

- **[!UICONTROL Edit Assigned ASIN]**: Wählen Sie die Änderung des Ihrem Katalogprodukt zugewiesenen ASIN aus. Diese Aktion wird verwendet, wenn ein Produkt in Ihrem Katalog mit dem falschen ASIN abgeglichen wurde. Siehe [Zugewiesenes ASIN bearbeiten](./edit-assigned-asin.md).

- **[!UICONTROL Create Alias Seller SKU]**: Wählen Sie die Erstellung einer Alias-SKU aus, die zum Erstellen einer Amazon-Liste aus demselben Katalogprodukt verwendet werden kann. Siehe [Alias-Verkäufer-SKU erstellen](./create-alias-seller-sku.md).

- **[!UICONTROL Switch to Fulfilled by Amazon/Merchant]**: Wählen Sie aus, ob die mit der Bestellung verknüpfte Ausführungsmethode geändert werden soll. Siehe [Einstellungen für &quot;Erfüllt durch&quot;konfigurieren](./fulfilled-by.md#configure-fulfilled-by-settings).

- **[!UICONTROL End Listing]**: Wählen Sie aus, die Liste aus dem [!DNL Amazon Marketplace]. Siehe [Beenden einer Amazon-Auflistung](./end-listings-manually.md).

>[!NOTE]
>Wenn Listen in Bearbeitung sind, wird die Anzahl der Auflistungen in einer Meldung über den Registerkarten angezeigt.

![Nicht infrage kommende Amazon-Listen](assets/amazon-ineligible-listings.png)

Die Startseiten der Amazon-Vertriebskanäle teilen sich einige gemeinsame [Arbeitsbereichssteuerelemente](./workspace-controls.md) die es Ihnen ermöglichen, die angezeigten Daten anzupassen.

## Standardspalten

| Spalte | Beschreibung |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | Die SKU (Stock Keeping Unit, Bestandseinheit), die von Amazon einem Produkt zugewiesen wurde, um das Produkt, die Optionen, den Preis und den Hersteller zu identifizieren. |
| [!UICONTROL ASIN] | Ein eindeutiger Block von 10 Buchstaben und/oder Zahlen zur Identifizierung von Elementen.<br><br>ASIN steht für die [!DNL Amazon Standard Identification Number]. Ein ASIN ist ein eindeutiger Block von 10 Buchstaben und/oder Zahlen, der Elemente identifiziert. Bei Büchern entspricht das ASIN der ISBN-Nummer, bei allen anderen Produkten wird jedoch beim Hochladen des Artikels in den Katalog ein neues ASIN erstellt. Sie finden einen Artikel-ASIN auf der Produktdetailseite in Amazon sowie weitere Details zum Artikel. |
| [!UICONTROL Product Listing Name] | Der Name des Produkts. |
| [!UICONTROL Condition] | Die [Bedingung](./product-listing-condition.md) des Erzeugnisses. |
| [!UICONTROL Landed Price] | Der Börsennotierungspreis für das Produkt zuzüglich des Versandpreises. |
| [!UICONTROL Amazon Quantity] | Die verfügbare Menge, wenn das Produkt aktiv in Amazon aufgeführt wird. |
| [!UICONTROL Action] | Liste der verfügbaren Aktionen, die auf eine bestimmte Liste angewendet werden können. Um eine Aktion anzuwenden, klicken Sie auf **[!UICONTROL Select]** im _[!UICONTROL Action]_und wählen Sie eine Option aus:<ul><li>[[!UICONTROL View Details]](./product-listing-details.md)</li><li>[Überschreibung erstellen](./creating-editing-overrides.md)</li><li>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)</li><li>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)</li><li>[[!UICONTROL Switch to Fulfilled By Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings)</li><li>[[!UICONTROL End Listing]](./end-listings-manually.md)</li></ul> |
