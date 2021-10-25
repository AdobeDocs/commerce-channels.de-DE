---
title: Beispiele für Preisregeln
description: Um Ihnen bei der Gestaltung Ihrer Preisregeln für Amazon-Auflistungen behilflich zu sein, sollten Sie sich diese Beispiele anhand gängiger Szenarien ansehen.
exl-id: 4d9717ba-4ad6-468d-b4ca-99f8620b60b4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 2%

---

# Price rule examples

## Standard price rule examples

### Discard Subsequent Rules

Die Möglichkeit, nachfolgende Regeln zu verwerfen, ist ein großartiges Merkmal innerhalb der Preisregeln, das verhindert, dass mehrere Preisregeln stapelbar sind und unbeabsichtigte zusätzliche Rabatte bieten. Um nachfolgende Regeln zu verwerfen, muss eine Preisregel die Prioritäten verwenden, die im _[!UICONTROL Priority]_Abschnitt von [Allgemeine Preisregel - Einstellungen](./pricing-rule-general-settings.md).

Falls **[!UICONTROL Discard Subsequent Rules]** ist eingestellt auf `Yes`gelten die Regeln mit einer niedrigeren Priorität (höhere Zahlen) nicht für die förderfähigen Erzeugnisse.

Nehmen wir zum Beispiel drei Preisregeln:

| Beispiel | Regelname | Priorität | Nachfolgende Regel verwerfen |
|----------|----|----|----|
| 1 | 10 % Rabatt auf Produkte | 1 | No |
| 2 | $2 verkaufte Produkte | 2 | Ja |
| 3 | 5 % aller Produkte | 3 | Nein |

In diesem Szenario gelten die Regeln #1 und #2 für die förderfähigen Produkte. Regel #3 gilt nur für förderfähige Produkte, die nicht in Regel #2 enthalten sind, da sie eine niedrigere Priorität hat als Beispiel #2 und **[!UICONTROL Discard Subsequent Rules]** ist eingestellt auf `Yes`. Die in der Kategorie aufgeführten Erzeugnisse würden also einen Rabatt von 10 % und zwei US-Dollar vom Amazon-Notierungspreis erhalten.

### Anwendung von zwei Standardpreisregeln

| Feld | Einstellung - Regel 1 | Einstellung - Artikel 2 |
|----------|----|----|
| [!UICONTROL Rule Name] | Regel 1 | Artikel 2 |
| [!UICONTROL Priority] | 1 | 2 |
| [!UICONTROL Rule Type] | Standardpreisregel | Standardpreisregel |
| [!UICONTROL Price action] | Verringern um | Verringern um |
| [!UICONTROL Apply] | Als Prozentsatz anwenden | Als festen Betrag anwenden |
| [!UICONTROL Adjustment Amount] | 10 | 10 |

#### Produkt 1

Preis: 45,49 $

Artikel 1 findet Anwendung: $ 45.49 x (0.9) = $ 40.94

Artikel 2 gilt: 40,94 $ - 10,00 $ = 30,94 $

Der endgültige Preis nach Artikel 1 und Artikel 2 wird angewandt: 30,94 $

#### Produkt 2

Preis: 47,76 $

Artikel 1 findet Anwendung: $ 47.76 x (0.9) = $ 42.98

Artikel 2 gilt: 42,98 $ - 10,00 $ = 32,98 $

Der Endpreis nach Regel 1 und Regel 2 wird angewandt: 32,98 $

## Beispiele für intelligente Preisanpassungsregeln

### Buy Box-Preis mit Floor-Preis-Quelle = Preis

| Feld | Einstellung |
|----------|----|
| [!UICONTROL Rule Name] | Regel 1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | Intelligente Preisanpassungsregel |
| [!UICONTROL Competitor Price Source] | &quot;Buy Box&quot;-Preis verwenden |
| [!UICONTROL Price Action] | Übereinstimmungspreis Konkurrent |
| [!UICONTROL Floor Price Source] | Preis |
| [!UICONTROL Floor Price Action] | Übereinstimmung |

#### Produkt 1

Preis: 15 $

[Buy Box](./buy-box-competitor-pricing.md) Preis aus Amazon: $10

weil [Buy Box](./buy-box-competitor-pricing.md) Der Preis ist niedriger als der ursprüngliche Preis, das Produkt wird zum ursprünglichen Preis aufgeführt.

Endpreis nach Anwendung der Regel: 15 $

#### Produkt 2

