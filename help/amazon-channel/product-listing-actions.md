---
title: Amazon-Vertriebskanal - Produktlistungsaktionen
description: Verwenden Sie die Einstellungen für Produktlistungsaktionen , um festzulegen, wie Ihr Commerce-Katalog mit Amazon interagiert.
redirect_from: /sales-channels/asc/ob-product-listing-actions.html
feature: Sales Channels, Products, Merchandising, Configuration
exl-id: c7d3f22c-05c6-4826-99eb-543bac462cf8
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Aktionen auf der Produktliste

Die Aktionseinstellungen für die Produktliste sind Teil Ihrer Einstellungen für die Store-Auflistung. Auf die Listening-Einstellungen kann über das [Dashboard speichern](./amazon-store-dashboard.md) zugegriffen werden.

Diese Einstellungen definieren, wie Ihr Katalog mit Amazon interagiert. Diese Einstellungen:

- Geben Sie an, ob Ihre [!DNL Commerce] -Katalogprodukte, die die Amazon-Eignungsanforderungen erfüllen, automatisch an Ihr [!DNL Amazon Seller Central] -Konto gesendet werden, um Auflistungen zu erstellen.

- Legen Sie die standardmäßige Bearbeitungszeit für eine Bestellung fest. Dieser Wert definiert die Anzahl der Tage, die Sie benötigen, um eine Bestellung zu verarbeiten und zu versenden. Wenn beispielsweise jemand 2 Tage Versand auswählt, beginnt diese Versanddurchlaufzeit erst nach Abschluss der Verarbeitung und die Pakete werden an einen Beförderer übergeben. Die Versandzeit beträgt insgesamt (Bearbeitungszeit + Versandzeit + Feiertage).

## Einstellungen konfigurieren

1. Klicken Sie im Store-Dashboard auf **[!UICONTROL Listing Settings]** .

1. Erweitern Sie den Abschnitt _[!UICONTROL Product Listing Actions]_.

1. Wählen Sie für &quot;**[!UICONTROL Automatic List Action]**&quot;(erforderlich) eine Option:

   - `Automatically List Eligible Products` - (Standard) Wählen Sie aus, wann Ihre [!DNL Commerce] -Katalogprodukte (die die Voraussetzungen für Amazon erfüllen) automatisch in Amazon veröffentlicht und Amazon-Listen erstellt werden sollen.

   - `Do Not Automatically List Eligible Products` - Wählen Sie aus, wann Sie manuell die entsprechenden [!DNL Commerce] -Katalogprodukte auswählen und Amazon-Listen erstellen möchten. Wenn diese Option ausgewählt ist, werden Katalogprodukte, die Ihre Listenkriterien erfüllen und alle erforderlichen Informationen enthalten, auf der Registerkarte &quot;[_[!UICONTROL Ready to List]_](./ready-to-list.md)&quot;angezeigt, um sie manuell in Amazon zu veröffentlichen.

1. Für **[!UICONTROL Default Handling Time]** (erforderlich) geben Sie die Anzahl der Tage an, die für die Vorlaufzeit vor dem Versand benötigt werden.

   Der Standardwert ist `2` Tage.

   >[!NOTE]
   >
   >Dieser standardmäßige Bereitstellungszeitwert gilt nur für Amazon-Auflistungen, die über den Amazon-Vertriebskanal erstellt werden. Alle Amazon-Listen, die in Ihrem [!DNL Amazon Seller Central] -Konto erstellt wurden, verwenden die in Amazon festgelegte standardmäßige Bearbeitungszeit.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save listing settings]**.

![Aktionen zur Produktauflistung](assets/amazon-product-listing-actions.png){width="600" zoomable="yes"}

| Feld | Beschreibung |
|------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Automatic List Action] | Optionen:<ul><li>**[!UICONTROL Automatically List Eligible Products]** - (Empfohlen) Wählen Sie aus, wann Ihre [!DNL Commerce] -Katalogprodukte (die die Voraussetzungen für Amazon erfüllen) automatisch in Amazon veröffentlicht und Amazon-Listen erstellt werden sollen. Wenn diese Option aktiviert ist, wird die Registerkarte [_[!UICONTROL Ready to List]_](./ready-to-list.md) nicht angezeigt. </li><li>**[!UICONTROL Do Not Automatically List Eligible Products]** - Wählen Sie aus, wann Sie die entsprechenden [!DNL Commerce] -Katalogprodukte manuell auswählen und Amazon-Listen erstellen möchten. Wenn diese Option ausgewählt ist, werden Katalogprodukte, die Ihren Listenkriterien entsprechen und alle erforderlichen Informationen enthalten, auf der Registerkarte &quot;[_[!UICONTROL Ready to List]_](./ready-to-list.md)&quot;für die manuelle Veröffentlichung angezeigt.</li></ul> |
| [!UICONTROL Default Handling Time] | Der numerische Wert, der die Anzahl der Tage angibt, die Sie für die Verarbeitung und den Versand Ihrer Bestellungen benötigen. Der Standardwert ist `2`. Dieser Wert wird für Amazon-Auflistungen verwendet, die in [!DNL Commerce] erstellt und in Amazon veröffentlicht wurden. Die standardmäßige Bearbeitungszeit für Amazon-Listen vor der Integration mit [!DNL Commerce] wird von dieser Einstellung nicht beeinflusst.<br><br>Der im Amazon-Verkaufskanal definierte Wert ersetzt nicht die standardmäßige Bearbeitungszeit, die in einer vorhandenen Amazon-Auflistung definiert ist. Wenn **[!UICONTROL Handling Time Override]** aktiviert und dann entfernt wird, wird die Verarbeitungszeit für eine Bestellung auf den hier definierten Wert zurückgesetzt.<br><br>Wenn Sie Produkte mit unterschiedlichen Verarbeitungszeiten haben, können Sie eine &quot;Handling Time Override&quot;auf produktspezifischer Ebene erstellen. Sie können die Handhabung von Zeitüberschreitungen auf der Registerkarte [_[!UICONTROL Overrides]_](./overrides.md) verwalten, um Ihnen die Flexibilität zu geben, Ihre Produkterfüllung zu verwalten. Wenn für ein Produkt keine Verarbeitungszeit-Überschreibung in [!DNL Commerce] vorhanden ist, ist der Standardwert für die Bearbeitungszeit der in der Amazon-Auflistung definierte Wert.<br><br>Die Verarbeitungszeit ist ein regionales Attribut. Wenn der Wert für eine Auflistung geändert wird, wirkt sich die Änderung auf alle Auflistungen aus, die den Wert &quot;[!DNL Amazon Seller SKU]&quot;in allen Amazon Stores teilen, die für dieselbe Region vorhanden sind (definiert in [Speicherintegration](./store-integration.md)). Eine Änderung des Werts für eine freigegebene [!DNL Amazon Seller SKU] in Nordamerika wirkt sich jedoch nicht auf dieselben Produkte aus, die in einem Store mit einer anderen definierten Region aufgeführt sind. Der Speicher für die Region mit dem ältesten Erstellungsdatum steuert die Priorität für die Standardeinstellungen für die Verarbeitungszeit. |

**Schnellzugriff** - [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
