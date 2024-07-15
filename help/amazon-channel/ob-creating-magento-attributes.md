---
title: Erstellen von Commerce-Attributen für Amazon
description: Bevor Sie das Onboarding des Amazon-Verkaufskanals abschließen, stellen Sie sicher, dass Sie über die erforderlichen [!UICONTROL Commerce] -Produktattribute verfügen.
role: Admin
feature: Sales Channels, Products, Configuration
exl-id: eebad794-c171-40a3-aa24-d5509e2b5797
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Erstellen von Commerce-Attributen für Amazon

Bevor Sie Ihre [!DNL Amazon Seller Central] -Konten integrieren, sollten Sie am besten [!DNL Commerce] [Produktattribute](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) hinzufügen, um Ihre Produktlisten zuzuordnen. Nachdem Sie das Onboarding abgeschlossen haben, können Sie Ihre Produktattribute auf der Registerkarte [Attribute](./managing-attributes.md) der Startseite des Amazon-Verkaufskanals ](./amazon-sales-channel-home.md) verwalten.[

In diesen Anweisungen wird beschrieben, wie Sie [!DNL Commerce] -Attribute für Amazon ASIN- und Amazon-Bedingungen erstellen. Es wird empfohlen, zusätzliche Attribute wie Amazon EAN, Amazon ISBN und Amazon UPC zu erstellen. Sie können auch ein Amazon-Preisattribut erstellen, wenn Sie Ihren Amazon-Listingpreis als Preisquelle für Preisregeln verwenden möchten. Diese Attribute werden bei der Konfiguration Ihrer Listen- und Preiseinstellungen beim Onboarding verwendet. Verwenden Sie diese Attribute auch beim Erstellen von Amazon-Listen und beim Aktualisieren und Synchronisieren Ihres [!DNL Commerce]-Katalogs mit Ihren Amazon-Listen.

Mit den Einstellungen für die Katalogsuche können Sie übereinstimmende Suchparameter festlegen, mit denen Sie geeignete [!DNL Commerce] -Produkte Amazon-Auflistungen zuordnen können. Sofern zugeordnet, aktiviert Amazon Aktionen im Zusammenhang mit Preisen, Menge, Außerkraftsetzungen sowie der Bestell- und Produktsynchronisierung.

Die Definition dieser Werte erhöht das Potenzial für exakte Übereinstimmungen, wodurch die Notwendigkeit einer manuellen Zuordnung von Produktlisten zu einem späteren Zeitpunkt minimiert wird. Durch das Hinzufügen der Attribute im Rahmen Ihrer Onboarding-Aufgaben [vor der Einrichtung](./amazon-pre-setup-tasks.md) bietet der Amazon-Vertriebskanal ein höheres Potenzial, Ihre Produkte beim Onboarding automatisch abzugleichen und die Produktdaten zwischen Amazon und [!DNL Commerce] nach dem Onboarding zu synchronisieren.

Wenn Sie nur das Amazon-ASIN-Attribut erstellen (ohne ASIN-Werte pro Produkt hinzuzufügen), stimmen Ihre [!DNL Commerce] -Produkte möglicherweise nicht automatisch mit Ihren Amazon-Auflistungen überein. Sie können Ihre Produkte manuell über _Store Review_ zuordnen. Beim manuellen Abgleich werden jedoch nicht die Datenelemente erstellt, die zum Freigeben und Synchronisieren Ihrer Produktdaten erforderlich sind.

>[!IMPORTANT]
>
>Wenn Sie ein ASIN-, UPC- oder anderes Datenelement für ein manuell übereinstimmendes Produkt aktualisieren, müssen Sie die Daten an beiden Stellen aktualisieren: in Ihrem [!DNL Commerce]-Katalog und in der Liste in Ihrem [!DNL Amazon Seller Central]-Konto.

## Amazon ASIN-Produktattribut erstellen

1. Melden Sie sich bei Ihrem [!DNL Commerce] -Administrator an.

1. Klicken Sie im Menü links auf **[!UICONTROL Stores]** .

1. Klicken Sie im Abschnitt _[!UICONTROL Attributes]_auf **[!UICONTROL Product]**.

1. Um die Attributeigenschaften zu öffnen, klicken Sie auf **[!UICONTROL Add New Attribute]**.

1. Geben Sie für **[!UICONTROL Default Label]** `Amazon ASIN` ein (den Namen für Ihr Attribut).

1. Wählen Sie für **[!UICONTROL Catalog Input Type for Store Owner]** `Text Field` aus.

1. Wählen Sie für **[!UICONTROL Values Required]** `No` aus.

   Obwohl ein Amazon-ASIN erforderlich ist, um ein Produkt in Amazon aufzulisten, werden einige Ihrer Katalogprodukte möglicherweise nicht in Amazon aufgeführt.

1. Erweitern Sie den Abschnitt _[!UICONTROL Advanced Attribute Properties]_und legen Sie die Optionen fest:

   - Geben Sie für **[!UICONTROL Attribute Code]** den Wert `amazon_asin` ein.

   - Wählen Sie für **[!UICONTROL Scope]** `Global` aus.

   - Wählen Sie für **[!UICONTROL Unique Value]** `No` aus.

   - Wählen Sie für **[!UICONTROL Input Validation for Store Owner]** `None` aus.

   - Wählen Sie für **[!UICONTROL Add to Column Options]** `Yes` aus.

   - Wählen Sie für **[!UICONTROL Use in Filter Options]** `Yes` aus.

1. Klicken Sie auf **[!UICONTROL Save Attribute]**.

![Amazon ASIN-Attribut](assets/creating-asin-attribute.png){width="600" zoomable="yes"}

## Erstellen des Amazon-Bedingungs-Produktattributs

1. Melden Sie sich bei Ihrem [!DNL Commerce] -Administrator an.

1. Klicken Sie im Menü links auf **[!UICONTROL Stores]** .

1. Klicken Sie im Abschnitt _[!UICONTROL Attributes]_auf **[!UICONTROL Product]**.

1. Um die Attributeigenschaften zu öffnen, klicken Sie auf **[!UICONTROL Add New Attribute]**.

1. Geben Sie für **[!UICONTROL Default Label]** `Amazon Condition` ein (den Namen für Ihr Attribut).

1. Wählen Sie für **[!UICONTROL Catalog Input Type for Store Owner]** `Dropdown` aus.

   Der Abschnitt _[!UICONTROL Manage Options (Values of your Attribute)]_wird angezeigt.

1. Wählen Sie für **[!UICONTROL Values Required]** `No` aus.

1. Fügen Sie für &quot;**[!UICONTROL Manage Options (Values for your Attribute)]**&quot;die einzelnen Bedingungsoptionen hinzu.

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

1. Wählen Sie die Option **[!UICONTROL Is Default]** für die Bedingung aus, die die Standardauswahl sein soll.

1. Geben Sie in der Spalte _[!UICONTROL Admin]_den Text für den Titel der hinzuzufügenden Bedingung ein (z. B. `New`, `Used` und `Used-Like New`)

1. Klicken Sie auf **[!UICONTROL Add Option]** , um nach Bedarf weitere Optionen hinzuzufügen.

1. Erweitern Sie den Abschnitt _[!UICONTROL Advanced Attribute Properties]_und legen Sie die Optionen fest.

   - Geben Sie für **[!UICONTROL Attribute Code]** den Wert `amazon_condition` ein.

   - Wählen Sie für **[!UICONTROL Scope]** `Global` aus.

   - Wählen Sie für **[!UICONTROL Unique Value]** `No` aus.

   - Wählen Sie für **[!UICONTROL Input Validation for Store Owner]** `None` aus.

   - Wählen Sie für **[!UICONTROL Add to Column Options]** `Yes` aus.

   - Wählen Sie für **[!UICONTROL Use in Filter Options]** `Yes` aus.

1. Klicken Sie auf **[!UICONTROL Save Attribute]**.

![Amazon-Bedingungsattribut](assets/creating-amazon-condition-attribute.png){width="600" zoomable="yes"}

![Nächstes Symbol](assets/btn-next.png) [**Hinzufügen oder Überprüfen des API-Schlüssels fortsetzen**](./amazon-verify-api-key.md)
