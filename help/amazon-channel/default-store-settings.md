---
title: Standardspeichereinstellungen
description: Ändern Sie die standardmäßigen Commerce-Einstellungen, um den Amazon-Sales Channel für Ihren Store anzupassen.
exl-id: 368e5e8e-2bf9-4f9c-86c6-6d375f8a8720
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Standardmäßige Store-Einstellungen

Nachdem Ihr Store verbunden ist und Sie Ihre erste Listening-Regel eingerichtet haben, beginnt die Synchronisierung der Daten zwischen Amazon und [!DNL Commerce]. Es gibt verschiedene Arten von Store-Einstellungen, mit denen Sie Ihren Store an Ihre Anforderungen anpassen können. Die Speichereinstellungen sind im Store [dashboard](./amazon-store-dashboard.md) verfügbar.

Zu den Store-Einstellungen gehören:

- [**[!UICONTROL Listing settings]**](./listing-settings.md) - Steuern Sie, wie Ihr Produktkatalog mit der interagiert  [!DNL Amazon Marketplace].

- [**[!UICONTROL Order settings]**](./order-settings.md) - Steuern der Verwaltung von Amazon-Bestellungen.

- [**[!UICONTROL Listing rules]**](./listing-rules.md) - Definieren Sie, welche Katalogprodukte für die Auflistung in Amazon infrage kommen.

- [**[!UICONTROL Pricing rules]**](./pricing-products.md) - Definieren Sie, wie der Listenpreis von Amazon für qualifizierte Auflistungen geändert wird.

- **[!UICONTROL Store reports]** -  [Wettbewerbsbezogene ](./competitive-price-analysis.md) Preisanalysen und  [Verbesserungen](./listing-improvements.md).

- **[!UICONTROL Logs]** -  [Auflisten von ](./listing-changes-log.md) Änderungen und  [Kommunikationsfehlern](./communication-errors-log.md).

- [**[!UICONTROL Store integration settings]**](./store-integration-settings.md) - Überprüfen Sie die Einstellungen für den E-Mail- und Amazon-Verkaufskanalspeichernamen in der  [!DNL Commerce] Admin-Konsole.

## Wichtige Standardeinstellungen

| Einstellung | Standard | Beschreibung | Standort |
|--- |--- |--- |--- |
| [!UICONTROL Import Amazon Orders] | `Enabled` | Erstellt entsprechende [!DNL Commerce]-Bestellungen, wenn neue Bestellungen von Amazon empfangen werden, sodass Bestellungen im Workflow [[!DNL Commerce] Bestellungen](https://docs.magento.com/user-guide/sales/orders.html){target=&quot;_blank&quot;} verwaltet werden können. Wenn `Disabled`, bestellt Amazon Informationen zur Importbestellung zur Überprüfung, aber Bestellungen müssen in Ihrem [!DNL Amazon Seller Central]-Konto verwaltet werden. | [Bestelleinstellungen](./order-settings.md) |
| [!UICONTROL Customer Creation] | `No Customer Creation (guest)` | Kundendaten aus Amazon-Bestellungen werden nicht in Ihre [!DNL Commerce]-Datenbank importiert. Importierte Amazon-Bestellungen werden als Gastkasse verarbeitet. Wenn Sie Ihre [!DNL Commerce] Kundendatenbank erstellen möchten, sollten Sie diese Einstellung in `Build New Customer Account` ändern. | [Bestelleinstellungen](./order-settings.md) |
| [!UICONTROL Automatic List Action] | `Automatically List Eligible Products` | [!DNL Commerce] -Katalogprodukte (die die Voraussetzungen für Amazon erfüllen), um sie automatisch in Amazon zu veröffentlichen und Amazon-Listen zu erstellen. Wenn Sie Ihre Produkte manuell überprüfen und veröffentlichen möchten, sollten Sie diese Einstellung auf `Do Not Automatically List Eligible Products` ändern. Produkte, die auf eine manuelle Veröffentlichung warten, werden auf der Registerkarte [_Bereit zur Liste_](./ready-to-list.md) angezeigt. | [Produktlistenaktionen](./product-listing-actions.md) |
| [!UICONTROL Magento Price Source] | `Price` | Definiert das Preisquellenattribut, das als Grundlage für Ihre Amazon-Auflistungen verwendet wird. Wenn Sie das Attribut [!DNL Commerce] `Price` nicht als Basispreis verwenden möchten, auf dem Ihre Preisregeln basieren, sollten Sie diese Einstellung in ein anderes Attribut ändern. | [Listenpreis](./listing-price.md) |
| [!UICONTROL Product Fulfilled By] | `Fulfilled by Merchant` | Der Händler erfüllt alle Bestellungen. Wenn Sie die Funktion Erfüllung durch Amazon verwenden oder eine Mischung aus Erfüllungsmethoden verwenden, sollten Sie diese Einstellung ändern. | [Erfüllt von](./listing-price.md) |
| [!UICONTROL Listing Product Condition] | `New` | Wenn alle Ihre Produkte dieselbe Bedingung aufweisen, können Sie eine der Amazon-Bedingungsoptionen auswählen, um alle Ihre Produkte darzustellen. Wenn Ihr Katalog Produkte mit unterschiedlichen Bedingungen enthält (z. B. Neu, Verwendet und renoviert), müssen Sie diese Einstellung auf `Assign Condition Using Product Attribute` ändern und Ihre [!DNL Commerce]-Bedingungsattribute Ihren Amazon-Listenbedingungen zuordnen. | [Produktlistenbedingung](./product-listing-condition.md) |
| [!UICONTROL Listing Rules] | Keine | Definieren Sie die Regeln, mit denen bestimmt wird, welche Produkte der Amazon-Vertriebskanal in Amazon veröffentlicht. Diese Regeln bieten viele Optionen zum Erstellen einfacher bis komplexer Regeln zum Ein- oder Ausschließen von Produkten als Listen. | [Listening-Regeln](./listing-rules.md) |
| Preisregeln | Keine | Definieren Sie Ihr Amazon-Listing-Preisattribut, das sich von dem definierten _[!UICONTROL Magento Price Source]_in Ihrem [Listing Price](./listing-price.md) unterscheidet. Um Ihren Listenpreis (oben oder unten) an Ihre_[!UICONTROL Magento Price Source]_-Einstellung anzupassen, erstellen Sie Regeln. | [Preisregeln](./pricing-products.md) |

Weitere Informationen finden Sie unter [Speichereinstellungen](./ob-store-review.md).
