---
title: Überschreibungen
description: Amazon Sales Channel enthält die Registerkarte Überschreibungen, mit der Sie erkennen und verwalten können, wie Sie Überschreibungen in Ihren Amazon-Listen anwenden.
exl-id: e31bbbf9-b20d-42fd-a419-93d596e40be2
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 0%

---

# Überschreibungen

Die _[!UICONTROL Overrides]_zeigt Ihre Amazon-Einträge an, auf die Sie eine Außerkraftsetzung angewendet haben. Bei einer Außerkraftsetzung handelt es sich um eine listenspezifische Einstellung, mit der ein definierter Wert auf eine Auflistung gesetzt werden kann. Eine auf eine Auflistung angewendete Außerkraftsetzung definiert die Einstellung für die Auflistung, unabhängig von anderen definierten Listeneinstellungen oder Regeln, für die die Auflistung zugelassen ist. Wenn eine Außerkraftsetzung auf eine Auflistung angewendet wird, wird die Liste im_[!UICONTROL Overrides]_ Tabulator. Der in der Überschreibung definierte Wert wird in der entsprechenden Spalte für die Auflistung angezeigt. Es gibt vier Arten von Überschreibungen, die angewendet werden können: Preis, Bearbeitungszeit, Bedingungen und Hinweise zum Verkäufer.

## Überschreibungen

