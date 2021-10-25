---
title: Produktlistungsaktionen
description: Verwenden Sie die Einstellungen für Produktlistungsaktionen, um zu definieren, wie Ihr Commerce-Katalog mit Amazon interagiert.
redirect_from: /sales-channels/asc/ob-product-listing-actions.html
exl-id: c7d3f22c-05c6-4826-99eb-543bac462cf8
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 0%

---

# Produktlistenkategorien

Die Einstellungen für die Produktlistungsaktionen sind Teil Ihrer Einstellungen für die Ladenliste. Auf die Listseinstellungen kann über folgende Optionen zugegriffen werden: [Dashboard speichern](./amazon-store-dashboard.md).

Diese Einstellungen definieren die Interaktion Ihres Katalogs mit Amazon. Diese Einstellungen:

- Geben Sie an, ob Ihre [!DNL Commerce] Katalogprodukte, die die Amazon-Teilnahmevoraussetzungen erfüllen, werden automatisch an Ihre [!DNL Amazon Seller Central] Konto zum Erstellen von Auflistungen.

- Legen Sie die Standardverarbeitungszeit für eine Bestellung fest. Dieser Wert definiert die Anzahl der Tage, die Sie zum Versenden und Verarbeiten einer Bestellung benötigen. Wenn jemand beispielsweise 2-Tage-Versand wählt, wird die Versandzeit nicht Beginn, bis die Verarbeitung abgeschlossen ist und die Pakete an einen Beförderer übergeben werden. Die Gesamtdauer des Versands beträgt (Bearbeitungszeit + Durchfahrtszeit + Feiertage).

## Einstellungen konfigurieren

1. Klick **[!UICONTROL Listing Settings]** auf dem Dashboard.

1. Erweitern der _[!UICONTROL Product Listing Actions]_Abschnitt.

1. für **[!UICONTROL Automatic List Action]** (erforderlich), wählen Sie eine Option aus:

   - `Automatically List Eligible Products` - (Standard) Wählen Sie aus, wann Sie möchten [!DNL Commerce] Katalogprodukte (die die Anspruchsvoraussetzungen von Amazon erfüllen) zur automatischen Veröffentlichung auf Amazon und Erstellung von Amazon-Listen.

   - `Do Not Automatically List Eligible Products` - Wählen Sie aus, wann Sie das gewünschte Element manuell auswählen möchten [!DNL Commerce] Katalogprodukte erstellen und Amazon-Listen erstellen. Wenn Sie diese Option wählen, werden Produkte katalogisiert, die Ihren Listungskriterien entsprechen und alle erforderlichen Informationen enthalten, auf der [_[!UICONTROL Ready to List]_](./ready-to-list.md) für die manuelle Veröffentlichung auf Amazon.

1. für **[!UICONTROL Default Handling Time]** (erforderlich), geben Sie die Anzahl der Tage an, die für die Vorlaufzeit vor dem Versand benötigt werden.

   Der Standardwert ist `2` Tagen.

   >[!NOTE]
   >
   >Dieser Standard-Ausgabezeitwert ist nur für Amazon-Auflistungen wirksam, die über Amazon Sales Kanal erstellt wurden. Alle Amazon-Auflistungen, die in Ihren [!DNL Amazon Seller Central] -Konto verwenden Sie die in Amazon festgelegte Standardverarbeitungszeit.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save listing settings]**.

![Produktlistenkategorien](assets/amazon-product-listing-actions.png)

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Automatic List Action] | Optionen:<ul><li>**[!UICONTROL Automatically List Eligible Products]** - (Empfohlen) Wählen Sie aus, wann Sie möchten [!DNL Commerce] Katalogprodukte (die die Anspruchsvoraussetzungen von Amazon erfüllen) zur automatischen Veröffentlichung auf Amazon und Erstellung von Amazon-Listen. Bei Auswahl der [_[!UICONTROL Ready to List]_](./ready-to-list.md) nicht angezeigt wird. </li><li>**[!UICONTROL Do Not Automatically List Eligible Products]** - Wählen Sie, wann Sie die Option &quot;Zulässig&quot; manuell auswählen möchten [!DNL Commerce] Katalogprodukte erstellen und Amazon-Listen erstellen. Wenn Sie diese Option wählen, werden Produkte katalogisiert, die Ihren Listungskriterien entsprechen und alle erforderlichen Informationen enthalten, auf der [_[!UICONTROL Ready to List]_](./ready-to-list.md) für die manuelle Veröffentlichung.</li></ul> |
| [!UICONTROL Default Handling Time] | Der numerische Wert, der die Anzahl der Tage angibt, an denen Sie Ihre Bestellungen bearbeiten und versenden müssen. Der Standardwert ist `2`. Dieser Wert wird für Amazon-Auflistungen verwendet, die in [!DNL Commerce] und in Amazon veröffentlicht. Die standardmäßige Bearbeitungszeit für Amazon-Auflistungen vor der Integration in [!DNL Commerce] sind von dieser Einstellung nicht betroffen.<br><br>Der im Amazon Sales Kanal definierte Wert ersetzt nicht die Standardverarbeitungszeit, die in einer bestehenden Amazon-Liste definiert ist. Wenn ein **[!UICONTROL Handling Time Override]** aktiviert und dann entfernt wird, kehrt die Bearbeitungszeit für eine Bestellung auf den hier definierten Wert zurück.<br><br>Wenn Sie Produkte mit unterschiedlichen Verarbeitungszeiten haben, können Sie eine &quot;Handling Time Override&quot;(Zeitüberschreibung für Handling Time Override) auf produktspezifischer Ebene erstellen. Sie können Zeitüberschreitungen im Bereich [_[!UICONTROL Overrides]_](./overrides.md) , damit Sie flexibel in der Verwaltung Ihrer Produkterfüllung sind. Wenn keine Verarbeitungszeit überschrieben wurde [!DNL Commerce] für ein Produkt der Standardwert für die Bearbeitungszeit ist der in der Amazon-Auflistung definierte Wert.<br><br>Die Bearbeitungszeit ist ein regionales Attribut. Wenn der Wert für eine Auflistung geändert wird, wirkt sich die Änderung auf alle Auflistungen aus, die die [!DNL Amazon Seller SKU] in allen Amazon Stores, die für dieselbe Region vorhanden sind (definiert unter [Speicherintegration](./store-integration.md)). Ändern des Werts für eine gemeinsame Nutzung [!DNL Amazon Seller SKU] in Nordamerika nicht die gleichen Erzeugnisse betreffen, die in einem Laden mit einer anderen definierten Region aufgeführt sind. Der Speicher für den Bereich mit dem ältesten Erstellungsdatum steuert die Priorität für die Standardeinstellungen für die Bearbeitungszeit. |

**Schnellzugriff** - [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
