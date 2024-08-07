---
title: Amazon-Vertriebskanal - Beispiele für Preisregeln
description: Um Sie bei der Erstellung Ihrer Preisregeln für Amazon-Auflistungen zu unterstützen, sollten Sie diese Beispiele anhand gängiger Szenarien durchlesen.
feature: Sales Channels, Price Rules
exl-id: 4d9717ba-4ad6-468d-b4ca-99f8620b60b4
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 1%

---

# Beispiele für Preisregeln

## Beispiele für standardmäßige Preisregeln

### Nachfolgende Regeln verwerfen

Die Möglichkeit, nachfolgende Regeln zu verwerfen, ist eine großartige Funktion innerhalb der Preisregeln, die verhindert, dass mehrere Preisregeln stapeln und unbeabsichtigte zusätzliche Rabatte gewähren. Um nachfolgende Regeln zu verwerfen, muss eine Preisregel die Prioritäten verwenden, die im Abschnitt &quot;_[!UICONTROL Priority]_&quot;der allgemeinen Einstellungen der Preisregel [ festgelegt sind.](./pricing-rule-general-settings.md)

Wenn **[!UICONTROL Discard Subsequent Rules]** auf `Yes` gesetzt ist, gelten die Regeln mit niedrigerer Priorität (höhere Zahlen) nicht für die förderfähigen Produkte.

Nehmen wir beispielsweise an, es gibt drei Preisregeln:

| Beispiel | Regelname | Priorität | Nachfolgende Regel verwerfen |
|---------|-----------------------|----------|-------------------------|
| 1 | 10 % Rabatt auf Verkaufsprodukte | 1 | Nein |
| 2 | 2 USD an Verkaufsprodukten | 2 | Ja |
| 3 | 5 % aller Produkte | 3 | Nein |

In diesem Szenario gelten die Regeln 1 und 2 für die entsprechenden Produkte. Regel 3 gilt nur für infrage kommende Produkte, die nicht in Regel 2 enthalten sind, da sie eine niedrigere Priorität als Beispiel 2 hat und **[!UICONTROL Discard Subsequent Rules]** auf `Yes` eingestellt ist. Die in der Verkaufskategorie infrage kommenden Produkte erhalten also einen 10-%-Rabatt und 2-Dollar-Rabatt auf den Amazon-Börsennotierungspreis.

### Anwendung von zwei Standardpreisregeln

| Feld | Einstellung - Regel 1 | Einstellung - Regel 2 |
|--------------------------------|---------------------|-----------------------|
| [!UICONTROL Rule Name] | Regel 1 | Artikel 2 |
| [!UICONTROL Priority] | 1 | 2 |
| [!UICONTROL Rule Type] | Standardpreisregel | Standardpreisregel |
| [!UICONTROL Price action] | Verringern um | Verringern um |
| [!UICONTROL Apply] | Anwenden als Prozentsatz | Anwenden als fester Betrag |
| [!UICONTROL Adjustment Amount] | 10 | 10 |

#### Produkt 1

Preis: 45,49 $

Regel 1 angewendet: 45,49 $ x (0,9) = 40,94 $

Regel 2 angewendet: 40,94 $ - 10,00 $ = 30,94 $

Der Endpreis nach Regel 1 und Regel 2 wird angewendet: 30,94 USD

#### Produkt 2

Preis: 47,76 $

Regel 1 angewendet: 47,76 $ x (0,9) = 42,98 $

Regel 2 angewendet: 42,98 $ - 10,00 $ = 32,98 $

Der Endpreis nach Regel 1 und Regel 2 wird angewendet: 32,98 USD

## Beispiele für intelligente Neuberechnungsregeln

### Buy Box price mit Floor Price Source = Price

| Feld | Einstellung |
|--------------------------------------|----------------------------|
| [!UICONTROL Rule Name] | Regel 1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | Intelligente Neupreisregel |
| [!UICONTROL Competitor Price Source] | &quot;Buy Box-Preis&quot;verwenden |
| [!UICONTROL Price Action] | Abgleichen des konkurrierenden Preises |
| [!UICONTROL Floor Price Source] | Preis |
| [!UICONTROL Floor Price Action] | Übereinstimmung |

