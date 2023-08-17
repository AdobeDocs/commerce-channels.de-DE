---
title: Amazon-Vertriebskanal - [!UICONTROL Ready to List]
description: Der Amazon-Vertriebskanal bietet die Registerkarte "Listenbereit", mit der Sie Commerce-Produkte überprüfen können, die die Voraussetzungen erfüllen, aber nicht automatisch aufgelistet werden.
feature: Sales Channels, Products, Merchandising
exl-id: f62017fb-964f-43f0-b76b-8f39f447466a
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# [!UICONTROL Ready to List]

Die _[!UICONTROL Ready to List]_-Registerkarte zeigt Ihre [!DNL Commerce] Katalogprodukte, die Ihren Listeneinstellungen entsprechen und in Amazon as a veröffentlicht werden können **new**Auflistung. Im Gegensatz zu anderen Listenregisterkarten wird diese Registerkarte nicht immer auf der [_[!UICONTROL Product Listings]_](./managing-product-listings.md) Seite.

Die _[!UICONTROL Ready to List]_nur angezeigt, wenn [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) in Ihren Listeneinstellungen auf `Do Not Automatically List Eligible Products`. Diese Einstellung teilt dem Amazon-Vertriebskanal mit, dass alle neuen Amazon-Auflistungen manuell veröffentlicht werden müssen.

Wann [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) auf `Automatically List Eligible Products`, veröffentlicht der Amazon-Vertriebskanal automatisch neue Einträge für Ihre entsprechenden Katalogprodukte. Da neue Listen automatisch veröffentlicht werden, wird die _[!UICONTROL Ready to List]_nicht angezeigt.

under _[!UICONTROL Actions]_:

- **[!UICONTROL Publish Product to Amazon]**: Wählen Sie aus, die Liste erneut im [!DNL Amazon Marketplace]. Siehe [Veröffentlichen von Amazon-Listen](./publish-listings-manually.md)

under **[!UICONTROL Select]** im _[!UICONTROL Action]_column:

- **[!UICONTROL Publish On Amazon]**: Wählen Sie aus, die Liste erneut im [!DNL Amazon Marketplace]. Siehe [Veröffentlichen von Amazon-Listen](./publish-listings-manually.md).

- **[!UICONTROL View Details]**: Wählen Sie aus, um Details zur Auflistung anzuzeigen, einschließlich der [Auflisten des Aktivitätsprotokolls](./product-listing-details.md#listing-activity-log), [Buy Box Konkurrentenpreise](./product-listing-details.md#buy-box-competitor-pricing), und [Niedrigste Preise für Wettbewerber](./product-listing-details.md#lowest-competitor-pricing). Diese Aktion dient nur der Anzeige. In den Listendetails können keine Änderungen vorgenommen werden. Siehe [Details anzeigen](./product-listing-details.md).

Sie haben einige Optionen zum manuellen [Neue Liste in Amazon veröffentlichen](./publish-listings-manually.md).

>[!NOTE]
>Wenn Listen in Bearbeitung sind, wird die Anzahl der Auflistungen in einer Meldung über den Registerkarten angezeigt.

![Listenbereit](assets/amazon-ready-to-list.png){width="600" zoomable="yes"}

## Standardspalten

| Spalte | Beschreibung |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Amazon Seller SKU] | Die von Amazon einem Produkt zugewiesene SKU (Stock Keeping Unit, Bestandseinheit) zur Identifizierung von Produkt, Optionen, Preis und Hersteller. |
| [!UICONTROL ASIN] | Ein eindeutiger Block von 10 Buchstaben und/oder Zahlen zur Identifizierung von Elementen.<br><br>ASIN steht für die [!DNL Amazon Standard Identification Number]. Ein ASIN ist ein eindeutiger Block von 10 Buchstaben und/oder Zahlen, der Elemente identifiziert. Bei Büchern entspricht das ASIN der ISBN-Nummer, bei allen anderen Produkten wird jedoch beim Hochladen des Artikels in den Katalog ein neues ASIN erstellt. Sie finden einen Artikel-ASIN auf der Produktdetailseite in Amazon sowie weitere Details zum Artikel. |
| [!UICONTROL Product Listing Name] | Der Name des Produkts. |
| [!UICONTROL Condition] | Die [Bedingung](./product-listing-condition.md) des Erzeugnisses. |
| [!UICONTROL Landed Price] | Der Börsennotierungspreis für das Produkt zuzüglich des Versandpreises. |
| [!UICONTROL Amazon Quantity] | Die verfügbare Menge, wenn das Produkt aktiv in Amazon aufgeführt wird. |
| [!UICONTROL Status] | Der von Amazon definierte Status der Auflistung. |
| [!UICONTROL Action] | Liste der verfügbaren Aktionen, die auf eine bestimmte Liste angewendet werden können. Um eine Aktion anzuwenden, klicken Sie auf **[!UICONTROL Select]** im _[!UICONTROL Action]_und wählen Sie eine Option aus:<ul><li>[[!UICONTROL Publish on Amazon]](./publish-listings-manually.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |

### Häufige Ursachen für Listen, die bereit zur Auflistung sind

- **[!UICONTROL Ready to List]** - Das Produkt wird mit einem Amazon-ASIN abgeglichen und für die Auflistung geplant. Wenn [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) in Ihren Listeneinstellungen auf `Do Not Automatically List Eligible Products`, stellt dieser Status die Produkte dar, die zur manuellen Auflistung bereit sind.

- **[!UICONTROL List in Progress]** - Die Produktliste wurde an Amazon übermittelt und wartet auf die Bestätigung der Annahme durch Amazon.
