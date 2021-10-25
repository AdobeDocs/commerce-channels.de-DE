---
title: '"Intelligente Preisanpassungsregel: Bedingte Abweichungen des Konkurrenten"'
description: Ermitteln Sie Ihren Amazon-Börsennotierungspreis anhand der Konkurrent-Preise und -Konditionen des Produkts, indem Sie eine intelligente Preiswiederholungsregel erstellen.
exl-id: c52230e3-4e47-45bc-80e0-170530f58987
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# Intelligente Preisanpassungsregel: Bedingte Abweichungen des Konkurrenten

Zu den Abschnitten einer intelligenten Neubewertungsregel gehören:

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [!UICONTROL Competitor Conditional Variances]
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [[!UICONTROL Floor Price]](./floor-price.md)
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

Eine intelligente Neupreisregel verwendet die Preise der Amazon Konkurrent, um Ihren Börsenpreis zu bestimmen. Konkurrent sind andere Verkäufer, die dieselben Produkte auflisten, die Sie auf Amazon auflisten.

Wenn ein Produkt mit derselben Bedingung vorhanden ist, entspricht der Basispreis der Übereinstimmung dem [kleinster Konkurrent](./lowest-competitor-pricing.md) Preis mit derselben Bedingung. Wenn kein Konkurrent-Produkt mit Ihrer Kondition übereinstimmt, durchläuft der Basispreis andere verfügbare Konkurrent, beginnend mit Neu, Renoviert und unter den verfügbaren Bedingungen. Nachdem eine Bedingung gefunden wurde, ist der Basispreis der Übereinstimmung der niedrigste Preis innerhalb dieser Bedingung.

Wenn Sie ein Produkt mit der Bedingung aufgeführt haben `Used; Good` und dem Basispreis der Übereinstimmung, und ein Konkurrent hat das gleiche Produkt in demselben Zustand zu einem niedrigeren Preis, wird der Konkurrent Preis verwendet. Wenn ein Konkurrent nicht mit der gleichen Bedingung vorhanden ist, prüft das System auf einen Konkurrent mit der folgenden Bedingung: `New`. Wird ein Konkurrent mit dieser Bedingung gefunden, wird der niedrigste Preis verwendet.

## Bedingte Varianten für Konkurrent konfigurieren

Definieren Sie die Bedingungsvarianten im _[!UICONTROL Competitor Conditional Variances]_Abschnitt.

für **[!UICONTROL Conditional Variance]**, wählen Sie eine Option aus:

- `Use all competitor's product conditions` - (Standard) Wählen Sie aus, wann Ihr Produkt mit einer beliebigen verfügbaren Bedingung verglichen werden soll (wenn für die aufgeführte Bedingung keine Übereinstimmung vorhanden ist).

- `Use Only Matching Competitor's Product Condition` - Wählen Sie aus, wann Ihr Produkt nur mit den Produkten des Konkurrenten in derselben Bedingung verglichen werden soll. Wenn keine Übereinstimmung vorhanden ist, wird der Preis des Produkts auf der _Magento-Preisquelle_ definiert in [Listingpreis](./listing-price.md).