#### Produkt 1

Preis: 15 USD

[Buy Box](./buy-box-competitor-pricing.md) Preis von Amazon: 10 USD

Da der Preis für [Buy Box](./buy-box-competitor-pricing.md) unter dem ursprünglichen Preis liegt, wird das Produkt zum ursprünglichen Preis aufgeführt.

Der Endpreis nach Anwendung der Regel: 15 USD

#### Produkt 2

Preis: 5 USD

[Buy Box](./buy-box-competitor-pricing.md) Preis von Amazon: 10 USD

Da der Preis für [Buy Box](./buy-box-competitor-pricing.md) höher ist als der Originalpreis, wird das Produkt zum Preis von [Buy Box](./buy-box-competitor-pricing.md) aufgeführt.

Der Endpreis nach Anwendung der Regel: 10 USD

### Buy Box-Preis mit Floor Price Source = Preis und 20% Preisrückgang

| Feld | Einstellung |
|--------------------------------------|----------------------------|
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

Preis: 20 USD

Errechneter Floor-Preis: 16 USD

[Buy Box](./buy-box-competitor-pricing.md) Preis von Amazon: 15 USD

Da der Preis für [Buy Box](./buy-box-competitor-pricing.md) kleiner ist als der berechnete [Floor Price](./floor-price.md), wird das Produkt unter dem berechneten [Floor Price](./floor-price.md) aufgeführt.

Der endgültige Preis nach Anwendung der Regel: 16 USD

#### Produkt 2

Preis: 15 USD

Errechneter [Floor-Preis](./floor-price.md): 12 USD

[Buy Box](./buy-box-competitor-pricing.md) Preis von Amazon: 15 USD

Da der Preis für [Buy Box](./buy-box-competitor-pricing.md) größer ist als der berechnete [Bodenpreis](./floor-price.md), wird das Produkt zum Preis von [Buy Box](./buy-box-competitor-pricing.md) aufgeführt.

Der Endpreis nach Anwendung der Regel: 15 USD

#### Produkt 3

Preis: 17 USD

Errechneter Floor-Preis: 13,60 USD

[Buy Box](./buy-box-competitor-pricing.md) Preis von Amazon: 15 USD

Da der Preis für [Buy Box](./buy-box-competitor-pricing.md) größer ist als der berechnete [Bodenpreis](./floor-price.md), wird das Produkt zum Preis von [Buy Box](./buy-box-competitor-pricing.md) aufgeführt.

Der Endpreis nach Anwendung der Regel: 15 USD

### Niedrigster Preis mit allen Preisen des Wettbewerbers und Verwendung aller Produktbedingungen des Wettbewerbers

| Feld | Einstellung |
|----------------------------------------|-----------------------------------------|
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
|-------|-----------------|
| 17$ | Neu |
| 15$ | Neu |
| 14$ | Verwendet; sehr gut |
| 13$ | Verwendet; gut |

#### Produkt 1

Preis: 10 USD

Bedingung: Neu

Da der niedrigste Konkurrenzpreis für die neue Bedingung 15 USD beträgt, wird das Produkt auf 15 USD aufgelistet.

Der Endpreis nach Anwendung der Regel: 15 USD

#### Produkt 2

Preis: 10 USD

Bedingung: Verwendet; akzeptabel

Da der [niedrigste Konkurrenzpreis](./lowest-competitor-pricing.md) für die verwendete Bedingung 13 USD beträgt, wird das Produkt bei 13 USD aufgeführt.

Der Endpreis nach Anwendung der Regel: 13 USD

### Intelligente Neupreisregelung, die Obergrenzen, Währungsumrechnung und Mehrwertsteuer kombiniert

| Feld | Einstellung |
|-----------------------------------|---------------|
| [!UICONTROL VAT] | 10 % |
| [!UICONTROL Ceiling price source] | 10$ |
| [!UICONTROL Currency conversion] | 1,25 Euro:1 USD |

[Höchstpreis](./optional-ceiling-price.md) auf dem europäischen (MwSt)-Markt: 10 x 1,25 USD = 12,50 USD

Wenn der [Plafonds} auf dem europäischen (MwSt.-)Markt erreicht ist, wird die MwSt berechnet und hinzugefügt.](./optional-ceiling-price.md)

