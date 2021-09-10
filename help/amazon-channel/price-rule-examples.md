---
title: Beispiele für Preisregeln
description: Um Sie bei der Erstellung Ihrer Preisregeln für Amazon-Auflistungen zu unterstützen, sollten Sie diese Beispiele anhand gängiger Szenarien durchlesen.
exl-id: 4d9717ba-4ad6-468d-b4ca-99f8620b60b4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 2%

---

# Beispiele für Preisregeln

## Beispiele für Standardpreisregeln

### Nachfolgende Regeln verwerfen

Die Möglichkeit, nachfolgende Regeln zu verwerfen, ist eine großartige Funktion innerhalb der Preisregeln, die verhindert, dass mehrere Preisregeln stapeln und unbeabsichtigte zusätzliche Rabatte gewähren. Um nachfolgende Regeln zu verwerfen, muss eine Preisregel die Prioritäten verwenden, die im Abschnitt _[!UICONTROL Priority]_von [Allgemeine Preisregel-Einstellungen](./pricing-rule-general-settings.md) festgelegt sind.

Wenn **[!UICONTROL Discard Subsequent Rules]** auf `Yes` gesetzt ist, gelten die Regeln mit niedrigerer Priorität (höhere Zahlen) nicht für die förderfähigen Produkte.

Angenommen, es gibt drei Preisregeln:

| Beispiel | Regelname | Priorität | Nachfolgende Regel verwerfen |
|----------|----|----|----|
| 1 | 10 % Rabatt auf Verkaufsprodukte | 1 | Nein |
| 2 | 2 USD an Verkaufsprodukten | 2 | Ja |
| 1 | 5 % aller Produkte | 1 | Nein |

In diesem Szenario gelten die Regeln 1 und 2 für die entsprechenden Produkte. Regel 3 gilt nur für infrage kommende Produkte, die nicht in Regel 2 enthalten sind, da sie eine niedrigere Priorität als Beispiel 2 und **[!UICONTROL Discard Subsequent Rules]** auf `Yes` eingestellt ist. Die in der Verkaufskategorie infrage kommenden Produkte erhalten also einen 10-%-Rabatt und 2-Dollar-Rabatt auf den Amazon-Börsennotierungspreis.

### Anwendung von zwei Preisregeln

| Feld | Einstellung - Regel 1 | Einstellung - Regel 2 |
|----------|----|----|
| [!UICONTROL Rule Name] | Regel 1 | Artikel 2 |
| [!UICONTROL Priority] | 1 | 2 |
| [!UICONTROL Rule Type] | Standardpreisregel | Standardpreisregel |
| [!UICONTROL Price action] | Verringern um | Verringern um |
| [!UICONTROL Apply] | Anwenden als Prozentsatz | Anwenden als fester Betrag |
| [!UICONTROL Adjustment Amount] | 10 | 10 |

#### Produkt 1

Preis: 45,49 $

Regel 1 gilt: 45,49 $ x (0,9) = 40,94 $

Regel 2 gilt: 40,94 $ - 10,00 $ = 30,94 $

Der Endpreis nach Regel 1 und Regel 2 wird angewandt: 30,94 $

#### Produkt 2

Preis: $ 47.76

Regel 1 gilt: 47,76 $ x (0,9) = 42,98 $

Regel 2 gilt: 42,98 $ - 10,00 $ = 32,98 $

Der Endpreis nach Regel 1 und Regel 2 wird angewendet: 32,98 $

## Beispiele für intelligente Neupreisregeln

### Buy Box price mit Floor Price Source = Price

| Feld | Einstellung |
|----------|----|
| [!UICONTROL Rule Name] | Regel 1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | Intelligente Neupreisregel |
| [!UICONTROL Competitor Price Source] | &quot;Buy Box-Preis&quot;verwenden |
| [!UICONTROL Price Action] | Abgleichen des konkurrierenden Preises |
| [!UICONTROL Floor Price Source] | Preis |
| [!UICONTROL Floor Price Action] | Übereinstimmung |

#### Produkt 1

Preis: 15$

[Buy ](./buy-box-competitor-pricing.md) Boxprice aus Amazon: 10$

Da der Preis [Buy Box](./buy-box-competitor-pricing.md) unter dem ursprünglichen Preis liegt, wird das Produkt zum ursprünglichen Preis aufgeführt.

Der Endpreis nach Anwendung der Regel: 15$

#### Produkt 2

Preis: 5$

