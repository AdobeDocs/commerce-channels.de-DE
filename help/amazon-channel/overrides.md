---
title: Amazon-Verkaufskanal - [!UICONTROL Overrides]
description: Amazon Sales Channel bietet die Registerkarte Überschreibungen , mit der Sie erkennen und verwalten können, wie Sie Überschreibungen in Ihren Amazon-Auflistungen anwenden.
feature: Sales Channels, Price Rules
exl-id: e31bbbf9-b20d-42fd-a419-93d596e40be2
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# [!UICONTROL Overrides]

Auf der Registerkarte _[!UICONTROL Overrides]_werden Ihre Amazon-Listen angezeigt, für die Sie eine Überschreibung vorgenommen haben. Eine Überschreibung ist eine auflistungsspezifische Einstellung, die verwendet werden kann, um einen definierten Wert auf eine Auflistung festzulegen. Eine auf eine Auflistung angewendete Überschreibung definiert die Einstellung für die Auflistung, unabhängig von anderen definierten Einstellungen für die Auflistung oder Regeln, für die die Auflistung zugelassen ist. Wenn eine Überschreibung auf eine Auflistung angewendet wird, wird die Liste auf der Registerkarte_[!UICONTROL Overrides]_ angezeigt. Der in der Überschreibung definierte Wert wird in der entsprechenden Spalte für die Auflistung angezeigt. Es gibt vier Arten von Außerkraftsetzungen, die angewendet werden können: Preis, Bearbeitungszeit, Bedingung und Verkaufshinweise.

## Arten von Außerkraftsetzungen

