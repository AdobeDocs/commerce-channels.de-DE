---
title: "Intelligente Preisänderungsregel: Konkurrierende bedingte Abweichungen"
description: Bestimmen Sie anhand einer intelligenten Neupreisregel Ihren Amazon-Listenpreis anhand der Preise und Bedingungen des Konkurrenten.
feature: Sales Channels, Configuration
exl-id: c52230e3-4e47-45bc-80e0-170530f58987
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Intelligente Neupreisregel: Bedingte Unterschiede zwischen Konkurrenten

Zu den Abschnitten einer intelligenten Neupreisregel gehören:

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [!UICONTROL Competitor Conditional Variances]
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [[!UICONTROL Floor Price]](./floor-price.md)
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

Eine intelligente Neupreisregel nutzt die Preise von Amazon-Konkurrenten, um Ihren Börsennotierungspreis zu bestimmen. Wettbewerber sind andere Verkäufer, die dieselben Produkte auflisten, die Sie in Amazon auflisten.

Wenn ein Produkt mit derselben Bedingung vorhanden ist, ist der Basisübereinstimmungspreis der Preis des [niedrigsten Konkurrenten](./lowest-competitor-pricing.md)-Preises mit derselben Bedingung. Wenn kein konkurrierendes Produkt Ihre Bedingung erfüllt, wird der Basispreis für die Übereinstimmung dann durch andere verfügbare Bedingungen für Konkurrenten ersetzt, die mit Neu, Neu und Fortgeführt werden. Nachdem eine Bedingung gefunden wurde, ist der Basis-Übereinstimmungspreis der niedrigste Preis innerhalb dieser Bedingung.

Wenn ein Produkt mit der Bedingung `Used; Good` und dem Basisübereinstimmungspreis aufgelistet ist und ein Wettbewerber dasselbe Produkt unter derselben Bedingung zu einem niedrigeren Preis hat, wird der Preis des Konkurrenten verwendet. Wenn ein Konkurrent nicht mit derselben Bedingung vorhanden ist, sucht das System nach einem Konkurrenten mit der nächsten Bedingung, nämlich `New`. Wird ein Wettbewerber mit dieser Bedingung gefunden, wird der niedrigste Preis verwendet.

## Bedingte Varianten von Konkurrenten konfigurieren

Definieren Sie Ihre Bedingungsabweichungen im Abschnitt _[!UICONTROL Competitor Conditional Variances]_.

Wählen Sie für **[!UICONTROL Conditional Variance]** eine Option:

- `Use all competitor's product conditions` - (Standard) Wählen Sie aus, wann Ihr Produkt mit einer beliebigen verfügbaren Bedingung verglichen werden soll (wenn für die aufgeführte Bedingung keine Übereinstimmung vorliegt).

- `Use Only Matching Competitor's Product Condition` - Wählen Sie aus, wann Ihr Produkt nur mit den Produkten des Konkurrenten in derselben Bedingung verglichen werden soll. Wenn keine Übereinstimmung vorliegt, wird der Preis des Produkts in dem in Ihrem [Listing Price](./listing-price.md) definierten _Magento Price Source_ festgelegt.

- `Apply Variance (if competitor's product condition differs)` - Wählen Sie aus, zunächst einen Vergleich mit Ihrer übereinstimmenden Produktbedingung durchzuführen. Wenn keine übereinstimmende Bedingung vorhanden ist, wird eine Abweichung (in Prozent) in Bezug auf Ihre Produktbedingung und die Bedingung des niedrigsten Konkurrenten angewendet.

  Wenn die Funktion _[!UICONTROL Apply Variance]_ausgewählt wird, werden für jede Ihrer Amazon-Bedingungen zusätzliche Varianzfelder angezeigt. Diese Funktion ermöglicht Ihnen die Verwendung intelligenter Regeln für die Neuberechnung, wenn Sie Produkte anbieten, die sich in einem anderen Zustand befinden als Ihre Konkurrenten. Um die Berechnung hinter bedingten Abweichungen zu verstehen, müssen Sie zunächst verstehen, dass alle Varianzen anhand eines Basis-Übereinstimmungspreises ermittelt werden.

  Die angezeigten bedingten Varianzoptionen basieren auf Ihren Listeneinstellungen für `Condition` , die mithilfe eines [!DNL Commerce] [Produktattributs](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) Bedingungswerten zugeordnet werden. Für alle zugeordneten Bedingungen können Sie einen Varianzprozentsatz von 1-100 definieren. Die Ausnahme sind Sammlerwerte. In diesem Fall kann ein Prozentsatz von mehr als 100 angewendet werden.

