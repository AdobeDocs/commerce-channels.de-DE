---
title: Erstellen [!DNL Commerce] Attribute für Amazon
description: Bevor Sie das Onboarding des Amazon-Verkaufskanals abschließen, stellen Sie sicher, dass Sie über die erforderlichen [!UICONTROL Commerce]-Produktattribute verfügen.
exl-id: eebad794-c171-40a3-aa24-d5509e2b5797
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 0%

---

# Erstellen von [!DNL Commerce]-Attributen für Amazon

Bevor Sie Ihre [!DNL Amazon Seller Central]-Konten integrieren, sollten Sie [!DNL Commerce] [Produktattribute](https://docs.magento.com/user-guide/stores/attributes-product.html){:target=&quot;_blank&quot;} hinzufügen, um Ihre Produktlisten zuzuordnen. Nach Abschluss des Onboarding können Sie Ihre Produktattribute über den Tab [Attribute](./managing-attributes.md) auf der Seite [Amazon Sales Channel home](./amazon-sales-channel-home.md) verwalten.

In diesen Anweisungen wird beschrieben, wie Sie [!DNL Commerce]-Attribute für Amazon ASIN- und Amazon-Bedingungen erstellen. Es wird empfohlen, zusätzliche Attribute wie Amazon EAN, Amazon ISBN und Amazon UPC zu erstellen. Sie können auch ein Amazon-Preisattribut erstellen, wenn Sie Ihren Amazon-Listingpreis als Preisquelle für Preisregeln verwenden möchten. Diese Attribute werden bei der Konfiguration Ihrer Listen- und Preiseinstellungen beim Onboarding verwendet. Verwenden Sie diese Attribute auch beim Erstellen von Amazon-Listen und beim Aktualisieren und Synchronisieren Ihres [!DNL Commerce]-Katalogs mit Ihren Amazon-Auflistungen.

Mit den Einstellungen für die Katalogsuche können Sie übereinstimmende Suchparameter festlegen, mit denen Sie geeignete [!DNL Commerce]-Produkte Amazon-Auflistungen zuordnen können. Sofern zugeordnet, aktiviert Amazon Aktionen im Zusammenhang mit Preisen, Menge, Außerkraftsetzungen sowie der Bestell- und Produktsynchronisierung.

Die Definition dieser Werte erhöht das Potenzial für exakte Übereinstimmungen, wodurch die Notwendigkeit einer manuellen Zuordnung von Produktlisten zu einem späteren Zeitpunkt minimiert wird. Durch das Hinzufügen der Attribute im Rahmen Ihrer Onboarding-Aufgaben [pre-setup ](./amazon-pre-setup-tasks.md) bietet der Amazon-Vertriebskanal ein höheres Potenzial für die automatische Abstimmung Ihrer Produkte beim Onboarding und die Synchronisierung von Produktdaten zwischen Amazon und [!DNL Commerce] nach dem Onboarding.

Wenn Sie nur das Amazon-ASIN-Attribut erstellen (ohne ASIN-Werte pro Produkt hinzuzufügen), stimmen Ihre [!DNL Commerce]-Produkte möglicherweise nicht automatisch mit Ihren Amazon-Auflistungen überein. Sie können Ihre Produkte manuell über _Store Review_ zuordnen. Beim manuellen Abgleich werden jedoch nicht die Datenelemente erstellt, die zum Freigeben und Synchronisieren Ihrer Produktdaten erforderlich sind.

>[!IMPORTANT]
>
>Wenn Sie ein ASIN-, UPC- oder anderes Datenelement für ein manuell übereinstimmendes Produkt aktualisieren, müssen Sie die Daten an beiden Stellen aktualisieren: den Katalog [!DNL Commerce] und die Auflistung in Ihrem [!DNL Amazon Seller Central] -Konto.

## Amazon ASIN-Produktattribut erstellen

1. Melden Sie sich bei Ihrem [!DNL Commerce] Admin an.

1. Klicken Sie im Menü links auf **[!UICONTROL Stores]** .

1. Klicken Sie im Abschnitt _[!UICONTROL Attributes]_auf **[!UICONTROL Product]**.

1. Um die Attributeigenschaften zu öffnen, klicken Sie auf **[!UICONTROL Add New Attribute]**.

1. Geben Sie für **[!UICONTROL Default Label]** `Amazon ASIN` (den Namen für Ihr Attribut) ein.

1. Wählen Sie für **[!UICONTROL Catalog Input Type for Store Owner]** `Text Field` aus.

1. Wählen Sie für **[!UICONTROL Values Required]** `No` aus.

   Obwohl ein Amazon-ASIN erforderlich ist, um ein Produkt in Amazon aufzulisten, werden einige Ihrer Katalogprodukte möglicherweise nicht in Amazon aufgeführt.

1. Erweitern Sie den Abschnitt _[!UICONTROL Advanced Attribute Properties]_und legen Sie die Optionen fest:

   - Geben Sie für **[!UICONTROL Attribute Code]** `amazon_asin` ein.

   - Wählen Sie für **[!UICONTROL Scope]** `Global` aus.

   - Wählen Sie für **[!UICONTROL Unique Value]** `No` aus.

   - Wählen Sie für **[!UICONTROL Input Validation for Store Owner]** `None` aus.

   - Wählen Sie für **[!UICONTROL Add to Column Options]** `Yes` aus.

   - Wählen Sie für **[!UICONTROL Use in Filter Options]** `Yes` aus.

1. Klicken Sie auf **[!UICONTROL Save Attribute]**.

![Amazon ASIN-Attribut](assets/creating-asin-attribute.png)

## Erstellen des Amazon-Bedingungs-Produktattributs

1. Melden Sie sich bei Ihrem [!DNL Commerce] Admin an.

1. Klicken Sie im Menü links auf **[!UICONTROL Stores]** .

1. Klicken Sie im Abschnitt _[!UICONTROL Attributes]_auf **[!UICONTROL Product]**.

1. Um die Attributeigenschaften zu öffnen, klicken Sie auf **[!UICONTROL Add New Attribute]**.

1. Geben Sie für **[!UICONTROL Default Label]** `Amazon Condition` (den Namen für Ihr Attribut) ein.

1. Wählen Sie für **[!UICONTROL Catalog Input Type for Store Owner]** `Dropdown` aus.

   Der Abschnitt _[!UICONTROL Manage Options (Values of your Attribute)]_wird angezeigt.

1. Wählen Sie für **[!UICONTROL Values Required]** `No` aus.

1. Fügen Sie für **[!UICONTROL Manage Options (Values for your Attribute)]** alle Bedingungsoptionen hinzu.

   Zu den standardmäßigen Amazon-Bedingungen gehören:

   - `New: Refurbished: Used`
   - `Like New: Used`
   - `Very Good: Used`
   - `Good: Used`
   - `Acceptable: Collectible`
   - `Like New; Collectible`
   - `Very Good: Collectible`
   - `Good: Collectible; Acceptable`

1. Klicken Sie auf **[!UICONTROL Add Option]**.

1. Wählen Sie die Option **[!UICONTROL Is Default]** für die Bedingung aus, die als Standardauswahl verwendet werden soll.

1. Geben Sie in der Spalte _[!UICONTROL Admin]_den Text für die Bezeichnung der hinzugefügten Bedingung ein (z. B. `New`, `Used` und `Used-Like New`).

1. Klicken Sie auf **[!UICONTROL Add Option]** , um nach Bedarf weitere Optionen hinzuzufügen.

1. Erweitern Sie den Abschnitt _[!UICONTROL Advanced Attribute Properties]_und legen Sie die Optionen fest.

   - Geben Sie für **[!UICONTROL Attribute Code]** `amazon_condition` ein.

   - Wählen Sie für **[!UICONTROL Scope]** `Global` aus.

   - Wählen Sie für **[!UICONTROL Unique Value]** `No` aus.

   - Wählen Sie für **[!UICONTROL Input Validation for Store Owner]** `None` aus.

   - Wählen Sie für **[!UICONTROL Add to Column Options]** `Yes` aus.

   - Wählen Sie für **[!UICONTROL Use in Filter Options]** `Yes` aus.

1. Klicken Sie auf **[!UICONTROL Save Attribute]**.

![Amazon-Bedingungsattribut](assets/creating-amazon-condition-attribute.png)

![Nächstes ](assets/btn-next.png) [**Symbol Hinzufügen oder Überprüfen des API-Schlüssels**](./amazon-verify-api-key.md)