Preis: $5

[Buy Box](./buy-box-competitor-pricing.md) Preis aus Amazon: $10

weil [Buy Box](./buy-box-competitor-pricing.md) der Preis ist größer als der ursprüngliche Preis, das Produkt wird am [Buy Box](./buy-box-competitor-pricing.md) Preis.

Endpreis nach Anwendung der Regel: $10

### Buy Box-Preis mit Floor-Preis-Quelle = Preis und 20 % Preisrückgang

| Feld | Einstellung |
|----------|----|
| [!UICONTROL Rule Name] | Rule-1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | Intelligent repricing rule |
| [!UICONTROL Competitor Price Source] | &quot;Buy Box&quot;-Preis verwenden |
| [!UICONTROL Price Action] | Übereinstimmungspreis Konkurrent |
| [!UICONTROL Floor Price Source] | Preis |
| [!UICONTROL Floor Price Action] | Verringern um |
| [!UICONTROL Apply] | Als Prozentsatz anwenden |
| [!UICONTROL Floor Adjustment Amount] | 20 |

#### Produkt 1

Preis: 20 $

Errechneter Floor-Preis: 16 $

[Buy Box](./buy-box-competitor-pricing.md) Preis aus Amazon: 15 $

weil [Buy Box](./buy-box-competitor-pricing.md) Preis ist kleiner als der berechnete [Floor-Preis](./floor-price.md), ist das Produkt unter der Liste Berechnete [Floor-Preis](./floor-price.md).

Endpreis nach Anwendung der Regel: 16 $

#### Produkt 2

Preis: 15 $

Berechnet [Floor-Preis](./floor-price.md): 12 $

[Buy Box](./buy-box-competitor-pricing.md) Preis aus Amazon: 15 $

weil [Buy Box](./buy-box-competitor-pricing.md) Preis ist größer als der berechnete [Floor-Preis](./floor-price.md), das Produkt ist unter [Buy Box](./buy-box-competitor-pricing.md) Preis.

Endpreis nach Anwendung der Regel: 15 $

#### Produkt 3

Preis: 17 $

Errechneter Floor-Preis: 13,60 $

[Buy Box](./buy-box-competitor-pricing.md) Preis aus Amazon: 15 $

weil [Buy Box](./buy-box-competitor-pricing.md) Preis ist größer als der berechnete [Floor-Preis](./floor-price.md), das Produkt ist unter [Buy Box](./buy-box-competitor-pricing.md) Preis.

Endpreis nach Anwendung der Regel: 15 $

### Niedrigster Preis mit allen Preisen des Konkurrenten und Verwendung aller Produktbedingungen des Konkurrenten

| Feld | Einstellung |
|----------|-----|
| [!UICONTROL Rule Name] | Regel 1 |
| [!UICONTROL Priority] | 1 |
| [!UICONTROL Rule Type] | Intelligente Preisanpassungsregel |
| [!UICONTROL Competitor Price Source] | Niedrigster Konkurrent-Preis verwenden |
| [!UICONTROL Minimum Positive Feedback] | Alle Konkurrent-Preise |
| [!UICONTROL Conditional Variance] | Alle Produktbedingungen des Konkurrenten verwenden |
| [!UICONTROL Price Action] | Übereinstimmungspreis Konkurrent |
| [!UICONTROL Floor Price Source] | Preis |
| [!UICONTROL Floor Price Action] | Übereinstimmung |

| Preis | Bedingung |
|----------|----|
| 17 $ | Neu |
| 15 $ | Neu |
| 14 $ | Verwendet; Sehr gut |
| 13 $ | Used; Good |

#### Produkt 1

Preis: $10

Bedingung: Neu

Da der niedrigste Konkurrent-Preis für die neue Bedingung 15 US-Dollar beträgt, wird das Produkt bei 15 US-Dollar aufgeführt.

Endpreis nach Anwendung der Regel: 15 $

#### Produkt 2

Preis: $10

Bedingung: Verwendet; Akzeptierbar

weil [niedrigster Konkurrent](./lowest-competitor-pricing.md) für die Gebrauchsbedingung $13, wird das Produkt auf $13 aufgelistet.

Endpreis nach Anwendung der Regel: 13 $

### Intelligente Preisanpassungsregel, die Höchstpreise, Währungsumrechnungen und Mehrwertsteuer kombiniert

