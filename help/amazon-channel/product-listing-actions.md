---
title: Produktlistenaktionen
description: Verwenden Sie die Einstellungen für Produktlistungsaktionen , um festzulegen, wie Ihr Commerce-Katalog mit Amazon interagiert.
redirect_from: /sales-channels/asc/ob-product-listing-actions.html
exl-id: c7d3f22c-05c6-4826-99eb-543bac462cf8
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 0%

---

# Aktionen auf der Produktliste

Die Aktionseinstellungen für die Produktliste sind Teil Ihrer Einstellungen für die Store-Auflistung. Auf die Listening-Einstellungen kann über die [Store-Dashboard](./amazon-store-dashboard.md).

Diese Einstellungen definieren, wie Ihr Katalog mit Amazon interagiert. Diese Einstellungen:

- Geben Sie an, ob Ihre [!DNL Commerce] Katalogprodukte, die die Amazon-Voraussetzungen erfüllen, werden automatisch an Ihre [!DNL Amazon Seller Central] -Konto zu erstellen.

- Legen Sie die standardmäßige Bearbeitungszeit für eine Bestellung fest. Dieser Wert definiert die Anzahl der Tage, die Sie benötigen, um eine Bestellung zu verarbeiten und zu versenden. Wenn beispielsweise jemand 2 Tage Versand auswählt, beginnt diese Versanddurchlaufzeit erst nach Abschluss der Verarbeitung und die Pakete werden an einen Beförderer übergeben. Die Versandzeit beträgt insgesamt (Bearbeitungszeit + Versandzeit + Feiertage).

## Einstellungen konfigurieren

1. Klicken **[!UICONTROL Listing Settings]** im Dashboard speichern.

1. Erweitern Sie die _[!UICONTROL Product Listing Actions]_Abschnitt.

1. Für **[!UICONTROL Automatic List Action]** (erforderlich), wählen Sie eine Option aus:

   - `Automatically List Eligible Products` - (Standard) Wählen Sie aus, wann Sie Ihre [!DNL Commerce] -Katalogprodukte (die die Voraussetzungen für Amazon erfüllen), um sie automatisch in Amazon zu veröffentlichen und Amazon-Listen zu erstellen.

   - `Do Not Automatically List Eligible Products` - Wählen Sie aus, wann Sie Ihre Berechtigung manuell auswählen möchten. [!DNL Commerce] -Produkte und erstellen Sie Amazon-Listen. Wenn ausgewählt, werden Produkte aus dem Katalog angezeigt, die Ihre Listenkriterien erfüllen und alle erforderlichen Informationen enthalten. [_[!UICONTROL Ready to List]_](./ready-to-list.md) Registerkarte für manuelle Veröffentlichung in Amazon.

1. Für **[!UICONTROL Default Handling Time]** (erforderlich) die Anzahl der Tage angeben, die für die Vorlaufzeit vor dem Versand benötigt werden.

   Der Standardwert ist `2` Tage.

   >[!NOTE]
   >
   >Dieser standardmäßige Bereitstellungszeitwert gilt nur für Amazon-Auflistungen, die über den Amazon-Vertriebskanal erstellt werden. Alle Amazon-Listen, die in Ihrer [!DNL Amazon Seller Central] -Konto verwenden die in Amazon festgelegte standardmäßige Bearbeitungszeit.

1. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Save listing settings]**.

![Aktionen auf der Produktliste](assets/amazon-product-listing-actions.png)

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Automatic List Action] | Optionen:<ul><li>**[!UICONTROL Automatically List Eligible Products]** - (Empfohlen) Wählen Sie aus, wann Sie Ihre [!DNL Commerce] -Katalogprodukte (die die Voraussetzungen für Amazon erfüllen), um sie automatisch in Amazon zu veröffentlichen und Amazon-Listen zu erstellen. Wenn ausgewählt, wird die [_[!UICONTROL Ready to List]_](./ready-to-list.md) nicht angezeigt. </li><li>**[!UICONTROL Do Not Automatically List Eligible Products]** - Wählen Sie aus, wann Sie die Berechtigung manuell auswählen möchten. [!DNL Commerce] -Produkte und erstellen Sie Amazon-Listen. Wenn ausgewählt, werden Produkte aus dem Katalog angezeigt, die Ihre Listenkriterien erfüllen und alle erforderlichen Informationen enthalten. [_[!UICONTROL Ready to List]_](./ready-to-list.md) Registerkarte für manuelles Veröffentlichen.</li></ul> |
| [!UICONTROL Default Handling Time] | Der numerische Wert, der die Anzahl der Tage angibt, die Sie für die Verarbeitung und den Versand Ihrer Bestellungen benötigen. Der Standardwert ist `2`. Dieser Wert wird für Amazon-Listen verwendet, die in [!DNL Commerce] und in Amazon veröffentlicht. Die standardmäßige Bearbeitungszeit für Amazon-Listen vor der Integration mit [!DNL Commerce] von dieser Einstellung nicht betroffen sind.<br><br>Der im Amazon-Vertriebskanal definierte Wert ersetzt nicht die standardmäßige Bearbeitungszeit, die in einer vorhandenen Amazon-Liste definiert ist. Wenn eine **[!UICONTROL Handling Time Override]** aktiviert und dann entfernt wird, wird die Verarbeitungszeit für eine Bestellung auf den hier definierten Wert zurückgesetzt.<br><br>Wenn Sie Produkte mit unterschiedlichen Verarbeitungszeiten haben, können Sie eine &quot;Handling Time Override&quot;auf produktspezifischer Ebene erstellen. Sie können die Handhabung von Zeitüberschreitungen im [_[!UICONTROL Overrides]_](./overrides.md) -Tab, der Ihnen Flexibilität bei der Verwaltung der Produkterfüllung gibt. Wenn keine Überschreibungszeit vorhanden ist: [!DNL Commerce] für ein Produkt ist der Standardwert für die Verarbeitungszeit der in der Amazon-Auflistung definierte Wert.<br><br>Die Verarbeitungszeit ist ein regionales Attribut. Wenn der Wert für eine Auflistung geändert wird, wirkt sich die Änderung auf alle Auflistungen aus, die die [!DNL Amazon Seller SKU] in allen Amazon-Stores, die für dieselbe Region vorhanden sind (definiert unter [Store-Integration](./store-integration.md)). Ändern des Werts für eine freigegebene [!DNL Amazon Seller SKU] in Nordamerika sind nicht die gleichen Produkte betroffen, die in einem Geschäft mit einer anderen definierten Region aufgeführt sind. Der Speicher für die Region mit dem ältesten Erstellungsdatum steuert die Priorität für die Standardeinstellungen für die Verarbeitungszeit. |

**Schnellzugriff** - [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
