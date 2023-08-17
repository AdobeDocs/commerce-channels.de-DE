---
title: Standardmäßige Store-Einstellungen für Amazon-Listen
description: Ändern Sie die standardmäßigen Commerce-Einstellungen, um die Amazon-Sales Channel für Ihren Store anzupassen.
role: Admin
feature: Sales Channels, Integration, Configuration
exl-id: 368e5e8e-2bf9-4f9c-86c6-6d375f8a8720
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# Standardmäßige Store-Einstellungen für Amazon-Listen

Nachdem Ihr Store verbunden ist und Sie Ihre erste Listening-Regel eingerichtet haben, wird die Datensynchronisation zwischen Amazon und [!DNL Commerce] beginnt. Es gibt verschiedene Arten von Store-Einstellungen, mit denen Sie Ihren Store an Ihre Anforderungen anpassen können. Store-Einstellungen werden im Store aufgerufen [Dashboard](./amazon-store-dashboard.md).

Zu den Store-Einstellungen gehören:

- [**[!UICONTROL Listing settings]**](./listing-settings.md) - Steuern Sie, wie Ihr Produktkatalog mit dem [!DNL Amazon Marketplace].

- [**[!UICONTROL Order settings]**](./order-settings.md) - Steuern der Verwaltung von Amazon-Bestellungen.

- [**[!UICONTROL Listing rules]**](./listing-rules.md) - Definieren Sie, welche Katalogprodukte zur Auflistung in Amazon zugelassen werden.

- [**[!UICONTROL Pricing rules]**](./pricing-products.md) - Definieren Sie, wie der Listenpreis von Amazon für qualifizierte Auflistungen geändert wird.

- **[!UICONTROL Store reports]** - [Wettbewerbsanalyse der Preise](./competitive-price-analysis.md) und [Auflistungsverbesserungen](./listing-improvements.md).

- **[!UICONTROL Logs]** - [Listenänderungen](./listing-changes-log.md) und [Kommunikationsfehler](./communication-errors-log.md).

- [**[!UICONTROL Store integration settings]**](./store-integration-settings.md) - Überprüfen Sie die Einstellungen für den E-Mail- und Amazon-Verkaufskanalspeichernamen in [!DNL Commerce] Admin.

## Wichtige Standardeinstellungen

| Einstellung | Standard | Beschreibung | Standort |
|----------------------------------------|----------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------|
| [!UICONTROL Import Amazon Orders] | `Enabled` | Erstellt entsprechende [!DNL Commerce] Bestellungen, wenn neue Bestellungen von Amazon empfangen werden, sodass Bestellungen im [[!DNL Commerce] Bestellungen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) Arbeitsablauf. Wann `Disabled`, bestellt Amazon Informationen zur Importbestellung zur Überprüfung, aber die Bestellungen müssen in Ihrer [!DNL Amazon Seller Central] -Konto. | [Bestelleinstellungen](./order-settings.md) |
| [!UICONTROL Customer Creation] | `No Customer Creation (guest)` | Kundendaten aus Amazon-Bestellungen werden nicht in Ihre [!DNL Commerce] Datenbank. Importierte Amazon-Bestellungen werden als Gastkasse verarbeitet. Wenn Sie Ihre [!DNL Commerce] Kundendatenbank, sollten Sie diese Einstellung ändern in `Build New Customer Account`. | [Bestelleinstellungen](./order-settings.md) |
| [!UICONTROL Automatic List Action] | `Automatically List Eligible Products` | [!DNL Commerce] -Katalogprodukte (die die Voraussetzungen für Amazon erfüllen), um sie automatisch in Amazon zu veröffentlichen und Amazon-Listen zu erstellen. Wenn Sie Ihre Produkte manuell überprüfen und veröffentlichen möchten, sollten Sie diese Einstellung in `Do Not Automatically List Eligible Products`. Produkte, die auf eine manuelle Veröffentlichung warten, werden auf [_Listenbereit_](./ready-to-list.md) Registerkarte. | [Produktlistenaktionen](./product-listing-actions.md) |
| [!UICONTROL Magento Price Source] | `Price` | Definiert das Preisquellenattribut, das als Grundlage für Ihre Amazon-Listen verwendet wird. Wenn Sie die [!DNL Commerce] `Price` als Basispreis festlegen, auf dem Ihre Preisregeln basieren, sollten Sie diese Einstellung in ein anderes Attribut ändern. | [Listingpreis](./listing-price.md) |
| [!UICONTROL Product Fulfilled By] | `Fulfilled by Merchant` | Der Händler erfüllt alle Bestellungen. Wenn Sie die Funktion Erfüllung durch Amazon verwenden oder eine Mischung aus Erfüllungsmethoden verwenden, sollten Sie diese Einstellung ändern. | [Erfüllt von](./listing-price.md) |
| [!UICONTROL Listing Product Condition] | `New` | Wenn alle Ihre Produkte dieselbe Bedingung aufweisen, können Sie eine der Amazon-Bedingungsoptionen auswählen, um alle Ihre Produkte darzustellen. Wenn Ihr Katalog Produkte mit unterschiedlichen Bedingungen enthält (z. B. Neu, Verwendet und Neu), müssen Sie diese Einstellung auf `Assign Condition Using Product Attribute` und ordnen Sie Ihre [!DNL Commerce] Bedingungsattribute zu Ihren Amazon-Auflistungsbedingungen hinzufügen. | [Produktlistenbedingung](./product-listing-condition.md) |
| [!UICONTROL Listing Rules] | Keine | Definieren Sie die Regeln, mit denen bestimmt wird, welche Produkte der Amazon-Vertriebskanal in Amazon veröffentlicht. Diese Regeln bieten viele Optionen zum Erstellen einfacher bis komplexer Regeln zum Ein- oder Ausschließen von Produkten als Listen. | [Listening-Regeln](./listing-rules.md) |
| Preisregeln | Keine | Definieren Sie Ihr Amazon-Listenpreisattribut, das sich von dem definierten unterscheidet _[!UICONTROL Magento Price Source]_in [Listingpreis](./listing-price.md). So passen Sie Ihren Listenpreis (oben oder unten) an Ihre_[!UICONTROL Magento Price Source]_ -Einstellung festlegen, erstellen Sie Regeln. | [Preisregeln](./pricing-products.md) |

Weitere Informationen finden Sie unter [Speichereinstellungen](./ob-store-review.md).
