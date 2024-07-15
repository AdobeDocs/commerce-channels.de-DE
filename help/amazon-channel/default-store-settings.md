---
title: Standardmäßige Store-Einstellungen für Amazon-Listen
description: Ändern Sie die standardmäßigen Commerce-Einstellungen, um die Amazon-Sales Channel für Ihren Store anzupassen.
role: Admin
feature: Sales Channels, Integration, Configuration
exl-id: 368e5e8e-2bf9-4f9c-86c6-6d375f8a8720
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Standardmäßige Store-Einstellungen für Amazon-Listen

Nachdem Ihr Store verbunden ist und Sie Ihre erste Listening-Regel eingerichtet haben, beginnt die Synchronisierung der Daten zwischen Amazon und [!DNL Commerce]. Es gibt verschiedene Arten von Store-Einstellungen, mit denen Sie Ihren Store an Ihre Anforderungen anpassen können. Auf die Speichereinstellungen kann über das Store-Dashboard [Dashboard](./amazon-store-dashboard.md) zugegriffen werden.

Zu den Store-Einstellungen gehören:

- [**[!UICONTROL Listing settings]**](./listing-settings.md) - Steuern Sie, wie Ihr Produktkatalog mit dem [!DNL Amazon Marketplace] interagiert.

- [**[!UICONTROL Order settings]**](./order-settings.md) - Steuern Sie, wie Amazon-Bestellungen verwaltet werden.

- [**[!UICONTROL Listing rules]**](./listing-rules.md) - Definieren Sie, welche Katalogprodukte für die Auflistung in Amazon geeignet sind.

- [**[!UICONTROL Pricing rules]**](./pricing-products.md) - Definieren Sie, wie der Amazon-Listenpreis für qualifizierte Auflistungen geändert wird.

- **[!UICONTROL Store reports]** - [Wettbewerbsbezogene Preisanalyse](./competitive-price-analysis.md) und [Auflistungsverbesserungen](./listing-improvements.md).

- **[!UICONTROL Logs]** - [Listing changes](./listing-changes-log.md) und [kommunikationsfehler](./communication-errors-log.md).

- [**[!UICONTROL Store integration settings]**](./store-integration-settings.md) - Überprüfen Sie die Einstellungen für den E-Mail- und Amazon-Verkaufskanalspeichernamen in der [!DNL Commerce] Admin.

## Wichtige Standardeinstellungen

| Einstellung | Standard | Beschreibung | Standort |
|----------------------------------------|----------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------|
| [!UICONTROL Import Amazon Orders] | `Enabled` | Erstellt entsprechende [!DNL Commerce] Bestellungen, wenn neue Bestellungen von Amazon empfangen werden, sodass Bestellungen im Workflow [[!DNL Commerce] Bestellungen](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html) verwaltet werden können. Wenn `Disabled`, bestellt Amazon Informationen zur Importbestellung zur Überprüfung, aber die Bestellungen müssen in Ihrem [!DNL Amazon Seller Central] -Konto verwaltet werden. | [Bestelleinstellungen](./order-settings.md) |
| [!UICONTROL Customer Creation] | `No Customer Creation (guest)` | Kundendaten aus Amazon-Bestellungen werden nicht in Ihre [!DNL Commerce] -Datenbank importiert. Importierte Amazon-Bestellungen werden als Gastkasse verarbeitet. Wenn Sie Ihre [!DNL Commerce] Kundendatenbank erstellen möchten, sollten Sie diese Einstellung auf `Build New Customer Account` ändern. | [Bestelleinstellungen](./order-settings.md) |
| [!UICONTROL Automatic List Action] | `Automatically List Eligible Products` | [!DNL Commerce] Katalogprodukte (die die Voraussetzungen für Amazon erfüllen) zur automatischen Veröffentlichung in Amazon und zur Erstellung von Amazon-Listen. Wenn Sie Ihre Produkte manuell überprüfen und veröffentlichen möchten, sollten Sie diese Einstellung auf `Do Not Automatically List Eligible Products` ändern. Produkte, die auf eine manuelle Veröffentlichung warten, werden auf der Registerkarte [_Bereit zur Liste_](./ready-to-list.md) angezeigt. | [Aktionen für Produktlisten](./product-listing-actions.md) |
| [!UICONTROL Magento Price Source] | `Price` | Definiert das Preisquellenattribut, das als Grundlage für Ihre Amazon-Listen verwendet wird. Wenn Sie das Attribut [!DNL Commerce] `Price` nicht als Basispreis verwenden möchten, auf dem Ihre Preisregeln basieren, sollten Sie diese Einstellung in ein anderes Attribut ändern. | [Listing Price](./listing-price.md) |
| [!UICONTROL Product Fulfilled By] | `Fulfilled by Merchant` | Der Händler erfüllt alle Bestellungen. Wenn Sie die Funktion Erfüllung durch Amazon verwenden oder eine Mischung aus Erfüllungsmethoden verwenden, sollten Sie diese Einstellung ändern. | [Erfüllt von ](./listing-price.md) |
| [!UICONTROL Listing Product Condition] | `New` | Wenn alle Ihre Produkte dieselbe Bedingung aufweisen, können Sie eine der Amazon-Bedingungsoptionen auswählen, um alle Ihre Produkte darzustellen. Wenn Ihr Katalog Produkte mit unterschiedlichen Bedingungen enthält (z. B. Neu, Verwendet und renoviert), müssen Sie diese Einstellung auf &quot;`Assign Condition Using Product Attribute`&quot;setzen und Ihre [!DNL Commerce] -Bedingungsattribute Ihren Amazon-Listenbedingungen zuordnen. | [Bedingung für die Produktauflistung](./product-listing-condition.md) |
| [!UICONTROL Listing Rules] | Keine | Definieren Sie die Regeln, mit denen bestimmt wird, welche Produkte der Amazon-Vertriebskanal in Amazon veröffentlicht. Diese Regeln bieten viele Optionen zum Erstellen einfacher bis komplexer Regeln zum Ein- oder Ausschließen von Produkten als Listen. | [Listening-Regeln](./listing-rules.md) |
| Preisregeln | Keine | Definieren Sie das Preisattribut für die Amazon-Auflistung, das sich von dem definierten _[!UICONTROL Magento Price Source]_in Ihrem [Listing Price](./listing-price.md) unterscheidet. Um Ihren Listenpreis (oben oder unten) an Ihre_[!UICONTROL Magento Price Source]_ -Einstellung anzupassen, erstellen Sie Regeln. | [Preisregeln](./pricing-products.md) |

Weitere Informationen finden Sie unter [Speichereinstellungen](./ob-store-review.md).