[Buy ](./buy-box-competitor-pricing.md) Boxprice aus Amazon: 10$

Da der Preis [Buy Box](./buy-box-competitor-pricing.md) höher ist als der Originalpreis, wird das Produkt zum Preis [Buy Box](./buy-box-competitor-pricing.md) aufgeführt.

Der Endpreis nach Anwendung der Regel: 10$

### Buy Box-Preis mit Floor Price Source = Preis und 20% Preisrückgang

| Feld | Einstellung |
|----------|----|
| [!UICONTROL Rule Name] | Regel 1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | Intelligente Neupreisregel |
| [!UICONTROL Competitor Price Source] | &quot;Buy Box-Preis&quot;verwenden |
| [!UICONTROL Price Action] | Abgleichen des konkurrierenden Preises |
| [!UICONTROL Floor Price Source] | Preis |
| [!UICONTROL Floor Price Action] | Verringern um |
| [!UICONTROL Apply] | Anwenden als Prozentsatz |
| [!UICONTROL Floor Adjustment Amount] | 20 |

#### Produkt 1

Preis: 20$

Errechneter Floor-Preis: 16$

[Buy ](./buy-box-competitor-pricing.md) Boxprice aus Amazon: 15$

Da der Preis [Buy Box](./buy-box-competitor-pricing.md) kleiner ist als der berechnete [Floor Price](./floor-price.md), wird das Produkt unter Berechneter [Floor Price](./floor-price.md) aufgeführt.

Der Endpreis nach Anwendung der Regel: 16$

#### Produkt 2

Preis: 15$

Berechnet [Floor Price](./floor-price.md): 12$

[Buy ](./buy-box-competitor-pricing.md) Boxprice aus Amazon: 15$

Da der Preis [Buy Box](./buy-box-competitor-pricing.md) größer ist als der berechnete [Floor Price](./floor-price.md), wird das Produkt zum Preis [Buy Box](./buy-box-competitor-pricing.md) aufgeführt.

Der Endpreis nach Anwendung der Regel: 15$

#### Produkt 3

Preis: 17$

Errechneter Floor-Preis: 13,60$

[Buy ](./buy-box-competitor-pricing.md) Boxprice aus Amazon: 15$

Da der Preis [Buy Box](./buy-box-competitor-pricing.md) größer ist als der berechnete [Floor Price](./floor-price.md), wird das Produkt zum Preis [Buy Box](./buy-box-competitor-pricing.md) aufgeführt.

Der Endpreis nach Anwendung der Regel: 15$

### Niedrigster Preis mit allen Preisen des Wettbewerbers und Verwendung aller Produktbedingungen des Wettbewerbers

| Feld | Einstellung |
|----------|-----|
| [!UICONTROL Rule Name] | Regel 1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | Intelligente Neupreisregel |
| [!UICONTROL Competitor Price Source] | Niedrigster Preis für Konkurrenten |
| [!UICONTROL Minimum Positive Feedback] | Alle konkurrierenden Preise |
| [!UICONTROL Conditional Variance] | Verwenden Sie alle Produktbedingungen des Konkurrenten |
| [!UICONTROL Price Action] | Abgleichen des konkurrierenden Preises |
| [!UICONTROL Floor Price Source] | Preis |
| [!UICONTROL Floor Price Action] | Übereinstimmung |

| Preis | Bedingung |
|----------|----|
| 17$ | Neu |
| 15$ | Neu |
| 14$ | Verwendet; Sehr gut |
| 13$ | Verwendet; Gut |

#### Produkt 1

Preis: 10$

Bedingung: Neu

Da der niedrigste Konkurrenzpreis für die neue Bedingung 15 USD beträgt, wird das Produkt auf 15 USD aufgelistet.

Der Endpreis nach Anwendung der Regel: 15$

#### Produkt 2

Preis: 10$

Bedingung: Verwendet; Acceptable

Da der [niedrigste Konkurrenzpreis](./lowest-competitor-pricing.md) für die verwendete Bedingung 13 USD beträgt, wird das Produkt bei 13 USD aufgeführt.

Der Endpreis nach Anwendung der Regel: 13$

### Intelligente Neupreisregelung, die Obergrenzen, Währungsumrechnung und Mehrwertsteuer kombiniert

| Feld | Einstellung |
|----------|-----|
| [!UICONTROL VAT] | 10 % |
| [!UICONTROL Ceiling price source] | 10$ |
| [!UICONTROL Currency conversion] | 1,25 Euro:1 USD |