| Typ | Beschreibung |
|---|---|
| Preis | Eine Außerkraftsetzung, die den Preis der Auflistung festlegt und dabei alle anderen Preiseinstellungen für die Auflistung ignoriert. <br><br>**Beispiel**: Sie haben eine Preisregel von 20 % festgelegt, die für alle Produkte in einer bestimmten Kategorie Ihres Katalogs gilt. Sie haben ein neues Produkt, das neu auf den Markt kommt und eine hohe Nachfrage aufweist. Daher wollen Sie nicht, dass der ermäßigte Preis auf die Auflistung angewendet wird, obwohl das Produkt in dieser Kategorie ist. Sie können die Liste auswählen. [Preisüberschreibung erstellen](./creating-editing-overrides.md#edit-override-single-listing), und legen Sie den Börsenkurs in einer Preisabweichung fest. |
| Bearbeitungszeit | Eine Außerkraftsetzung, die die Bearbeitungszeit für eine Auflistung festlegt und dabei die Standardeinstellung für die Bearbeitungszeit in den Listeneinstellungen ignoriert.<br><br>**Beispiel**: Ihre standardmäßige Bearbeitungszeit für Ihre Auflistungen ist auf 2 Tage eingestellt. Sie haben ein Produkt, das zerbrechlich ist und einen zusätzlichen Tag benötigt, um seine spezielle Verpackung für den Versand sicherzustellen. Sie können die Liste Ansicht haben, [Zeitüberschreibung für die Bearbeitung erstellen](./creating-editing-overrides.md#edit-override-single-listing)und legen die Bearbeitungszeit auf drei Tage fest.<br><br>**Hinweis:** Nicht verfügbar für Produkte, festgelegt auf `Fulfilled by Amazon`. |
| Bedingung | Eine Außerkraftsetzung, die den Bedingungswert einer Auflistung festlegt, unabhängig vom Bedingungsattribut, das der Auflistung zugewiesen ist.<br><br>**Beispiel**: Die meisten Produkte in Ihrem Katalog sind neu, aber Sie haben ein Produkt, das in einem renovierten Zustand ist. Sie können die Liste Ansicht haben, [Bedingungsüberschreibungen erstellen](./creating-editing-overrides.md#edit-override-single-listing), und definieren Sie die erneuerte Bedingung für die Auflistung.<br><br>**Hinweis:** Nicht verfügbar für Produkte, festgelegt auf `Fulfilled by Amazon`. |
| Hinweise für Verkäufer | Eine Außerkraftsetzung, die die _Hinweise für Verkäufer_ Abschnitt der Auflistung. Dieses Feld kann verwendet werden, um zusätzliche Informationen zu dem Produkt oder der angewendeten Außerkraftsetzung hinzuzufügen, die normalerweise zur Beschreibung der Bedingung &quot;nicht neue&quot; Produkte verwendet werden. Text in diesem Feld wird mit der Liste für den Käufer angezeigt. Für eine Auflistung mit einem Bedingungswert von `New`. <br><br>**Beispiel**: Sie haben ein Produkt, in dem `Refurbished` Bedingung. Normalerweise enthalten die Produkte in diesem Zustand keine Handbücher oder Dokumente, aber Sie haben einen anderen Anbieter für dieses Produkt, das eine Anleitung enthält. Sie können die Liste Ansicht haben, [Überschreibung von Verkäufernotizen erstellen](./creating-editing-overrides.md#edit-override-single-listing), und fügen Sie Ihren Text Notiz, dass ist einzigartig in dieser Auflistung über das Handbuch, sodass der Käufer weiß, dass es enthalten ist.<br><br>**Hinweis**: Wenn ein Produkt eine bestimmte Bedingung hat von `New`, können Sie eine Überschreibung der Verkaufsnotizen eingeben, aber Amazon zeigt keine Verkaufsnotizen für ein `New` Produkt. |

Sie können eine Außerkraftsetzung für ein [einzelne Auflistung](./creating-editing-overrides.md#edit-override-single-listing). Auf _[!UICONTROL Inactive]_,_[!UICONTROL Active]_ und _[!UICONTROL Ineligible]_Registerkarten, können Sie **[!UICONTROL Select]**in_[!UICONTROL Action]_ Spalte und wählen Sie **[!UICONTROL Create Override]**. Die _[!UICONTROL Edit Overrides]_Aktion ist nur verfügbar, wenn auf eine Auflistung eine Außerkraftsetzung angewendet wurde und sie auf der_[!UICONTROL Overrides]_ Tabulator.

Sie können auch eine Überschreibung erstellen, bearbeiten oder entfernen, um [mehrere Auflistungen](./creating-editing-overrides.md#edit-override-multiple-listings). Auf _[!UICONTROL Inactive]_,_[!UICONTROL Active]_ und _[!UICONTROL Ineligible]_Registerkarten, können Sie **[!UICONTROL Select]**in_[!UICONTROL Action]_ Spalte und wählen Sie **[!UICONTROL Edit Listing Overrides]**.

Durch das Entfernen einer Außerkraftsetzung wird der Auflistung mitgeteilt, dass sie die Werte verwendet, die in den Listeneinstellungen und -regeln definiert sind.

Wenn Sie eine Außerkraftsetzung definieren, können Sie auch einen einzelnen Überschreibungstyp oder eine beliebige Kombination dieser Typen eingeben.

Siehe [Überschreibungen erstellen und bearbeiten](./creating-editing-overrides.md).

>[!NOTE]
>
>Wenn Sie Listen in Bearbeitung haben, wird die Anzahl der Einträge in einer Meldung über den Registerkarten angezeigt.

![Überschreibt Registerkarte](assets/amazon-overrides.png)

Amazon Sales Kanal Startseite teilen einige gemeinsame [Arbeitsbereichssteuerelemente](./workspace-controls.md) , mit denen Sie die angezeigten Daten anpassen können.

## Standardspalten

| Spalte | Beschreibung |
|---|---|
| [!UICONTROL Amazon Seller SKU] | Die von Amazon einem Produkt zugewiesene SKU (Stock Keeping Unit) zur Identifizierung des Produkts, der Optionen, des Preises und des Herstellers. |
| [!UICONTROL ASIN] | Ein eindeutiger Block mit 10 Buchstaben und/oder Zahlen, die Elemente identifizieren.<br><br>ASIN steht für die Amazon Standard Identification Numbers. Ein ASIN ist ein eindeutiger Block mit 10 Buchstaben und/oder Ziffern, der Elemente identifiziert. Für Bücher ist die ASIN die gleiche ISBN-Nummer, aber für alle anderen Produkte wird ein neues ASIN erstellt, wenn das Element in ihren Katalog hochgeladen wird. Auf der Produktdetailseite auf Amazon finden Sie ASIN und weitere Details zum Artikel. |
| [!UICONTROL Condition Override] | Die neue Bedingung, die in der Überschreibung definiert ist. Wenn die auf die Auflistung angewendete Außerkraftsetzung keine Bedingungsüberschreibungen ist, `Not Selected` wird in dieser Spalte angezeigt. |
| [!UICONTROL Product Listing Name] | Der Name des Produkts. |
| [!UICONTROL Seller Notes Override] | Die neuen Verkaufshinweise, die in der Überschreibung definiert sind. Wenn die auf die Auflistung angewendete Außerkraftsetzung nicht dieser Überschreibungstyp ist, ist diese Spalte leer. |
| [!UICONTROL Handling Override] | Die neue Bearbeitungszeit, die in der Außerkraftsetzung definiert ist (in Tagen). Wenn die auf die Auflistung angewendete Außerkraftsetzung keine Überschreibungsdauer ist, ist diese Spalte leer. |
| [!UICONTROL List Price Override] | Der neue Börsenkurs, der in der Außerkraftsetzung definiert ist. Wenn die auf die Auflistung angewendete Außerkraftsetzung keine Preisabweichung ist, `N/A` wird in dieser Spalte angezeigt. |
| [!UICONTROL Action] | Liste der verfügbaren Aktionen, die auf eine bestimmte Auflistung angewendet werden können. So wenden Sie eine Aktion an im _[!UICONTROL Action]_Spalte, klicken **[!UICONTROL Select]**und wählen Sie eine Option:<ul><li>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md#edit-override-single-listing)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
