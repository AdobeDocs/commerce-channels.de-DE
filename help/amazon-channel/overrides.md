---
title: Überschreibungen
description: Amazon Sales Channel bietet die Registerkarte Überschreibungen , mit der Sie erkennen und verwalten können, wie Sie Überschreibungen in Ihren Amazon-Auflistungen anwenden.
exl-id: e31bbbf9-b20d-42fd-a419-93d596e40be2
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 0%

---

# Überschreibungen

Die _[!UICONTROL Overrides]_zeigt Ihre Amazon-Listen an, auf die Sie eine Überschreibung angewendet haben. Eine Überschreibung ist eine auflistungsspezifische Einstellung, die verwendet werden kann, um einen definierten Wert auf eine Auflistung festzulegen. Eine auf eine Auflistung angewendete Überschreibung definiert die Einstellung für die Auflistung, unabhängig von anderen definierten Einstellungen für die Auflistung oder Regeln, für die die Auflistung zugelassen ist. Wenn eine Überschreibung auf eine Auflistung angewendet wird, wird die Liste im_[!UICONTROL Overrides]_ Registerkarte. Der in der Überschreibung definierte Wert wird in der entsprechenden Spalte für die Auflistung angezeigt. Es gibt vier Arten von Außerkraftsetzungen, die angewendet werden können: Preis, Bearbeitungszeit, Bedingung und Verkaufshinweise.

## Arten von Außerkraftsetzungen

