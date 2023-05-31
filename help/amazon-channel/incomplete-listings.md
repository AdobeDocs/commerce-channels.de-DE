---
title: Unvollständige Amazon-Listen
description: Der Amazon-Vertriebskanal stellt die [!UICONTROL Incomplete] -Tab, damit Sie die Voraussetzungen für eine unvollständige Amazon-Auflistung identifizieren und erfüllen können.
exl-id: f943c9cc-fa1d-4f3e-a3de-3a8d00f87890
source-git-commit: df26834c81b5e26ad0ea8c94c14292eb7c24bae8
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# Unvollständige Amazon-Listen

Die _[!UICONTROL Incomplete]_enthält [!DNL Commerce] Katalogprodukte, die Ihren Amazon-Eignungsanforderungen entsprechen (definiert in Ihrem [Auflistungsregeln](./listing-rules.md)), fehlen jedoch Informationen, die von Amazon benötigt werden (z. B. Amazon ASIN oder eine definierte Produktbedingung).

Es gibt vier mögliche Ursachen für eine unvollständige Auflistung, die jeweils durch ihren Status identifiziert werden.

| Status | Grund | Aktion |
|--- |--- |--- |
| Fehlende Bedingung | Amazon akzeptiert Auflistungen unter verschiedenen Bedingungen (z. B. _Neu_, _renoviert_, _Verwendet: Like New_) erfordert eine definierte Bedingung. | Erforderliche Informationen und manuell aktualisieren [Zuweisen einer Bedingung](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) auf eine Liste. |
| Der Amazon-Auflistung kann nicht zugewiesen werden | Die automatische Übereinstimmung dieser Auflistung mit Ihrem Katalog ist fehlgeschlagen. Wenn keine Übereinstimmung gefunden wird, kann die Auflistung nicht vom Amazon-Sales Channel verwaltet werden | Erforderliche Informationen und manuell aktualisieren [ZUWEISEN VON ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) zum Katalogprodukt, um mit der Auflistung abzugleichen. |
| Mehrere gefundene Übereinstimmungen | Die automatische Übereinstimmung dieser Auflistung mit Ihrem Katalog ist fehlgeschlagen. Wenn mehrere mögliche Übereinstimmungen gefunden werden, müssen Sie die richtige Übereinstimmung für Ihr Produkt auswählen. | Erforderliche Informationen und manuell aktualisieren [Produktabgleich auswählen](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) für das Produkt und die Auflistung. |
| Hat Varianten | Wenn Ihr Produkt Varianten aufweist, z. B. ein T-Shirt, das in unterschiedlichen Größen oder Farben verfügbar ist, müssen Sie die Variante in Ihrem Katalog auswählen, damit sie korrekt zugeordnet und mit der Auflistung abgeglichen wird | Erforderliche Informationen und manuell aktualisieren [die richtige Variante auswählen](./amazon-manually-update-incomplete-listing.md#update-required-info-has-variants) , um dieser Auflistung zuzuweisen und sie zuzuordnen. |

>[!NOTE]
>Wenn unvollständige Listen ordnungsgemäß mit Ihren Katalogprodukten übereinstimmen, wird die Liste von der _[!UICONTROL Incomplete]_und basierend auf Ihrer [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) -Einstellungen.

Die verfügbaren Aktionen für die _[!UICONTROL Incomplete]_einschließen:

under _[!UICONTROL Actions]_:

- **[!UICONTROL Re-attempt to auto match to Amazon listings]**: Wählen Sie aus, den automatischen Prozess für die Zuordnung Ihrer Amazon-Listendaten zu Ihren [!DNL Commerce] Katalog. Wenn Produkte nicht automatisch übereinstimmen, rufen Sie Ihre [_[!UICONTROL Catalog Search]_](./catalog-search.md) Optionen in Ihren Listeneinstellungen. Wenn Auflistungen nach der Aktualisierung Ihrer _[!UICONTROL Catalog Search]_-Optionen verwenden, können Sie Produkte manuell in der [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) Aktion.

under **[!UICONTROL Select]** im _[!UICONTROL Action]_column:

- **[!UICONTROL Update Required Info]**: Wählen Sie aus, wann die Listen nicht automatisch mit Ihrem Katalog übereinstimmen. Sie können [Übereinstimmung von Katalogprodukten mit Listen](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found)manuell [ZUWEISEN VON ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) einer Katalogübereinstimmung oder [fehlende Bedingung zuweisen](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) für die Auflistung.

- **[!UICONTROL View Details]**: Wählen Sie aus, um Details zur Auflistung anzuzeigen, einschließlich der [Auflisten des Aktivitätsprotokolls](./product-listing-details.md#listing-activity-log), [Buy Box Konkurrentenpreise](./product-listing-details.md#buy-box-competitor-pricing)und [Niedrigste Preise für Wettbewerber](./product-listing-details.md#lowest-competitor-pricing). Diese Aktion dient nur der Anzeige. In den Listendetails können keine Änderungen vorgenommen werden. Siehe [Details anzeigen](./product-listing-details.md).

>[!NOTE]
>
>Wenn Listen in Bearbeitung sind, wird die Anzahl der Auflistungen in einer Meldung über den Registerkarten angezeigt.

![Unvollständige Amazon-Listen](assets/amazon-incomplete-listings.png){width="600" zoomable="yes"}

Die Startseiten der Amazon-Vertriebskanäle teilen sich einige gemeinsame [Arbeitsbereichssteuerelemente](./workspace-controls.md) die es Ihnen ermöglichen, die angezeigten Daten anzupassen.

| Spalte | Beschreibung |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | Die SKU (Stock Keeping Unit, Bestandseinheit), die von Amazon einem Produkt zugewiesen wurde, um das Produkt, die Optionen, den Preis und den Hersteller zu identifizieren. |
| [!UICONTROL ASIN] | Ein eindeutiger Block von 10 Buchstaben und/oder Zahlen zur Identifizierung von Elementen.<br><br>ASIN steht für die [!DNL Amazon Standard Identification Number]. Ein ASIN ist ein eindeutiger Block von 10 Buchstaben und/oder Zahlen, der Elemente identifiziert. Bei Büchern entspricht das ASIN der ISBN-Nummer, bei allen anderen Produkten wird jedoch beim Hochladen des Artikels in den Katalog ein neues ASIN erstellt. Sie finden einen Artikel-ASIN auf der Produktdetailseite in Amazon sowie weitere Details zum Artikel. |
| [!UICONTROL Product Listing Name] | Der Name des Produkts. |
| [!UICONTROL Condition] | Die [Bedingung](./product-listing-condition.md) des Erzeugnisses. |
| [!UICONTROL Landed Price] | Der Börsennotierungspreis für das Produkt zuzüglich des Versandpreises. |
| [!UICONTROL Amazon Quantity] | Die verfügbare Menge, wenn das Produkt aktiv in Amazon aufgeführt wird. |
| [!UICONTROL Status] | Der von Amazon definierte Status der Auflistung. Siehe Tabelle Status weiter oben. |
| [!UICONTROL Action] | Liste der verfügbaren Aktionen, die auf eine bestimmte Liste angewendet werden können. Um eine Aktion anzuwenden, klicken Sie auf **[!UICONTROL Select]** im _[!UICONTROL Action]_und wählen Sie eine Option aus:<ul><li>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
