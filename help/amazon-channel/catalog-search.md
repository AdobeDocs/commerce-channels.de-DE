---
title: Katalogsuche nach Amazon-Listen
description: Um die Attributzuordnung festzulegen, mit der die geeigneten Commerce-Katalogprodukte Amazon-Auflistungen zugeordnet werden können, aktualisieren Sie die Einstellungen für die Katalogsuche .
feature: Sales Channels, Search, Catalogs, Products, Configuration
exl-id: 9fcaa924-cba3-498f-8e21-1a1f91b1ad04
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '987'
ht-degree: 0%

---

# Katalogsuche nach Amazon-Listen

_Katalogsuche_ -Einstellungen sind Teil Ihrer Einstellungen für die Store-Auflistung. Auf die Listening-Einstellungen kann über die [Store-Dashboard](./amazon-store-dashboard.md).

Mit diesen Einstellungen können Sie die Zuordnung von Attributen festlegen, die Ihnen dabei helfen, die Voraussetzungen zuzuordnen [!DNL Commerce] Produkte mit Amazon-Listen. Sofern zugeordnet, aktiviert Amazon Aktionen im Zusammenhang mit Preisen, Menge, Außerkraftsetzungen sowie der Bestell- und Produktsynchronisierung.

Die Definition dieser Zuordnungswerte erhöht das Potenzial für exakte Übereinstimmungen, wodurch die Notwendigkeit einer manuellen Übereinstimmung mit Produktlisten minimiert wird. Hinzufügen der Attribute als Teil Ihrer [Aufgaben vor der Einrichtung](./amazon-pre-setup-tasks.md)bietet der Amazon-Vertriebskanal ein höheres Potenzial, Ihre Produkte beim Onboarding automatisch abzugleichen und die Produktdaten zwischen Amazon und zu synchronisieren. [!DNL Commerce].

Wenn Sie nur das Amazon-ASIN-Attribut erstellen (ohne ASIN-Werte pro Produkt hinzuzufügen), wird Ihre [!DNL Commerce] -Produkte stimmen möglicherweise nicht automatisch mit Ihren Amazon-Listen überein. Sie können [manuell zuweisen](./creating-assigning-catalog-products.md) Ihre Produkte. Beim manuellen Abgleich werden jedoch nicht die Datenelemente erstellt, die zum Freigeben und Synchronisieren Ihrer Produktdaten erforderlich sind.

>[!IMPORTANT]
>
>Wenn Sie manuell ein Produkt zugeordnet haben und ein ASIN-, UPC- oder anderes Datenelement für das Produkt aktualisieren möchten, müssen Sie die Daten an zwei Stellen aktualisieren. Aktualisieren Sie es in Ihrer [!DNL Commerce] und in Ihrer Amazon-Liste in [!DNL Amazon Seller Central] -Konto.

Es empfiehlt sich, diese Attribute und Werte zuzuordnen, sofern verfügbar. Das Abschließen dieser Zuordnung ist nicht erforderlich, ist jedoch für die Produktabstimmung von Vorteil und für eine ordnungsgemäße Katalogsynchronisierung zwischen Amazon und erforderlich [!DNL Commerce].

Informationen zum Hinzufügen von Attributen finden Sie unter [Erstellen von Produktattributen für Amazon-Übereinstimmung](./ob-creating-magento-attributes.md).

## Konfigurieren [!UICONTROL Catalog Search] settings

1. Klicken **[!UICONTROL Listing Settings]** im Dashboard speichern.

1. Erweitern Sie die _[!UICONTROL Catalog Search]_Abschnitt.

1. Für **[!UICONTROL ASIN]** wählen Sie das Produktattribut aus, das Sie für den Amazon ASIN-Wert erstellt haben.

   EIN ASIN ([!DNL Amazon Standard Identification Number]) ist ein eindeutiger Block von zehn Buchstaben und/oder Zahlen, der Elemente kennzeichnet. Bei Büchern entspricht das ASIN der ISBN-Nummer, bei allen anderen Produkten wird jedoch beim Hochladen des Artikels in den Katalog ein neues ASIN erstellt. Sie finden einen Artikel-ASIN auf der Produktdetailseite in Amazon sowie weitere Details zum Artikel.

1. Für **[!UICONTROL EAN]** wählen Sie das Produktattribut aus, das Sie für den Amazon EAN-Wert erstellt haben.

   Die europäische Artikelnummer (European Article Number, EAN) ist ein Barcode-Standard, ein 12- oder 13-stelliger Produktidentifizierungscode. Jede EAN identifiziert das Produkt, den Hersteller und seine Attribute eindeutig. Normalerweise wird das EAN auf einem Produktetikett oder einer Verpackung als Barcode gedruckt. Amazon benötigt EAN-Codes, um die Qualität der Suchergebnisse und die Qualität des Katalogs zu verbessern. Sie können EANs vom Hersteller erhalten.

1. Für **[!UICONTROL GCID]** wählen Sie das Produktattribut aus, das Sie für den Amazon GCIN-Wert erstellt haben.

   Die globale Katalogkennung (GCID) ist eine ID für Produkte ohne UPC-Code oder ISBN. Mit der Brand Registry von Amazon können Sie sich als Markeninhaber registrieren und eine eindeutige ID für Produkte erstellen.