![Intelligente Neupreisregel - bedingte Abweichungen von Konkurrenten](assets/amazon-competitor-cond-variances.png){width="500" zoomable="yes"}

| Feld | Beschreibung |
|-----------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Competitor Conditional Variances] | Optionen: <ul><li>**[!UICONTROL Use all competitor's product conditions]** - Wenn für die Bedingung, mit der Sie Ihr Produkt auflisten, keine Übereinstimmung vorhanden ist, wird diese Option mit jeder verfügbaren Bedingung abgeglichen. Er versucht zunächst, Ihre Bedingung zu erfüllen, und arbeitet dann von der `New` -Bedingung zu `Used; Acceptable`.</li><li>**[!UICONTROL Use only matching competitor's product condition]** - Diese Option entspricht der Bedingung Ihres Produkts. Wenn keine Übereinstimmung vorliegt, werden die Produktpreise mit dem Wert _[!UICONTROL Magento Price Source]_berechnet.</li><li>>**[!UICONTROL Apply variance (if competitor's product condition differs)]** - Diese Option versucht zunächst, eine Übereinstimmung mit Ihrer Produktbedingung herzustellen. Wenn keine übereinstimmende Bedingung vorhanden ist, wird eine Varianz (in Prozent) in Bezug auf Ihre Produktbedingung und die Bedingung des niedrigsten Konkurrenten angewendet.</li></ul><br><br>Die bedingten Varianzoptionen, die basierend auf Ihren Listeneinstellungen für Bedingungen angezeigt werden, die mithilfe eines [!DNL Commerce] [Produktattributs](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html) Bedingungswerten zugeordnet werden. Bei allen zugeordneten Bedingungen können Sie einen Varianzprozentsatz von 1-100 angeben. Die Ausnahme sind Sammlerwerte. In diesem Fall kann ein Prozentsatz von mehr als 100 angewendet werden.<br><br>Mit dieser Funktion können Sie intelligente Preisänderungsregeln verwenden, wenn Sie Produkte anbieten, die sich in einer anderen Bedingung als Ihre Konkurrenten befinden. Um die Berechnung hinter bedingten Abweichungen zu verstehen, müssen Sie zunächst verstehen, dass alle Varianzen anhand eines Basis-Übereinstimmungspreises ermittelt werden. |

## Bedingte Varianzbasis berechnen

- Base Match Condition Variance (BMC) = Die Varianz für die Bedingung Ihres Basis-Match-Preiswettbewerbers. Beim vorherigen Beispiel ist BMC die Varianz für die `New` -Bedingung.
- Varianz der Merchant Condition (MCV) = Varianz für die Bedingung Ihres Produkts. Unter Verwendung des vorherigen Beispiels ist MCV = die Varianz für die `Used; Good` -Bedingung.
- Basis-Übereinstimmungspreis (BMP) = 7,99 USD (Erklärung oben)

Die Formel zur Berechnung der bedingten Varianzbasis lautet wie folgt:

![Formel zur Berechnung der bedingten Varianz ](assets/amazon-cond-variance-calc-1.png){width="300"}

## Beispiel

Die bedingten Variableneinstellungen lauten wie folgt:

![Beispiel für bedingte Variableneinstellungen](assets/amazon-cond-variances.png){width="500" zoomable="yes"}

- BMC = 100 (Konkurrierende Bedingung = Neu)
- MCV = 80 (Handelsbedingung = Verwendet; Gut)
- BMP = 7,99 USD (Basis-Übereinstimmungspreis = niedrigster Preis der übereinstimmenden Konkurrenzbedingung)

Beispiel für die Berechnung der bedingten Varianz ](assets/amazon-cond-variance-calc-2.png){width="300"}![

Bei Verwendung der obigen Berechnung der bedingten Varianz beträgt Ihre bedingte Varianzbasis = 6,39 USD. Diese Berechnung ist die Preisquelle des Konkurrenten, die für Ihre Preisregel-Aktionen verwendet wird. Weitere Informationen dazu finden Sie unter [Preisanpassung](./price-adjustment.md).
