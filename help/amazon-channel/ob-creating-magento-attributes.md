---
title: Erstellen [!DNL Commerce] Attribute für Amazon
description: Stellen Sie vor Abschluss des Amazon Sales Kanal-Onboarding-Prozesses sicher, dass Sie über die erforderlichen [!UICONTROL Commerce] Produktattribute.
exl-id: eebad794-c171-40a3-aa24-d5509e2b5797
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 0%

---

# Erstellen [!DNL Commerce] Attribute für Amazon

Bevor Sie Ihre [!DNL Amazon Seller Central] , ist es empfehlenswert, [!DNL Commerce] [Produktattribute](https://docs.magento.com/user-guide/stores/attributes-product.html){Zielgruppe=&quot;_blank&quot;}, um Ihre Produktauflistungen zuzuordnen. Nach Abschluss der Onboarding-Aktivitäten können Sie Ihre Produktattribute verwalten über [Attribute](./managing-attributes.md) des [Amazon Sales Kanal Home](./amazon-sales-channel-home.md) Seite.

In diesen Anweisungen wird das Erstellen von [!DNL Commerce] Attribute für Amazon ASIN und Amazon Condition. Es wird empfohlen, zusätzliche Attribute wie Amazon EAN, Amazon ISBN und Amazon UPC zu erstellen. Sie können auch ein Amazon Price-Attribut erstellen, wenn Sie Ihren Amazon-Listungspreis als Preisquelle für Preisregeln verwenden möchten. Diese Attribute werden bei der Konfiguration Ihrer Listen- und Preiseinstellungen während des Einstiegs verwendet. Verwenden Sie diese Attribute auch beim Erstellen von Amazon-Auflistungen und beim Aktualisieren und Synchronisieren Ihrer [!DNL Commerce] mit Ihren Amazon-Listen.

Mit den Einstellungen der Katalogsuche können Sie passende Suchparameter festlegen, die zur Zuordnung förderfähiger Dateien beitragen. [!DNL Commerce] Produkte mit Amazon-Auflistungen. Wenn Amazon zugeordnet ist, aktiviert es Aktionen in Bezug auf Preisgestaltung, Quantität, Aufhebung von Beschränkungen sowie Bestellung und Produktsynchronisation.

Die Definition dieser Werte erhöht das Potenzial für exakte Übereinstimmungen und minimiert die Notwendigkeit, die Produktauflistungen später manuell anzupassen. Hinzufügen der Attribute als Teil Ihres Einstiegs [Aufgaben vor dem Setup](./amazon-pre-setup-tasks.md), hat Amazon Sales Kanal ein höheres Potenzial, Ihre Produkte während des Einbodens automatisch anzupassen und die Produktdaten zwischen Amazon und [!DNL Commerce] nach dem Einsteigen.

Wenn Sie nur das Amazon ASIN-Attribut erstellen (ohne ASIN-Werte pro Produkt hinzuzufügen), [!DNL Commerce] Produkte stimmen möglicherweise nicht automatisch mit Ihren Amazon-Listen überein. Sie können Ihre Produkte manuell anpassen über _Überprüfung speichern_. Durch manuelle Zuordnung werden jedoch keine Datenelemente erstellt, die zur Freigabe und Synchronisierung Ihrer Produktdaten erforderlich sind.

>[!IMPORTANT]
>
>Wenn Sie ein ASIN-, UPC- oder anderes Datenelement für ein manuell übereinstimmendes Produkt aktualisieren, müssen Sie die Daten an beiden Orten aktualisieren: Ihre [!DNL Commerce] Katalog und die Auflistung in Ihrer [!DNL Amazon Seller Central] Konto.

## Amazon ASIN-Produktattribut erstellen

1. Melden Sie sich bei [!DNL Commerce] Admin.

1. Klick **[!UICONTROL Stores]** im Menü links.

1. In _[!UICONTROL Attributes]_Abschnitt, klicken Sie **[!UICONTROL Product]**.

1. Klicken Sie zum Öffnen der Attributeigenschaften auf **[!UICONTROL Add New Attribute]**.

1. für **[!UICONTROL Default Label]**, eingeben `Amazon ASIN` (der Name für Ihr Attribut).

1. für **[!UICONTROL Catalog Input Type for Store Owner]**, wählen `Text Field`.

1. für **[!UICONTROL Values Required]**, wählen `No`.

   Obwohl ein Amazon ASIN erforderlich ist, um ein Produkt auf Amazon Liste, werden einige Ihrer Katalogprodukte möglicherweise nicht auf Amazon aufgelistet.

1. Erweitern der _[!UICONTROL Advanced Attribute Properties]_und legen Sie die Optionen fest:

   - für **[!UICONTROL Attribute Code]**, eingeben `amazon_asin`.

   - für **[!UICONTROL Scope]**, wählen `Global`.

   - für **[!UICONTROL Unique Value]**, wählen `No`.

   - für **[!UICONTROL Input Validation for Store Owner]**, wählen `None`.

   - für **[!UICONTROL Add to Column Options]**, wählen `Yes`.

   - für **[!UICONTROL Use in Filter Options]**, wählen `Yes`.

1. Klick **[!UICONTROL Save Attribute]**.

![Amazon ASIN-Attribut](assets/creating-asin-attribute.png)

## Amazon Condition-Produktattribut erstellen

1. Melden Sie sich bei [!DNL Commerce] Admin.

1. Klick **[!UICONTROL Stores]** im Menü links.

1. In _[!UICONTROL Attributes]_Abschnitt, klicken Sie **[!UICONTROL Product]**.

1. Klicken Sie zum Öffnen der Attributeigenschaften auf **[!UICONTROL Add New Attribute]**.

1. für **[!UICONTROL Default Label]**, eingeben `Amazon Condition` (der Name für Ihr Attribut).

1. für **[!UICONTROL Catalog Input Type for Store Owner]**, wählen `Dropdown`.

   Die _[!UICONTROL Manage Options (Values of your Attribute)]_angezeigt.

1. für **[!UICONTROL Values Required]**, wählen `No`.

1. für **[!UICONTROL Manage Options (Values for your Attribute)]**, fügen Sie jede Ihrer Bedingungsoptionen hinzu.

   Die Amazon-Standardbedingungen umfassen:

   - `New: Refurbished: Used`
   - `Like New: Used`
   - `Very Good: Used`
   - `Good: Used`
   - `Acceptable: Collectible`
   - `Like New; Collectible`
   - `Very Good: Collectible`
   - `Good: Collectible; Acceptable`

1. Klick **[!UICONTROL Add Option]**.

1. Wählen Sie **[!UICONTROL Is Default]** für die Bedingung, die als Standardauswahl verwendet werden soll.

1. In _[!UICONTROL Admin]_-Spalte, geben Sie den Text für die Bezeichnung der hinzuzufügenden Bedingung ein (z. B. `New`, `Used`und `Used-Like New`)

1. Klick **[!UICONTROL Add Option]** um bei Bedarf weitere Optionen hinzuzufügen.

1. Erweitern _[!UICONTROL Advanced Attribute Properties]_und legen die Optionen fest.

   - für **[!UICONTROL Attribute Code]**, eingeben `amazon_condition`.

   - für **[!UICONTROL Scope]**, wählen `Global`.

   - für **[!UICONTROL Unique Value]**, wählen `No`.

   - für **[!UICONTROL Input Validation for Store Owner]**, wählen `None`.

   - für **[!UICONTROL Add to Column Options]**, wählen `Yes`.

   - für **[!UICONTROL Use in Filter Options]**, wählen `Yes`.

1. Klick **[!UICONTROL Save Attribute]**.

![Amazon Condition-Attribut](assets/creating-amazon-condition-attribute.png)

![Nächstes Symbol](assets/btn-next.png) [**Weiter zum Hinzufügen oder Überprüfen des API-Schlüssels**](./amazon-verify-api-key.md)