1. Für **[!UICONTROL ISBN]** wählen Sie das Produktattribut aus, das Sie für den Amazon ISBN-Wert erstellt haben.

   Die International Standard Book Number (ISBN) ist ein eindeutiger Barcode für die Handelsbuchkennung. Jeder ISBN-Code identifiziert ein Buch eindeutig. Eine ISBN hat entweder zehn oder 13 Stellen. Alle nach dem 1. Januar 2007 zugewiesenen ISBN haben 13 Stellen.

1. Für **[!UICONTROL UPC]** wählen Sie das Produktattribut aus, das Sie für den UPC-Wert von Amazon erstellt haben.

   Der Universal Product Code (UPC) ist ein 12-stelliger Barcode, der in den Vereinigten Staaten in großem Umfang für Einzelhandelspackungen verwendet wird.

1. Für **[!UICONTROL General Search]** wählen Sie das Produktattribut aus, das Sie für eine allgemeine Suchübereinstimmung verwenden möchten.

   Dieses Attribut können Sie auswählen, ob eine Übereinstimmung gefunden werden soll [!DNL Commerce] Produkte in die entsprechende Amazon-Liste. Die allgemeine Suche verwendet Suchbegriffe aus Ihrem Katalog. Daher wird empfohlen, eine [!DNL Commerce] -Attribut, das relevante Schlüsselwörter wie die Produkt-SKU oder den Produktnamen enthält. Die allgemeine Suche kann viele mögliche Übereinstimmungen zurückgeben. In diesem Fall können Sie die entsprechende Amazon-Liste aus den möglichen Übereinstimmungen auswählen. Eine gängige Auswahl für dieses Feld ist `Product Name`.

1. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Save listing settings]**.

![Katalogsuche](assets/amazon-catalog-search.png){width="500" zoomable="yes"}

| Feld | Beschreibung |
|--------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL ASIN] | Ein eindeutiger Block von 10 Buchstaben und/oder Zahlen zur Identifizierung von Elementen.<br><br>ASIN steht für die [!DNL Amazon Standard Identification Number]. Ein ASIN ist ein eindeutiger Block von 10 Buchstaben und/oder Zahlen, der Elemente identifiziert. Bei Büchern entspricht das ASIN der ISBN-Nummer, bei allen anderen Produkten wird jedoch beim Hochladen des Artikels in den Katalog ein neues ASIN erstellt. Sie finden einen Artikel-ASIN auf der Produktdetailseite in Amazon sowie weitere Details zum Artikel. |
| [!UICONTROL EAN (European Article Number)] | Ein 12- oder 13-stelliger Produktidentifizierungscode. Die europäische Artikelnummer (European Article Number, EAN) ist ein Barcode-Standard, ein 12- oder 13-stelliger Produktidentifizierungscode. Jede EAN identifiziert das Produkt, den Hersteller und seine Attribute eindeutig. Normalerweise wird das EAN auf einem Produktetikett oder einer Verpackung als Barcode gedruckt. Amazon benötigt EAN-Codes, um die Qualität der Suchergebnisse und die Qualität des Katalogs zu verbessern. Sie können EANs vom Hersteller erhalten. |
| [!UICONTROL GCID (Global Catalog Identifier)] | Die globale Katalogkennung (GCID) ist eine ID für Produkte ohne UPC-Code oder ISBN. Mit der Brand Registry von Amazon können Sie sich als Markeninhaber registrieren und eine eindeutige ID für Produkte erstellen, die möglicherweise keine UPC oder ISBN besitzen. |
| [!UICONTROL ISBN (International Standard Book Number)] | Ein 10- oder 13-stelliger eindeutiger Handelsbuchkennungsbarcode. Die International Standard Book Number (ISBN) ist ein eindeutiger Barcode für die Handelsbuchkennung. Jeder ISBN-Code identifiziert ein Buch eindeutig. Eine ISBN hat entweder zehn oder 13 Stellen. Alle nach dem 1. Januar 2007 zugewiesenen ISBN haben 13 Stellen. |
| UPC (Universal Product Code) | Ein 12-stelliger Barcode. Der Universal Product Code (UPC) ist ein 12-stelliger Barcode, der in den Vereinigten Staaten in großem Umfang für Einzelhandelspackungen verwendet wird. |
| [!UICONTROL General Search] | Wählen Sie ein Attribut aus. Dieses Attribut können Sie auswählen, ob eine Übereinstimmung gefunden werden soll [!DNL Commerce] Produkte in die entsprechende Amazon-Liste. Die allgemeine Suche verwendet Suchbegriffe aus Ihrem Katalog. Daher wird empfohlen, eine [!DNL Commerce] -Attribut, das relevante Schlüsselwörter wie die Produkt-SKU oder den Produktnamen enthält. Die allgemeine Suche kann viele mögliche Übereinstimmungen zurückgeben. In diesem Fall können Sie die entsprechende Amazon-Liste aus den möglichen Übereinstimmungen auswählen. Eine gängige Auswahl für dieses Feld ist `Product Name`. |

**Schnellzugriff** - [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
