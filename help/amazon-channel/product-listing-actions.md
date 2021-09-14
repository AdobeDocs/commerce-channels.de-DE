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

Die Aktionseinstellungen für die Produktliste sind Teil Ihrer Einstellungen für die Store-Auflistung. Auf die Listening-Einstellungen kann über das [Store-Dashboard](./amazon-store-dashboard.md) zugegriffen werden.

Diese Einstellungen definieren, wie Ihr Katalog mit Amazon interagiert. Diese Einstellungen:

- Geben Sie an, ob Ihre [!DNL Commerce] -Katalogprodukte, die die Amazon-Voraussetzungen erfüllen, automatisch an Ihr [!DNL Amazon Seller Central] -Konto gesendet werden, um Auflistungen zu erstellen.

- Legen Sie die standardmäßige Bearbeitungszeit für eine Bestellung fest. Dieser Wert definiert die Anzahl der Tage, die Sie benötigen, um eine Bestellung zu verarbeiten und zu versenden. Wenn beispielsweise jemand 2 Tage Versand auswählt, beginnt diese Versanddurchlaufzeit erst nach Abschluss der Verarbeitung und die Pakete werden an einen Beförderer übergeben. Die Versandzeit beträgt insgesamt (Bearbeitungszeit + Versandzeit + Feiertage).

## Einstellungen konfigurieren

1. Klicken Sie im Store-Dashboard auf **[!UICONTROL Listing Settings]** .

1. Erweitern Sie den Abschnitt _[!UICONTROL Product Listing Actions]_.

1. Wählen Sie für **[!UICONTROL Automatic List Action]** (erforderlich) eine Option:

   - `Automatically List Eligible Products` - (Standard) Wählen Sie aus, wann Ihre  [!DNL Commerce] Katalogprodukte (die die Voraussetzungen für Amazon erfüllen) automatisch in Amazon veröffentlicht und Amazon-Listen erstellt werden sollen.

   - `Do Not Automatically List Eligible Products` - Wählen Sie aus, wann Sie die entsprechenden  [!DNL Commerce] Katalogprodukte manuell auswählen und Amazon-Listen erstellen möchten. Falls ausgewählt, werden Katalogprodukte, die Ihren Listenkriterien entsprechen und alle erforderlichen Informationen enthalten, auf dem Tab [_[!UICONTROL Ready to List]_](./ready-to-list.md) angezeigt, um sie manuell in Amazon zu veröffentlichen.

1. Geben Sie für **[!UICONTROL Default Handling Time]** (erforderlich) die Anzahl der Tage an, die für die Vorlaufzeit vor dem Versand benötigt werden.

   Der Standardwert ist `2` Tage.

   >[!NOTE]
   >
   >Dieser standardmäßige Bereitstellungszeitwert gilt nur für Amazon-Auflistungen, die über den Amazon-Vertriebskanal erstellt werden. Alle Amazon-Listen, die in Ihrem [!DNL Amazon Seller Central]-Konto erstellt wurden, verwenden die in Amazon festgelegte standardmäßige Bearbeitungszeit.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save listing settings]**.

![Aktionen auf der Produktliste](assets/amazon-product-listing-actions.png)

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Automatic List Action] | Optionen:<ul><li>**[!UICONTROL Automatically List Eligible Products]** - (Empfohlen) Wählen Sie aus, wann Ihre  [!DNL Commerce] Katalogprodukte (die die Voraussetzungen für Amazon erfüllen) automatisch in Amazon veröffentlicht und Amazon-Listen erstellt werden sollen. Wenn diese Option aktiviert ist, wird die Registerkarte [_[!UICONTROL Ready to List]_](./ready-to-list.md) nicht angezeigt. </li><li>**[!UICONTROL Do Not Automatically List Eligible Products]** - Wählen Sie aus, wann Sie die geeigneten  [!DNL Commerce] Katalogprodukte manuell auswählen und Amazon-Listen erstellen möchten. Falls ausgewählt, werden Katalogprodukte, die Ihren Listenkriterien entsprechen und alle erforderlichen Informationen enthalten, auf dem Tab [_[!UICONTROL Ready to List]_](./ready-to-list.md) angezeigt, um sie manuell zu veröffentlichen.</li></ul> |
| [!UICONTROL Default Handling Time] | Der numerische Wert, der die Anzahl der Tage angibt, die Sie für die Verarbeitung und den Versand Ihrer Bestellungen benötigen. Der Standardwert ist `2`. Dieser Wert wird für Amazon-Auflistungen verwendet, die in [!DNL Commerce] erstellt und in Amazon veröffentlicht wurden. Die standardmäßige Bearbeitungszeit für Amazon-Auflistungen vor der Integration mit [!DNL Commerce] wird von dieser Einstellung nicht beeinflusst.<br><br>Der im Amazon-Vertriebskanal definierte Wert ersetzt nicht die standardmäßige Bearbeitungszeit, die in einer vorhandenen Amazon-Liste definiert ist. Wenn **[!UICONTROL Handling Time Override]** aktiviert und dann entfernt wird, wird die Verarbeitungszeit für eine Bestellung auf den hier definierten Wert zurückgesetzt.<br><br>Wenn Sie Produkte mit unterschiedlichen Verarbeitungszeiten haben, können Sie eine &quot;Handling Time Override&quot;auf produktspezifischer Ebene erstellen. Sie können Überschreibungen von Bearbeitungszeiten im Tab [_[!UICONTROL Overrides]_](./overrides.md) verwalten, sodass Sie Ihre Produkterfüllung flexibel verwalten können. Wenn [!DNL Commerce] für ein Produkt keine Überschreibungszeit enthält, ist der Standardwert für die Bearbeitungszeit der in der Amazon-Auflistung definierte Wert.<br><br>Die Verarbeitungszeit ist ein regionales Attribut. Wenn der Wert für eine Auflistung geändert wird, wirkt sich die Änderung auf alle Auflistungen aus, die den [!DNL Amazon Seller SKU] in allen Amazon Stores teilen, die für dieselbe Region vorhanden sind (definiert unter [Speicherintegration](./store-integration.md)). Eine Änderung des Werts für ein freigegebenes [!DNL Amazon Seller SKU] in Nordamerika wirkt sich jedoch nicht auf dieselben Produkte aus, die in einem Store mit einer anderen definierten Region aufgeführt sind. Der Speicher für die Region mit dem ältesten Erstellungsdatum steuert die Priorität für die Standardeinstellungen für die Verarbeitungszeit. |

**Schnellzugriff**  -  [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
