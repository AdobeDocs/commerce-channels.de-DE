---
title: Listenbereit
description: Der Amazon-Vertriebskanal bietet die Registerkarte "Listenbereit", mit der Sie Commerce-Produkte überprüfen können, die die Voraussetzungen erfüllen, aber nicht automatisch aufgelistet werden.
exl-id: f62017fb-964f-43f0-b76b-8f39f447466a
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# [!UICONTROL Ready to List]

Der Tab _[!UICONTROL Ready to List]_zeigt Ihre [!DNL Commerce] -Katalogprodukte an, die Ihren Listeneinstellungen entsprechen und bereit sind, sie als **neue**-Auflistung in Amazon zu veröffentlichen. Im Gegensatz zu anderen Listenregisterkarten wird diese Registerkarte nicht immer auf der Seite [_[!UICONTROL Product Listings]_](./managing-product-listings.md) angezeigt.

Die Registerkarte _[!UICONTROL Ready to List]_wird nur angezeigt, wenn [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) in Ihren Listeneinstellungen auf `Do Not Automatically List Eligible Products` festgelegt ist. Diese Einstellung teilt dem Amazon-Vertriebskanal mit, dass alle neuen Amazon-Auflistungen manuell veröffentlicht werden müssen.

Wenn [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) auf `Automatically List Eligible Products` gesetzt ist, veröffentlicht der Amazon-Vertriebskanal automatisch neue Einträge für Ihre entsprechenden Katalogprodukte. Da neue Listen automatisch veröffentlicht werden, wird die Registerkarte _[!UICONTROL Ready to List]_nicht angezeigt.

Unter _[!UICONTROL Actions]_:

- **[!UICONTROL Publish Product to Amazon]**: Wählen Sie aus, die Liste erneut in der  [!DNL Amazon Marketplace]zu veröffentlichen. Siehe [Veröffentlichen einer Amazon-Liste](./publish-listings-manually.md)

Unter **[!UICONTROL Select]** in der Spalte _[!UICONTROL Action]_:

- **[!UICONTROL Publish On Amazon]**: Wählen Sie aus, die Liste erneut in der  [!DNL Amazon Marketplace]zu veröffentlichen. Siehe [Veröffentlichen einer Amazon-Liste](./publish-listings-manually.md).

- **[!UICONTROL View Details]**: Wählen Sie aus, ob Sie Details zur Liste anzeigen möchten, darunter das Protokoll zu den  [Listing-Aktivitäten](./product-listing-details.md#listing-activity-log), die  [Buy Box-Preise für Wettbewerber](./product-listing-details.md#buy-box-competitor-pricing) und die Preise für  [Niedrigste Konkurrenz](./product-listing-details.md#lowest-competitor-pricing). Diese Aktion dient nur der Anzeige. In den Listendetails können keine Änderungen vorgenommen werden. Siehe [Details anzeigen](./product-listing-details.md).

Sie haben einige Optionen, um [eine neue Liste in Amazon](./publish-listings-manually.md) manuell zu veröffentlichen.

>[!NOTE]
>Wenn Listen in Bearbeitung sind, wird die Anzahl der Auflistungen in einer Meldung über den Registerkarten angezeigt.

![Listenbereit](assets/amazon-ready-to-list.png)

## Standardspalten

| Spalte | Beschreibung |
|---|---|
| [!UICONTROL Amazon Seller SKU] | Die SKU (Stock Keeping Unit, Bestandseinheit), die von Amazon einem Produkt zugewiesen wurde, um das Produkt, die Optionen, den Preis und den Hersteller zu identifizieren. |
| [!UICONTROL ASIN] | Ein eindeutiger Block von 10 Buchstaben und/oder Zahlen zur Identifizierung von Elementen.<br><br>ASIN steht für die  [!DNL Amazon Standard Identification Number]. Ein ASIN ist ein eindeutiger Block von 10 Buchstaben und/oder Zahlen, der Elemente identifiziert. Bei Büchern entspricht das ASIN der ISBN-Nummer, bei allen anderen Produkten wird jedoch beim Hochladen des Artikels in den Katalog ein neues ASIN erstellt. Sie finden einen Artikel-ASIN auf der Produktdetailseite in Amazon sowie weitere Details zum Artikel. |
| [!UICONTROL Product Listing Name] | Der Name des Produkts. |
| [!UICONTROL Condition] | Die [Bedingung](./product-listing-condition.md) des Produkts. |
| [!UICONTROL Landed Price] | Der Börsennotierungspreis für das Produkt zuzüglich des Versandpreises. |
| [!UICONTROL Amazon Quantity] | Die verfügbare Menge, wenn das Produkt aktiv in Amazon aufgeführt wird. |
| [!UICONTROL Status] | Der von Amazon definierte Status der Auflistung. |
| [!UICONTROL Action] | Liste der verfügbaren Aktionen, die auf eine bestimmte Liste angewendet werden können. Um eine Aktion anzuwenden, klicken Sie in der Spalte _[!UICONTROL Action]_auf **[!UICONTROL Select]**und wählen Sie eine Option:<ul><li>[[!UICONTROL Publish on Amazon]](./publish-listings-manually.md)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |

### Häufige Ursachen für Listen vom Typ &quot;Bereit zum Auflisten&quot;

- **[!UICONTROL Ready to List]** - Das Produkt wird mit einem Amazon-ASIN abgeglichen und für die Auflistung geplant. Wenn [**[!UICONTROL Automatic List Action]**](./product-listing-actions.md) in Ihren Listeneinstellungen auf `Do Not Automatically List Eligible Products` festgelegt ist, stellt dieser Status die Produkte dar, die zur manuellen Auflistung bereit sind.

- **[!UICONTROL List in Progress]** - Die Produktliste wurde an Amazon übermittelt und wartet auf die Bestätigung der Annahme durch Amazon.
