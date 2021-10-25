---
title: Standard-Store-Einstellungen
description: Ändern Sie die standardmäßigen Commerce-Einstellungen, um den Amazon-Sales Channel für Ihren Store anzupassen.
exl-id: 368e5e8e-2bf9-4f9c-86c6-6d375f8a8720
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Standardspeichereinstellungen

Nachdem Ihr Store verbunden ist und Sie Ihre erste Listingregel eingerichtet haben, die Datensynchronisierung zwischen Amazon und [!DNL Commerce] Beginn. Es gibt verschiedene Arten von Store-Einstellungen, mit denen Sie Ihren Store für Ihre Anforderungen anpassen können. Auf Speichereinstellungen wird im Store zugegriffen. [Dashboard](./amazon-store-dashboard.md).

Zu den Store-Einstellungen gehören:

- [**[!UICONTROL Listing settings]**](./listing-settings.md) - Steuerung der Interaktion Ihres Produktkatalogs mit [!DNL Amazon Marketplace].

- [**[!UICONTROL Order settings]**](./order-settings.md) - Steuerung der Verwaltung von Amazon-Aufträgen.

- [**[!UICONTROL Listing rules]**](./listing-rules.md) - Definieren Sie, welche Katalogprodukte für eine Liste auf Amazon infrage kommen.

- [**[!UICONTROL Pricing rules]**](./pricing-products.md) - Legen Sie fest, wie der Preis der Amazon-Liste für qualifizierte Auflistungen geändert wird.

- **[!UICONTROL Store reports]** - [Analyse der Wettbewerbspreise](./competitive-price-analysis.md) und [Verbesserungen in der Auflistung](./listing-improvements.md).

- **[!UICONTROL Logs]** - [Listungsänderungen](./listing-changes-log.md) und [Kommunikationsfehler](./communication-errors-log.md).

- [**[!UICONTROL Store integration settings]**](./store-integration-settings.md) - Überprüfen Sie die Namenseinstellungen für den Amazon Sales Kanal unter [!DNL Commerce] Admin.

## Wichtige Standardeinstellungen

| Einstellung | Standard | Beschreibung | Standort |
|--- |--- |--- |--- |
| [!UICONTROL Import Amazon Orders] | `Enabled` | Erstellt entsprechende [!DNL Commerce] Bestellungen, wenn neue Bestellungen von Amazon eingegangen sind, sodass Bestellungen im [[!DNL Commerce] Bestellungen](https://docs.magento.com/user-guide/sales/orders.html)Workflow für {Zielgruppe=&quot;_blank&quot;}. Wann `Disabled`, bestellt Amazon Auftragseingangsdaten zur Überprüfung, muss jedoch in Ihrer [!DNL Amazon Seller Central] Konto. | [Auftragseinstellungen](./order-settings.md) |
| [!UICONTROL Customer Creation] | `No Customer Creation (guest)` | Kundendaten aus Amazon-Bestellungen werden nicht in Ihre [!DNL Commerce] Datenbank. Importierte Amazon-Bestellungen werden als Gast-Checkout verarbeitet. Wenn Sie Ihren [!DNL Commerce] Kundendatenbank, sollten Sie diese Einstellung ändern in `Build New Customer Account`. | [Auftragseinstellungen](./order-settings.md) |
| [!UICONTROL Automatic List Action] | `Automatically List Eligible Products` | [!DNL Commerce] Katalogprodukte (die die Anspruchsvoraussetzungen von Amazon erfüllen) zur automatischen Veröffentlichung auf Amazon und Erstellung von Amazon-Listen. Wenn Sie Ihre Produkte manuell überprüfen und veröffentlichen möchten, ändern Sie diese Einstellung in `Do Not Automatically List Eligible Products`. Produkte, die auf die manuelle Veröffentlichung warten, werden auf [_Bereit für Liste_](./ready-to-list.md) Tabulator. | [Produktlistungsaktionen](./product-listing-actions.md) |
| [!UICONTROL Magento Price Source] | `Price` | Definiert das Preisquellattribut, das als Grundlage für Ihre Amazon-Auflistungen verwendet wird. Wenn Sie die [!DNL Commerce] `Price` als Basispreis, auf dem Ihre Preisregeln basieren, sollten Sie diese Einstellung in ein anderes Attribut ändern. | [Listingpreis](./listing-price.md) |
| [!UICONTROL Product Fulfilled By] | `Fulfilled by Merchant` | Der Händler erfüllt alle Bestellungen. Wenn Sie Fulfillment von Amazon verwenden oder eine Kombination aus Fulfillment-Methoden verwenden, sollten Sie diese Einstellung ändern. | [Erfüllt von](./listing-price.md) |
| [!UICONTROL Listing Product Condition] | `New` | Wenn alle Ihre Produkte gleich sind, können Sie eine der Amazon-Bedingungsoptionen auswählen, um alle Ihre Produkte darzustellen. Wenn Ihr Katalog Produkte unter verschiedenen Bedingungen (z. B. Neu, Verwendet und Renoviert) enthält, müssen Sie diese Einstellung ändern auf `Assign Condition Using Product Attribute` und zuordnen [!DNL Commerce] Bedingungsattribute zu Ihren Amazon-Listungsbedingungen. | [Produktauflistungsbedingung](./product-listing-condition.md) |
| [!UICONTROL Listing Rules] | keine | Legen Sie die Regeln fest, anhand derer bestimmt wird, welche Produkte Amazon Sales Kanal in Amazon veröffentlicht. Diese Regeln bieten viele Möglichkeiten, einfache bis komplexe Regeln zu erstellen, um Produkte als Auflistung einzubeziehen oder auszuschließen. | [Listungsregeln](./listing-rules.md) |
| Preisregeln | keine | Definieren Sie das Preisattribut der Amazon-Auflistung, das sich von dem definierten _[!UICONTROL Magento Price Source]_in [Listingpreis](./listing-price.md). So passen Sie Ihren Listingpreis (oben oder unten) an Ihren_[!UICONTROL Magento Price Source]_ festlegen, Regeln erstellen. | [Preisregeln](./pricing-products.md) |

Weitere Informationen finden Sie unter [Speichereinstellungen](./ob-store-review.md).
