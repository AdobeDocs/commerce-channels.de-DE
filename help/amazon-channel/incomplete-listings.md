---
title: Unvollständige Amazon-Listen
description: Der Amazon-Vertriebskanal enthält den Tab [!UICONTROL Incomplete] , mit dem Sie die Voraussetzungen für Ihre unvollständigen Amazon-Auflistungen identifizieren und erfüllen können.
feature: Sales Channels, Products
exl-id: f943c9cc-fa1d-4f3e-a3de-3a8d00f87890
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# Unvollständige Amazon-Listen

Auf der Registerkarte &quot;_[!UICONTROL Incomplete]_&quot;werden die [!DNL Commerce] -Katalogprodukte aufgelistet, die Ihren (in Ihren [Listening-Regeln](./listing-rules.md) definierten) Amazon-Eignungsanforderungen entsprechen, aber Informationen fehlen, die für Amazon erforderlich sind (z. B. Amazon-ASIN oder eine definierte Produktbedingung).

Es gibt vier mögliche Ursachen für eine unvollständige Auflistung, die jeweils durch ihren Status identifiziert werden.

| Status | Grund | Aktion |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Fehlende Bedingung | Amazon akzeptiert Auflistungen unter verschiedenen Bedingungen (z. B. _Neu_, _Neu renoviert_, _Verwendet: Wie Neu_). Für die Auflistung ist eine definierte Bedingung erforderlich. | Aktualisieren Sie die erforderlichen Informationen und weisen Sie einer Auflistung manuell [eine Bedingung](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) zu. |
| Der Amazon-Auflistung kann nicht zugewiesen werden | Die automatische Übereinstimmung dieser Auflistung mit Ihrem Katalog ist fehlgeschlagen. Wenn keine Übereinstimmung gefunden wird, kann die Auflistung nicht von Amazon Sales Channel verwaltet werden | Aktualisieren Sie die erforderlichen Informationen und weisen Sie dem Katalogprodukt manuell [ein ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) zu, damit es mit der Auflistung übereinstimmt. |
| Mehrere Treffer gefunden | Die automatische Übereinstimmung dieser Auflistung mit Ihrem Katalog ist fehlgeschlagen. Wenn mehrere mögliche Übereinstimmungen gefunden werden, müssen Sie die richtige Übereinstimmung für Ihr Produkt auswählen. | Aktualisieren Sie die erforderlichen Informationen und wählen Sie manuell [eine Produktübereinstimmung](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) für das Produkt und die Auflistung aus. |
| Hat Varianten | Wenn Ihr Produkt Varianten aufweist, z. B. ein T-Shirt, das in unterschiedlichen Größen oder Farben verfügbar ist, müssen Sie die Variante in Ihrem Katalog auswählen, damit sie korrekt zugeordnet und mit der Auflistung abgeglichen wird | Aktualisieren Sie die erforderlichen Informationen und wählen Sie manuell [die richtige Variante](./amazon-manually-update-incomplete-listing.md#update-required-info-has-variants) aus, die dieser Auflistung zugewiesen und zugeordnet werden soll. |

>[!NOTE]
>Wenn unvollständige Listen ordnungsgemäß mit Ihren Katalogprodukten übereinstimmen, wird die Liste vom Tab _[!UICONTROL Incomplete]_aus verschoben und basierend auf Ihren [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) -Einstellungen in Amazon veröffentlicht.

Zu den verfügbaren Aktionen auf der Registerkarte _[!UICONTROL Incomplete]_gehören:

Unter _[!UICONTROL Actions]_:

- **[!UICONTROL Re-attempt to auto match to Amazon listings]**: Wählen Sie aus, den automatischen Prozess für die Zuordnung Ihrer Amazon-Listings-Daten zu Ihrem [!DNL Commerce] -Katalog zu starten. Wenn Produkte nicht automatisch übereinstimmen, überprüfen Sie Ihre [_[!UICONTROL Catalog Search]_](./catalog-search.md) -Optionen in Ihren Listeneinstellungen erneut. Wenn Auflistungen nach der Aktualisierung Ihrer _[!UICONTROL Catalog Search]_-Optionen nicht automatisch übereinstimmen, können Sie Produkte in der Aktion [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found) manuell zuordnen.

Unter **[!UICONTROL Select]** in der Spalte _[!UICONTROL Action]_:

- **[!UICONTROL Update Required Info]**: Wählen Sie aus, wann die Auflistungen nicht automatisch mit Ihrem Katalog übereinstimmen. Sie können Katalogprodukte manuell [ mit Auflistungen zuordnen](./amazon-manually-update-incomplete-listing.md#update-required-info-multiple-matches-found), manuell [einem Katalogabgleich ein ASIN](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) zuweisen oder [eine fehlende Bedingung](./amazon-manually-update-incomplete-listing.md#update-required-info-missing-condition) für die Auflistung zuweisen.

- **[!UICONTROL View Details]**: Wählen Sie diese Option, um Details zur Auflistung anzuzeigen, einschließlich des [Protokoll zu den Listing-Aktivitäten](./product-listing-details.md#listing-activity-log), des [Buy Box Konkurrenz-Preises](./product-listing-details.md#buy-box-competitor-pricing) und des [Niedrigsten konkurrierenden Preises](./product-listing-details.md#lowest-competitor-pricing). Diese Aktion dient nur der Anzeige. In den Listendetails können keine Änderungen vorgenommen werden. Siehe [Details anzeigen](./product-listing-details.md).

>[!NOTE]
>
>Wenn Listen in Bearbeitung sind, wird die Anzahl der Auflistungen in einer Meldung über den Registerkarten angezeigt.

![Unvollständige Amazon-Listen](assets/amazon-incomplete-listings.png){width="600" zoomable="yes"}

Die Startseiten der Amazon-Verkaufskanäle teilen einige gängige [Arbeitsbereichssteuerelemente](./workspace-controls.md), mit denen Sie die angezeigten Daten anpassen können.

| Spalte | Beschreibung |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Amazon Seller SKU] | Die von Amazon einem Produkt zugewiesene SKU (Stock Keeping Unit, Bestandseinheit) zur Identifizierung von Produkt, Optionen, Preis und Hersteller. |
| [!UICONTROL ASIN] | Ein eindeutiger Block von 10 Buchstaben und/oder Zahlen zur Identifizierung von Elementen.<br><br>ASIN steht für den [!DNL Amazon Standard Identification Number]. Ein ASIN ist ein eindeutiger Block von 10 Buchstaben und/oder Zahlen, der Elemente identifiziert. Bei Büchern entspricht das ASIN der ISBN-Nummer, bei allen anderen Produkten wird jedoch beim Hochladen des Artikels in den Katalog ein neues ASIN erstellt. Sie finden einen Artikel-ASIN auf der Produktdetailseite in Amazon sowie weitere Details zum Artikel. |
| [!UICONTROL Product Listing Name] | Der Name des Produkts. |
| [!UICONTROL Condition] | Die [Bedingung](./product-listing-condition.md) des Produkts. |
| [!UICONTROL Landed Price] | Der Börsennotierungspreis für das Produkt zuzüglich des Versandpreises. |
| [!UICONTROL Amazon Quantity] | Die verfügbare Menge, wenn das Produkt aktiv in Amazon aufgeführt wird. |
| [!UICONTROL Status] | Der von Amazon definierte Status der Auflistung. Siehe Tabelle Status weiter oben. |
| [!UICONTROL Action] | Liste der verfügbaren Aktionen, die auf eine bestimmte Liste angewendet werden können. Um eine Aktion anzuwenden, klicken Sie in der Spalte _[!UICONTROL Action]_auf **[!UICONTROL Select]**und wählen Sie eine Option aus:<ul><li>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