Endpreis nach Mehrwertsteuer: 12,50 $ x (1,1) = 13,75 $

### Kombinieren mehrerer Preisregeln, des Plafonds, der Währungsumrechnung und der Mehrwertsteuer

#### Intelligente Preisregel (aus dem vorherigen Beispiel)

| Feld | Einstellung |
|----------------------|---------------|
| Priorität | 1 |
| Mehrwertsteuer | 10 % |
| Obergrenze der Preisquelle | 10$ |
| Währungsumrechnung | 1,25 Euro:1 USD |

[Höchstpreis](./optional-ceiling-price.md) auf dem europäischen (MwSt)-Markt: 10 x 1,25 USD = 12,50 USD

Endpreis nach Mehrwertsteuer: 12,50 $ x (1,1) = 13,75 $

#### Standardmäßige Preisregel

| Feld | Einstellung |
|--------------------------------|-----------------------|
| [!UICONTROL Priority] | 2 |
| [!UICONTROL Price Action] | Erhöhen um |
| [!UICONTROL Apply] | Anwenden als fester Betrag |
| [!UICONTROL Adjustment Amount] | 5,00$ |

Wenn der [Plafonds price](./optional-ceiling-price.md) erreicht wird, wird zusätzlich zur intelligenten Preisregel die standardmäßige Preisregel angewendet.

Endpreis nach Anwendung der standardmäßigen Preisregel: $13.75 + $5.00 = $18.75

### Preisanpassung

In diesem Beispiel wird der wettbewerbsfähigste Preis definiert, indem man sich den niedrigsten Preis des Amazon-Konkurrenten [anschaut, der 95 % positive Rückmeldungen und eine minimale Feedback-Anzahl von 1.000 Händlerbewertungen aufweist.](./lowest-competitor-pricing.md)

![Beispiel für Preisanpassung](assets/amazon-price-adjustment-example.png){width="600" zoomable="yes"}

Nachdem Sie diese Suche anhand dieser Parameter ausgeführt haben, wird der Wettbewerbspreis wieder auf 25 USD gesetzt.

Von hier aus gibt es drei verschiedene Optionen für [Preisregel-Aktion](./pricing-rule-actions.md), die auf diesem niedrigsten Preis basieren.

| Feld | Beschreibung |
|--------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Price Action] | Optionen:<ul><li>**[!UICONTROL Decrease By]** - Diese Option senkt Ihren Listenkurs im Verhältnis zum [niedrigsten Konkurrenzpreis](./lowest-competitor-pricing.md).</li><li>**[!UICONTROL Increase By]** - Diese Option erhöht Ihren Listenpreis relativ zum [niedrigsten Konkurrenzpreis](./lowest-competitor-pricing.md).</li><li>**[!UICONTROL Match Competitor Price]** - Mit dieser Option wird Ihr Amazon-Auflistungspreis so geändert, dass er basierend auf den Parametern dem niedrigsten Preis entspricht. In diesem Beispiel beträgt der Amazon-Listingpreis 25 USD.</li></ul> |
| [!UICONTROL Apply] | Optionen: Anwenden als Prozentsatz / Anwenden als Festbetrag |
| [!UICONTROL Adjustment Amount] | Numerischer Wert : Angabe des Prozentsatzes oder Festbetrags für den anzuwendenden Rabatt. <br>Diese Auswahlen führen dazu, dass der niedrigste Preis angenommen und auf 0,01 USD weniger festgelegt wird. |

### Floor-Preis

| Feld | Einstellung |
|--------------------------------------|---------------------|
| [!UICONTROL Floor Price Source] | Kosten = 5 USD |
| [!UICONTROL Floor Price Action] | Erhöhen um |
| [!UICONTROL Apply] | Anwenden als Prozentsatz |
| [!UICONTROL Floor Adjustment Amount] | 5 |

[Floor price](./floor-price.md) calculate = Floor Price Source `$5` x Floor Adjustment Amount `5%` = $5,25

Wenn die intelligente Preisregel angewendet wird, ist es möglich, dass der Listenpreis für dieses bestimmte Produkt unter 5,25 USD liegt, wenn die Kosten 5 USD betragen.
