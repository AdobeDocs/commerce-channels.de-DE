---
title: Katalogsuche
description: Um die Attributzuordnung festzulegen, mit der die geeigneten Commerce-Katalogprodukte Amazon-Auflistungen zugeordnet werden können, aktualisieren Sie die Einstellungen für die Katalogsuche .
redirect_from: /sales-channels/asc/ob-catalog-search.html
exl-id: 9fcaa924-cba3-498f-8e21-1a1f91b1ad04
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '981'
ht-degree: 0%

---

# Katalogsuche

_Einstellungen_ für die Katalogsuche sind Teil Ihrer Einstellungen für die Store-Auflistung. Auf die Listening-Einstellungen kann über das [Store-Dashboard](./amazon-store-dashboard.md) zugegriffen werden.

Mit diesen Einstellungen können Sie Attributabgleiche festlegen, mit denen Sie geeignete [!DNL Commerce]-Produkte Amazon-Listen zuordnen können. Sofern zugeordnet, aktiviert Amazon Aktionen im Zusammenhang mit Preisen, Menge, Außerkraftsetzungen sowie der Bestell- und Produktsynchronisierung.

Die Definition dieser Zuordnungswerte erhöht das Potenzial für exakte Übereinstimmungen, wodurch die Notwendigkeit einer manuellen Übereinstimmung mit Produktlisten minimiert wird. Durch das Hinzufügen der Attribute als Teil Ihrer [Pre-Setup-Aufgaben](./amazon-pre-setup-tasks.md) bietet der Amazon-Vertriebskanal ein höheres Potenzial, Ihre Produkte beim Onboarding automatisch abzugleichen und die Produktdaten zwischen Amazon und [!DNL Commerce] zu synchronisieren.

Wenn Sie nur das Amazon-ASIN-Attribut erstellen (ohne ASIN-Werte pro Produkt hinzuzufügen), stimmen Ihre [!DNL Commerce]-Produkte möglicherweise nicht automatisch mit Ihren Amazon-Auflistungen überein. Sie können [Ihre Produkte manuell zuweisen](./creating-assigning-catalog-products.md). Beim manuellen Abgleich werden jedoch nicht die Datenelemente erstellt, die zum Freigeben und Synchronisieren Ihrer Produktdaten erforderlich sind.

>[!IMPORTANT]
>
>Wenn Sie manuell ein Produkt zugeordnet haben und ein ASIN-, UPC- oder anderes Datenelement für das Produkt aktualisieren möchten, müssen Sie die Daten an zwei Stellen aktualisieren. Aktualisieren Sie sie in Ihrem [!DNL Commerce]-Katalog und in Ihrer Amazon-Liste in Ihrem [!DNL Amazon Seller Central]-Konto.

Es empfiehlt sich, diese Attribute und Werte zuzuordnen, sofern verfügbar. Das Abschließen dieser Zuordnung ist nicht erforderlich, ist jedoch für die Produktabstimmung von Vorteil und für eine ordnungsgemäße Katalogsynchronisierung zwischen Amazon und [!DNL Commerce] erforderlich.

Wenn Sie Attribute hinzufügen möchten, finden Sie weitere Informationen unter [Erstellen von Produktattributen für die Amazon-Übereinstimmung](./ob-creating-magento-attributes.md).

## Einstellungen für [!UICONTROL Catalog Search] konfigurieren

1. Klicken Sie im Store-Dashboard auf **[!UICONTROL Listing Settings]** .

1. Erweitern Sie den Abschnitt _[!UICONTROL Catalog Search]_.

1. Wählen Sie für **[!UICONTROL ASIN]** das Produktattribut aus, das Sie für den Amazon ASIN-Wert erstellt haben.

   Ein ASIN ([!DNL Amazon Standard Identification Number]) ist ein eindeutiger Block von zehn Buchstaben und/oder Zahlen, der Elemente identifiziert. Bei Büchern entspricht das ASIN der ISBN-Nummer, bei allen anderen Produkten wird jedoch beim Hochladen des Artikels in den Katalog ein neues ASIN erstellt. Sie finden einen Artikel-ASIN auf der Produktdetailseite in Amazon sowie weitere Details zum Artikel.

1. Wählen Sie für **[!UICONTROL EAN]** das Produktattribut, das Sie für den Amazon EAN-Wert erstellt haben.

   Die europäische Artikelnummer (European Article Number, EAN) ist ein Barcode-Standard, ein 12- oder 13-stelliger Produktidentifizierungscode. Jede EAN identifiziert das Produkt, den Hersteller und seine Attribute eindeutig. Normalerweise wird das EAN auf einem Produktetikett oder einer Verpackung als Barcode gedruckt. Amazon benötigt EAN-Codes, um die Qualität der Suchergebnisse und die Qualität des Katalogs zu verbessern. Sie können EANs vom Hersteller erhalten.

1. Wählen Sie für **[!UICONTROL GCID]** das Produktattribut aus, das Sie für den Amazon GCIN-Wert erstellt haben.

   Die globale Katalogkennung (GCID) ist eine ID für Produkte ohne UPC-Code oder ISBN. Mit der Brand Registry von Amazon können Sie sich als Markeninhaber registrieren und eine eindeutige ID für Produkte erstellen.