| Typ | Beschreibung |
|---|---|
| Preis | Eine Überschreibung, die den Preis der Auflistung festlegt und alle anderen Preiseinstellungen für die Auflistung ignoriert. <br><br>**Beispiel**: Sie haben eine Preisregel von 20 % definiert, die für alle Produkte in einer bestimmten Kategorie Ihres Katalogs gilt. Sie haben ein Produkt, das neu auf dem Markt ist und die Nachfrage hoch ist, sodass Sie nicht möchten, dass der ermäßigte Preis auf die Auflistung angewendet wird, auch wenn das Produkt in dieser Kategorie enthalten ist. Sie können die Liste auswählen, [Preisüberschreibungen erstellen](./creating-editing-overrides.md#edit-override-single-listing)und legen Sie den Börsenkurs in einer Preisüberschreibung fest. |
| Verarbeitungszeit | Eine Überschreibung, die die Verarbeitungszeit für eine Auflistung festlegt und dabei die standardmäßige Bearbeitungszeit ignoriert, die in den Listeneinstellungen festgelegt wurde.<br><br>**Beispiel**: Ihre standardmäßige Bearbeitungszeit für Ihre Listen ist auf 2 Tage eingestellt. Sie haben ein Produkt, das zerbrechlich ist und einen zusätzlichen Tag benötigt, um seine spezielle Verpackung für den Versand sicherzustellen. Sie können die Liste anzeigen, [Erstellen einer Zeitüberschreitung für die Verarbeitung](./creating-editing-overrides.md#edit-override-single-listing)und legen Sie die Bearbeitungszeit auf drei Tage fest.<br><br>**Hinweis:** Nicht verfügbar für Produkte, die auf `Fulfilled by Amazon`. |
| Bedingung | Eine Überschreibung, die den Bedingungswert einer Auflistung festlegt, unabhängig vom Bedingungsattribut, das der Auflistung zugewiesen ist.<br><br>**Beispiel**: Die meisten Produkte in Ihrem Katalog sind neue Bedingungen, aber Sie haben ein Produkt, das sich in einem Zustand befindet, in dem es renoviert wurde. Sie können die Liste anzeigen, [Bedingungsüberschreibungen erstellen](./creating-editing-overrides.md#edit-override-single-listing)und definieren Sie die Bedingung Neu erstellt für die Auflistung.<br><br>**Hinweis:** Nicht verfügbar für Produkte, die auf `Fulfilled by Amazon`. |
| Verkaufshinweise | Eine Überschreibung, die die _Verkaufshinweise_ -Abschnitt der Auflistung. Dieses Feld kann verwendet werden, um zusätzliche Informationen zum Produkt oder zur angewendeten Überschreibung hinzuzufügen, die normalerweise zur Beschreibung der Bedingung für &quot;nicht neue&quot;Produkte verwendet werden. Text in diesem Feld wird mit der Liste für den Käufer angezeigt. Für eine Liste mit dem Bedingungswert `New`. <br><br>**Beispiel**: Sie haben ein Produkt, das `Refurbished` Bedingung. Normalerweise enthalten Produkte in dieser Bedingung keine Handbücher oder Dokumente, aber Sie haben einen anderen Anbieter für dieses Produkt, der ein Handbuch enthält. Sie können die Liste anzeigen, [eine Außerkraftsetzung von Verkaufshinweisen erstellen](./creating-editing-overrides.md#edit-override-single-listing)und fügen Sie Ihre Textanmerkung hinzu, die für diese Auflistung des Handbuchs eindeutig ist, damit der Käufer weiß, dass sie enthalten ist.<br><br>**Hinweis**: Wenn ein Produkt eine definierte Bedingung von `New`können Sie eine Überschreibung der Verkaufsnotizen eingeben, Amazon zeigt jedoch keine Verkaufsnotizen für eine `New` Produkt. |

Sie können eine Überschreibung für eine [Einzelliste](./creating-editing-overrides.md#edit-override-single-listing). Im _[!UICONTROL Inactive]_,_[!UICONTROL Active]_ und _[!UICONTROL Ineligible]_Registerkarten, können Sie auf **[!UICONTROL Select]**im_[!UICONTROL Action]_ und wählen Sie **[!UICONTROL Create Override]**. Die _[!UICONTROL Edit Overrides]_-Aktion ist nur verfügbar, wenn auf eine Liste eine Überschreibung angewendet wurde und sie auf der_[!UICONTROL Overrides]_ Registerkarte.

Sie können auch eine Überschreibung erstellen, bearbeiten oder entfernen, um [mehrere Listen](./creating-editing-overrides.md#edit-override-multiple-listings). Im _[!UICONTROL Inactive]_,_[!UICONTROL Active]_ und _[!UICONTROL Ineligible]_Registerkarten, können Sie auf **[!UICONTROL Select]**im_[!UICONTROL Action]_ und wählen Sie **[!UICONTROL Edit Listing Overrides]**.

Wenn Sie eine Überschreibung entfernen, wird die Auflistung angewiesen, die in Ihren Listeneinstellungen und Regeln definierten Werte zu verwenden.

Bei der Definition einer Überschreibung können Sie auch einen einzelnen Überschreibungstyp oder eine beliebige Kombination dieser Typen eingeben.

Siehe [Erstellen und Bearbeiten von Überschreibungen](./creating-editing-overrides.md).

>[!NOTE]
>
>Wenn Listen in Bearbeitung sind, wird die Anzahl der Auflistungen in einer Meldung über den Registerkarten angezeigt.

![Registerkarte &quot;Außerkraftsetzungen&quot;](assets/amazon-overrides.png)

Die Startseiten der Amazon-Vertriebskanäle teilen sich einige gemeinsame [Arbeitsbereichssteuerelemente](./workspace-controls.md) die es Ihnen ermöglichen, die angezeigten Daten anzupassen.

## Standardspalten

| Spalte | Beschreibung |
|---|---|
| [!UICONTROL Amazon Seller SKU] | Die SKU (Stock Keeping Unit, Bestandseinheit), die von Amazon einem Produkt zugewiesen wurde, um das Produkt, die Optionen, den Preis und den Hersteller zu identifizieren. |
| [!UICONTROL ASIN] | Ein eindeutiger Block von 10 Buchstaben und/oder Zahlen zur Identifizierung von Elementen.<br><br>ASIN steht für die Amazon Standard-Identifikationsnummern. Ein ASIN ist ein eindeutiger Block von 10 Buchstaben und/oder Zahlen, der Elemente identifiziert. Bei Büchern entspricht das ASIN der ISBN-Nummer, bei allen anderen Produkten wird jedoch beim Hochladen des Artikels in den Katalog ein neues ASIN erstellt. Sie finden einen Artikel-ASIN auf der Produktdetailseite in Amazon sowie weitere Details zum Artikel. |
| [!UICONTROL Condition Override] | Die neue Bedingung, die in der Überschreibung definiert wird. Wenn die auf die Auflistung angewendete Überschreibung keine Bedingungsüberschreibungen ist, `Not Selected` in dieser Spalte angezeigt. |
| [!UICONTROL Product Listing Name] | Der Name des Produkts. |
| [!UICONTROL Seller Notes Override] | Die neuen, in der Überschreibung definierten Verkaufshinweise. Wenn die auf die Auflistung angewendete Überschreibung nicht dieser Überschreibungstyp ist, ist diese Spalte leer. |
| [!UICONTROL Handling Override] | Die neue im Außerkraftsetzen definierte Bearbeitungszeit (in Tagen). Wenn die auf die Auflistung angewendete Überschreibung keine Überschreibungszeit ist, ist diese Spalte leer. |
| [!UICONTROL List Price Override] | Der neue, in der Überschreibung definierte Börsenkurs. Wenn die auf die Auflistung angewendete Außerkraftsetzung kein Preisüberschuss ist, `N/A` in dieser Spalte angezeigt. |
| [!UICONTROL Action] | Liste der verfügbaren Aktionen, die auf eine bestimmte Liste angewendet werden können. So wenden Sie eine Aktion an: im _[!UICONTROL Action]_Spalte, klicken Sie auf **[!UICONTROL Select]**und wählen Sie eine Option:<ul><li>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md#edit-override-single-listing)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