- `Apply Variance (if competitor's product condition differs)` - Wählen Sie aus, ob Sie zunächst versuchen möchten, den Vergleich mit der entsprechenden Produktbedingung durchzuführen. Wenn keine Übereinstimmungsbedingung vorhanden ist, wird eine Varianz (als Prozentsatz) angewendet, die sich auf Ihre Produktbedingung und die Bedingung des niedrigsten Konkurrenten bezieht.

   Wann _[!UICONTROL Apply Variance]_-Funktion ausgewählt wurde, werden zusätzliche Varianzfelder für jede Ihrer Amazon-Bedingungen angezeigt. Mit dieser Funktion können Sie intelligente Preisanpassungsregeln verwenden, wenn Sie Produkte in einem anderen Zustand als Ihre Konkurrent Angebot haben. Um die Berechnung hinter der bedingten Varianz zu verstehen, müssen Sie zunächst verstehen, dass alle Varianzen von einem Basis-Übereinstimmungspreis bestimmt werden.

   Die angezeigten Bedingungsvariablenoptionen basieren auf Ihren Listeneinstellungen für `Condition` , die Bedingungswerten mit einem [!DNL Commerce] [Produktattribut](https://docs.magento.com/user-guide/catalog/product-attributes.html){Zielgruppe=&quot;_blank&quot;}. Für alle zugeordneten Bedingungen können Sie einen Varianzprozentsatz von 1-100 definieren. Die Ausnahme ist Sammelcharakter; in diesem Fall kann ein Prozentsatz von mehr als 100 angewandt werden.

![Intelligente Preisanpassungsregel - bedingte Varianten des Konkurrenten](assets/amazon-competitor-cond-variances.png)

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Competitor Conditional Variances] | Optionen: <ul><li>**[!UICONTROL Use all competitor's product conditions]** - Wenn für die Bedingung, mit der Sie Ihr Produkt auflisten, keine Übereinstimmung vorhanden ist, stimmt diese Option mit jeder verfügbaren Bedingung überein. Zuerst versucht es, Ihre Bedingung zu erfüllen, und arbeitet dann von der `New` Bedingung für `Used; Acceptable`.</li><li>**[!UICONTROL Use only matching competitor's product condition]** - Diese Option stimmt mit Ihrem Produkt überein. Wenn keine Übereinstimmung besteht, werden die Produktpreise auf der _[!UICONTROL Magento Price Source]_.</li><li>>**[!UICONTROL Apply variance (if competitor's product condition differs)]** - Diese Option versucht zunächst, eine Übereinstimmung mit Ihrer Produktbedingung zu erzielen. Wenn keine Übereinstimmungsbedingung vorhanden ist, wird eine Varianz (als Prozentsatz) in Bezug auf Ihre Produktbedingung und den Zustand des niedrigsten Konkurrenten angewendet.</li></ul><br><br>Die bedingten Variablenoptionen, die basierend auf Ihren Listeneinstellungen für Bedingung angezeigt werden und den Bedingungswerten mithilfe eines [!DNL Commerce] [Produktattribut](https://docs.magento.com/user-guide/catalog/product-attributes.html){Zielgruppe=&quot;_blank&quot;}. Für alle zugeordneten Bedingungen können Sie einen Varianzprozentsatz von 1-100 angeben. Die Ausnahme ist Sammelcharakter; in diesem Fall kann ein Prozentsatz von mehr als 100 angewandt werden.<br><br>Mit dieser Funktion können Sie intelligente Preisanpassungsregeln verwenden, wenn Sie Produkte in einem anderen Zustand als Ihre Konkurrent Angebot haben. Um die Berechnung hinter der bedingten Varianz zu verstehen, müssen Sie zunächst verstehen, dass alle Varianzen von einem Basis-Übereinstimmungspreis bestimmt werden. |

## Bedingte Varianz berechnen

- Base Match Condition Variance (BMC) = Die Varianz für den Zustand Ihres Basis-Match-Preis-Konkurrenten. Im vorangegangenen Beispiel ist BMC die Varianz für die `New` Bedingung.
- Merchant Condition Variance (MCV) = Die Varianz für den Zustand Ihres Produkts. MCV = Variation für die `Used; Good` Bedingung.
- Basis-Übereinstimmungspreis (BMP) = $7.99 (oben erläutert)

Für die Berechnung der bedingten Varianzgrundlage gilt folgende Formel:

![Berechnungsformel für bedingte Abweichungen](assets/amazon-cond-variance-calc-1.png)

## Beispiel

Die bedingten Variableneinstellungen lauten wie folgt:

![Beispiel für bedingte Variableneinstellungen](assets/amazon-cond-variances.png)

- BMC = 100 (Konkurrent-Zustand = neu)
- MCV = 80 (Handelsbedingung = verwendet; Gut)
- BMP = $7.99 (Basis-Übereinstimmungspreis = der niedrigste Preis der Bedingungen für ausgeglichene Konkurrent)

![Beispiel für bedingte Variantenbasisberechnung](assets/amazon-cond-variance-calc-2.png)

Bei der Berechnung der bedingten Varianzbasis von oben wird Ihre bedingte Varianzbasis = $6.39 verwendet. Diese Berechnung ist die Konkurrent-Preisquelle, die für Ihre Preisregelaktionen verwendet wird. Weitere Informationen finden Sie in [Preisanpassung](./price-adjustment.md).