1. Wählen Sie für **[!UICONTROL ISBN]** das Produktattribut, das Sie für den Amazon ISBN-Wert erstellt haben.

   Die International Standard Book Number (ISBN) ist ein eindeutiger Barcode für die Handelsbuchkennung. Jeder ISBN-Code identifiziert ein Buch eindeutig. Eine ISBN hat entweder zehn oder 13 Stellen. Alle nach dem 1. Januar 2007 zugewiesenen ISBN haben 13 Stellen.

1. Wählen Sie für **[!UICONTROL UPC]** das Produktattribut aus, das Sie für den Amazon UPC-Wert erstellt haben.

   Der Universal Product Code (UPC) ist ein 12-stelliger Barcode, der in den Vereinigten Staaten in großem Umfang für Einzelhandelspackungen verwendet wird.

1. Wählen Sie für **[!UICONTROL General Search]** das Produktattribut aus, das Sie für eine allgemeine Suchübereinstimmung verwenden möchten.

   Dieses Attribut können Sie auswählen, ob [!DNL Commerce]-Produkte mit der entsprechenden Amazon-Liste übereinstimmen sollen. Die allgemeine Suche verwendet Suchbegriffe aus Ihrem Katalog. Daher wird empfohlen, ein [!DNL Commerce] -Attribut zu verwenden, das relevante Schlüsselwörter wie die Produkt-SKU oder den Produktnamen enthält. Die allgemeine Suche kann viele mögliche Übereinstimmungen zurückgeben. In diesem Fall können Sie die entsprechende Amazon-Liste aus den möglichen Übereinstimmungen auswählen. Eine gängige Auswahl für dieses Feld ist `Product Name`.

1. Klicken Sie nach Abschluss des Vorgangs auf **[!UICONTROL Save listing settings]**.

![Katalogsuche](assets/amazon-catalog-search.png)

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL ASIN] | Ein eindeutiger Block von 10 Buchstaben und/oder Zahlen zur Identifizierung von Elementen.<br><br>ASIN steht für die  [!DNL Amazon Standard Identification Number]. Ein ASIN ist ein eindeutiger Block von 10 Buchstaben und/oder Zahlen, der Elemente identifiziert. Bei Büchern entspricht das ASIN der ISBN-Nummer, bei allen anderen Produkten wird jedoch beim Hochladen des Artikels in den Katalog ein neues ASIN erstellt. Sie finden einen Artikel-ASIN auf der Produktdetailseite in Amazon sowie weitere Details zum Artikel. |
| [!UICONTROL EAN (European Article Number)] | Ein 12- oder 13-stelliger Produktidentifizierungscode. Die europäische Artikelnummer (European Article Number, EAN) ist ein Barcode-Standard, ein 12- oder 13-stelliger Produktidentifizierungscode. Jede EAN identifiziert das Produkt, den Hersteller und seine Attribute eindeutig. Normalerweise wird das EAN auf einem Produktetikett oder einer Verpackung als Barcode gedruckt. Amazon benötigt EAN-Codes, um die Qualität der Suchergebnisse und die Qualität des Katalogs zu verbessern. Sie können EANs vom Hersteller erhalten. |
| [!UICONTROL GCID (Global Catalog Identifier)] | Die globale Katalogkennung (GCID) ist eine ID für Produkte ohne UPC-Code oder ISBN. Mit der Brand Registry von Amazon können Sie sich als Markeninhaber registrieren und eine eindeutige ID für Produkte erstellen, die möglicherweise keine UPC oder ISBN besitzen. |
| [!UICONTROL ISBN (International Standard Book Number)] | Ein 10- oder 13-stelliger eindeutiger Handelsbuchkennungsbarcode. Die International Standard Book Number (ISBN) ist ein eindeutiger Barcode für die Handelsbuchkennung. Jeder ISBN-Code identifiziert ein Buch eindeutig. Eine ISBN hat entweder zehn oder 13 Stellen. Alle nach dem 1. Januar 2007 zugewiesenen ISBN haben 13 Stellen. |
| UPC (Universal Product Code) | Ein 12-stelliger Barcode. Der Universal Product Code (UPC) ist ein 12-stelliger Barcode, der in den Vereinigten Staaten in großem Umfang für Einzelhandelspackungen verwendet wird. |
| [!UICONTROL General Search] | Wählen Sie ein Attribut aus. Dieses Attribut können Sie auswählen, ob [!DNL Commerce]-Produkte mit der entsprechenden Amazon-Liste übereinstimmen sollen. Die allgemeine Suche verwendet Suchbegriffe aus Ihrem Katalog. Daher wird empfohlen, ein [!DNL Commerce] -Attribut zu verwenden, das relevante Schlüsselwörter wie die Produkt-SKU oder den Produktnamen enthält. Die allgemeine Suche kann viele mögliche Übereinstimmungen zurückgeben. In diesem Fall können Sie die entsprechende Amazon-Liste aus den möglichen Übereinstimmungen auswählen. Eine gängige Auswahl für dieses Feld ist `Product Name`. |

**Schnellzugriff**  -  [!UICONTROL Listing Settings] Abschnitte

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
