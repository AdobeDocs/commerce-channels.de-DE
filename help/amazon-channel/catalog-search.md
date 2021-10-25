---
title: Katalogsuche
description: Aktualisieren Sie die Katalogsucheinstellungen, um die Attributzuordnung festzulegen, mit der Sie förderfähige Commerce-Katalogprodukte mit Amazon-Auflistungen zuordnen können.
redirect_from: /sales-channels/asc/ob-catalog-search.html
exl-id: 9fcaa924-cba3-498f-8e21-1a1f91b1ad04
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '981'
ht-degree: 0%

---

# Katalogsuche

_Katalogsuche_ -Einstellungen Teil Ihrer Einstellungen für die Ladenliste sind. Auf die Listseinstellungen kann über folgende Optionen zugegriffen werden: [Dashboard speichern](./amazon-store-dashboard.md).

Mit diesen Einstellungen können Sie Attributzuordnungen festlegen, die eine Zuordnung der zulässigen Werte ermöglichen [!DNL Commerce] Produkte mit Amazon-Auflistungen. Wenn Amazon zugeordnet ist, aktiviert es Aktionen in Bezug auf Preisgestaltung, Quantität, Aufhebung von Beschränkungen sowie Bestellung und Produktsynchronisation.

Die Definition dieser Zuordnungswerte erhöht das Potenzial für exakte Übereinstimmungen und minimiert die Notwendigkeit, die Produktauflistungen manuell anzupassen. Hinzufügen der Attribute als Teil Ihrer [Aufgaben vor dem Setup](./amazon-pre-setup-tasks.md), hat Amazon Sales Kanal ein höheres Potenzial, Ihre Produkte während des Einbodens automatisch anzupassen und die Produktdaten zwischen Amazon und [!DNL Commerce].

Wenn Sie nur das Amazon ASIN-Attribut erstellen (ohne ASIN-Werte pro Produkt hinzuzufügen), [!DNL Commerce] Produkte stimmen möglicherweise nicht automatisch mit Ihren Amazon-Auflistungen überein. Sie können [manuell zuweisen](./creating-assigning-catalog-products.md) Ihre Produkte. Die manuelle Zuordnung erstellt jedoch nicht die Datenelemente, die zum Freigeben und Synchronisieren Ihrer Produktdaten erforderlich sind.

>[!IMPORTANT]
>
>Wenn Sie ein Produkt manuell zugeordnet haben und ein ASIN-, UPC- oder anderes Datenelement für das Produkt aktualisieren möchten, müssen Sie die Daten an zwei Stellen aktualisieren. Aktualisieren Sie es in Ihrem [!DNL Commerce] im Katalog und in der Amazon-Auflistung in Ihrem [!DNL Amazon Seller Central] Konto.

Es ist empfehlenswert, diese Attribute und Werte zuzuordnen, falls verfügbar. Das Ausfüllen dieser Zuordnung ist nicht erforderlich, ist jedoch für die Produktübereinstimmung von Vorteil und für eine ordnungsgemäße Katalogsynchronisierung zwischen Amazon und erforderlich. [!DNL Commerce].

Informationen zum Hinzufügen von Attributen finden Sie unter [Produktattribute für Amazon Matching erstellen](./ob-creating-magento-attributes.md).

## Konfigurieren [!UICONTROL Catalog Search] Einstellungen

1. Klick **[!UICONTROL Listing Settings]** auf dem Dashboard.

1. Erweitern der _[!UICONTROL Catalog Search]_Abschnitt.

1. für **[!UICONTROL ASIN]**, wählen Sie das Produktattribut aus, das Sie für den Amazon ASIN-Wert erstellt haben.

   Ein ASIN ([!DNL Amazon Standard Identification Number]) ist ein eindeutiger Block von zehn Buchstaben und/oder Zahlen, die Elemente identifizieren. Für Bücher ist die ASIN die gleiche ISBN-Nummer, aber für alle anderen Produkte wird ein neues ASIN erstellt, wenn das Element in ihren Katalog hochgeladen wird. Auf der Produktdetailseite auf Amazon finden Sie ASIN und weitere Details zum Artikel.

1. für **[!UICONTROL EAN]**, wählen Sie das Produktattribut aus, das Sie für den Amazon EAN-Wert erstellt haben.

   Die Europäische Artikelnummer (EAN) ist ein Strichcode-Standard, ein 12- oder 13-stelliger Produktkenncode. Jedes EAN identifiziert das Produkt, den Hersteller und seine Eigenschaften eindeutig. In der Regel wird das EAN auf einem Produktetikett oder einer Verpackung als Strichcode gedruckt. Amazon benötigt EAN-Codes, um die Qualität der Suchergebnisse und die Qualität des Katalogs zu verbessern. Sie können EANs vom Hersteller beziehen.

1. für **[!UICONTROL GCID]**, wählen Sie das Produktattribut aus, das Sie für den Amazon GCIN-Wert erstellt haben.

   Die globale Katalogkennung (GCID) ist eine ID für Produkte, die keinen UPC-Code oder ISBN haben. Amazons Markenregister ermöglicht es Ihnen, sich als Markeninhaber zu registrieren und eine eindeutige ID für Produkte zu erstellen.

