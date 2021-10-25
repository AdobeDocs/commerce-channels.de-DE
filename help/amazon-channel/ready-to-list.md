---
title: Bereit für Liste
description: Der Amazon Sales Kanal bietet die Registerkarte "Bereit für Liste", mit der Sie Commerce-Produkte überprüfen können, die die Voraussetzungen erfüllen, aber nicht automatisch aufgelistet werden.
exl-id: f62017fb-964f-43f0-b76b-8f39f447466a
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# [!UICONTROL Ready to List]

Die _[!UICONTROL Ready to List]_auf der Registerkarte angezeigt wird [!DNL Commerce] Katalogprodukte, die Ihren Listeneinstellungen entsprechen und auf Amazon als **neu**Auflistung. Im Gegensatz zu anderen Listenregisterkarten erscheint diese Registerkarte nicht immer auf der [_[!UICONTROL Product Listings]_](./managing-product-listings.md) Seite.

Die _[!UICONTROL Ready to List]_nur dann angezeigt wird, wenn [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) in Ihren Listeneinstellungen auf `Do Not Automatically List Eligible Products`. Diese Einstellung teilt dem Amazon Sales Kanal mit, dass alle neuen Amazon-Auflistungen manuell veröffentlicht werden müssen.

Wann [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) ist eingestellt auf `Automatically List Eligible Products`, veröffentlicht Amazon Sales Kanal automatisch neue Einträge für Ihre Katalogprodukte. Da neue Einträge automatisch veröffentlicht werden, _[!UICONTROL Ready to List]_nicht angezeigt wird.

Unter _[!UICONTROL Actions]_:

- **[!UICONTROL Publish Product to Amazon]**: Wählen Sie, um die Liste erneut im [!DNL Amazon Marketplace]. Siehe [Amazon-Liste veröffentlichen](./publish-listings-manually.md)

Unter **[!UICONTROL Select]** in _[!UICONTROL Action]_Spalte:

- **[!UICONTROL Publish On Amazon]**: Wählen Sie, um die Liste erneut im [!DNL Amazon Marketplace]. Siehe [Amazon-Liste veröffentlichen](./publish-listings-manually.md).

- **[!UICONTROL View Details]**: Wählen Sie eine Ansicht aus, in der Details wie [Listing-Aktivität-Protokoll](./product-listing-details.md#listing-activity-log), [Buy Box Konkurrent-Preise](./product-listing-details.md#buy-box-competitor-pricing)und [Niedrigste Konkurrent-Preise](./product-listing-details.md#lowest-competitor-pricing). Diese Aktion dient nur zum Anzeigen. In den Details der Auflistung können keine Änderungen vorgenommen werden. Siehe [Ansicht - Details](./product-listing-details.md).

Sie haben einige Optionen zum manuellen [eine neue Liste auf Amazon veröffentlichen](./publish-listings-manually.md).

>[!NOTE]
>Wenn Sie Listen bearbeiten, wird die Anzahl der Einträge in einer Meldung über den Registerkarten angezeigt.

![Bereit für Liste](assets/amazon-ready-to-list.png)

## Standardspalten

| Spalte | Beschreibung |
|---|---|
| [!UICONTROL Amazon Seller SKU] | Die von Amazon einem Produkt zugewiesene SKU (Stock Keeping Unit) zur Identifizierung des Produkts, der Optionen, des Preises und des Herstellers. |
| [!UICONTROL ASIN] | Ein eindeutiger Block mit 10 Buchstaben und/oder Zahlen, die Elemente identifizieren.<br><br>ASIN steht für [!DNL Amazon Standard Identification Number]. Ein ASIN ist ein eindeutiger Block mit 10 Buchstaben und/oder Ziffern, der Elemente identifiziert. Für Bücher ist die ASIN die gleiche ISBN-Nummer, aber für alle anderen Produkte wird ein neues ASIN erstellt, wenn das Element in ihren Katalog hochgeladen wird. Auf der Produktdetailseite auf Amazon finden Sie ASIN und weitere Details zum Artikel. |
| [!UICONTROL Product Listing Name] | Der Name des Produkts. |
| [!UICONTROL Condition] | Die [Bedingung](./product-listing-condition.md) des Erzeugnisses. |
| [!UICONTROL Landed Price] | Der Listenpreis des Produkts zuzüglich des Versandpreises. |
| [!UICONTROL Amazon Quantity] | Die Menge, die verfügbar ist, wenn das Produkt aktiv auf Amazon aufgeführt wird. |
| [!UICONTROL Status] | Der von Amazon definierte Status der Auflistung. |
| [!UICONTROL Action] | Liste der verfügbaren Aktionen, die auf eine bestimmte Auflistung angewendet werden können. Klicken Sie zum Anwenden einer Aktion auf **[!UICONTROL Select]** in _[!UICONTROL Action]_-Spalte und wählen Sie eine Option aus:<ul><li>[[!UICONTROL Publish on Amazon]](./publish-listings-manually.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |

### Häufige Ursachen für Auflistungen zur Liste

- **[!UICONTROL Ready to List]** - Das Produkt wurde einem Amazon ASIN zugeordnet und ist für die Auflistung geplant. Falls [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) in Ihren Listeneinstellungen auf `Do Not Automatically List Eligible Products`, stellt dieser Status die Produkte dar, die zur manuellen Auflistung bereit sind.

- **[!UICONTROL List in Progress]** - Die Produktliste wurde bei Amazon eingereicht und wartet auf die Bestätigung der Annahme durch Amazon.
