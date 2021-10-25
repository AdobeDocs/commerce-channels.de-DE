---
title: Unvollständige Auflistungen
description: Amazon Sales Kanal bietet [!UICONTROL Incomplete] , um Ihnen zu helfen, die Voraussetzungen für eine unvollständige Amazon-Auflistung zu ermitteln und zu erfüllen.
exl-id: f943c9cc-fa1d-4f3e-a3de-3a8d00f87890
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# Unvollständige Auflistungen

Die _[!UICONTROL Incomplete]_Tabulator-Listen [!DNL Commerce] Katalogprodukte, die Ihren Amazon-Förderkriterien entsprechen (siehe [Listungsregeln](./listing-rules.md)), fehlen jedoch Informationen, die von Amazon benötigt werden (z. B. Amazon ASIN oder eine bestimmte Produktbedingung).

Es gibt vier mögliche Gründe für eine unvollständige Auflistung, die jeweils durch ihren Status gekennzeichnet sind.

| Status | Grund | Aktion |
|--- |--- |--- |
| Fehlende Bedingung | Amazon akzeptiert Auflistungen unter verschiedenen Bedingungen (z. B. _Neu_, _Renoviert_, _Verwendet: Neu_) Auflistung erfordert eine definierte Bedingung. | Erforderliche Informationen manuell aktualisieren [Bedingung zuweisen](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) in eine Liste. |
| Amazon-Liste kann nicht zugewiesen werden | Automatische Übereinstimmung dieser Auflistung mit Ihrem Katalog fehlgeschlagen. Wenn keine Übereinstimmung gefunden wird, kann die Liste nicht vom Amazon Sales Channel verwaltet werden | Erforderliche Informationen manuell aktualisieren [ASIN zuweisen](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) zum Katalog-Produkt, um mit der Liste abzustimmen. |
| Mehrere Übereinstimmungen gefunden | Automatische Übereinstimmung dieser Auflistung mit Ihrem Katalog fehlgeschlagen. Wenn mehrere mögliche Übereinstimmungen gefunden werden, müssen Sie die richtige Übereinstimmung für Ihr Produkt auswählen. | Erforderliche Informationen manuell aktualisieren [Produktübereinstimmung auswählen](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) für das Produkt und die Auflistung. |
| Enthält Varianten | Wenn Ihr Produkt Varianten enthält, z. B. ein T-Shirt, das in verschiedenen Größen oder Farben erhältlich ist, müssen Sie die Variante in Ihrem Katalog auswählen, damit sie korrekt zugeordnet und der Liste zugeordnet werden kann. | Erforderliche Informationen manuell aktualisieren [richtige Variante wählen](./amazon-manually-update-incomplete-listing.md#update-required-info-has-variants) , um dieser Auflistung zuzuweisen und ihr zu entsprechen. |

>[!NOTE]
>Wenn unvollständige Auflistungen Ihren Katalogprodukten korrekt zugeordnet sind, wird die Liste von der _[!UICONTROL Incomplete]_und auf Amazon basierend auf Ihrem [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) Einstellungen.

Die verfügbaren Maßnahmen im Rahmen der _[!UICONTROL Incomplete]_Registereinschluss:

Unter _[!UICONTROL Actions]_:

- **[!UICONTROL Re-attempt to auto match to Amazon listings]**: Wählen Sie, ob Sie den automatischen Prozess zur Zuordnung Ihrer Amazon-Listendaten zu Ihren [!DNL Commerce] Katalog. Wenn die Produkte nicht automatisch übereinstimmen, besuchen Sie Ihre [_[!UICONTROL Catalog Search]_](./catalog-search.md) Optionen in Ihren Listeneinstellungen. Wenn Auflistungen nach der Aktualisierung Ihrer _[!UICONTROL Catalog Search]_können Sie die Produkte manuell in der [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) Aktion.

Unter **[!UICONTROL Select]** in _[!UICONTROL Action]_Spalte:

- **[!UICONTROL Update Required Info]**: Wählen Sie aus, ob Auflistungen nicht automatisch mit Ihrem Katalog übereinstimmen. Sie können [Katalogprodukte mit Listen abgleichen](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found), manuell [ASIN zuweisen](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) zu einer Katalogübereinstimmung oder [fehlende Bedingung zuweisen](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) für die Auflistung.

- **[!UICONTROL View Details]**: Wählen Sie eine Ansicht aus, in der Details wie [Listing-Aktivität-Protokoll](./product-listing-details.md#listing-activity-log), [Buy Box Konkurrent-Preise](./product-listing-details.md#buy-box-competitor-pricing)und [Niedrigste Konkurrent-Preise](./product-listing-details.md#lowest-competitor-pricing). Diese Aktion dient nur zum Anzeigen. In den Details der Auflistung können keine Änderungen vorgenommen werden. Siehe [Ansicht - Details](./product-listing-details.md).

>[!NOTE]
>
>Wenn Sie Listen bearbeiten, erscheint die Anzahl der Einträge in einer Meldung über den Registerkarten.

![Unvollständige Amazon-Auflistungen](assets/amazon-incomplete-listings.png)

Amazon Sales Kanal Startseite teilen einige gemeinsame [Arbeitsbereichssteuerelemente](./workspace-controls.md) , mit denen Sie die angezeigten Daten anpassen können.

| Spalte | Beschreibung |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | Die von Amazon einem Produkt zugewiesene SKU (Stock Keeping Unit) zur Identifizierung des Produkts, der Optionen, des Preises und des Herstellers. |
| [!UICONTROL ASIN] | Ein eindeutiger Block mit 10 Buchstaben und/oder Zahlen, die Elemente identifizieren.<br><br>ASIN steht für [!DNL Amazon Standard Identification Number]. Ein ASIN ist ein eindeutiger Block mit 10 Buchstaben und/oder Ziffern, der Elemente identifiziert. Für Bücher ist die ASIN die gleiche ISBN-Nummer, aber für alle anderen Produkte wird ein neues ASIN erstellt, wenn das Element in ihren Katalog hochgeladen wird. Auf der Produktdetailseite auf Amazon finden Sie ASIN und weitere Details zum Artikel. |
| [!UICONTROL Product Listing Name] | Der Name des Produkts. |
| [!UICONTROL Condition] | Die [Bedingung](./product-listing-condition.md) des Erzeugnisses. |
| [!UICONTROL Landed Price] | Der Listenpreis des Produkts zuzüglich des Versandpreises. |
| [!UICONTROL Amazon Quantity] | Die Menge, die verfügbar ist, wenn das Produkt aktiv auf Amazon aufgeführt wird. |
| [!UICONTROL Status] | Der von Amazon definierte Status der Auflistung. Siehe die obige Statustabelle. |
| [!UICONTROL Action] | Liste der verfügbaren Aktionen, die auf eine bestimmte Auflistung angewendet werden können. Klicken Sie zum Anwenden einer Aktion auf **[!UICONTROL Select]** in _[!UICONTROL Action]_-Spalte und wählen Sie eine Option aus:<ul><li>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