| Feld | Setting |
|----------|-----|
| [!UICONTROL VAT] | 10% |
| [!UICONTROL Ceiling price source] | $10 |
| [!UICONTROL Currency conversion] | 1,25 Euro:1 USD |

[Höchstpreis](./optional-ceiling-price.md) auf dem europäischen Markt (MwSt.): $10 x 1.25 = $12.50

Wann [Höchstpreis](./optional-ceiling-price.md) auf dem europäischen Markt (MwSt.), wird die MwSt. berechnet und addiert.

Endpreis nach MwSt.: $12.50 x (1.1) = $13.75

### Kombination mehrerer Preisregeln, Höchstpreise, Währungsumrechnung und Mehrwertsteuer

#### Intelligente Preisregel (aus dem vorherigen Beispiel)

| Feld | Einstellung |
|----------|----|
| Priorität | 1 |
| Mehrwertsteuer | 10% |
| Höchstpreisquelle | $10 |
| Währungsumrechnung | 1,25 Euro:1 USD |

[Höchstpreis](./optional-ceiling-price.md) auf dem europäischen Markt (MwSt.): $10 x 1.25 = $12.50

Endpreis nach MwSt.: $12.50 x (1.1) = $13.75

#### Standardpreisregel

| Feld | Einstellung |
|----------|-----|
| [!UICONTROL Priority] | 2 |
| [!UICONTROL Price Action] | Erhöhen um |
| [!UICONTROL Apply] | Als festen Betrag anwenden |
| [!UICONTROL Adjustment Amount] | 5,00 $ |

Wann [Höchstpreis](./optional-ceiling-price.md) wird getroffen, wird die Standardpreisregel zusätzlich zur intelligenten Preisregel angewendet.

Endpreis nach Anwendung der Standardpreisregel: 13,75 $ + 5,00 $ = 18,75 $

### Preisanpassung

In diesem Beispiel wird der wettbewerbsfähigste Preis durch den Blick auf die Amazon definiert [Niedrigstpreis des Konkurrenten](./lowest-competitor-pricing.md) mit einer positiven Rückmeldung von 95% und einer Mindestanzahl von 1.000 Handelsbewertungen.

![Beispiel für Preisanpassung](assets/amazon-price-adjustment-example.png)

Nachdem Sie diese Suche anhand dieser Parameter durchgeführt haben, wird der Wettbewerbspreis auf $25 zurückgesetzt.

Von hier aus gibt es drei verschiedene [Preisregel](./pricing-rule-actions.md) Entscheidungen auf der Grundlage dieses niedrigsten Preises.

| Feld | Beschreibung |
|--- |--- |
| [!UICONTROL Price Action] | Optionen:<ul><li>**[!UICONTROL Decrease By]** - Diese Option senkt Ihren Börsennotierungspreis im Verhältnis zu [niedrigster Konkurrent](./lowest-competitor-pricing.md).</li><li>**[!UICONTROL Increase By]** - Mit dieser Option erhöhen Sie Ihren Börsenpreis im Verhältnis zu [niedrigster Konkurrent](./lowest-competitor-pricing.md).</li><li>**[!UICONTROL Match Competitor Price]** - Mit dieser Option wird der Amazon-Börsennotierungspreis auf der Grundlage der Parameter auf den niedrigsten Preis angepasst. In diesem Beispiel liegt der Börsennotierungspreis Amazon bei 25 Dollar.</li></ul> |
| [!UICONTROL Apply] | Optionen: Als Prozentsatz anwenden/Festbetrag anwenden |
| [!UICONTROL Adjustment Amount] | Zahlenwert zur Bestimmung des Prozentsatzes oder des Festbetrags für den anzuwendenden Rabatt. <br>Diese Auswahlen führen dazu, dass der niedrigste Preis gewählt und auf $0,01 reduziert wird. |

### Floor-Preis

| Feld | Setting |
|----------|----|
| [!UICONTROL Floor Price Source] | Cost = $5 |
| [!UICONTROL Floor Price Action] | Erhöhen um |
| [!UICONTROL Apply] | Als Prozentsatz anwenden |
| [!UICONTROL Floor Adjustment Amount] | 5 |

[Floor-Preis](./floor-price.md) Berechnung = Floor Price Source `$5` x Floor Adjustment Betrag `5%` = 5,25 $

Wenn die intelligente Preisregel angewendet wird, kann der Börsennotierungspreis für dieses Produkt unter 5,25 US-Dollar liegen, wenn die Kosten 5 US-Dollar betragen.