[Höchstpreis ](./optional-ceiling-price.md) auf dem europäischen (MwSt)-Markt: $10 x 1,25 = $12,50

Wenn der [Plafonds](./optional-ceiling-price.md) auf dem europäischen (MwSt)-Markt erreicht wird, wird die MwSt berechnet und hinzugefügt.

Endpreis nach MwSt: 12,50 $ x (1,1) = 13,75 $

### Kombinieren mehrerer Preisregeln, des Plafonds, der Währungsumrechnung und der Mehrwertsteuer

#### Intelligente Preisregel (aus dem vorherigen Beispiel)

| Feld | Einstellung |
|----------|----|
| Priorität | 1 |
| Mehrwertsteuer | 10 % |
| Obergrenze der Preisquelle | 10$ |
| Währungsumrechnung | 1,25 Euro:1 USD |

[Höchstpreis ](./optional-ceiling-price.md) auf dem europäischen (MwSt)-Markt: $10 x 1,25 = $12,50

Endpreis nach MwSt: 12,50 $ x (1,1) = 13,75 $

#### Standardmäßige Preisregel

| Feld | Einstellung |
|----------|-----|
| [!UICONTROL Priority] | 2 |
| [!UICONTROL Price Action] | Erhöhen um |
| [!UICONTROL Apply] | Anwenden als fester Betrag |
| [!UICONTROL Adjustment Amount] | 5,00$ |

Wenn der [Plafonds-Preis](./optional-ceiling-price.md) erreicht wird, wird die Standardpreisregel zusätzlich zur intelligenten Preisregel angewendet.

Endpreis nach Anwendung der Standardpreisregel: $13.75 + $5.00 = $18.75

### Preisanpassung

In diesem Beispiel wird der wettbewerbsfähigste Preis definiert, indem man sich den niedrigsten Preis des Amazon [Konkurrenten](./lowest-competitor-pricing.md) mit einem 95-%-positiven Feedback und einer minimalen Feedback-Anzahl von 1.000 Händlern ansieht.

![Beispiel für Preisanpassung](assets/amazon-price-adjustment-example.png)

Nachdem Sie diese Suche anhand dieser Parameter ausgeführt haben, wird der Wettbewerbspreis wieder auf 25 USD gesetzt.

Von hier aus gibt es drei verschiedene [Aktionen für Preisregeln](./pricing-rule-actions.md) Optionen, die auf diesem niedrigsten Preis basieren.

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Price Action] | Optionen:<ul><li>**[!UICONTROL Decrease By]** - Mit dieser Option wird Ihr Börsennotierungspreis im Verhältnis zum  [niedrigsten Konkurrenzpreis](./lowest-competitor-pricing.md) gesenkt.</li><li>**[!UICONTROL Increase By]** - Mit dieser Option erhöhen Sie Ihren Listenpreis im Verhältnis zum  [niedrigsten Konkurrenzpreis](./lowest-competitor-pricing.md).</li><li>**[!UICONTROL Match Competitor Price]** - Mit dieser Option wird Ihr Amazon-Listingpreis so geändert, dass er anhand der Parameter dem niedrigsten Preis entspricht. In diesem Beispiel beträgt der Amazon-Listingpreis 25 USD.</li></ul> |
| [!UICONTROL Apply] | Optionen: Anwenden als Prozentsatz/Anwenden als festen Betrag |
| [!UICONTROL Adjustment Amount] | Numerischer Wert : Angabe des Prozentsatzes oder Festbetrags für den anzuwendenden Rabatt. <br>Diese Auswahl führt dazu, dass der niedrigste Preis angenommen und auf 0,01 USD weniger gesetzt wird. |

### Floor-Preis

| Feld | Einstellung |
|----------|----|
| [!UICONTROL Floor Price Source] | Kosten = 5 USD |
| [!UICONTROL Floor Price Action] | Erhöhen um |
| [!UICONTROL Apply] | Anwenden als Prozentsatz |
| [!UICONTROL Floor Adjustment Amount] | 5 |

[Floor-](./floor-price.md) Preisberechnung = Floor Price Source  `$5` x Floor Adjustment Amount  `5%` = 5,25 USD

Wenn die intelligente Preisregel angewendet wird, ist es möglich, dass der Listenpreis für dieses bestimmte Produkt unter 5,25 USD liegt, wenn die Kosten 5 USD betragen.