1. für **[!UICONTROL ISBN]**, wählen Sie das Produktattribut aus, das Sie für den Amazon ISBN-Wert erstellt haben.

   Die International Standard Book Number (ISBN) ist ein eindeutiger Barcode für die Handelsbuchkennung. Jeder ISBN-Code identifiziert ein Buch eindeutig. Eine ISBN hat zehn oder 13 Ziffern. Alle nach dem 1. Januar 2007 zugewiesenen ISBN haben 13 Ziffern.

1. für **[!UICONTROL UPC]**, wählen Sie das Produktattribut aus, das Sie für den Amazon UPC-Wert erstellt haben.

   Der Universal Product Code (UPC) ist ein 12-stelliger Strichcode, der in den Vereinigten Staaten umfassend für Einzelhandelspackungen verwendet wird.

1. für **[!UICONTROL General Search]**, wählen Sie das Produktattribut aus, das Sie für eine allgemeine Suche verwenden möchten.

   Dieses Attribut kann zur Übereinstimmung ausgewählt werden [!DNL Commerce] Erzeugnisse in die entsprechende Amazon-Liste aufgenommen. Bei der allgemeinen Suche werden Suchbegriffe aus Ihrem Katalog verwendet. Daher wird empfohlen, [!DNL Commerce] Attribut, das relevante Keywords enthält, wie z. B. die Produkt-SKU oder den Produktnamen. Eine allgemeine Suche kann viele mögliche Treffer zurückgeben, und in solchen Fällen können Sie die entsprechende Amazon-Liste aus den möglichen Treffern auswählen. Eine allgemeine Auswahl für dieses Feld ist `Product Name`.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save listing settings]**.

![Katalogsuche](assets/amazon-catalog-search.png)

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL ASIN] | Ein eindeutiger Block mit 10 Buchstaben und/oder Zahlen, die Elemente identifizieren.<br><br>ASIN steht für [!DNL Amazon Standard Identification Number]. Ein ASIN ist ein eindeutiger Block mit 10 Buchstaben und/oder Ziffern, der Elemente identifiziert. Für Bücher ist die ASIN die gleiche ISBN-Nummer, aber für alle anderen Produkte wird ein neues ASIN erstellt, wenn das Element in ihren Katalog hochgeladen wird. Auf der Produktdetailseite auf Amazon finden Sie ASIN und weitere Details zum Artikel. |
| [!UICONTROL EAN (European Article Number)] | Ein 12- oder 13-stelliger Produktkenncode. Die Europäische Artikelnummer (EAN) ist ein Strichcode-Standard, ein 12- oder 13-stelliger Produktkenncode. Jedes EAN identifiziert das Produkt, den Hersteller und seine Eigenschaften eindeutig. In der Regel wird das EAN auf einem Produktetikett oder einer Verpackung als Strichcode gedruckt. Amazon benötigt EAN-Codes, um die Qualität der Suchergebnisse und die Qualität des Katalogs zu verbessern. Sie können EANs vom Hersteller beziehen. |
| [!UICONTROL GCID (Global Catalog Identifier)] | Die globale Katalogkennung (GCID) ist eine ID für Produkte, die keinen UPC-Code oder ISBN haben. Amazons Markenregister ermöglicht es Ihnen, sich als Markeninhaber zu registrieren und eine eindeutige ID für Produkte zu erstellen, die keine UPC oder ISBN besitzen. |
| [!UICONTROL ISBN (International Standard Book Number)] | Ein 10- oder 13-stelliger eindeutiger Handelsbuchkennung-Strichcode. Die International Standard Book Number (ISBN) ist ein eindeutiger Barcode für die Handelsbuchkennung. Jeder ISBN-Code identifiziert ein Buch eindeutig. Eine ISBN hat zehn oder 13 Ziffern. Alle nach dem 1. Januar 2007 zugewiesenen ISBN haben 13 Ziffern. |
| UPC (Universeller Produktcode) | Ein 12-stelliger Strichcode. Der Universal Product Code (UPC) ist ein 12-stelliger Strichcode, der in den Vereinigten Staaten umfassend für Einzelhandelspackungen verwendet wird. |
| [!UICONTROL General Search] | Wählen Sie ein Attribut aus. Dieses Attribut kann zur Übereinstimmung ausgewählt werden [!DNL Commerce] Erzeugnisse in die entsprechende Amazon-Liste aufgenommen. Bei der allgemeinen Suche werden Suchbegriffe aus Ihrem Katalog verwendet. Daher wird empfohlen, [!DNL Commerce] Attribut, das relevante Keywords enthält, wie z. B. die Produkt-SKU oder den Produktnamen. Eine allgemeine Suche kann viele mögliche Treffer zurückgeben, und in solchen Fällen können Sie die entsprechende Amazon-Liste aus den möglichen Treffern auswählen. Eine allgemeine Auswahl für dieses Feld ist `Product Name`. |

**Schnellzugriff** - [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