| Typ | Beschreibung |
|---------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Preis | Eine Überschreibung, die den Preis der Auflistung festlegt und alle anderen Preiseinstellungen für die Auflistung ignoriert. <br><br>**Beispiel**: Sie haben eine 20-%-Rabattpreisregel definiert, die für alle Produkte in einer bestimmten Kategorie Ihres Katalogs gilt. Sie haben ein Produkt, das neu auf dem Markt ist und die Nachfrage hoch ist, sodass Sie nicht möchten, dass der ermäßigte Preis auf die Auflistung angewendet wird, auch wenn das Produkt in dieser Kategorie enthalten ist. Sie können die Liste auswählen, [eine Preisüberschreibung erstellen](./creating-editing-overrides.md#edit-override-single-listing) und den Listenpreis in einer Preisüberschreibung definieren. |
| Verarbeitungszeit | Eine Überschreibung, die die Verarbeitungszeit für eine Auflistung festlegt und dabei die standardmäßige Bearbeitungszeit ignoriert, die in den Listeneinstellungen festgelegt wurde.<br><br>**Beispiel**: Ihre standardmäßige Bearbeitungszeit für Ihre Listen ist auf 2 Tage eingestellt. Sie haben ein Produkt, das zerbrechlich ist und einen zusätzlichen Tag benötigt, um seine spezielle Verpackung für den Versand sicherzustellen. Sie können die Auflistung anzeigen, [eine Überschreibungszeit für die Handhabung erstellen](./creating-editing-overrides.md#edit-override-single-listing) und die Bearbeitungszeit auf drei Tage festlegen.<br><br>**Hinweis:** Nicht verfügbar für Produkte mit dem Wert `Fulfilled by Amazon`. |
| Bedingung | Eine Überschreibung, die den Bedingungswert einer Auflistung festlegt, unabhängig vom Bedingungsattribut, das der Auflistung zugewiesen ist.<br><br>**Beispiel**: Die meisten Produkte in Ihrem Katalog sind eine neue Bedingung, aber Sie haben ein Produkt, das sich in der Bedingung &quot;Aktualisiert&quot;befindet. Sie können die Liste anzeigen, [eine Bedingungsüberschreibung erstellen](./creating-editing-overrides.md#edit-override-single-listing) und die Bedingung &quot;Neu erstellt&quot;für die Auflistung definieren.<br><br>**Hinweis:** Nicht verfügbar für Produkte mit dem Wert `Fulfilled by Amazon`. |
| Verkaufshinweise | Eine Überschreibung, die den Abschnitt _Verkaufsnotizen_ der Auflistung definiert. Dieses Feld kann verwendet werden, um zusätzliche Informationen zum Produkt oder zur angewendeten Überschreibung hinzuzufügen, die normalerweise zur Beschreibung der Bedingung für &quot;nicht neue&quot;Produkte verwendet werden. Text in diesem Feld wird mit der Liste für den Käufer angezeigt. Für eine Auflistung mit dem Bedingungswert `New` können keine Verkaufshinweise hinzugefügt werden. <br><br>**Beispiel**: Sie haben ein Produkt, das sich in der Bedingung `Refurbished` befindet. Normalerweise enthalten Produkte in dieser Bedingung keine Handbücher oder Dokumente, aber Sie haben einen anderen Anbieter für dieses Produkt, der ein Handbuch enthält. Sie können die Auflistung anzeigen, [eine Außerkraftsetzung der Verkaufsnotizen ](./creating-editing-overrides.md#edit-override-single-listing) erstellen und Ihre Textanmerkung hinzufügen, die für diese Auflistung des Handbuchs eindeutig ist, sodass der Käufer weiß, dass sie enthalten ist.<br><br>**Hinweis**: Wenn ein Produkt eine definierte Bedingung von `New` aufweist, können Sie eine Außerkraftsetzung der Verkaufsnotizen eingeben, Amazon zeigt jedoch keine Verkaufsnotizen für ein `New` -Produkt an. |

Sie können eine Überschreibung für eine [einzelne Auflistung](./creating-editing-overrides.md#edit-override-single-listing) erstellen, bearbeiten oder entfernen. Auf den Registerkarten _[!UICONTROL Inactive]_,_[!UICONTROL Active]_ und _[!UICONTROL Ineligible]_können Sie auf **[!UICONTROL Select]**in der Spalte_[!UICONTROL Action]_ klicken und **[!UICONTROL Create Override]** auswählen. Die Aktion _[!UICONTROL Edit Overrides]_ist nur verfügbar, wenn auf eine Auflistung eine Überschreibung angewendet wurde, und wird auf der Registerkarte_[!UICONTROL Overrides]_ angezeigt.

Sie können auch eine Überschreibung für [mehrere Auflistungen](./creating-editing-overrides.md#edit-override-multiple-listings) erstellen, bearbeiten oder entfernen. Auf den Registerkarten _[!UICONTROL Inactive]_,_[!UICONTROL Active]_ und _[!UICONTROL Ineligible]_können Sie auf **[!UICONTROL Select]**in der Spalte_[!UICONTROL Action]_ klicken und **[!UICONTROL Edit Listing Overrides]** auswählen.

Wenn Sie eine Überschreibung entfernen, wird die Auflistung angewiesen, die in Ihren Listeneinstellungen und Regeln definierten Werte zu verwenden.

Bei der Definition einer Überschreibung können Sie auch einen einzelnen Überschreibungstyp oder eine beliebige Kombination dieser Typen eingeben.

Siehe [Außerkraftsetzungen erstellen und bearbeiten](./creating-editing-overrides.md).

>[!NOTE]
>
>Wenn Listen in Bearbeitung sind, wird die Anzahl der Auflistungen in einer Meldung über den Registerkarten angezeigt.

![Registerkarte &quot;Außerkraftsetzungen&quot;](assets/amazon-overrides.png){width="600" zoomable="yes"}

Die Startseiten der Amazon-Verkaufskanäle teilen einige gängige [Arbeitsbereichssteuerelemente](./workspace-controls.md), mit denen Sie die angezeigten Daten anpassen können.

## Standardspalten

| Spalte | Beschreibung |
|------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Amazon Seller SKU] | Die von Amazon einem Produkt zugewiesene SKU (Stock Keeping Unit, Bestandseinheit) zur Identifizierung von Produkt, Optionen, Preis und Hersteller. |
| [!UICONTROL ASIN] | Ein eindeutiger Block von 10 Buchstaben und/oder Zahlen zur Identifizierung von Elementen.<br><br>ASIN steht für die Amazon Standard-Identifikationsnummern. Ein ASIN ist ein eindeutiger Block von 10 Buchstaben und/oder Zahlen, der Elemente identifiziert. Bei Büchern entspricht das ASIN der ISBN-Nummer, bei allen anderen Produkten wird jedoch beim Hochladen des Artikels in den Katalog ein neues ASIN erstellt. Sie finden einen Artikel-ASIN auf der Produktdetailseite in Amazon sowie weitere Details zum Artikel. |
| [!UICONTROL Condition Override] | Die neue Bedingung, die in der Überschreibung definiert wird. Wenn die auf die Auflistung angewendete Außerkraftsetzung keine Außerkraftsetzung von Bedingungen ist, wird in dieser Spalte `Not Selected` angezeigt. |
| [!UICONTROL Product Listing Name] | Der Name des Produkts. |
| [!UICONTROL Seller Notes Override] | Die neuen Verkaufshinweise, die in der Überschreibung definiert sind. Wenn die auf die Auflistung angewendete Überschreibung nicht dieser Überschreibungstyp ist, ist diese Spalte leer. |
| [!UICONTROL Handling Override] | Die neue im Außerkraftsetzen definierte Bearbeitungszeit (in Tagen). Wenn die auf die Auflistung angewendete Überschreibung keine Überschreibungszeit ist, ist diese Spalte leer. |
| [!UICONTROL List Price Override] | Der neue, in der Überschreibung definierte Börsenkurs. Wenn die auf die Auflistung angewendete Außerkraftsetzung kein Preisüberschuss ist, wird in dieser Spalte `N/A` angezeigt. |
| [!UICONTROL Action] | Liste der verfügbaren Aktionen, die auf eine bestimmte Liste angewendet werden können. Um eine Aktion anzuwenden, klicken Sie in der Spalte _[!UICONTROL Action]_auf **[!UICONTROL Select]**und wählen Sie eine Option aus:<ul><li>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md#edit-override-single-listing)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
